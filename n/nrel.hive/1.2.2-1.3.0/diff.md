# Comparing `tmp/nrel.hive-1.2.2.tar.gz` & `tmp/nrel.hive-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nrel.hive-1.2.2.tar", last modified: Mon Apr 17 22:07:28 2023, max compression
+gzip compressed data, was "dist/nrel.hive-1.3.0.tar", last modified: Fri Jun  9 22:07:12 2023, max compression
```

## Comparing `nrel.hive-1.2.2.tar` & `nrel.hive-1.3.0.tar`

### file list

```diff
@@ -1,456 +1,456 @@
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.337108 nrel.hive-1.2.2/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1529 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/LICENSE
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       74 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/MANIFEST.in
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    19691 2023-04-17 22:07:28.336689 nrel.hive-1.2.2/PKG-INFO
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    18750 2023-04-17 19:40:31.000000 nrel.hive-1.2.2/README.md
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.022535 nrel.hive-1.2.2/nrel/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       56 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.027147 nrel.hive-1.2.2/nrel/hive/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1327 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       99 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/__main__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.029400 nrel.hive-1.2.2/nrel/hive/app/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       34 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/app/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3093 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/app/hive_cosim.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3811 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/app/run.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2553 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/app/run_batch.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2709 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/app/run_tune.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.033406 nrel.hive-1.2.2/nrel/hive/config/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      296 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/config/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1157 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/config/config_builder.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1816 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/config/dispatcher_config.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2954 2023-02-27 22:55:12.000000 nrel.hive-1.2.2/nrel/hive/config/global_config.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6768 2023-02-27 22:55:12.000000 nrel.hive-1.2.2/nrel/hive/config/hive_config.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6665 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/config/input.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      854 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/config/network.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2130 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/config/sim.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.033819 nrel.hive-1.2.2/nrel/hive/dispatcher/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       93 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.035796 nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      238 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2375 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/basic_forecaster.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      190 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/forecast.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      717 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/forecaster_interface.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.038210 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      264 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1221 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instruction.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6877 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instruction_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      269 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instruction_result.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    13393 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instructions.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.042429 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    17527 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/assignment_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4206 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/charging_fleet_manager.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      964 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/charging_search_type.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5156 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/dispatcher.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1252 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/instruction_generator.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    12308 2023-03-16 22:23:46.000000 nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/instruction_generator_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.049705 nrel.hive-1.2.2/nrel/hive/initialization/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/initialization/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1929 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/initialization/initialize_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    17315 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/initialization/initialize_simulation.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7721 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/initialization/initialize_simulation_with_sampling.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3882 2023-04-03 21:41:45.000000 nrel.hive-1.2.2/nrel/hive/initialization/load.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2460 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/initialization/sample_requests.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6508 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/initialization/sample_vehicles.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.054549 nrel.hive-1.2.2/nrel/hive/model/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5472 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/model/base.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.055677 nrel.hive-1.2.2/nrel/hive/model/energy/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      108 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/energy/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.056815 nrel.hive-1.2.2/nrel/hive/model/energy/charger/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2365 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/energy/charger/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      340 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/energy/charger/charger.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      563 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/energy/energytype.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1247 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/entity.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      332 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/model/entity_position.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3390 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/model/membership.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2100 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/model/passenger.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.060244 nrel.hive-1.2.2/nrel/hive/model/request/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      132 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/request/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     9718 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/model/request/request.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      986 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/request/request_rate_structure.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.065906 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      557 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1505 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/geofence.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      930 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/haversine_link_id_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3507 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/haversine_roadnetwork.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2759 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/link.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2137 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/link_id.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5529 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/linktraversal.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.079369 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1386 2023-04-05 15:51:28.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_builders.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    10081 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_road_network_link_helper.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     9702 2023-04-05 15:51:28.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_roadnetwork.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4862 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_roadnetwork_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3385 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/roadnetwork.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3801 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/route.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5159 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/model/roadnetwork/routetraversal.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2027 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/sim_time.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.081930 nrel.hive-1.2.2/nrel/hive/model/station/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/station/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5552 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/station/charger_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    17894 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/model/station/station.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3927 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/station/station_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.083698 nrel.hive-1.2.2/nrel/hive/model/vehicle/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.088097 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3661 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8479 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/bev.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6682 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/ice.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3229 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/mechatronics_interface.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.091599 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1238 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      720 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1403 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3565 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/tabular_powercurve.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.094575 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1241 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      963 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/powertrain.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3164 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/tabular_powertrain.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.097292 nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1265 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      355 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/schedule.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      828 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/schedule_type.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2534 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/time_range_schedule.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      120 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/trip_phase.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8110 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/model/vehicle/vehicle.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/py.typed
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.101755 nrel.hive-1.2.2/nrel/hive/reporting/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/reporting/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1282 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/reporting/driver_event_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.106668 nrel.hive-1.2.2/nrel/hive/reporting/handler/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2078 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/eventful_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      762 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1440 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/instruction_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4562 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/stateful_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2744 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/stats_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3924 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/summary_stats.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    15954 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/time_step_stats_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1974 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/handler/vehicle_charge_events_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1487 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/instruction_generator_event_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1432 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/reporting/report_type.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3025 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/reporter.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1872 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/reporter_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    10883 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/reporting/vehicle_event_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.108174 nrel.hive-1.2.2/nrel/hive/resources/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    10244 2023-02-07 23:38:57.000000 nrel.hive-1.2.2/nrel/hive/resources/.DS_Store
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.112258 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      159 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      153 2023-02-27 23:04:49.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      157 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      157 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    19849 2023-01-18 23:36:57.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/mock_lobster.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    21397 2022-10-27 20:49:00.000000 nrel.hive-1.2.2/nrel/hive/resources/__pycache__/mock_lobster.cpython-38.pyc
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.113397 nrel.hive-1.2.2/nrel/hive/resources/chargers/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.115690 nrel.hive-1.2.2/nrel/hive/resources/chargers/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      162 2023-02-27 23:05:28.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      166 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      166 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      161 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/chargers/default_chargers.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.117864 nrel.hive-1.2.2/nrel/hive/resources/defaults/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1697 2023-02-27 22:55:12.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/.hive.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.120056 nrel.hive-1.2.2/nrel/hive/resources/defaults/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      162 2023-02-27 23:05:28.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      166 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      166 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2761 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/hive_config.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       55 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/defaults/sample.batch.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.121077 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.122733 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      172 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      170 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      170 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      438 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/mechatronics/mechatronics.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    22632 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/resources/mock_lobster.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.123831 nrel.hive-1.2.2/nrel/hive/resources/powercurve/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.126508 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      170 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      164 2023-02-27 23:05:28.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1741 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/powercurve/normalized.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.128385 nrel.hive-1.2.2/nrel/hive/resources/powertrain/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.131046 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      170 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      164 2023-02-27 23:05:28.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      168 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      816 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/normalized-electric.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1067 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/powertrain/normalized-gasoline.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.132430 nrel.hive-1.2.2/nrel/hive/resources/scenarios/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8196 2023-02-14 15:54:20.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/.DS_Store
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.134778 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      169 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      163 2023-02-27 23:04:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      167 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      167 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.138811 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    10244 2023-02-07 23:38:52.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/.DS_Store
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.141338 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      185 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      179 2023-02-27 23:04:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      183 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      183 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.145076 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      335 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      104 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_bases.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      138 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_fleets_bases.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       68 2023-03-16 22:23:46.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_no_stations.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       67 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/bases/denver_rl_toy_bases.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.146719 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/chargers/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      270 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/chargers/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/chargers/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      151 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/chargers/chargers_varied.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.150303 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      687 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.151370 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      201 2022-11-29 19:20:22.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      199 2022-10-20 17:48:02.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      503 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_geoid.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      543 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_station_id.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      151 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_constrained_prices.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      330 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_rl_toy_charging_prices.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.153021 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/demand_forecast/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/demand_forecast/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    25934 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/demand_forecast/denver_demand.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       24 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/demand_forecast/denver_rl_toy_demand.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3352 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      992 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo_constrained_charging.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      743 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo_fleets.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3323 2023-03-16 22:23:46.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_no_stations.yaml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      828 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_rl_toy.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.154660 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      810 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.155744 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      192 2022-11-29 19:20:23.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      190 2022-10-20 17:48:03.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      491 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/denver_duel_fleets.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.157289 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/geofence/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      157 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/geofence/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/geofence/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      979 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/geofence/downtown_denver.geojson
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.159081 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/mechatronics/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      206 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/mechatronics/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/mechatronics/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      263 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/mechatronics/denver_rl_toy_mechatronics.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.163284 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      447 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.164538 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      194 2022-11-29 19:20:22.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      192 2022-10-20 17:48:02.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)   234550 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_fleets_requests.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)   190195 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_requests.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1090 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_rl_toy_requests.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.166365 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      369 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.167764 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      198 2022-11-29 19:20:23.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      196 2022-10-20 17:48:03.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    92920 2023-04-05 15:51:28.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/downtown_denver_network.json
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.169993 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      294 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.171067 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      200 2022-11-29 19:20:26.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      198 2022-10-20 17:48:07.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       45 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/denver_rl_toy_rate_structure.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       49 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/service_prices/rate_structure.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.175090 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      431 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      398 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_fleets_stations.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       60 2023-03-16 22:23:46.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_no_stations.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      354 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      300 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations_constrained.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       98 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/stations/denver_rl_toy_stations.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.189861 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      540 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/README.md
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      885 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      872 2023-03-16 22:23:46.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles_no_stations.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      801 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_rl_toy_vehicles.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.201645 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8196 2023-02-07 23:38:52.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/.DS_Store
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.212944 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      179 2022-11-15 17:21:24.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      173 2023-02-27 23:04:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      177 2022-10-20 17:50:49.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      177 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.214239 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/bases/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/bases/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      172 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/bases/nyc_bases.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.215436 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/charging_prices/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/charging_prices/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5204 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/charging_prices/nyc_fixed.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.216708 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/demand_forecast/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/demand_forecast/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    12677 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/demand_forecast/nyc_demand.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.217838 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/geofence/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/geofence/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)   474130 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/geofence/nyc_single_polygon.geojson
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      682 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/manhattan.yaml
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.220296 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/requests/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/requests/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)  1089600 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/requests/nyc_20k.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.224175 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/road_network/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/road_network/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)  1265357 2023-04-05 15:51:28.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/road_network/manhattan_network.json
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.229926 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/service_prices/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/service_prices/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       49 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/service_prices/rate_structure.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.232198 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/stations/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/stations/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      794 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/stations/nyc_stations.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.234586 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    51472 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_1200.csv
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8492 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_200.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.236091 nrel.hive-1.2.2/nrel/hive/resources/schedules/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.239035 nrel.hive-1.2.2/nrel/hive/resources/schedules/__pycache__/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      169 2022-11-02 23:03:49.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      163 2023-02-27 23:05:28.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      167 2022-10-20 17:47:45.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      167 2022-12-07 18:39:27.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      117 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/resources/schedules/default_schedules.csv
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.242091 nrel.hive-1.2.2/nrel/hive/runner/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      186 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/runner/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1363 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/runner/environment.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2129 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/runner/local_simulation_runner.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      763 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/runner/runner_payload.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3115 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/runner/runner_payload_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.242659 nrel.hive-1.2.2/nrel/hive/state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      266 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.245876 nrel.hive-1.2.2/nrel/hive/state/driver_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/__init__.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.248752 nrel.hive-1.2.2/nrel/hive/state/driver_state/autonomous_driver_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/autonomous_driver_state/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2621 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_available.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      251 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_driver_attributes.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     9152 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/driver_instruction_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5190 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/driver_state.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.251319 nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      391 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/human_driver_attributes.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    11713 2023-02-28 18:13:24.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/human_driver_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3223 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/human_unavailable_charge_parameters.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.252552 nrel.hive-1.2.2/nrel/hive/state/entity_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/entity_state/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1704 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/entity_state/entity_state_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.255782 nrel.hive-1.2.2/nrel/hive/state/simulation_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      730 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/at_location_response.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    11305 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/simulation_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    25198 2023-02-27 22:55:12.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/simulation_state_ops.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.262674 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3084 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/cancel_requests.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    10482 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/charging_price_update.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      850 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/simulation_update.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6275 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/step_simulation.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7608 2023-03-07 18:37:42.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/step_simulation_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4720 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7687 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update_requests_from_file.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4066 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update_requests_sampling.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.274772 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8920 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charge_queueing.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    11663 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charging_base.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8637 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charging_station.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5605 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_base.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6876 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8270 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_pooling_trip.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6585 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_station.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8882 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_trip.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4410 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/idle.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2807 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/out_of_service.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     4318 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/repositioning.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5523 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/reserve_base.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    11725 2023-02-27 22:55:12.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     9711 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_pooling_trip.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8560 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_trip.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8472 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/vehicle_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8967 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/vehicle_state_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      370 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/state/vehicle_state/vehicle_state_type.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.285542 nrel.hive-1.2.2/nrel/hive/util/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      919 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7030 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/dict_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      113 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/error_or_result.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3381 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/util/exception.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1473 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/fp.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6903 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/util/fs.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1020 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/util/geo.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     9219 2023-02-23 16:22:48.000000 nrel.hive-1.2.2/nrel/hive/util/h3_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7955 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/nrel/hive/util/iterators.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1318 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/time_helpers.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2950 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/nrel/hive/util/tuple_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      818 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/typealiases.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3020 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/nrel/hive/util/units.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      776 2022-10-20 17:47:42.000000 nrel.hive-1.2.2/nrel/hive/util/validation.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2007 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/nrel/hive/util/wkt.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.025702 nrel.hive-1.2.2/nrel.hive.egg-info/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    19691 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/PKG-INFO
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    19468 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/SOURCES.txt
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        1 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/dependency_links.txt
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       88 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/entry_points.txt
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      250 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/requires.txt
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        5 2023-04-17 22:07:25.000000 nrel.hive-1.2.2/nrel.hive.egg-info/top_level.txt
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1862 2023-04-17 21:37:22.000000 nrel.hive-1.2.2/pyproject.toml
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       38 2023-04-17 22:07:28.337264 nrel.hive-1.2.2/setup.cfg
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)       38 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/setup.py
-drwxr-xr-x   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)        0 2023-04-17 22:07:28.335989 nrel.hive-1.2.2/tests/
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      140 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/__init__.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2920 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_base.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2787 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_bev_mechatronics.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2441 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_build_mechatronics_table.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1436 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_cancel_requests.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5133 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/tests/test_charging_price_update.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2520 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_config_builder.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3034 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_dict_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     6368 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_dict_reader_stepper.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1784 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_driver_instruction_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1467 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_fs.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3276 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_h3_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1564 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_haversine_roadnetwork.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     8711 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_human_driver_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2369 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_ice_mechatronics.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1166 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_initialize_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3148 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/tests/test_initialize_simulation.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2876 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_instruction_generator_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5295 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_instruction_generators.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2642 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_local_simulation_runner.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1972 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_osm_roadnetwork.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3407 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_request.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2957 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_routetraversal.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1368 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_run_cosim.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3521 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_sample_functions.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2501 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_schedules.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    12930 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_simulation_state_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)    25185 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/tests/test_simulationstate.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     7983 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_station.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2034 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_station_load_handler.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1162 2023-01-18 23:36:55.000000 nrel.hive-1.2.2/tests/test_step_simulation_ops.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     1024 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/tests/test_time.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     5075 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_update_requests.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)      875 2022-11-29 19:20:11.000000 nrel.hive-1.2.2/tests/test_update_requests_sampling.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     2021 2022-11-02 21:45:19.000000 nrel.hive-1.2.2/tests/test_vehicle.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)   103126 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/tests/test_vehicle_state.py
--rw-r--r--   0 rfitzger (1525561519) NREL_NT\Domain Users (18434217)     3361 2023-02-23 16:22:51.000000 nrel.hive-1.2.2/tests/test_vehicle_state_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.310955 nrel.hive-1.3.0/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1529 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/LICENSE
+-rw-r--r--   0 rfitzger (1525561519) 18434217       74 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/MANIFEST.in
+-rw-r--r--   0 rfitzger (1525561519) 18434217    14581 2023-06-09 22:07:12.310488 nrel.hive-1.3.0/PKG-INFO
+-rw-r--r--   0 rfitzger (1525561519) 18434217    13640 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/README.md
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.017911 nrel.hive-1.3.0/nrel/
+-rw-r--r--   0 rfitzger (1525561519) 18434217       56 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.022712 nrel.hive-1.3.0/nrel/hive/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1303 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217       99 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/__main__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.024780 nrel.hive-1.3.0/nrel/hive/app/
+-rw-r--r--   0 rfitzger (1525561519) 18434217       34 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/app/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3141 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/app/hive_cosim.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3955 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/app/run.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2499 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/app/run_batch.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.029783 nrel.hive-1.3.0/nrel/hive/config/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      296 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/config/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1157 2023-02-23 16:22:51.000000 nrel.hive-1.3.0/nrel/hive/config/config_builder.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1809 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/config/dispatcher_config.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3001 2023-04-26 17:07:25.000000 nrel.hive-1.3.0/nrel/hive/config/global_config.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6238 2023-04-26 20:40:51.000000 nrel.hive-1.3.0/nrel/hive/config/hive_config.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6214 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/config/input.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      854 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/config/network.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2228 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/config/sim.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.030303 nrel.hive-1.3.0/nrel/hive/dispatcher/
+-rw-r--r--   0 rfitzger (1525561519) 18434217       93 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.032447 nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      238 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2363 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/basic_forecaster.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      190 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/forecast.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      717 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/forecaster_interface.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.035282 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      264 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1221 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instruction.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6876 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instruction_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      270 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instruction_result.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    13393 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instructions.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.039687 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    18118 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/assignment_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4206 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/charging_fleet_manager.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      964 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/charging_search_type.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5094 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/dispatcher.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1562 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/instruction_function.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1252 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/instruction_generator.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    12284 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/instruction_generator_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.043980 nrel.hive-1.3.0/nrel/hive/initialization/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/initialization/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1930 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/initialization/initialize_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    18253 2023-04-26 17:07:25.000000 nrel.hive-1.3.0/nrel/hive/initialization/initialize_simulation.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     7686 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/initialization/initialize_simulation_with_sampling.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4333 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/initialization/load.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2468 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/initialization/sample_requests.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6754 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/initialization/sample_vehicles.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.047835 nrel.hive-1.3.0/nrel/hive/model/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5541 2023-04-26 17:39:37.000000 nrel.hive-1.3.0/nrel/hive/model/base.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.049030 nrel.hive-1.3.0/nrel/hive/model/energy/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      108 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/energy/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.050125 nrel.hive-1.3.0/nrel/hive/model/energy/charger/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2341 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/energy/charger/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      340 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/energy/charger/charger.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      563 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/energy/energytype.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1246 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/entity.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      332 2023-02-23 16:22:48.000000 nrel.hive-1.3.0/nrel/hive/model/entity_position.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3390 2023-02-23 16:22:48.000000 nrel.hive-1.3.0/nrel/hive/model/membership.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2100 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/passenger.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.051738 nrel.hive-1.3.0/nrel/hive/model/request/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      132 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/request/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9706 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/request/request.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      986 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/request/request_rate_structure.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.057233 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      557 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1505 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/geofence.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      930 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/haversine_link_id_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3499 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/haversine_roadnetwork.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2759 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/link.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2138 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/link_id.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5529 2023-02-23 16:22:48.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/linktraversal.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.060084 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1444 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_builders.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    10081 2023-01-18 23:36:55.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_road_network_link_helper.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    11407 2023-06-05 18:53:00.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_roadnetwork.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4862 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_roadnetwork_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3332 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/roadnetwork.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3751 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/route.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5835 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/nrel/hive/model/roadnetwork/routetraversal.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2027 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/model/sim_time.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.062356 nrel.hive-1.3.0/nrel/hive/model/station/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/station/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5499 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/station/charger_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    18709 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/model/station/station.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3926 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/station/station_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.063899 nrel.hive-1.3.0/nrel/hive/model/vehicle/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.066132 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3660 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8939 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/bev.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     7136 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/ice.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3220 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/mechatronics_interface.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.068346 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1238 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      720 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2707 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3565 2023-02-23 16:22:51.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/tabular_powercurve.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.070165 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1241 2023-01-18 23:36:55.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      963 2023-01-18 23:36:55.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/powertrain.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3164 2023-01-18 23:36:55.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/tabular_powertrain.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.072373 nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1264 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      355 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/schedule.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      828 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/schedule_type.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2534 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/time_range_schedule.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      120 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/trip_phase.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9215 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/model/vehicle/vehicle.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/py.typed
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.077839 nrel.hive-1.3.0/nrel/hive/reporting/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/reporting/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1250 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/driver_event_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.084863 nrel.hive-1.3.0/nrel/hive/reporting/handler/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2068 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/eventful_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      761 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1380 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/instruction_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2783 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/kepler_feature.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3018 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/kepler_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4594 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/stateful_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2653 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/stats_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5640 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/summary_stats.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    15342 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/time_step_stats_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1938 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/handler/vehicle_charge_events_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1488 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/instruction_generator_event_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1432 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/reporting/report_type.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2920 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/reporting/reporter.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1851 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/reporting/reporter_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    10881 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/reporting/vehicle_event_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.085987 nrel.hive-1.3.0/nrel/hive/resources/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.095050 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      159 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      153 2023-02-27 23:04:49.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      157 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      157 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217    19849 2023-01-18 23:36:57.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/mock_lobster.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217    21397 2022-10-27 20:49:00.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/mock_lobster.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217    21726 2023-06-05 16:23:56.000000 nrel.hive-1.3.0/nrel/hive/resources/__pycache__/mock_lobster.cpython-39.pyc
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.096604 nrel.hive-1.3.0/nrel/hive/resources/chargers/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.100737 nrel.hive-1.3.0/nrel/hive/resources/chargers/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      162 2023-02-27 23:05:28.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      166 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      166 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      161 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/chargers/default_chargers.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.104049 nrel.hive-1.3.0/nrel/hive/resources/defaults/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1757 2023-04-26 17:07:25.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/.hive.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.108187 nrel.hive-1.3.0/nrel/hive/resources/defaults/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      162 2023-02-27 23:05:28.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      166 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      166 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2797 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/hive_config.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217       55 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/defaults/sample.batch.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.109910 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.112718 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      172 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      170 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      170 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      438 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/mechatronics/mechatronics.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217    26653 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/nrel/hive/resources/mock_lobster.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.114203 nrel.hive-1.3.0/nrel/hive/resources/powercurve/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.117924 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      170 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      164 2023-02-27 23:05:28.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1741 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/powercurve/normalized.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.120106 nrel.hive-1.3.0/nrel/hive/resources/powertrain/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.123823 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      170 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      164 2023-02-27 23:05:28.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      168 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      816 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/normalized-electric.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1067 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/powertrain/normalized-gasoline.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.124866 nrel.hive-1.3.0/nrel/hive/resources/scenarios/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.128163 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      169 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      163 2023-02-27 23:04:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      167 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      167 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.131828 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.135041 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      185 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      179 2023-02-27 23:04:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      183 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      183 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.139378 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      335 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      104 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_bases.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      138 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_fleets_bases.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217       68 2023-03-16 22:23:46.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/denver_demo_no_stations.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217       67 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/bases/denver_rl_toy_bases.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.141377 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/chargers/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      274 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/chargers/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/chargers/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      151 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/chargers/chargers_varied.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.145202 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      716 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.147451 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      201 2022-11-29 19:20:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      199 2022-10-20 17:48:02.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      199 2023-06-05 18:53:03.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      503 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_geoid.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      543 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_station_id.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      151 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_constrained_prices.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      330 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_rl_toy_charging_prices.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3164 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217      909 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo_constrained_charging.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217      660 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo_fleets.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3135 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_no_stations.yaml
+-rw-r--r--   0 rfitzger (1525561519) 18434217      738 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_rl_toy.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.149162 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      811 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.151469 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      192 2022-11-29 19:20:23.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      190 2022-10-20 17:48:03.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      190 2023-06-05 18:53:03.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      491 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/denver_duel_fleets.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.153255 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/geofence/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      157 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/geofence/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/geofence/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      979 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/geofence/downtown_denver.geojson
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.155206 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/mechatronics/
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2135 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/mechatronics/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/mechatronics/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      263 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/mechatronics/denver_rl_toy_mechatronics.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.161269 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      451 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.163614 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      194 2022-11-29 19:20:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      192 2022-10-20 17:48:02.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      192 2023-06-05 18:53:03.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217   234550 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_fleets_requests.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217   190195 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_requests.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1090 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_rl_toy_requests.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.165556 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      369 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.167966 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      198 2022-11-29 19:20:23.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      196 2022-10-20 17:48:03.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      196 2023-06-05 18:53:04.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217    92920 2023-04-26 17:41:35.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/downtown_denver_network.json
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.170147 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      341 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.172449 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      200 2022-11-29 19:20:26.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      198 2022-10-20 17:48:07.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      198 2023-06-05 18:53:08.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217       45 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/denver_rl_toy_rate_structure.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217       49 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/service_prices/rate_structure.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.177045 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      435 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      398 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_fleets_stations.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217       60 2023-03-16 22:23:46.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_no_stations.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      354 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      300 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations_constrained.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217       98 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/stations/denver_rl_toy_stations.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.186157 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      544 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/README.md
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      885 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      872 2023-03-16 22:23:46.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles_no_stations.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217      801 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_rl_toy_vehicles.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.187714 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.191753 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      179 2022-11-15 17:21:24.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      173 2023-02-27 23:04:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      177 2022-10-20 17:50:49.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      177 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.194130 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/bases/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/bases/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      172 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/bases/nyc_bases.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.199181 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/charging_prices/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/charging_prices/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5204 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/charging_prices/nyc_fixed.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.200611 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/geofence/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/geofence/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217   474130 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/geofence/nyc_single_polygon.geojson
+-rw-r--r--   0 rfitzger (1525561519) 18434217      631 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/manhattan.yaml
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.204861 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/requests/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/requests/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217  1370933 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/requests/nyc_20k.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.208976 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/road_network/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/road_network/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217  1265357 2023-04-05 15:51:28.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/road_network/manhattan_network.json
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.214450 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/service_prices/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/service_prices/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217       49 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/service_prices/rate_structure.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.218112 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/stations/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/stations/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      794 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/stations/nyc_stations.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.220350 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    51472 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_1200.csv
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8492 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_200.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.221435 nrel.hive-1.3.0/nrel/hive/resources/schedules/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.225504 nrel.hive-1.3.0/nrel/hive/resources/schedules/__pycache__/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      169 2022-11-02 23:03:49.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      163 2023-02-27 23:05:28.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      167 2022-10-20 17:47:45.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      167 2022-12-07 18:39:27.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rfitzger (1525561519) 18434217      117 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/resources/schedules/default_schedules.csv
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.229026 nrel.hive-1.3.0/nrel/hive/runner/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      186 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/runner/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1363 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/runner/environment.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2129 2023-02-23 16:22:51.000000 nrel.hive-1.3.0/nrel/hive/runner/local_simulation_runner.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      762 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/runner/runner_payload.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3114 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/runner/runner_payload_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.229922 nrel.hive-1.3.0/nrel/hive/state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      266 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.231435 nrel.hive-1.3.0/nrel/hive/state/driver_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/__init__.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.232993 nrel.hive-1.3.0/nrel/hive/state/driver_state/autonomous_driver_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/autonomous_driver_state/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2574 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_available.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      251 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_driver_attributes.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9234 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/driver_instruction_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5190 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/driver_state.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.235069 nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      391 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/human_driver_attributes.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    11713 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/human_driver_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3223 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/human_unavailable_charge_parameters.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.236023 nrel.hive-1.3.0/nrel/hive/state/entity_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/entity_state/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1705 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/entity_state/entity_state_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.238393 nrel.hive-1.3.0/nrel/hive/state/simulation_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      730 2023-02-23 16:22:48.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/at_location_response.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8340 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/simulation_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    25174 2023-06-05 19:28:42.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/simulation_state_ops.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.243882 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3073 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/cancel_requests.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    10507 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/charging_price_update.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      850 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/simulation_update.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6260 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/step_simulation.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     7815 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/step_simulation_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4622 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     7675 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update_requests_from_file.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4054 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update_requests_sampling.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.253909 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/
+-rw-r--r--   0 rfitzger (1525561519) 18434217        0 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8908 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charge_queueing.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    11651 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charging_base.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8625 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charging_station.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5594 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_base.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6876 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8270 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_pooling_trip.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6585 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_station.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8870 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_trip.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4409 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/idle.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2794 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/out_of_service.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     4241 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/repositioning.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5511 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/reserve_base.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    11725 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9711 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_pooling_trip.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8560 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_trip.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8470 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/vehicle_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9378 2023-06-05 18:05:14.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/vehicle_state_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      370 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/state/vehicle_state/vehicle_state_type.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.262940 nrel.hive-1.3.0/nrel/hive/util/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      919 2023-04-26 17:07:22.000000 nrel.hive-1.3.0/nrel/hive/util/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    10370 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/util/dict_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      113 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/util/error_or_result.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3381 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/util/exception.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1441 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/fp.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6903 2023-02-23 16:22:51.000000 nrel.hive-1.3.0/nrel/hive/util/fs.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      998 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/geo.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9288 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/nrel/hive/util/h3_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      427 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/io.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     7938 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/iterators.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1318 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/nrel/hive/util/time_helpers.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2950 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/nrel/hive/util/tuple_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      817 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/typealiases.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3020 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/units.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      776 2022-10-20 17:47:42.000000 nrel.hive-1.3.0/nrel/hive/util/validation.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2006 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/nrel/hive/util/wkt.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.020916 nrel.hive-1.3.0/nrel.hive.egg-info/
+-rw-r--r--   0 rfitzger (1525561519) 18434217    14581 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/PKG-INFO
+-rw-r--r--   0 rfitzger (1525561519) 18434217    19654 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/SOURCES.txt
+-rw-r--r--   0 rfitzger (1525561519) 18434217        1 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/dependency_links.txt
+-rw-r--r--   0 rfitzger (1525561519) 18434217       88 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/entry_points.txt
+-rw-r--r--   0 rfitzger (1525561519) 18434217      254 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/requires.txt
+-rw-r--r--   0 rfitzger (1525561519) 18434217        5 2023-06-09 22:07:09.000000 nrel.hive-1.3.0/nrel.hive.egg-info/top_level.txt
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1897 2023-06-09 22:03:33.000000 nrel.hive-1.3.0/pyproject.toml
+-rw-r--r--   0 rfitzger (1525561519) 18434217       38 2023-06-09 22:07:12.311137 nrel.hive-1.3.0/setup.cfg
+-rw-r--r--   0 rfitzger (1525561519) 18434217       38 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/setup.py
+drwxr-xr-x   0 rfitzger (1525561519) 18434217        0 2023-06-09 22:07:12.304781 nrel.hive-1.3.0/tests/
+-rw-r--r--   0 rfitzger (1525561519) 18434217      140 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/tests/__init__.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3424 2023-04-26 17:39:37.000000 nrel.hive-1.3.0/tests/test_base.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3012 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_bev_mechatronics.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2441 2022-11-29 19:20:11.000000 nrel.hive-1.3.0/tests/test_build_mechatronics_table.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1533 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_cancel_requests.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5347 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_charging_price_update.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2517 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_config_builder.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3005 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_dict_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     6412 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_dict_reader_stepper.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1988 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_driver_instruction_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1541 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/tests/test_fs.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3501 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_h3_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1586 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_haversine_roadnetwork.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     9605 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_human_driver_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2553 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_ice_mechatronics.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1166 2022-11-02 21:45:19.000000 nrel.hive-1.3.0/tests/test_initialize_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5987 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_initialize_simulation.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2946 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_instruction_generator_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5878 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_instruction_generators.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2949 2023-05-01 19:21:39.000000 nrel.hive-1.3.0/tests/test_kepler_feature.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3084 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_local_simulation_runner.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1998 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_osm_roadnetwork.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1604 2023-04-26 17:07:23.000000 nrel.hive-1.3.0/tests/test_powercurve_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3571 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_request.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3262 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_routetraversal.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1437 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_run_cosim.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3729 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_sample_functions.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2520 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_schedules.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    13122 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_simulation_state_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    26049 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_simulationstate.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     8191 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_station.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2231 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_station_load_handler.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1193 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_step_simulation_ops.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     1024 2023-02-23 16:22:51.000000 nrel.hive-1.3.0/tests/test_time.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     5182 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_update_requests.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217      966 2023-06-09 15:12:07.000000 nrel.hive-1.3.0/tests/test_update_requests_sampling.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     2157 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_vehicle.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217    99323 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_vehicle_state.py
+-rw-r--r--   0 rfitzger (1525561519) 18434217     3790 2023-05-24 20:21:36.000000 nrel.hive-1.3.0/tests/test_vehicle_state_ops.py
```

### Comparing `nrel.hive-1.2.2/LICENSE` & `nrel.hive-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/README.md` & `nrel.hive-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+Metadata-Version: 2.1
+Name: nrel.hive
+Version: 1.3.0
+Summary: HIVE is a mobility services research platform developed by the Mobility and Advanced Powertrains (MBAP) group at the National Renewable Energy Laboratory in Golden, Colorado, USA.
+Author: National Renewable Energy Laboratory
+License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
+Project-URL: Homepage, https://github.com/NREL/hive
+Keywords: simulation,transportation,ride-sharing,agent-based
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: dev
+License-File: LICENSE
+
 # <img src="docs/source/images/hive-icon.png" alt="drawing" width="100"/>
 
-**H**ighly  
-**I**ntegrated  
-**V**ehicle  
-**E**cosystem  
+**H**ighly
+**I**ntegrated
+**V**ehicle
+**E**cosystem
 
 HIVE™ is an open-source mobility services research platform developed by the Mobility, Behavior, and Advanced Powertrains (MBAP) group at the National Renewable Energy Laboratory in Golden, Colorado, USA.
 
 HIVE supports researchers who explore **Electric Vehicle (EV) fleet control**, **Electric Vehicle Supply Equipment (EVSE) siting**, and **fleet composition** problems, and is designed for _ease-of-use_, _scalability_, and _co-simulation_.
 Out-of-the-box, it provides a baseline set of algorithms for fleet dispatch, but provides a testbed for exploring alternatives from leading research in model-predictive control (MPC) and deep reinforcement learning.
 HIVE is designed to integrate with vehicle power and energy grid power models in real-time for accurate, high-fidelity energy estimation over arbitrary road networks and demand scenarios.
 
@@ -15,58 +36,64 @@
 
 For technical details about the HIVE platform, please see the [Technical Report](https://www.nrel.gov/docs/fy21osti/80682.pdf).
 
 For more documentation on how to use HIVE, please see the [HIVE documentation](https://nrelhive.readthedocs.io/en/latest/).
 
 ## Installation
 
-HIVE depends on a Python installation [3.7, 3.8, 3.9, 3.10] and the pip package manager ( [python.org](https://www.python.org/downloads/).
-In our installation example we use [conda](https://www.anaconda.com/products/distribution) |  for managing a HIVE Python environment.
+HIVE depends on a Python installation [3.8, 3.9, 3.10, 3.11] and the pip package manager ( [python.org](https://www.python.org/downloads/).
+In our installation example we use [conda](https://www.anaconda.com/products/distribution) | for managing a HIVE Python environment.
 
 ### (optional) set up a virtual environment using conda
 
 We recommend setting up a virtual environment to install HIVE.
+This helps avoiding conflicts with other Python dependencies.
+Conda compared to other virtualenv managers like Poetry or Pipenv can be better at managing projects such as this one that use large dependencies (such as SciPy).
 One way to do this is to use Anaconda:
-    1. Install [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
-    1. Open a terminal or Anaconda Prompt.
-    1. Create a new virtual environment: `conda create --name hive python=3.10`
-    1. Activate the virtual environment `conda activate hive`
+
+1. Install [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+1. Open a terminal or Anaconda Prompt.
+1. Create a new virtual environment with the desired Python version: `conda create --name hive python=3.11`
+1. Activate the virtual environment `conda activate hive`
+1. Continue with the installation instructions below.
+   Now your dependencies will be stored within the new virtual environment.
 
 ### via pip
 
     > pip install nrel.hive
 
 ### build from source
 
 Clone the repository and install the code via pip:
+
     > git clone <https://github.com/NREL/hive.git>
     > cd hive
     > pip install -e .
 
 ## Run HIVE
 
-run a test of hive using a [built-in scenario](#built-in-scenarios):
+run a test of hive using a [built-in scenario](#built-in-scenarios), which are hardcoded:
 
     > hive denver_demo.yaml
 
-if you want the program to use a file outside of this location, provide a valid path:
+if you want the program to use a file that is not built-in, provide a valid path:
 
     > hive some_other_directory/my_scenario.yaml
 
 ## Built-In Scenarios
 
 The following built-in scenario files come out-of-the-box, and available directly by name:
 
-scenario | description
----------|------------
-denver_demo.yaml | default demo scenario with 20 vehicles and 2.5k requests synthesized with uniform time/location sampling
-denver_rl_toy.yaml | extremely simple scenario for testing RL
-denver_demo_constrained_charging.yaml | default scenario with limited charging supply
-denver_demo_fleets.yaml | default scenario with two competing TNC fleets
-manhattan.yaml | larger test scenario with 200 vehicles and 20k requests sampled from the NY Taxi Dataset
+| scenario                              | description                                                                                              |
+| ------------------------------------- | -------------------------------------------------------------------------------------------------------- |
+| denver_demo.yaml                      | default demo scenario with 20 vehicles and 2.5k requests synthesized with uniform time/location sampling |
+| denver_rl_toy.yaml                    | extremely simple scenario for testing RL                                                                 |
+| denver_demo_constrained_charging.yaml | default scenario with limited charging supply                                                            |
+| denver_demo_fleets.yaml               | default scenario with two competing TNC fleets                                                           |
+| manhattan.yaml                        | larger test scenario with 200 vehicles and 20k requests sampled from the NY Taxi Dataset                 |
 
 For more information on how to build your own scenario, please see the [HIVE documentation](https://nrelhive.readthedocs.io/en/latest/inputs.html).
 
 ## Dependencies
 
 HIVE attempts to rely on as few dependencies as possible. For the most part, these dependencies are obvious choices from the open-source Python analysis ecosystem:
 
@@ -96,172 +123,64 @@
 - easy integration/co-simulation (can be called alongside other software tools)
 - dynamic dispatch, trip energy, routing, and economics
 - simple to define/share scenarios via configuration files and simulation snapshots
 - 100% Python (v 3.7) code with a small(ish) set of dependencies and well-documented code
 
 HIVE is _not_ a fully-featured [Activity-Based Model](https://en.wikipedia.org/wiki/Transportation_forecasting#Activity-based_models), does _not_ simulate all vehicles on the network, and does not simulate congestion. It also assumes demand is fixed. If these assumptions are too strong for your research question, then one of the other mesoscopic models capable of ridehail simulation may be a more appropriate fit. The following (opinionated) chart attempts to compare features of HIVE against LBNL's BEAM and ANL's POLARIS models.
 
-| feature                                            | HIVE       | BEAM      | POLARIS |
-| -------------------------------------------------- | ---------- | --------- | ------- |
-| Agent-Based Ridehail Model                         | :honeybee: | :red_car: | :train: |
-| Designed for large-scale inputs                    | :honeybee: | :red_car: | :train: |
-| Integrates with NREL energy models                 | :honeybee: | :red_car: | :train: |
-| Charging infrastructure & charge events            | :honeybee: | :red_car: | :train: |
-| Service pricing and income model                   | :honeybee: | :red_car: | :train: |
-| Data-driven ridehail dispatcher                    | :honeybee: |           |         |
-| Does not require socio-demographic data            | :honeybee: |           |         |
-| Built-in example scenario                          | :honeybee: | :red_car: |         |
-| Written entirely in Python, installed via pip      | :honeybee: |           |         |
-| Activity-Based Demand Model                        |            | :red_car: | :train: |
-| Dynamic demand using behavioral models             |            | :red_car: | :train: |
-| Robust assignment of population demographics       |            | :red_car: | :train: |
-| Supports broad set of travel modes                 |            | :red_car: | :train: |
-| Endogenous traffic congestion modeling             |            | :red_car: | :train: |
+| feature                                       | HIVE       | BEAM      | POLARIS |
+| --------------------------------------------- | ---------- | --------- | ------- |
+| Agent-Based Ridehail Model                    | :honeybee: | :red_car: | :train: |
+| Designed for large-scale inputs               | :honeybee: | :red_car: | :train: |
+| Integrates with NREL energy models            | :honeybee: | :red_car: | :train: |
+| Charging infrastructure & charge events       | :honeybee: | :red_car: | :train: |
+| Service pricing and income model              | :honeybee: | :red_car: | :train: |
+| Data-driven ridehail dispatcher               | :honeybee: |           |         |
+| Does not require socio-demographic data       | :honeybee: |           |         |
+| Built-in example scenario                     | :honeybee: | :red_car: |         |
+| Written entirely in Python, installed via pip | :honeybee: |           |         |
+| Activity-Based Demand Model                   |            | :red_car: | :train: |
+| Dynamic demand using behavioral models        |            | :red_car: | :train: |
+| Robust assignment of population demographics  |            | :red_car: | :train: |
+| Supports broad set of travel modes            |            | :red_car: | :train: |
+| Endogenous traffic congestion modeling        |            | :red_car: | :train: |
 
 ## Looking at a default scenario
 
-![Map of Denver Downtown](docs/source/_static/denver_demo.jpg?raw=true)
+![Manhattan Animation](docs/source/images/manhattan.gif?raw=true)
 
-Running HIVE takes one argument, which is a configuration file. Hive comes packaged with a demo scenario for Downtown Denver, located at `hive/resources/scenarios/denver_demo.yaml`. This file names the inputs and the configuration Parameters for running HIVE.
+Running HIVE takes one argument, which is a configuration file. Hive comes packaged with a demo scenario for Manhattan, located at `hive/resources/scenarios/manhattan/manhattan.yaml`. This file names the inputs and the configuration Parameters for running HIVE.
 
-the Denver demo scenario is configured to log output to a folder named `denver_demo_outputs` which is also tagged with a timestamp. These output files can be parsed by Pandas (for Pandas > 0.19.0):
+One the scenario is finished, the console will indicate where the output files have been written and you can load them using pandas:
 
 ```python
 import pandas as pd
 # log files store JSON rows, like a document store
-output_file = "~/hive/output/denver_demo_2021-02-08_11-00-07/state.log"
+output_file = "manhattan_2021-02-08_11-00-07/state.log"
 pd.read_json(output_file, lines=True)
 ```
 
 By default, these outputs are generated:
 
-file name                        | file type | description
--------------------------------- | --------- | -----------
-\<config\>.yaml                  | YAML      | the input configuration serialized (can be read back by HIVE)
-run.log                          | text      | console log output
-event.log                        | JSON rows | events that occur, such as vehicle movement, pickup + dropoff events, etc
-instruction.log                  | JSON rows | instructions sent from dispatcher to drivers
-state.log                        | JSON rows | entity states at every time step
-station_capacities.csv           | CSV       | energy load capacity for each station
-summary_stats.json               | JSON      | summary stats as displayed in run.log but in JSON format
-time_step_stats_{$FLEET|all}.csv | CSV       | aggregated data across a fleet (or all fleets) by time step
+| file name               | file type | description                                                               |
+| ----------------------- | --------- | ------------------------------------------------------------------------- |
+| \<config\>.yaml         | YAML      | the input configuration serialized (can be read back by HIVE)             |
+| run.log                 | text      | console log output                                                        |
+| event.log               | JSON rows | events that occur, such as vehicle movement, pickup + dropoff events, etc |
+| instruction.log         | JSON rows | instructions sent from dispatcher to drivers                              |
+| state.log               | JSON rows | entity states at every time step                                          |
+| station_capacities.csv  | CSV       | energy load capacity for each station                                     |
+| summary_stats.json      | JSON      | summary stats as displayed in run.log but in JSON format                  |
+| time_step_stats_all.csv | CSV       | aggregated data across a fleet (or all fleets) by time step               |
 
 Running this scenario should also feed some logging into the console.
-First, HIVE announces where it is loading configuration from (1).
-It then dumps the global and scenario configuration to the console (2).
-Finally, after around 65 lines, it begins running the simulation with a progress bar (3).
-After, it prints the summary stats to the console and exits (4).
-
-```console
-INFO
-         ##     ##  ####  ##     ##  #######
-         ##     ##   ##   ##     ##  ##
-         #########   ##   ##     ##  ######
-         ##     ##   ##    ##   ##   ##
-         ##     ##  ####     ###     #######
-
-                         .' '.            __
-                .        .   .           (__\_
-                 .         .         . -{{_(|8)
-                   ' .  . ' ' .  . '     (__/
-
-/Users/nreinick/dev/repos/hive/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml
-INFO     global hive configuration loaded from /Users/nreinick/dev/repos/hive/nrel/hive/resources/defaults/.hive.yaml
-INFO       global_settings_file_path: /Users/nreinick/dev/repos/hive/nrel/hive/resources/defaults/.hive.yaml
-INFO       output_base_directory: .
-INFO       local_parallelism: 1
-INFO       local_parallelism_timeout_sec: 60
-INFO       log_run: True
-INFO       log_events: True
-INFO       log_states: True
-INFO       log_instructions: True
-INFO       log_stats: True
-INFO       log_level: INFO
-INFO       log_sim_config: {<ReportType.INSTRUCTION: 8>, <ReportType.VEHICLE_STATE: 2>, <ReportType.DRIVER_SCHEDULE_EVENT: 13>,
-         <ReportType.DRIVER_STATE: 3>, <ReportType.VEHICLE_CHARGE_EVENT: 9>, <ReportType.CANCEL_REQUEST_EVENT: 7>,
-         <ReportType.DROPOFF_REQUEST_EVENT: 6>, <ReportType.STATION_LOAD_EVENT: 11>, <ReportType.VEHICLE_MOVE_EVENT: 10>,
-         <ReportType.REFUEL_SEARCH_EVENT: 12>, <ReportType.STATION_STATE: 1>, <ReportType.PICKUP_REQUEST_EVENT: 5>,
-         <ReportType.ADD_REQUEST_EVENT: 4>}
-INFO       log_station_capacities: True
-INFO       log_time_step_stats: True
-INFO       log_fleet_time_step_stats: True
-INFO       lazy_file_reading: False
-INFO       wkt_x_y_ordering: True
-INFO     output directory set to /Users/nreinick/dev/repos/hive/nrel/hive/resources/scenarios/denver_downtown
-INFO     hive config loaded from /Users/nreinick/dev/repos/hive/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml
-INFO
-         dispatcher:
-           base_charging_range_km_threshold: 100
-           charging_range_km_soft_threshold: 50
-           charging_range_km_threshold: 20
-           charging_search_type: nearest_shortest_queue
-           default_update_interval_seconds: 600
-           ideal_fastcharge_soc_limit: 0.8
-           idle_time_out_seconds: 1800
-           matching_range_km_threshold: 20
-           max_search_radius_km: 100.0
-           valid_dispatch_states:
-           - Idle
-           - Repositioning
-         input:
-           bases_file: denver_demo_bases.csv
-           charging_price_file: denver_charging_prices_by_geoid.csv
-           demand_forecast_file: denver_demand.csv
-           geofence_file: downtown_denver.geojson
-           mechatronics_file: mechatronics.yaml
-           rate_structure_file: rate_structure.csv
-           requests_file: denver_demo_requests.csv
-           road_network_file: downtown_denver_network.json
-           stations_file: denver_demo_stations.csv
-           vehicles_file: denver_demo_vehicles.csv
-         network:
-           default_speed_kmph: 40.0
-           network_type: osm_network
-         sim:
-           end_time: '1970-01-02T00:00:00'
-           request_cancel_time_seconds: 600
-           schedule_type: time_range
-           sim_h3_resolution: 15
-           sim_h3_search_resolution: 7
-           sim_name: denver_demo
-           start_time: '1970-01-01T00:00:00'
-           timestep_duration_seconds: 60
-
-INFO     creating run log at denver_demo_2022-10-27_16-36-43/run.log with log level INFO
-INFO     running denver_demo for time 1970-01-01T00:00:00 to 1970-01-02T00:00:00:
-100%|██████████████████████████████████████████████████████████████████████████████████████| 1440/1440 [00:09<00:00, 144.72it/s]
-INFO     done! time elapsed: 9.97 seconds
-INFO     96.84 %         Requests Served
-                        Summary Stats
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━┓
-┃ Stat                                         ┃ Value      ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━┩
-│ Mean Final SOC                               │ 51.1%      │
-│ Requests Served                              │ 96.84%     │
-│ Time in State Idle                           │ 28.03%     │
-│ Time in State DispatchBase                   │ 0.07%      │
-│ Time in State DispatchTrip                   │ 20.89%     │
-│ Time in State ChargingBase                   │ 3.62%      │
-│ Time in State ServicingTrip                  │ 27.51%     │
-│ Time in State ReserveBase                    │ 15.3%      │
-│ Time in State DispatchStation                │ 0.29%      │
-│ Time in State ChargingStation                │ 4.3%       │
-│ Time in State Repositioning                  │ 0.0%       │
-│ Total Kilometers Traveled                    │ 8032.26 km │
-│ Kilometers Traveled in State DispatchBase    │ 11.41 km   │
-│ Kilometers Traveled in State DispatchTrip    │ 3304.36 km │
-│ Kilometers Traveled in State ServicingTrip   │ 4665.25 km │
-│ Kilometers Traveled in State DispatchStation │ 50.54 km   │
-│ Kilometers Traveled in State Repositioning   │ 0.69 km    │
-│ Station Revenue                              │ $ 196.72   │
-│ Fleet Revenue                                │ $ 12017.56 │
-└──────────────────────────────────────────────┴────────────┘
-INFO     summary stats written to denver_demo_2022-10-27_16-36-43/summary_stats.json
-INFO     time step stats written to denver_demo_2022-10-27_16-36-43/time_step_stats_all.csv
-```
+First, HIVE announces where it is loading configuration from.
+It then dumps the global and scenario configuration to the console.
+Finally, after around 65 lines, it begins running the simulation with a progress bar.
+After, it prints the summary stats to the console and exits.
 
 ## Roadmap
 
 _Updated October, 2022_
 
 HIVE intends to implement the following features in the near-term:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/__init__.py` & `nrel.hive-1.3.0/nrel/hive/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,21 @@
 mobility as a service (MaaS) applications on 
 infrastructure, levels of service, and additional energy outcomes. Developed in
 2019 at the National Renewable Energy Laboratory (NREL), HIVE is an
 agent-based model that simulates MaaS operations over real world trip data.
 """
 
 import logging
-
 from pathlib import Path
 
-from tqdm import tqdm
-
 from nrel.hive.app import run
 from nrel.hive.config import HiveConfig
 from nrel.hive.dispatcher import *
-from nrel.hive.state.simulation_state.update.update import Update
 from nrel.hive.state.simulation_state.update.step_simulation import StepSimulation
+from nrel.hive.state.simulation_state.update.update import Update
 
 
 def package_root() -> Path:
     return Path(__file__).parent
 
 
 from rich.logging import RichHandler
```

### Comparing `nrel.hive-1.2.2/nrel/hive/app/hive_cosim.py` & `nrel.hive-1.3.0/nrel/hive/app/hive_cosim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import functools as ft
 from pathlib import Path
 from typing import Iterable, Tuple, NamedTuple, Optional, TypeVar
 
-import pandas as pd
-from pandas import DataFrame
 from tqdm import tqdm
+import random
+import numpy
 
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
-from nrel.hive.initialization.load import load_simulation, load_config
 from nrel.hive.initialization.initialize_simulation import InitFunction
+from nrel.hive.initialization.load import load_simulation, load_config
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.reporting.handler.vehicle_charge_events_handler import VehicleChargeEventsHandler
 from nrel.hive.runner import RunnerPayload
-from nrel.hive.util import SimulationStateError
 
 T = TypeVar("T", bound=InstructionGenerator)
 
 
 def load_scenario(
     scenario_file: Path,
     custom_instruction_generators: Optional[Tuple[T, ...]] = None,
@@ -26,14 +25,19 @@
     """
     load a HIVE scenario from file and return the initial simulation state
     :param scenario_file: the HIVE scenario file to read
     :return: the initial simulation state payload
     :raises: Error when issues with files
     """
     config = load_config(scenario_file, output_suffix)
+
+    if config.sim.seed is not None:
+        random.seed(config.sim.seed)
+        numpy.random.seed(config.sim.seed)
+
     initial_payload = load_simulation(config, custom_instruction_generators, custom_init_functions)
 
     # add a specialized Reporter handler that catches vehicle charge events
     initial_payload.e.reporter.add_handler(VehicleChargeEventsHandler())
 
     return initial_payload
```

### Comparing `nrel.hive-1.2.2/nrel/hive/app/run.py` & `nrel.hive-1.3.0/nrel/hive/app/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import logging
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Optional, Tuple, TypeVar, Union
 
 import pkg_resources
 import yaml
+import random
+import numpy
 
-from nrel.hive.initialization.load import load_simulation, load_config
-from nrel.hive.initialization.initialize_simulation import InitFunction
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
+from nrel.hive.initialization.initialize_simulation import InitFunction
+from nrel.hive.initialization.load import load_simulation, load_config
 from nrel.hive.runner.local_simulation_runner import LocalSimulationRunner
 
 if TYPE_CHECKING:
     pass
 
 parser = argparse.ArgumentParser(description="run hive")
 parser.add_argument(
@@ -48,14 +50,18 @@
 
     :return: 0 for success
     """
     _welcome_to_hive()
 
     config = load_config(scenario_file)
 
+    if config.sim.seed is not None:
+        random.seed(config.sim.seed)
+        numpy.random.seed(config.sim.seed)
+
     initial_payload = load_simulation(
         config,
         custom_instruction_generators=custom_instruction_generators,
         custom_init_functions=custom_init_functions,
     )
 
     log.info(
```

### Comparing `nrel.hive-1.2.2/nrel/hive/app/run_batch.py` & `nrel.hive-1.3.0/nrel/hive/app/run_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import traceback
 from multiprocessing import Pool
 from pathlib import Path
 from typing import TYPE_CHECKING, NamedTuple, List
 
 import yaml
 
-from nrel.hive.initialization.load import load_config
 from nrel.hive.app.run import run_sim
 from nrel.hive.util import fs
 
 if TYPE_CHECKING:
     pass
 
 parser = argparse.ArgumentParser(description="run hive")
```

### Comparing `nrel.hive-1.2.2/nrel/hive/config/config_builder.py` & `nrel.hive-1.3.0/nrel/hive/config/config_builder.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/config/dispatcher_config.py` & `nrel.hive-1.3.0/nrel/hive/config/dispatcher_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import NamedTuple, Dict, Union, Tuple, Optional
+from typing import NamedTuple, Dict, Tuple, Optional
 
 from nrel.hive.config.config_builder import ConfigBuilder
 from nrel.hive.dispatcher.instruction_generator.charging_search_type import ChargingSearchType
 from nrel.hive.util.units import Ratio, Seconds, Kilometers
 
 
 class DispatcherConfig(NamedTuple):
```

### Comparing `nrel.hive-1.2.2/nrel/hive/config/global_config.py` & `nrel.hive-1.3.0/nrel/hive/config/global_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     output_base_directory: str
     local_parallelism: int
     local_parallelism_timeout_sec: int
     log_run: bool
     log_events: bool
     log_states: bool
     log_instructions: bool
+    log_kepler: bool
     log_stats: bool
     log_level: str
     log_sim_config: Set[ReportType]
     log_station_capacities: bool
     log_time_step_stats: bool
     log_fleet_time_step_stats: bool
     lazy_file_reading: bool
@@ -36,14 +37,15 @@
             "output_base_directory",
             "local_parallelism",
             "local_parallelism_timeout_sec",
             "log_run",
             "log_states",
             "log_events",
             "log_instructions",
+            "log_kepler",
             "log_stats",
             "log_level",
             "log_sim_config",
             "log_time_step_stats",
             "log_fleet_time_step_stats",
             "lazy_file_reading",
             "wkt_x_y_ordering",
```

### Comparing `nrel.hive-1.2.2/nrel/hive/config/hive_config.py` & `nrel.hive-1.3.0/nrel/hive/config/hive_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import hashlib
 import logging
 import os
 from datetime import datetime
 from pathlib import Path
-from typing import NamedTuple, Dict, Union, Tuple, Optional
+from typing import NamedTuple, Dict, Union, Optional
 
 import pkg_resources
 import yaml
 
 from nrel.hive.config.config_builder import ConfigBuilder
 from nrel.hive.config.dispatcher_config import DispatcherConfig
 from nrel.hive.config.global_config import GlobalConfig
@@ -38,15 +38,15 @@
         output_suffix: Optional[str] = None,
     ) -> Union[Exception, HiveConfig]:
         """
         builds a hive config by reading from a scenario file. optionally append additional key/value
         pairs and modify the datetime convention for naming output directories.
         :param scenario_file_path: path to the file to load as a HiveConfig
         :param config: optional overrides to the default config values (Default: None)
-        :param output_suffix: directory name suffix to append to sim_name (by default, timestamp for now)
+        :param output_suffix: directory name suffix to append to sim_name (by default, timestamp)
         :return: a hive config or an error
         """
         return ConfigBuilder.build(
             default_config={},
             required_config=(),
             config_constructor=lambda c: HiveConfig.from_dict(c, scenario_file_path, output_suffix),
             config=config,
@@ -55,20 +55,14 @@
     @classmethod
     def from_dict(
         cls, d: Dict, scenario_file_path: Path, output_suffix: Optional[str]
     ) -> HiveConfig:
         # collect the global hive configuration
         global_config = fs.global_hive_config_search()
 
-        # i wish to make these comprehensive print-outs DEBUG-only, but, i am totally perplexed by Python Logging's
-        # behavior for setting log level
-        # https://stackoverflow.com/questions/43109355/logging-setlevel-is-being-ignored
-        # https://stackoverflow.com/questions/44312978/python-logger-is-not-printing-debug-messages-although-it-is-set-correctly
-
-        # logging.basicConfig(level=global_config.log_level)
         root_logger = logging.getLogger("")
         root_logger.setLevel(global_config.log_level)
 
         if global_config.verbose:
             log.info(
                 f"global hive configuration loaded from {global_config.global_settings_file_path}"
             )
@@ -86,15 +80,14 @@
 
             # append input_config file to default configuration with overwrite
             conf["input"].update(d["input"])
             conf["sim"].update(d["sim"])
             conf["network"].update(d["network"])
             conf["dispatcher"].update(d["dispatcher"])
 
-            # is this still possible now with the default config loading from nrel.hive.resources.defaults?
             warn_missing_config_keys = ["input", "sim", "network"]
             for key in warn_missing_config_keys:
                 if key not in conf:
                     log.warning(f"scenario file is missing a '{key}' section may cause errors")
 
             sconfig = Sim.build(conf.get("sim"))
             iconfig = Input.build(conf.get("input"), scenario_file_path, conf.get("cache"))
@@ -156,14 +149,15 @@
         return self._replace(scenario_output_directory=output_directory)
 
     def suppress_logging(self) -> HiveConfig:
         updated_gconfig = self.global_config._replace(
             log_run=False,
             log_states=False,
             log_events=False,
+            log_kepler=False,
             log_stats=False,
             log_station_capacities=False,
             log_instructions=False,
             log_time_step_stats=False,
             log_fleet_time_step_stats=False,
         )
         return self._replace(global_config=updated_gconfig)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/config/input.py` & `nrel.hive-1.3.0/nrel/hive/config/input.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import hashlib
 import logging
 from pathlib import Path
-from typing import NamedTuple, Tuple, Dict, Optional, Union
+from typing import NamedTuple, Tuple, Dict, Optional
 
 from nrel.hive.config.config_builder import ConfigBuilder
 from nrel.hive.util import fs
 
 log = logging.getLogger(__name__)
 
 
@@ -21,15 +21,14 @@
     mechatronics_file: str
     chargers_file: str
     schedules_file: Optional[str] = None
     road_network_file: Optional[str] = None
     geofence_file: Optional[str] = None
     rate_structure_file: Optional[str] = None
     charging_price_file: Optional[str] = None
-    demand_forecast_file: Optional[str] = None
     fleets_file: Optional[str] = None
 
     @classmethod
     def default_config(cls) -> Dict:
         return {}
 
     @classmethod
@@ -104,23 +103,14 @@
         charging_price_file = (
             fs.construct_scenario_asset_path(
                 d["charging_price_file"], scenario_directory, "charging_prices"
             )
             if d.get("charging_price_file")
             else None
         )
-        demand_forecast_file = (
-            fs.construct_scenario_asset_path(
-                d["demand_forecast_file"],
-                scenario_directory,
-                "demand_forecast",
-            )
-            if d.get("demand_forecast_file")
-            else None
-        )
         fleets_file = (
             fs.construct_scenario_asset_path(d["fleets_file"], scenario_directory, "fleets")
             if d.get("fleets_file")
             else None
         )
 
         input_config = {
@@ -133,15 +123,14 @@
             "schedules_file": schedules_file,
             "chargers_file": chargers_file,
             "mechatronics_file": mechatronics_file,
             "road_network_file": road_network_file,
             "geofence_file": geofence_file,
             "rate_structure_file": rate_structure_file,
             "charging_price_file": charging_price_file,
-            "demand_forecast_file": demand_forecast_file,
             "fleets_file": fleets_file,
         }
 
         # if cache provided, check the file has a correct md5 hash value
         if cache:
             for (
                 name,
@@ -160,15 +149,14 @@
             schedules_file=schedules_file,
             chargers_file=chargers_file,
             mechatronics_file=mechatronics_file,
             road_network_file=road_network_file,
             geofence_file=geofence_file,
             rate_structure_file=rate_structure_file,
             charging_price_file=charging_price_file,
-            demand_forecast_file=demand_forecast_file,
             fleets_file=fleets_file,
         )
 
     @staticmethod
     def _check_md5_checksum(filepath: str, existing_md5_sum: str):
         with open(filepath, "rb") as f:
             data = f.read()
```

### Comparing `nrel.hive-1.2.2/nrel/hive/config/network.py` & `nrel.hive-1.3.0/nrel/hive/config/network.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/config/sim.py` & `nrel.hive-1.3.0/nrel/hive/config/sim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
-from typing import NamedTuple, Dict, Optional, Union, Tuple
+from typing import NamedTuple, Dict, Optional, Tuple
 
 from nrel.hive.config.config_builder import ConfigBuilder
-from nrel.hive.model.vehicle.schedules.schedule_type import ScheduleType
 from nrel.hive.model.sim_time import SimTime
+from nrel.hive.model.vehicle.schedules.schedule_type import ScheduleType
 from nrel.hive.util.units import Seconds
+from nrel.hive.util import Ratio
 
 
 class Sim(NamedTuple):
     sim_name: str
     timestep_duration_seconds: Seconds
     start_time: SimTime
     end_time: SimTime
     sim_h3_resolution: int
     sim_h3_search_resolution: int
     request_cancel_time_seconds: int
     schedule_type: ScheduleType
+    min_delta_energy_change: Ratio = 0.0001
+    seed: Optional[int] = 0
 
     @classmethod
     def default_config(cls) -> Dict:
         return {}
 
     @classmethod
     def required_config(cls) -> Tuple[str, ...]:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/basic_forecaster.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/basic_forecaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Tuple, NamedTuple, TYPE_CHECKING
+from typing import Tuple, TYPE_CHECKING
 
-from nrel.hive.model.sim_time import SimTime
 from nrel.hive.dispatcher.forecaster.forecast import Forecast, ForecastType
 from nrel.hive.dispatcher.forecaster.forecaster_interface import ForecasterInterface
+from nrel.hive.model.sim_time import SimTime
 from nrel.hive.util.iterators import DictReaderStepper
 
 if TYPE_CHECKING:
     from hive.state.simulation_state.simulation_state import SimulationState
 
 
 @dataclass(frozen=True)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/forecaster/forecaster_interface.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/forecaster/forecaster_interface.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instruction.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instruction.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instruction_ops.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instruction_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-from typing import Tuple, Optional, FrozenSet, TYPE_CHECKING
 import functools as ft
-
 import logging
+from typing import Tuple, Optional, FrozenSet, TYPE_CHECKING
 
 from nrel.hive.model.vehicle.trip_phase import TripPhase
 from nrel.hive.model.vehicle.vehicle import RequestId
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.state.vehicle_state.servicing_pooling_trip import ServicingPoolingTrip
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction/instructions.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction/instructions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
+from dataclasses import dataclass
 from typing import Optional, TYPE_CHECKING, Tuple
 
 from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.dispatcher.instruction.instruction_ops import (
     trip_plan_ordering_is_valid,
     trip_plan_all_requests_allow_pooling,
     trip_plan_covers_previous,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/assignment_ops.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/assignment_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import functools as ft
+import logging
 from typing import Dict, Tuple, Callable, NamedTuple, Optional, TYPE_CHECKING
 
-import logging
 import h3
 import numpy as np
 from scipy.optimize import linear_sum_assignment
 
 from nrel.hive.model.roadnetwork.route import (
     route_distance_km,
     route_travel_time_seconds,
@@ -282,34 +282,40 @@
         def _time_to_full_by_charger_id(c: ChargerId):
             def _time_to_full(v: Vehicle) -> Seconds:
                 _mech = env.mechatronics.get(v.mechatronics_id)
                 _charger = env.chargers.get(c)
                 if not _mech or not _charger:
                     return 0
                 else:
+                    max_iter = (
+                        int(env.config.sim.end_time - sim.sim_time)
+                        / sim.sim_timestep_duration_seconds
+                    )
                     time_est = powercurve_ops.time_to_full(
                         v,
                         _mech,
                         _charger,
                         target_soc,
                         sim.sim_timestep_duration_seconds,
+                        min_delta_energy_change=env.config.sim.min_delta_energy_change,
+                        max_iterations=int(max_iter),
                     )
                     return time_est
 
             return _time_to_full
 
-        def _sort_enqueue_time(v: Vehicle) -> int:
+        def _sort_enqueue_time(v: Vehicle) -> Tuple[int, str]:
             if isinstance(v.vehicle_state, ChargeQueueing):
                 enqueue_time = int(v.vehicle_state.enqueue_time)
             else:
                 log.error(
                     "calling _sort_enqueue_time on a vehicle state that is not ChargeQueueing"
                 )
                 enqueue_time = 0
-            return enqueue_time
+            return (enqueue_time, v.id)
 
         def _greedy_assignment(
             _charging: Tuple[Seconds, ...],
             _enqueued: Tuple[Seconds, ...],
             _charger_id: ChargerId,
             time_passed: Seconds = 0,
         ) -> Seconds:
@@ -364,34 +370,38 @@
                         time_passed=updated_time_passed,
                     )
 
         # collect all vehicles that are either charging or enqueued at this station
         vehicles_at_station = sim.get_vehicles(filter_function=_veh_at_station)
         vehicles_enqueued = sim.get_vehicles(
             filter_function=_veh_enqueued,
-            sort=True,
             sort_key=_sort_enqueue_time,
         )
 
         estimates: Dict[ChargerId, int] = {}
-        for charger_id in station.state.keys():
+        for charger_id in sorted(station.state.keys()):
             charger_state = station.state.get(charger_id)
             charger = charger_state.charger if charger_state is not None else None
 
             if charger is None or not vehicle_mechatronics.valid_charger(charger):
                 # vehicle can't use this charger so we skip it
                 continue
 
             # compute the charge time for the vehicle we are ranking
+            max_iter = (
+                int(env.config.sim.end_time - sim.sim_time) / sim.sim_timestep_duration_seconds
+            )
             this_vehicle_charge_time = powercurve_ops.time_to_full(
                 vehicle,
                 vehicle_mechatronics,
                 charger,
                 target_soc,
                 sim.sim_timestep_duration_seconds,
+                min_delta_energy_change=env.config.sim.min_delta_energy_change,
+                max_iterations=int(max_iter),
             )
 
             def _using_charger(charging_vehicle: Vehicle) -> bool:
                 if isinstance(charging_vehicle.vehicle_state, ChargingStation):
                     if charging_vehicle.vehicle_state.charger_id == charger_id:
                         return True
                 return False
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/charging_fleet_manager.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/charging_fleet_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
+from dataclasses import dataclass
 from typing import Tuple, TYPE_CHECKING
 
 from nrel.hive.reporting import instruction_generator_event_ops
 from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.repositioning import Repositioning
 
 if TYPE_CHECKING:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/charging_search_type.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/charging_search_type.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/dispatcher.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
-import logging
 import functools as ft
+import logging
+from dataclasses import dataclass
 from typing import Tuple, TYPE_CHECKING, Optional
 
 from nrel.hive.dispatcher.instruction_generator import assignment_ops
 from nrel.hive.state.vehicle_state.charging_base import ChargingBase
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
@@ -92,17 +92,15 @@
 
             # collect the vehicles and requests for the assignment algorithm
             available_vehicles = simulation_state.get_vehicles(
                 filter_function=_is_valid_for_dispatch,
             )
 
             unassigned_requests = simulation_state.get_requests(
-                sort=True,
-                sort_key=lambda r: r.value,
-                sort_reversed=True,
+                sort_key=lambda r: -r.value,
                 filter_function=_valid_request,
             )
 
             # select assignment of vehicles to requests
             solution = assignment_ops.find_assignment(
                 available_vehicles,
                 unassigned_requests,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/instruction_generator.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/instruction_generator.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/dispatcher/instruction_generator/instruction_generator_ops.py` & `nrel.hive-1.3.0/nrel/hive/dispatcher/instruction_generator/instruction_generator_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 
 import immutables
 
 from nrel.hive.dispatcher.instruction.instructions import *
 from nrel.hive.dispatcher.instruction_generator import assignment_ops
 from nrel.hive.dispatcher.instruction_generator.charging_search_type import ChargingSearchType
 from nrel.hive.model.station.station import Station
-from nrel.hive.util.h3_ops import H3Ops
 from nrel.hive.util.dict_ops import DictOps
+from nrel.hive.util.h3_ops import H3Ops
 from nrel.hive.util.units import Kilometers
 
 log = logging.getLogger(__name__)
 
-random.seed(123)
-
 if TYPE_CHECKING:
     from nrel.hive.model.vehicle.vehicle import Vehicle
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.dispatcher.instruction_generator.instruction_generator import (
         InstructionGenerator,
     )
     from nrel.hive.util.typealiases import GeoId
@@ -81,15 +79,15 @@
                 v.driver_state.generate_instruction(
                     simulation_state,
                     environment,
                     self.instruction_stack.get(v.id),
                 ),
             )
             + acc,
-            simulation_state.vehicles.values(),
+            simulation_state.get_vehicles(),
             (),
         )
 
         updated_instruction_stack = ft.reduce(
             lambda acc, i: DictOps.add_to_stack_dict(acc, i.vehicle_id, i) if i else acc,
             new_instructions,
             self.instruction_stack,
@@ -309,15 +307,15 @@
             sim=simulation_state,
             env=environment,
             target_soc=target_soc,
         )
 
     nearest_station = H3Ops.nearest_entity(
         geoid=geoid,
-        entities=simulation_state.stations.values(),
+        entities=simulation_state.get_stations(),
         entity_search=simulation_state.s_search,
         sim_h3_search_resolution=simulation_state.sim_h3_search_resolution,
         max_search_distance_km=max_search_radius_km,
         is_valid=valid_station_for_vehicle(vehicle, environment),
         distance_function=distance_fn,
     )
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/initialize_ops.py` & `nrel.hive-1.3.0/nrel/hive/initialization/initialize_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
-import yaml
-import immutables
 from typing import TYPE_CHECKING, FrozenSet
 
+import immutables
+import yaml
+
 if TYPE_CHECKING:
     from nrel.hive.util.typealiases import EntityId, MembershipMap
 
 
 def process_fleet_file(fleet_file: str, entity_type: str) -> MembershipMap:
     """
     creates an immutable map that contains all of the fleet ids associated with the appropriate entity ids
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/initialize_simulation.py` & `nrel.hive-1.3.0/nrel/hive/initialization/initialize_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 import csv
 import functools as ft
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable, Iterable, Optional, Tuple, Dict
 
 import immutables
@@ -11,37 +12,37 @@
 from nrel.hive.config import HiveConfig
 from nrel.hive.initialization.initialize_ops import (
     process_fleet_file,
     read_fleet_ids_from_file,
 )
 from nrel.hive.model.base import Base
 from nrel.hive.model.energy.charger import build_chargers_table
+from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
+from nrel.hive.model.station.station import Station
+from nrel.hive.model.vehicle.mechatronics import build_mechatronics_table
+from nrel.hive.model.vehicle.schedules import build_schedules_table
+from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.handler.eventful_handler import EventfulHandler
 from nrel.hive.reporting.handler.instruction_handler import InstructionHandler
+from nrel.hive.reporting.handler.kepler_handler import KeplerHandler
 from nrel.hive.reporting.handler.stateful_handler import StatefulHandler
 from nrel.hive.reporting.handler.stats_handler import StatsHandler
 from nrel.hive.reporting.handler.time_step_stats_handler import TimeStepStatsHandler
 from nrel.hive.reporting.reporter import Reporter
-from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
-from nrel.hive.model.station.station import Station
-from nrel.hive.model.vehicle.mechatronics import build_mechatronics_table
-from nrel.hive.model.vehicle.schedules import build_schedules_table
-from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.util.dict_ops import DictOps
 
 if TYPE_CHECKING:
     from nrel.hive.util.typealiases import ScheduleId
     from nrel.hive.model.vehicle.schedules import ScheduleFunction
 
 log = logging.getLogger(__name__)
 
-
 # All initialization functions must adhere to the following type signature.
 # These functions are called to initialize the simulation state and the environment
 # and are abstracted such that an external init function can be added to enable custom
 # initialization.
 InitFunction = Callable[
     [HiveConfig, SimulationState, Environment], Tuple[SimulationState, Environment]
 ]
@@ -194,14 +195,16 @@
         reporter.add_handler(
             StatefulHandler(config.global_config, config.scenario_output_directory)
         )
     if config.global_config.log_instructions:
         reporter.add_handler(
             InstructionHandler(config.global_config, config.scenario_output_directory)
         )
+    if config.global_config.log_kepler:
+        reporter.add_handler(KeplerHandler(config.scenario_output_directory))
     if config.global_config.log_stats:
         reporter.add_handler(StatsHandler())
     if config.global_config.log_time_step_stats or config.global_config.log_fleet_time_step_stats:
         reporter.add_handler(
             TimeStepStatsHandler(config, config.scenario_output_directory, environment.fleet_ids)
         )
 
@@ -223,35 +226,58 @@
         vehicle_init_function,
         station_init_function,
         base_init_function,
     ]
 
 
 def osm_init_function(
-    config: HiveConfig, simulation_state: SimulationState, environment: Environment
+    config: HiveConfig,
+    simulation_state: SimulationState,
+    environment: Environment,
+    cache_dir=Path.home(),
 ) -> Tuple[SimulationState, Environment]:
     """
     Initialize an OSMRoadNetwork and add to the simulation
 
     :param config: the hive config
     :param simulation_state: the partially-constructed simulation state
     :param environment: the partially-constructed environment
 
     :return: the SimulationState with the OSMRoadNetwork in it
 
     :raises Exception: from IOErrors parsing the road network
     """
-    if config.input_config.road_network_file is None:
-        raise IOError("Must supply a road network file when using the osm_network")
 
-    road_network = OSMRoadNetwork.from_file(
-        sim_h3_resolution=config.sim.sim_h3_resolution,
-        road_network_file=Path(config.input_config.road_network_file),
-        default_speed_kmph=config.network.default_speed_kmph,
-    )
+    if config.input_config.road_network_file:
+        road_network = OSMRoadNetwork.from_file(
+            sim_h3_resolution=config.sim.sim_h3_resolution,
+            road_network_file=config.input_config.road_network_file,
+            default_speed_kmph=config.network.default_speed_kmph,
+        )
+    elif config.input_config.geofence_file:
+        try:
+            import geopandas
+        except ImportError as e:
+            raise ImportError(
+                "Must have geopandas installed if you want to load from geofence file"
+            ) from e
+
+        dataframe = geopandas.read_file(config.input_config.geofence_file)
+        polygon_union = dataframe["geometry"].unary_union
+
+        road_network = OSMRoadNetwork.from_polygon(
+            sim_h3_resolution=config.sim.sim_h3_resolution,
+            default_speed_kmph=config.network.default_speed_kmph,
+            polygon=polygon_union,
+            cache_dir=cache_dir,
+        )
+    else:
+        raise IOError(
+            "Must supply either a road network or geofence file when using the osm_network"
+        )
 
     sim_w_osm = simulation_state._replace(road_network=road_network)
 
     return sim_w_osm, environment
 
 
 def vehicle_init_function(
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/initialize_simulation_with_sampling.py` & `nrel.hive-1.3.0/nrel/hive/initialization/initialize_simulation_with_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 from nrel.hive.initialization.sample_vehicles import (
     sample_vehicles,
     build_default_location_sampling_fn,
     build_default_soc_sampling_fn,
 )
 from nrel.hive.model.base import Base
 from nrel.hive.model.energy.charger import build_chargers_table
-from nrel.hive.model.roadnetwork.link import Link
-from nrel.hive.model.roadnetwork.geofence import GeoFence
 from nrel.hive.model.roadnetwork.haversine_roadnetwork import HaversineRoadNetwork
+from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
 from nrel.hive.model.station.station import Station
 from nrel.hive.model.vehicle.mechatronics import build_mechatronics_table
 from nrel.hive.model.vehicle.schedules import build_schedules_table, ScheduleId, ScheduleFunction
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
@@ -183,12 +182,11 @@
     with open(stations_file, "r", encoding="utf-8-sig") as bf:
         reader = csv.DictReader(bf)
         stations_builder: immutables.Map[str, Station] = ft.reduce(
             _add_row_unsafe, reader, immutables.Map()
         )
 
     # add all stations to the simulation once we know they are complete
-    sim_with_stations = simulation_state_ops.add_entities(
-        simulation_state, stations_builder.values()
-    )
+    stations = DictOps.iterate_vals(stations_builder)
+    sim_with_stations = simulation_state_ops.add_entities(simulation_state, stations)
 
     return sim_with_stations
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/load.py` & `nrel.hive-1.3.0/nrel/hive/initialization/load.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 import os
 from pathlib import Path
 from typing import Iterable, Optional, Tuple, TypeVar, Union
 
 import yaml
 
 from nrel.hive.config import HiveConfig
-from nrel.hive.reporting import reporter_ops
+from nrel.hive.dispatcher.instruction_generator.charging_fleet_manager import ChargingFleetManager
+from nrel.hive.dispatcher.instruction_generator.dispatcher import Dispatcher
+from nrel.hive.dispatcher.instruction_generator.instruction_function import (
+    instruction_generator_from_function,
+    InstructionFunction,
+)
+from nrel.hive.dispatcher.instruction_generator.instruction_generator import (
+    InstructionGenerator,
+)
 from nrel.hive.initialization.initialize_simulation import (
     default_init_functions,
     osm_init_function,
     initialize,
     InitFunction,
 )
-from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
-from nrel.hive.util.fp import throw_on_failure
+from nrel.hive.reporting import reporter_ops
 from nrel.hive.runner.runner_payload import RunnerPayload
 from nrel.hive.state.simulation_state.update.update import Update
-from nrel.hive.dispatcher.instruction_generator.charging_fleet_manager import ChargingFleetManager
-from nrel.hive.dispatcher.instruction_generator.dispatcher import Dispatcher
 from nrel.hive.util import fs
-
+from nrel.hive.util.fp import throw_on_failure
 
 log = logging.getLogger(__name__)
 
-T = TypeVar("T", bound=InstructionGenerator)
+T = TypeVar("T", bound=Union[InstructionGenerator, InstructionFunction])
 
 
 def load_config(scenario_file: Union[Path, str], output_suffix: Optional[str] = None) -> HiveConfig:
     try:
         scenario_file_path = fs.find_scenario(str(scenario_file))
     except FileNotFoundError as fe:
         raise FileNotFoundError(
@@ -92,10 +97,17 @@
     if custom_instruction_generators is None:
         instruction_generators = (
             Dispatcher(env.config.dispatcher),
             ChargingFleetManager(env.config.dispatcher),
         )
         update = Update.build(env.config, instruction_generators)
     else:
-        update = Update.build(env.config, custom_instruction_generators)
+        # map all instruction functions to generators
+        mapped_instruction_generators = tuple(
+            map(
+                lambda ig_or_if: instruction_generator_from_function(ig_or_if),
+                custom_instruction_generators,
+            )
+        )
+        update = Update.build(env.config, mapped_instruction_generators)
 
     return RunnerPayload(sim, env, update)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/sample_requests.py` & `nrel.hive-1.3.0/nrel/hive/initialization/sample_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 from typing import Tuple, List
 
 from nrel.hive.model.request import Request
+from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.runner import Environment
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
-from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
 
 
 def default_request_sampler(
     count: int,
     simulation_state: SimulationState,
     environment: Environment,
     allow_pooling: bool = False,
@@ -63,10 +63,10 @@
             allows_pooling=allow_pooling,
         )
 
         requests.append(request)
 
         id_counter += 1
 
-    sorted_reqeusts = sorted(requests, key=lambda r: r.departure_time)
+    sorted_reqeusts = sorted(requests, key=lambda r: (r.departure_time, r.id))
 
     return tuple(sorted_reqeusts)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/initialization/sample_vehicles.py` & `nrel.hive-1.3.0/nrel/hive/initialization/sample_vehicles.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import random
 from typing import Callable
 
 from returns.result import Result, Failure, Success
 
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.membership import Membership
 from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
 from nrel.hive.model.vehicle.vehicle import Vehicle
-from nrel.hive.model.membership import Membership
 from nrel.hive.runner import Environment
 from nrel.hive.state.driver_state.autonomous_driver_state.autonomous_available import (
     AutonomousAvailable,
 )
 from nrel.hive.state.driver_state.autonomous_driver_state.autonomous_driver_attributes import (
     AutonomousDriverAttributes,
 )
@@ -71,22 +71,26 @@
                 """
                 if not mechatronics:
                     return Failure(KeyError(f"mechatronics with id {mechatronics_id} not found"))
                 try:
                     vehicle_id = f"v{i}"
                     initial_soc = soc_sampling_function()
                     energy = mechatronics.initial_energy(initial_soc)
+                    energy_expended = mechatronics.initial_energy(0)
+                    energy_gained = mechatronics.initial_energy(0)
                     link = location_sampling_function(s)
                     position = EntityPosition(link.link_id, link.start)
                     vehicle_state = Idle.build(vehicle_id)
                     driver_state = AutonomousAvailable(AutonomousDriverAttributes(vehicle_id))
                     vehicle = Vehicle(
                         id=vehicle_id,
                         mechatronics_id=mechatronics_id,
                         energy=energy,
+                        energy_expended=energy_expended,
+                        energy_gained=energy_gained,
                         position=position,
                         vehicle_state=vehicle_state,
                         driver_state=driver_state,
                         total_seats=total_seats,
                         membership=Membership(),
                     )
                     add_result = add_vehicle_safe(s, vehicle)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/base.py` & `nrel.hive-1.3.0/nrel/hive/model/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-from typing import Optional, Dict, TYPE_CHECKING
 from dataclasses import dataclass, replace
+from typing import Optional, Dict, Tuple, TYPE_CHECKING
 
 import h3
 
 from nrel.hive.model.entity import Entity
 from nrel.hive.model.entity_position import EntityPosition
 from nrel.hive.model.membership import Membership
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.util.exception import SimulationStateError
 
 if TYPE_CHECKING:
-    from nrel.hive.util.typealiases import *
+    from nrel.hive.util.typealiases import BaseId, GeoId, MembershipId, StationId
 
 
 @dataclass(frozen=True)
 class Base(Entity):
     """
     Represents a base within the simulation.
 
@@ -96,32 +96,33 @@
         else:
             base_id = row["base_id"]
             try:
                 lat, lon = float(row["lat"]), float(row["lon"])
                 geoid = h3.geo_to_h3(lat, lon, road_network.sim_h3_resolution)
                 stall_count = int(row["stall_count"])
 
-                # allow user to leave station_id blank or use the word "none" to signify no station at base
+                # allow user to leave station_id blank or use the word "none" to signify
+                # no station at base
                 station_id_name = row["station_id"] if len(row["station_id"]) > 0 else "none"
                 station_id = None if station_id_name.lower() == "none" else station_id_name
 
-                # TODO: think about how to assing vehicles to bases based on fleet membership
+                # TODO: think about how to assign vehicles to bases based on fleet membership
 
                 return Base.build(
                     id=base_id,
                     geoid=geoid,
                     road_network=road_network,
                     station_id=station_id,
                     stall_count=stall_count,
                 )
 
-            except ValueError:
+            except ValueError as e:
                 raise IOError(
-                    f"unable to parse request {base_id} from row due to invalid value(s): {row}"
-                )
+                    f"unable to parse id {base_id} from row due to invalid value(s): {row}"
+                ) from e
 
     def has_available_stall(self, membership: Membership) -> bool:
         """
         Does base have a stall or not.
 
         :return: Boolean
         """
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/energy/charger/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/energy/charger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from csv import DictReader
 from pathlib import Path
-from typing import Dict
 
 from immutables import Map
 
 from nrel.hive.model.energy.charger.charger import Charger
 from nrel.hive.model.energy.energytype import EnergyType
 from nrel.hive.util.typealiases import ChargerId
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/energy/energytype.py` & `nrel.hive-1.3.0/nrel/hive/model/energy/energytype.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/entity.py` & `nrel.hive-1.3.0/nrel/hive/model/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
 from typing import Tuple
 
-
 from nrel.hive.model.entity_position import EntityPosition
 from nrel.hive.model.membership import Membership
 from nrel.hive.util.typealiases import MembershipId
 
 
 @dataclass(frozen=True)
 class EntityMixin:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/membership.py` & `nrel.hive-1.3.0/nrel/hive/model/membership.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/passenger.py` & `nrel.hive-1.3.0/nrel/hive/model/passenger.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import functools as ft
-from typing import Optional, TYPE_CHECKING
 from dataclasses import dataclass, replace
+from typing import Optional, TYPE_CHECKING
 
 from nrel.hive.model.membership import Membership
 from nrel.hive.model.sim_time import SimTime
 
 if TYPE_CHECKING:
     from nrel.hive.util.typealiases import *
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/request/request.py` & `nrel.hive-1.3.0/nrel/hive/model/request/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-from typing import NamedTuple, Optional, Dict, TYPE_CHECKING
 from dataclasses import dataclass, replace
+from typing import Optional, Dict, TYPE_CHECKING
 
 import h3
 
 from nrel.hive.model.entity import Entity
+from nrel.hive.model.entity_position import EntityPosition
 from nrel.hive.model.membership import Membership
 from nrel.hive.model.passenger import Passenger, create_passenger_id
-from nrel.hive.model.entity_position import EntityPosition
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.util.exception import TimeParseError
 from nrel.hive.util.units import Currency, KM_TO_MILE
 
 if TYPE_CHECKING:
     from nrel.hive.model.request import RequestRateStructure
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/request/request_rate_structure.py` & `nrel.hive-1.3.0/nrel/hive/model/request/request_rate_structure.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/geofence.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/geofence.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/haversine_link_id_ops.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/haversine_link_id_ops.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/haversine_roadnetwork.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/haversine_roadnetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-from typing import Tuple, Optional
+from typing import Optional
 
-from nrel.hive.model.roadnetwork.geofence import GeoFence
+import nrel.hive.model.roadnetwork.haversine_link_id_ops as h_ops
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.roadnetwork.geofence import GeoFence
 from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.linktraversal import LinkTraversal
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.model.roadnetwork.route import Route, empty_route
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.util.h3_ops import H3Ops
 from nrel.hive.util.typealiases import GeoId, LinkId, H3Resolution
 from nrel.hive.util.units import Kilometers
 
-import nrel.hive.model.roadnetwork.haversine_link_id_ops as h_ops
-
 
 class HaversineRoadNetwork(RoadNetwork):
     """
     Implements a simple haversine road network where a unique node exists for each unique GeoId in the simulation.
     This assumes a fully connected graph between each node in which the shortest path is the link that connects any
     two nodes. LinkId is specified as a concatenation of the GeoId of its endpoints in which the order is given by
     origin and destination respectively.
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/link.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/link.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/link_id.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/link_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from nrel.hive.util.typealiases import LinkId
-from typing import Optional, Tuple, Any
 from ast import literal_eval
+from typing import Optional, Tuple, Any
+
+from nrel.hive.util.typealiases import LinkId
 
 NodeId = Any
 
 
 def create_link_id(src: int, dst: int) -> LinkId:
     """
     creates a LinkId from its source and destination node ids
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/linktraversal.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/linktraversal.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_builders.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_builders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import TYPE_CHECKING
 
 
-def osm_graph_from_polygon(polygon):
+def osm_graph_from_polygon(polygon, cache_folder):
     """
     builds a OSM networkx graph using a shapely polygon and the osmnx package
     """
     try:
         import osmnx as ox
     except ImportError as e:
         raise ImportError(
             "the osmnx package is required for building an OSMRoadNetwork from a polygon"
         ) from e
 
     ox.settings.all_oneway = True
+    ox.settings.cache_folder = cache_folder
 
     G = ox.graph_from_polygon(polygon, network_type="drive")
 
     G = ox.utils_graph.get_largest_component(G, strongly=True)
 
     G = ox.add_edge_speeds(G)
     G = ox.add_edge_travel_times(G)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_road_network_link_helper.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_road_network_link_helper.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_roadnetwork.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_roadnetwork.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
-from typing import Optional, Union, TYPE_CHECKING
+from typing import Optional, Union
 
+import h3
 import networkx as nx
 
-from nrel.hive.model.roadnetwork.geofence import GeoFence
 from nrel.hive.model.entity_position import EntityPosition
 from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.link_id import extract_node_ids
 from nrel.hive.model.roadnetwork.osm.osm_builders import osm_graph_from_polygon
 from nrel.hive.model.roadnetwork.osm.osm_road_network_link_helper import OSMRoadNetworkLinkHelper
 from nrel.hive.model.roadnetwork.osm.osm_roadnetwork_ops import (
     route_from_nx_path,
@@ -20,21 +20,22 @@
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_distance_km,
     empty_route,
 )
 from nrel.hive.model.sim_time import SimTime
-from nrel.hive.util import LinkId
+from nrel.hive.util import LinkId, H3Ops
 from nrel.hive.util.typealiases import GeoId, H3Resolution
-from nrel.hive.util.units import Kmph, Kilometers
-from nrel.hive.model.roadnetwork.link_id import extract_node_ids
+from nrel.hive.util.units import Hours, Kmph, Kilometers, SECONDS_IN_HOUR
 
 log = logging.getLogger(__name__)
 
+TIME_WEIGHT = "travel_time"
+
 
 class OSMRoadNetwork(RoadNetwork):
     """
     Implements an open street maps road network utilizing the osmnx and networkx libraries
 
     """
 
@@ -61,59 +62,86 @@
             else:
                 return False
 
         if not all(map(_valid_node_id, graph.nodes())):
             raise TypeError("all node ids must be either an integer or a tuple of integers")
 
         #   check to make sure the graph has the right information on the links
-        missing_length = 0
         missing_speed = 0
-        for _, _, d in graph.edges(data=True):
+        missing_time = 0
+        for u, v, d in graph.edges(data=True):
             if "length" not in d:
-                missing_length += 1
+                raise Exception(
+                    "all links in the road network must have a 'length' edge "
+                    f"attribute but link {u} -> {v} does not have one."
+                )
             if "speed_kmph" not in d:
                 missing_speed += 1
-        if missing_length > 0:
-            raise Exception(
-                f"found {missing_length} links in the road network that don't have length information"
+                d["speed_kmph"] = default_speed_kmph
+            if TIME_WEIGHT not in d:
+                distance_km = d["length"] / 1000  # meters to kilometers
+                speed_kmph = d["speed_kmph"]
+                time_hours = distance_km / speed_kmph
+                time_seconds = time_hours * 3600
+                d[TIME_WEIGHT] = time_seconds
+                missing_time += 1
+
+        if missing_speed > 0:
+            log.warning(
+                f"found {missing_speed} links in the road network that don't have speed "
+                f"information.\nhive will automatically set these to {default_speed_kmph} kmph."
             )
-        elif missing_speed > 0:
+        elif missing_time > 0:
             log.warning(
-                f"found {missing_speed} links in the road network that don't have speed information.\n"
-                f"hive will automatically set these to {default_speed_kmph} kmph."
+                f"found {missing_time} links in the road network that don't have time information."
+                f"\nhive will automatically set these to the time it takes to traverse the link at "
+                "the speed specified in the 'speed_kmph' attribute."
             )
 
         # build tables on the network edges for spatial lookup and LinkId lookup
         link_helper_error, link_helper = OSMRoadNetworkLinkHelper.build(
             graph, sim_h3_resolution, default_speed_kmph
         )
+
+        for _, node_data in graph.nodes(data=True):
+            # Replace lat/lon with geoid
+            node_data["geoid"] = h3.geo_to_h3(
+                node_data.get("x", node_data.get("lat")),
+                node_data.get("y", node_data.get("lon")),
+                sim_h3_resolution,
+            )
+            for key in ["x", "y", "lat", "lon"]:
+                node_data.pop(key, None)
+
         if link_helper_error:
             raise link_helper_error
         elif link_helper is None:
             raise Exception("Was not able to build link helper")
         else:
+            self.min_speed_kmph: Kmph = min(link.speed_kmph for link in link_helper.links.values())
             # finish constructing OSMRoadNetwork instance
             self.graph = graph
             self.link_helper = link_helper
 
     @classmethod
     def from_polygon(
         cls,
         polygon,
         sim_h3_resolution: H3Resolution = 15,
         default_speed_kmph: Kmph = 40.0,
+        cache_dir=Path.home(),
     ) -> OSMRoadNetwork:
         """
         Build an OSMRoadNetwork from a shapely polygon
 
         :param polygon: The polygon to build the road network from
         :param sim_h3_resolution: The h3 resolution of the simulation
         :param default_speed_kmph: The network will fill in missing speed values with this
         """
-        graph = osm_graph_from_polygon(polygon)
+        graph = osm_graph_from_polygon(polygon, cache_dir)
         return OSMRoadNetwork(graph, sim_h3_resolution, default_speed_kmph)
 
     @classmethod
     def from_file(
         cls,
         road_network_file: Union[Path, str],
         sim_h3_resolution: H3Resolution = 15,
@@ -126,15 +154,16 @@
         # read in the network file
         if road_network_path.suffix == ".json":
             with road_network_path.open("r") as f:
                 graph = nx.node_link_graph(json.load(f))
             return OSMRoadNetwork(graph, sim_h3_resolution, default_speed_kmph)
         else:
             raise TypeError(
-                f"road network file of type {road_network_path.suffix} not supported by OSMRoadNetwork."
+                f"road network file of type {road_network_path.suffix} not supported by "
+                "OSMRoadNetwork."
             )
 
     def to_file(self, file: Union[str, Path]):
         path = Path(file)
 
         with path.open("w") as f:
             json.dump(nx.node_link_data(self.graph), f)
@@ -146,15 +175,23 @@
         :param origin: the origin Link
         :param destination: the destination Link
         :return: a route between the origin and destination on the OSM road network
         """
         if origin == destination:
             return empty_route()
 
-        # start path search from the end of the origin link, terminate search at the start of the destination link
+        def _astar_cost_heuristic(source, dest) -> float:
+            dist: Kilometers = H3Ops.great_circle_distance(
+                self.graph.nodes[source]["geoid"], self.graph.nodes[dest]["geoid"]
+            )
+            time: Hours = dist / self.min_speed_kmph
+            return time * SECONDS_IN_HOUR
+
+        # start path search from the end of the origin link, terminate search at the start of the
+        # destination link
         extract_src_err, src_nodes = extract_node_ids(origin.link_id)
         extract_dst_err, dst_nodes = extract_node_ids(destination.link_id)
         if extract_src_err:
             log.error(extract_src_err)
             return empty_route()
         elif extract_dst_err:
             log.error(extract_dst_err)
@@ -163,37 +200,44 @@
             return empty_route()
         elif dst_nodes is None:
             return empty_route()
         else:
             _, origin_node_id = src_nodes
             destination_node_id, _ = dst_nodes
 
-            # node-oriented shortest path from the end of the origin link to the beginning of the destination link
-            nx_path = nx.shortest_path(
-                self.graph, origin_node_id, destination_node_id, weight="travel_time"
+            # node-oriented shortest path from the end of the origin link to the beginning of the
+            # destination link
+            nx_path = nx.astar_path(
+                self.graph,
+                origin_node_id,
+                destination_node_id,
+                heuristic=_astar_cost_heuristic,
+                weight=TIME_WEIGHT,
             )
             link_path_error, inner_link_path = route_from_nx_path(nx_path, self.link_helper.links)
 
             if link_path_error:
                 log.error(f"unable to build route from {origin} to {destination}")
                 log.error(link_path_error)
                 log.error(
-                    f"origin node {origin_node_id}, destination node {destination_node_id}, shortest path node list result: {nx_path}"
+                    f"origin node {origin_node_id}, destination node {destination_node_id}, "
+                    f"shortest path node list result: {nx_path}"
                 )
                 return empty_route()
             elif inner_link_path is None:
                 return empty_route()
             else:
                 # modify the start and end GeoIds based on the positions in the src/dst links
                 resolved_route = resolve_route_src_dst_positions(
                     inner_link_path, origin, destination, self
                 )
                 if not resolved_route:
                     log.error(
-                        f"unable to resolve the route from/to/via:\n {origin}\n{destination}\n{inner_link_path}"
+                        f"unable to resolve the route from/to/via:\n"
+                        f"{origin}\n{destination}\n{inner_link_path}"
                     )
                     return empty_route()
                 else:
                     return resolved_route
 
     def distance_by_geoid_km(self, origin: GeoId, destination: GeoId) -> Kilometers:
         """
@@ -203,15 +247,16 @@
         :param destination: the geoid of the destination
         :return: the road network distance in kilometers
         """
         o = self.position_from_geoid(origin)
         d = self.position_from_geoid(destination)
         if not o or not d:
             log.error(
-                f"failed finding nearest links to distance query between GeoIds {origin}, {destination}"
+                "failed finding nearest links to distance query between GeoIds "
+                f"{origin}, {destination}"
             )
             return 0.0
         else:
             distance = route_distance_km(self.route(o, d))
             return distance
 
     def link_from_geoid(self, geoid: GeoId) -> Optional[Link]:
@@ -243,12 +288,12 @@
         Determines if a specific geoid is contained within the road network geofence.
 
 
         :param geoid: the geoid to test
         :return: True/False
         """
         return True
-        # TODO: the geofence is slated to be modified and so we're bypassing this check in the meantime.
-        #  we'll need to add it back once we update the geofence implementation.
+        # TODO: the geofence is slated to be modified and so we're bypassing this check in the
+        #  meantime. We'll need to add it back once we update the geofence implementation.
 
     def update(self, sim_time: SimTime) -> RoadNetwork:
         raise NotImplementedError("updates are not implemented")
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/osm/osm_roadnetwork_ops.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/osm/osm_roadnetwork_ops.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/roadnetwork.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/roadnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import h3
 
-from nrel.hive.model.roadnetwork.link import Link
-from nrel.hive.model.roadnetwork.geofence import GeoFence
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.util.typealiases import GeoId, H3Resolution, LinkId
 from nrel.hive.util.units import Kilometers
 
 
 class RoadNetwork(ABC):
@@ -76,15 +75,15 @@
             return None
         else:
             hexes_on_link = h3.h3_line(link.start, link.end)
             if geoid in hexes_on_link:
                 position = EntityPosition(link.link_id, geoid)
                 return position
             else:
-                hexes_by_dist = sorted(hexes_on_link, key=lambda h: h3.h3_distance(geoid, h))
+                hexes_by_dist = sorted(hexes_on_link, key=lambda h: (h3.h3_distance(geoid, h), h))
                 closest_hex_to_query = hexes_by_dist[0]
                 position = EntityPosition(link.link_id, closest_hex_to_query)
                 return position
 
     @abstractmethod
     def geoid_within_geofence(self, geoid: GeoId) -> bool:
         """
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/route.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import functools as ft
 from typing import Any, Tuple, Optional
 
 import h3
 
 from nrel.hive.model.entity_position import EntityPosition
-from nrel.hive.model.roadnetwork.link import Link
 from nrel.hive.model.roadnetwork.linktraversal import LinkTraversal
 from nrel.hive.runner import Environment
 from nrel.hive.util import TupleOps, wkt
 from nrel.hive.util.units import Kilometers, Seconds
 
 Route = Tuple[LinkTraversal, ...]
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/roadnetwork/routetraversal.py` & `nrel.hive-1.3.0/nrel/hive/model/roadnetwork/routetraversal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import functools as ft
-from typing import Optional, NamedTuple
+from typing import Optional, NamedTuple, Tuple
 
 from nrel.hive.model.roadnetwork.linktraversal import (
     LinkTraversalResult,
     LinkTraversal,
 )
 from nrel.hive.model.roadnetwork.linktraversal import traverse_up_to
+from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.util import TupleOps
-from nrel.hive.util.typealiases import *
 from nrel.hive.util.units import Kilometers, Seconds
 
 
 class RouteTraversal(NamedTuple):
     """
     A tuple that represents the result of traversing a route.
 
@@ -80,23 +80,25 @@
         :param link: a link traversal for the remaining route
         :return: the updated RouteTraversal
         """
         return self._replace(remaining_route=self.remaining_route + (link,))
 
 
 def traverse(
-    route_estimate: Route, duration_seconds: Seconds
+    route_estimate: Route, duration_seconds: Seconds, road_network: RoadNetwork
 ) -> Tuple[Optional[Exception], Optional[RouteTraversal]]:
     """
-    step through the route from the current agent position (assumed to be start.link_id) toward the destination
+    step through the route from the current agent position
+    (assumed to be start.link_id) toward the destination
 
 
     :param route_estimate: the current route estimate
-
     :param duration_seconds: size of the time step for this traversal, in seconds
+    :param road_network: the road network; used to get current travel times
+
     :return: a route experience and updated route estimate;
              or, nothing (None, Empty RouteTraversal) if the route is consumed.
              an exception is possible if the current step is not found on the link or
              the route is malformed.
     """
     if len(route_estimate) == 0:
         return None, RouteTraversal()
@@ -112,22 +114,33 @@
             if acc_failures:
                 return acc
             elif acc_traversal is None:
                 return acc
 
             if acc_traversal.no_time_left():
                 return acc_failures, acc_traversal.add_link_not_traversed(link)
+
+            # update the link traversal speed with a current speed from the road network
+            ground_truth_link = road_network.link_from_link_id(link.link_id)
+            if ground_truth_link is None:
+                response = Exception("failure during traverse")
+                response.__cause__ = Exception(f"link {link.link_id} not found in road network")
+                return response, None
+            updated_speed_link = link._replace(speed_kmph=ground_truth_link.speed_kmph)
+
             # traverse this link as far as we can go
-            error, traverse_result = traverse_up_to(link, acc_traversal.remaining_time_seconds)
+            error, traverse_result = traverse_up_to(
+                updated_speed_link, acc_traversal.remaining_time_seconds
+            )
             if error:
-                response = Exception(f"failure during traverse")
+                response = Exception("failure during traverse")
                 response.__cause__ = error
                 return response, None
             elif traverse_result is None:
-                response = Exception(f"failure during traverse")
+                response = Exception("failure during traverse")
                 return response, None
             else:
                 updated_experienced_route = acc_traversal.add_traversal(traverse_result)
                 return acc_failures, updated_experienced_route
 
         # initial search state has a route traversal and an Optional[Exception]
         initial: Tuple[Optional[Exception], Optional[RouteTraversal]] = (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/sim_time.py` & `nrel.hive-1.3.0/nrel/hive/model/sim_time.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/station/charger_state.py` & `nrel.hive-1.3.0/nrel/hive/model/station/charger_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from typing import NamedTuple
 
 from returns.result import ResultE, Success, Failure
 
 from nrel.hive.model.energy.charger.charger import Charger
-from nrel.hive.util.typealiases import ChargerId
-from nrel.hive.util.units import Currency, KwH
 from nrel.hive.util.error_or_result import ErrorOr
-from nrel.hive.runner.environment import Environment
 from nrel.hive.util.exception import SimulationStateError
+from nrel.hive.util.typealiases import ChargerId
+from nrel.hive.util.units import Currency, KwH
 
 
 class ChargerState(NamedTuple):
     id: ChargerId
     charger: Charger
     total_chargers: int
     available_chargers: int
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/station/station.py` & `nrel.hive-1.3.0/nrel/hive/model/station/station.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from __future__ import annotations
 
-from distutils.util import strtobool
 import functools as ft
-from typing import Dict, Optional, Union
+import logging
 from dataclasses import dataclass, replace
+from distutils.util import strtobool
+from typing import Dict, Optional, Union
 
 import h3
 import immutables
-import logging
-
 from returns.result import ResultE, Success, Failure
 
-from nrel.hive.model.entity import Entity
-from nrel.hive.runner.environment import Environment
-from nrel.hive.model.station.charger_state import ChargerState
 from nrel.hive.model.energy.charger import Charger
-from nrel.hive.model.membership import Membership
+from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.model.entity import Entity
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.membership import Membership
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
+from nrel.hive.model.station.charger_state import ChargerState
 from nrel.hive.model.station.station_ops import (
     station_state_update,
     station_state_optional_update,
     station_state_updates,
 )
+from nrel.hive.runner.environment import Environment
+from nrel.hive.util.dict_ops import DictOps
 from nrel.hive.util.error_or_result import ErrorOr
-from nrel.hive.util.typealiases import *
 from nrel.hive.util.exception import H3Error, SimulationStateError
+from nrel.hive.util.typealiases import *
 from nrel.hive.util.units import Currency, KwH
 from nrel.hive.util.validation import validate_fields
 
 log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
@@ -54,14 +55,15 @@
     :type balance: :py:obj:`Currency`
     """
 
     id: StationId
     position: EntityPosition
     membership: Membership
     state: immutables.Map[ChargerId, ChargerState]
+    energy_dispensed: immutables.Map[EnergyType, float]
     on_shift_access_chargers: FrozenSet[ChargerId]
     balance: Currency = 0.0
 
     @property
     def geoid(self) -> GeoId:
         return self.position.geoid
 
@@ -104,32 +106,35 @@
                     return TypeError(msg), None
                 else:
                     charger_state = ChargerState.build(charger, charger_count)
                     updated_builder = builder.set(charger_id, charger_state)
                     return None, updated_builder
 
         initial = None, immutables.Map[ChargerId, ChargerState]()
-        error, charger_states = ft.reduce(_chargers, chargers.items(), initial)
+        error, charger_states = ft.reduce(_chargers, DictOps.iterate_items(chargers), initial)
         if error is not None:
             raise error
         if charger_states is None:
             msg = f"internal error after building station chargers for station {id}"
             raise Exception(msg)
 
+        energy_dispensed = immutables.Map({energy_type: 0.0 for energy_type in EnergyType})
         position = road_network.position_from_geoid(geoid)
         if position is None:
             msg = (
                 "could not find a road network position matching the position "
                 f"provided for station {id}"
             )
             raise H3Error(msg)
+
         return Station(
             id=id,
             position=position,
             state=charger_states,
+            energy_dispensed=energy_dispensed,
             on_shift_access_chargers=on_shift_access,
             membership=membership,
         )
 
     def append_chargers(
         self, charger_id: ChargerId, charger_count: int, env: Environment
     ) -> ErrorOr[Station]:
@@ -405,14 +410,27 @@
         pay for charging costs
 
         :param currency_received: the currency received for a charge event
         :return: the updated Station
         """
         return replace(self, balance=self.balance + currency_received)
 
+    def tick_energy_dispensed(self, delta_energy: immutables.Map[EnergyType, float]) -> Station:
+        """
+        adds energy dispensed to vehicle
+
+        :param delta_energy: the energy dispensed for a charge event
+        :return: the updated Station
+        """
+        energy_dispensed = {
+            k: self.energy_dispensed[k] + delta_energy.get(k, 0)
+            for k in self.energy_dispensed.keys()
+        }
+        return replace(self, energy_dispensed=immutables.Map(energy_dispensed))
+
     def enqueue_for_charger(self, charger_id: ChargerId) -> ErrorOr[Station]:
         """
         increment the count of vehicles enqueued for a specific charger_id type - no limit
 
         :param charger_id: the charger_id type
         :return: the updated Station
         """
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/station/station_ops.py` & `nrel.hive-1.3.0/nrel/hive/model/station/station_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Iterable, Optional, TypeVar, Callable, TYPE_CHECKING
+import functools as ft
 from dataclasses import replace
+from typing import Iterable, Optional, TypeVar, Callable, TYPE_CHECKING
 
 from nrel.hive.util.error_or_result import ErrorOr
 from nrel.hive.util.typealiases import *
 
-import functools as ft
-
 if TYPE_CHECKING:
     from nrel.hive.model.station.charger_state import ChargerState
     from nrel.hive.model.station.station import Station
 
 
 _EXPECTED_FIELDS = [
     "station_id",
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Dict, Optional
 
 import yaml
-
 from immutables import Map
 
 from nrel.hive.model.vehicle.mechatronics.bev import BEV
 from nrel.hive.model.vehicle.mechatronics.ice import ICE
 from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
 from nrel.hive.model.vehicle.mechatronics.powercurve.powercurve import Powercurve
 from nrel.hive.model.vehicle.mechatronics.powertrain.powertrain import Powertrain
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/bev.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/bev.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-
-from typing import Any, Callable, Dict, NamedTuple, TYPE_CHECKING, Optional, Tuple
+from dataclasses import dataclass
+from typing import Any, Callable, TYPE_CHECKING, Optional, Tuple
 
 import immutables
 
 from nrel.hive.model.energy.energytype import EnergyType
 from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
 from nrel.hive.model.vehicle.mechatronics.powercurve import build_powercurve
 from nrel.hive.model.vehicle.mechatronics.powertrain import build_powertrain
@@ -170,14 +169,17 @@
             self.powertrain.energy_units, Unit.KILOWATT_HOUR
         )
         vehicle_energy_kwh = vehicle.energy[EnergyType.ELECTRIC]
         new_energy_kwh = max(0.0, vehicle_energy_kwh - energy_used_kwh)
         updated_vehicle = vehicle.modify_energy(
             immutables.Map({EnergyType.ELECTRIC: new_energy_kwh})
         )
+        updated_vehicle = updated_vehicle.tick_energy_expended(
+            immutables.Map({EnergyType.ELECTRIC: vehicle_energy_kwh - new_energy_kwh})
+        )
         return updated_vehicle
 
     def idle(self, vehicle: Vehicle, time_seconds: Seconds) -> Vehicle:
         """
         idle for a set amount of time
 
 
@@ -188,14 +190,17 @@
         """
         idle_energy_kwh = self.idle_kwh_per_hour * time_seconds * SECONDS_TO_HOURS
         vehicle_energy_kwh = vehicle.energy[EnergyType.ELECTRIC]
         new_energy_kwh = max(0.0, vehicle_energy_kwh - idle_energy_kwh)
         updated_vehicle = vehicle.modify_energy(
             immutables.Map({EnergyType.ELECTRIC: new_energy_kwh})
         )
+        updated_vehicle = updated_vehicle.tick_energy_expended(
+            immutables.Map({EnergyType.ELECTRIC: vehicle_energy_kwh - new_energy_kwh})
+        )
 
         return updated_vehicle
 
     def add_energy(
         self, vehicle: Vehicle, charger: Charger, time_seconds: Seconds
     ) -> Tuple[Vehicle, Seconds]:
         """
@@ -231,9 +236,12 @@
                 duration_seconds=time_seconds,
             )
             new_energy_kwh = min(self.battery_capacity_kwh, charger_energy_kwh)
 
         updated_vehicle = vehicle.modify_energy(
             immutables.Map({EnergyType.ELECTRIC: new_energy_kwh})
         )
+        updated_vehicle = updated_vehicle.tick_energy_gained(
+            immutables.Map({EnergyType.ELECTRIC: new_energy_kwh - start_energy_kwh})
+        )
 
         return updated_vehicle, time_charging_seconds
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/ice.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/ice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-
-from typing import Any, Callable, Dict, NamedTuple, TYPE_CHECKING, Optional, Tuple
+from dataclasses import dataclass
+from typing import Any, Callable, TYPE_CHECKING, Optional, Tuple
 
 import immutables
 
 from nrel.hive.model.energy.energytype import EnergyType
 from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
 from nrel.hive.model.vehicle.mechatronics.powertrain import build_powertrain
 from nrel.hive.util.typealiases import MechatronicsId
@@ -147,14 +146,17 @@
         )
 
         vehicle_energy_gal_gas = vehicle.energy[EnergyType.GASOLINE]
         new_energy_gal_gas = max(0.0, vehicle_energy_gal_gas - energy_used_gal_gas)
         updated_vehicle = vehicle.modify_energy(
             immutables.Map({EnergyType.GASOLINE: new_energy_gal_gas})
         )
+        updated_vehicle = vehicle.tick_energy_expended(
+            immutables.Map({EnergyType.GASOLINE: vehicle_energy_gal_gas - new_energy_gal_gas})
+        )
         return updated_vehicle
 
     def idle(self, vehicle: Vehicle, time_seconds: Seconds) -> Vehicle:
         """
         idle for a set amount of time
 
 
@@ -165,14 +167,17 @@
         """
         idle_energy_gal_gas = self.idle_gallons_per_hour * time_seconds * SECONDS_TO_HOURS
         vehicle_energy_gal_gas = vehicle.energy[EnergyType.GASOLINE]
         new_energy_gal_gas = max(0.0, vehicle_energy_gal_gas - idle_energy_gal_gas)
         updated_vehicle = vehicle.modify_energy(
             immutables.Map({EnergyType.GASOLINE: new_energy_gal_gas})
         )
+        updated_vehicle = vehicle.tick_energy_expended(
+            immutables.Map({EnergyType.GASOLINE: vehicle_energy_gal_gas - new_energy_gal_gas})
+        )
 
         return updated_vehicle
 
     def add_energy(
         self, vehicle: Vehicle, charger: Charger, time_seconds: Seconds
     ) -> Tuple[Vehicle, Seconds]:
         """
@@ -193,9 +198,12 @@
             return vehicle, 0
         start_gal_gas = vehicle.energy[EnergyType.GASOLINE]
 
         pump_gal_gas = start_gal_gas + charger.rate * time_seconds
         new_gal_gas = min(self.tank_capacity_gallons, pump_gal_gas)
 
         updated_vehicle = vehicle.modify_energy(immutables.Map({EnergyType.GASOLINE: new_gal_gas}))
+        updated_vehicle = updated_vehicle.tick_energy_gained(
+            immutables.Map({EnergyType.GASOLINE: new_gal_gas - start_gal_gas})
+        )
 
         return updated_vehicle, time_seconds
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/mechatronics_interface.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/mechatronics_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
 from typing import Dict, TYPE_CHECKING, Tuple
 
 import immutables
 
-from nrel.hive.model.energy import EnergyType, Charger
+from nrel.hive.model.energy import EnergyType
 
 if TYPE_CHECKING:
     from nrel.hive.util.units import Seconds, Ratio, Kilometers
     from nrel.hive.util.typealiases import MechatronicsId
     from nrel.hive.model.energy.charger import Charger
     from nrel.hive.model.vehicle.vehicle import Vehicle
     from nrel.hive.model.roadnetwork.route import Route
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/__init__.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/powercurve.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powercurve/tabular_powercurve.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powercurve/tabular_powercurve.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/__init__.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/powertrain.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/powertrain.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/mechatronics/powertrain/tabular_powertrain.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/mechatronics/powertrain/tabular_powertrain.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/__init__.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from immutables import Map
 
-from nrel.hive.model.vehicle.schedules.time_range_schedule import time_range_schedules_from_file
-from nrel.hive.util.typealiases import ScheduleId
 from nrel.hive.model.vehicle.schedules.schedule import ScheduleFunction
 from nrel.hive.model.vehicle.schedules.schedule_type import ScheduleType
-
+from nrel.hive.model.vehicle.schedules.time_range_schedule import time_range_schedules_from_file
+from nrel.hive.util.typealiases import ScheduleId
 
 # each is expected to be a one-argument function that takes a file path
 _constructors = {ScheduleType.TIME_RANGE: time_range_schedules_from_file}
 
 
 def build_schedules_table(
     schedule_type: ScheduleType, schedules_file: str
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/schedule_type.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/schedule_type.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/schedules/time_range_schedule.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/schedules/time_range_schedule.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from csv import DictReader
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, Optional
 
 from immutables import Map
 
+from nrel.hive.model.vehicle.schedules.schedule import ScheduleFunction
 from nrel.hive.util.time_helpers import read_time_string, time_in_range
 from nrel.hive.util.typealiases import VehicleId, ScheduleId
-from nrel.hive.model.vehicle.schedules.schedule import ScheduleFunction
 
 
 def time_range_schedules_from_file(
     file: str,
 ) -> Map[ScheduleId, ScheduleFunction]:
     """
     given a CSV file of time ranges by ScheduleId, construct a time range schedule table
```

### Comparing `nrel.hive-1.2.2/nrel/hive/model/vehicle/vehicle.py` & `nrel.hive-1.3.0/nrel/hive/model/vehicle/vehicle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-from typing import Dict
 from dataclasses import dataclass, replace
+from typing import Dict
 
 import h3
 import immutables
 
-from nrel.hive.model.entity import Entity
 from nrel.hive.model.energy.energytype import EnergyType
-from nrel.hive.model.membership import Membership
+from nrel.hive.model.entity import Entity
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.membership import Membership
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.driver_state.driver_state import DriverState
 from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.vehicle_state import VehicleState
 from nrel.hive.util.typealiases import *
 from nrel.hive.util.units import Kilometers, Currency
@@ -41,14 +41,16 @@
     position: EntityPosition
 
     membership: Membership
 
     # mechatronic properties
     mechatronics_id: MechatronicsId
     energy: immutables.Map[EnergyType, float]
+    energy_gained: immutables.Map[EnergyType, float]
+    energy_expended: immutables.Map[EnergyType, float]
 
     # vehicle planning/operational properties
     vehicle_state: VehicleState
     driver_state: DriverState
     total_seats: int
     # available_seats: int
 
@@ -97,14 +99,16 @@
                 mechatronics = environment.mechatronics.get(mechatronics_id)
                 if not mechatronics:
                     found = set(environment.mechatronics.keys())
                     raise IOError(
                         f"was not able to find mechatronics '{mechatronics_id}' for vehicle {vehicle_id} in environment: found {found}"
                     )
                 energy = mechatronics.initial_energy(float(row["initial_soc"]))
+                energy_expended = mechatronics.initial_energy(0.0)
+                energy_gained = mechatronics.initial_energy(0.0)
 
                 schedule_id = row.get(
                     "schedule_id"
                 )  # if None, it signals an autonomous vehicle, otherwise, human with schedule
                 home_base_id = row.get("home_base_id")
                 if schedule_id and not schedule_id in environment.schedules.keys():
                     raise IOError(
@@ -126,14 +130,16 @@
                         f"vehicle {vehicle_id} cannot be positioned on the road network; check the input lat/lon"
                     )
 
                 return Vehicle(
                     id=vehicle_id,
                     mechatronics_id=mechatronics_id,
                     energy=energy,
+                    energy_expended=energy_expended,
+                    energy_gained=energy_gained,
                     membership=Membership(),
                     position=start_position,
                     vehicle_state=Idle.build(vehicle_id),
                     driver_state=driver_state,
                     total_seats=available_seats,
                     # available_seats=available_seats
                 )
@@ -203,14 +209,34 @@
         adds distance to vehicle
 
         :param delta_d_km:
         :return:
         """
         return replace(self, distance_traveled_km=self.distance_traveled_km + delta_d_km)
 
+    def tick_energy_expended(self, delta_energy: immutables.Map[EnergyType, float]) -> Vehicle:
+        """
+        adds energy expenditure to vehicle
+
+        :param delta_energy:
+        :return:
+        """
+        energy_expended = {k: self.energy_expended[k] + delta_energy[k] for k in self.energy.keys()}
+        return replace(self, energy_expended=immutables.Map(energy_expended))
+
+    def tick_energy_gained(self, delta_energy: immutables.Map[EnergyType, float]) -> Vehicle:
+        """
+        adds energy gain to vehicle
+
+        :param delta_energy:
+        :return:
+        """
+        energy_gained = {k: self.energy_gained[k] + delta_energy[k] for k in self.energy.keys()}
+        return replace(self, energy_gained=immutables.Map(energy_gained))
+
     def set_membership(self, member_ids: Tuple[str, ...]) -> Vehicle:
         """
         sets the membership(s) of the vehicle
 
         :param member_ids: a Tuple containing updated membership(s) of the vehicle
         :return:
         """
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/driver_event_ops.py` & `nrel.hive-1.3.0/nrel/hive/reporting/driver_event_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import TYPE_CHECKING
+from enum import Enum
 
 import h3
+
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
-from nrel.hive.util import wkt
 from nrel.hive.runner import Environment
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
-from enum import Enum
+from nrel.hive.util import wkt
 
 
 class ScheduleEventType(Enum):
     OFF = "off"
     ON = "on"
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/eventful_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/eventful_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import json
 import logging
-import os
 from pathlib import Path
 from typing import TYPE_CHECKING, List
 
 from nrel.hive.reporting import vehicle_event_ops
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.report_type import ReportType
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List
-
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from nrel.hive.reporting.reporter import Report
     from nrel.hive.runner.runner_payload import RunnerPayload
 
 
 class Handler(ABC):
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/instruction_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/instruction_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 import json
 import logging
-import os
 from pathlib import Path
 from typing import TYPE_CHECKING, List
 
-from nrel.hive.reporting import vehicle_event_ops
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.report_type import ReportType
 
 if TYPE_CHECKING:
     from nrel.hive.config.global_config import GlobalConfig
     from nrel.hive.runner.runner_payload import RunnerPayload
     from nrel.hive.reporting.reporter import Report
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/stateful_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/stateful_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
+from dataclasses import asdict
 from pathlib import Path
 from typing import List
-from dataclasses import asdict
 
 from nrel.hive.config.global_config import GlobalConfig
 from nrel.hive.model.station.station import Station
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
@@ -31,31 +31,31 @@
         :param reports: ignored
 
         :param runner_payload: provides the current simulation state
         """
         sim_state = runner_payload.s
         if ReportType.DRIVER_STATE in self.global_config.log_sim_config:
             self._report_entities(
-                entities=sim_state.vehicles.values(),
+                entities=sim_state.get_vehicles(),
                 asdict=self.driver_asdict,
                 sim_time=sim_state.sim_time,
                 report_type=ReportType.DRIVER_STATE,
             )
 
         if ReportType.VEHICLE_STATE in self.global_config.log_sim_config:
             self._report_entities(
-                entities=sim_state.vehicles.values(),
+                entities=sim_state.get_vehicles(),
                 asdict=self.vehicle_asdict,
                 sim_time=sim_state.sim_time,
                 report_type=ReportType.VEHICLE_STATE,
             )
 
         if ReportType.STATION_STATE in self.global_config.log_sim_config:
             self._report_entities(
-                entities=sim_state.stations.values(),
+                entities=sim_state.get_stations(),
                 asdict=self.station_asdict,
                 sim_time=sim_state.sim_time,
                 report_type=ReportType.STATION_STATE,
             )
 
     def close(self, runner_payload: RunnerPayload):
         self.log_file.close()
@@ -98,14 +98,15 @@
         return output
 
     @staticmethod
     def station_asdict(station: Station) -> dict:
         out_dict = asdict(station)
         del out_dict["id"]
         del out_dict["state"]
+        del out_dict["energy_dispensed"]
 
         out_dict["station_id"] = station.id
         out_dict["memberships"] = str(station.membership)
 
         # deconstruct origin_link
         out_dict["link_id"] = station.position.link_id
         out_dict["geoid"] = station.position.geoid
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/stats_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/stats_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from __future__ import annotations
 
 import json
-
 import logging
 from collections import Counter
-from dataclasses import dataclass, field
-from functools import reduce
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Dict
 
-import numpy as np
-
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.handler.summary_stats import SummaryStats
 from nrel.hive.reporting.report_type import ReportType
 
 if TYPE_CHECKING:
     from nrel.hive.reporting.reporter import Report
     from nrel.hive.runner.runner_payload import RunnerPayload
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/time_step_stats_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/time_step_stats_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
-from collections import Counter
-from immutables import Map
 import logging
-import numpy as np
 import os
-import pandas as pd
-from pandas import DataFrame
+from collections import Counter
+from collections.abc import Sequence
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, FrozenSet, List, Optional
+from typing import TYPE_CHECKING, Callable, Dict, FrozenSet, Optional, List
+
+import numpy as np
+from immutables import Map
 
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
+from nrel.hive.util.io import to_csv, to_csv_dicts
 
 if TYPE_CHECKING:
     from nrel.hive.config import HiveConfig
     from nrel.hive.model.vehicle.vehicle import Vehicle
     from nrel.hive.runner.runner_payload import RunnerPayload
     from nrel.hive.reporting.reporter import Report
     from nrel.hive.util.typealiases import MembershipId
@@ -37,59 +38,54 @@
         self.start_time = config.sim.start_time
         self.timestep_duration_seconds = config.sim.timestep_duration_seconds
 
         self.vehicle_state_names = tuple(vs.name for vs in VehicleStateType)
 
         if config.global_config.log_time_step_stats:
             self.log_time_step_stats = True
-            self.data: List[Dict[str, Any]] = []
+            self.data: list = []
             self.time_step_stats_outpath = scenario_output_directory.joinpath(
                 f"{file_name}_all.csv"
             )
         else:
             self.log_time_step_stats = False
 
         if config.global_config.log_fleet_time_step_stats and len(fleet_ids) > 0:
             self.log_fleet_time_step_stats = True
             self.fleets_timestep_stats_outpath = scenario_output_directory.joinpath(
                 "fleet_time_step_stats/"
             )
-            self.fleets_data: Dict[str, List[Dict[str, Any]]] = {}
+            self.fleets_data: dict = {}
             for fleet_id in fleet_ids:
                 if fleet_id is None:
                     self.fleets_data["none"] = []
                 else:
                     self.fleets_data[fleet_id] = []
         else:
             self.log_fleet_time_step_stats = False
 
-    def get_time_step_stats(self) -> Optional[DataFrame]:
+    def get_time_step_stats(self) -> list:
         """
         return a DataFrame of the time step level statistics.
 
         :return: the time step stats DataFrame
         """
-        if not self.log_time_step_stats:
-            return None
 
-        return DataFrame(self.data)
+        return self.data
 
     def get_fleet_time_step_stats(
         self,
-    ) -> Map[MembershipId, DataFrame]:
+    ) -> Map[MembershipId, Sequence]:
         """
-        return an immutable map of time step stat DataFrames by membership id.
+        return an immutable map of time step stat data by membership id.
 
-        :return: the immutable map containing time step stats DataFrames by membership id
+        :return: the immutable map containing time step stats data by membership id
         """
         result = Map(
-            {
-                fleet_id: DataFrame(data) if len(data) > 0 else None
-                for fleet_id, data in self.fleets_data.items()
-            }
+            {fleet_id: data if data else None for fleet_id, data in self.fleets_data.items()}
         )
         return result
 
     def handle(self, reports: List[Report], runner_payload: RunnerPayload):
         """
         called at each log step. aggregates various statistics to the time bin level
 
@@ -118,15 +114,15 @@
 
         # get number of assigned requests in this time step
         assigned_requests_count = len(
             sim_state.get_requests(filter_function=lambda r: r.dispatched_vehicle is not None)
         )
 
         # get number of active requests in this time step (unassigned)
-        active_requests_count = len(sim_state.get_requests()) - assigned_requests_count
+        active_requests_count = len(sim_state.requests) - assigned_requests_count
 
         # get number of canceled requests in this time step
         if ReportType.CANCEL_REQUEST_EVENT in reports_by_type.keys():
             canceled_requests_count = len(reports_by_type[ReportType.CANCEL_REQUEST_EVENT])
         else:
             canceled_requests_count = 0
 
@@ -135,27 +131,24 @@
             veh_pooling = sim_state.get_vehicles(
                 filter_function=lambda v: v.vehicle_state.vehicle_state_type
                 == VehicleStateType.SERVICING_POOLING_TRIP
             )
 
             # count the number of vehicles in each vehicle state
             veh_state_counts = Counter(
-                map(
-                    lambda v: v.vehicle_state.vehicle_state_type.name,
-                    sim_state.get_vehicles(),
-                )
+                v.vehicle_state.vehicle_state_type.name for v in sim_state.get_vehicles()
             )
 
             stats_row = {
                 "time_step": time_step,
                 "sim_time": sim_time.as_iso_time(),
             }
 
             # get average SOC of vehicles
-            if len(sim_state.get_vehicles()) > 0:
+            if len(sim_state.vehicles) > 0:
                 stats_row["avg_soc_percent"] = 100 * np.mean(
                     [
                         env.mechatronics[v.mechatronics_id].fuel_source_soc(v)
                         for v in sim_state.get_vehicles()
                     ]
                 )
             else:
@@ -191,29 +184,24 @@
 
             # add the number of vehicles in each vehicle state
             stats_row["vehicles"] = len(sim_state.vehicles)
             for state in self.vehicle_state_names:
                 stats_row[f"vehicles_{state.lower()}"] = veh_state_counts[state]
 
             available_driver_counts = Counter(
-                map(
-                    lambda v: v.driver_state.available,
-                    sim_state.get_vehicles(),
-                )
+                v.driver_state.available for v in sim_state.get_vehicles()
             )
+
             stats_row["drivers_available"] = available_driver_counts[True]
             stats_row["drivers_unavailable"] = available_driver_counts[False]
 
             # count number of chargers in use by type
             if ReportType.VEHICLE_CHARGE_EVENT in reports_by_type.keys():
                 charger_counts = Counter(
-                    map(
-                        lambda r: r.report["charger_id"],
-                        reports_by_type[ReportType.VEHICLE_CHARGE_EVENT],
-                    )
+                    r.report["charger_id"] for r in reports_by_type[ReportType.VEHICLE_CHARGE_EVENT]
                 )
                 for charger in env.chargers.keys():
                     stats_row[f"charger_{charger.lower()}"] = charger_counts[charger]
             else:
                 for charger in env.chargers.keys():
                     stats_row[f"charger_{charger.lower()}"] = 0
 
@@ -276,18 +264,15 @@
                         == VehicleStateType.DISPATCH_POOLING_TRIP,
                         veh_in_fleet,
                     )
                 )
 
                 # count the number of vehicles in each vehicle state in this fleet
                 veh_state_counts_in_fleet = Counter(
-                    map(
-                        lambda v: v.vehicle_state.vehicle_state_type.name,
-                        veh_in_fleet,
-                    )
+                    v.vehicle_state.vehicle_state_type.name for v in veh_in_fleet
                 )
 
                 # create stats row with the time step
                 fleet_stats_row = {
                     "time_step": time_step,
                     "sim_time": sim_time.as_iso_time(),
                 }
@@ -338,54 +323,51 @@
 
                 # add the number of vehicles in each vehicle state in this fleet
                 fleet_stats_row["vehicles"] = len(veh_in_fleet)
                 for state in self.vehicle_state_names:
                     fleet_stats_row[f"vehicles_{state.lower()}"] = veh_state_counts_in_fleet[state]
 
                 available_driver_counts_in_fleet = Counter(
-                    map(lambda v: v.driver_state.available, veh_in_fleet)
+                    v.driver_state.available for v in veh_in_fleet
                 )
                 fleet_stats_row["drivers_available"] = available_driver_counts_in_fleet[True]
                 fleet_stats_row["drivers_unavailable"] = available_driver_counts_in_fleet[False]
 
                 # count number of chargers in use by type
                 if ReportType.VEHICLE_CHARGE_EVENT in requests_in_fleet.keys():
                     charger_counts_in_fleet = Counter(
-                        map(
-                            lambda r: r.report["charger_id"],
-                            requests_in_fleet[ReportType.VEHICLE_CHARGE_EVENT],
-                        )
+                        r.report["charger_id"]
+                        for r in requests_in_fleet[ReportType.VEHICLE_CHARGE_EVENT]
                     )
                     for charger in env.chargers.keys():
                         fleet_stats_row[f"charger_{charger.lower()}"] = charger_counts_in_fleet[
                             charger
                         ]
                 else:
                     for charger in env.chargers.keys():
                         fleet_stats_row[f"charger_{charger.lower()}"] = 0
 
                 # append the statistics row to the fleet's data list
                 self.fleets_data[fleet_id].append(fleet_stats_row)
 
     def close(self, runner_payload: RunnerPayload):
         """
-        saves all time step stat DataFrames as csv files to the scenario output directory.
+        saves all time step stat data as csv files to the scenario output directory.
 
         :return:
         """
         if self.log_time_step_stats:
-            pd.DataFrame.to_csv(
+            to_csv_dicts(
                 self.get_time_step_stats(),
                 self.time_step_stats_outpath,
-                index=False,
             )
             log.info(f"time step stats written to {self.time_step_stats_outpath}")
 
         if self.log_fleet_time_step_stats:
             os.mkdir(self.fleets_timestep_stats_outpath)
-            for fleet_id, fleet_df in self.get_fleet_time_step_stats().items():
-                if fleet_df is not None:
+            for fleet_id, fleet_data in self.get_fleet_time_step_stats().items():
+                if fleet_data is not None:
                     outpath = self.fleets_timestep_stats_outpath.joinpath(
                         f"{self.file_name}_{fleet_id}.csv"
                     )
-                    pd.DataFrame.to_csv(fleet_df, outpath, index=False)
+                    to_csv(fleet_data, outpath)
                     log.info(f"fleet id: {fleet_id} time step stats written to {outpath}")
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/handler/vehicle_charge_events_handler.py` & `nrel.hive-1.3.0/nrel/hive/reporting/handler/vehicle_charge_events_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List, Dict
 
-import pandas as pd
 from nrel.hive.reporting.handler.handler import Handler
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
 from nrel.hive.runner import RunnerPayload
 from nrel.hive.util import SimulationStateError
 
 
@@ -33,21 +32,20 @@
                     self.events["energy"].append(report.report["energy"])
                     self.events["units"].append(report.report["energy_units"])
                 except KeyError as e:
                     raise SimulationStateError(
                         f"unable to parse charge event from report {report}, missing entry for {e}"
                     )
 
-    def get_events(self):
+    def get_events(self) -> Dict[str, list]:
         """
         grabs the events as a pandas dataframe
         :return: a pandas dataframe containing charge events
         """
-        df = pd.DataFrame(data=self.events)
-        return df
+        return self.events
 
     def clear(self):
         """
         clears the stored events
         :return:
         """
         self.events = self.prototype.copy()
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/instruction_generator_event_ops.py` & `nrel.hive-1.3.0/nrel/hive/reporting/instruction_generator_event_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import h3
 
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
 from nrel.hive.util import wkt
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/report_type.py` & `nrel.hive-1.3.0/nrel/hive/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/reporter.py` & `nrel.hive-1.3.0/nrel/hive/reporting/reporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING, Dict, NamedTuple, Optional, Tuple, Any
+
 from immutables import Map
-from pandas import DataFrame
-from typing import TYPE_CHECKING, Dict, List, NamedTuple, Optional, Tuple
 
-from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.handler.stats_handler import StatsHandler
 from nrel.hive.reporting.handler.time_step_stats_handler import TimeStepStatsHandler
+from nrel.hive.reporting.report_type import ReportType
 
 if TYPE_CHECKING:
     from nrel.hive.model.membership import MembershipId
     from nrel.hive.runner.runner_payload import RunnerPayload
     from nrel.hive.reporting.handler.handler import Handler
 
 
@@ -68,18 +68,18 @@
         for handler in self.handlers:
             if isinstance(handler, StatsHandler):
                 final_report = handler.get_stats(rp)
         return final_report
 
     def get_time_step_stats(
         self,
-    ) -> Tuple[Optional[DataFrame], Optional[Map[MembershipId, DataFrame]]]:
+    ) -> Tuple[Optional[Any], Optional[Any]]:
         """
-        if a TimeStepStatsHandler exists, return the time step stats DataFrame and the fleet time step stats DataFrames
-        :return: the time step stats DataFrame and the fleet time step stats collection of DataFrames if they exist
+        if a TimeStepStatsHandler exists, return the time step stats and the fleet time step stats
+        :return: the time step stats and the fleet time step stats collection if they exist
         """
         time_step_stats, fleet_time_step_stats = None, None
         for handler in self.handlers:
             if isinstance(handler, TimeStepStatsHandler):
                 time_step_stats = handler.get_time_step_stats()
                 fleet_time_step_stats = handler.get_fleet_time_step_stats()
         return time_step_stats, fleet_time_step_stats
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/reporter_ops.py` & `nrel.hive-1.3.0/nrel/hive/reporting/reporter_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 import functools as ft
 from pathlib import Path
 from typing import Dict, Tuple, Any
 
-import immutables
 from returns.io import IOResult, IOResultE
 
 from nrel.hive.model.station.station import Station
 from nrel.hive.runner import Environment
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 
 
@@ -37,15 +36,15 @@
         )
 
         return {"station_id": station.id, "rate": rate}
 
     try:
         result: Tuple[Dict[str, Any], ...] = ft.reduce(
             lambda acc, s: acc + (_station_energy(s),),
-            sim.stations.values(),
+            sim.get_stations(),
             (),
         )
 
         output_file = Path(env.config.scenario_output_directory).joinpath("station_capacities.csv")
         with output_file.open("w") as f:
             writer = csv.DictWriter(f, fieldnames=["station_id", "rate"])
             writer.writeheader()
```

### Comparing `nrel.hive-1.2.2/nrel/hive/reporting/vehicle_event_ops.py` & `nrel.hive-1.3.0/nrel/hive/reporting/vehicle_event_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 import functools as ft
 from typing import TYPE_CHECKING, Tuple, Set
 
 import h3
 import immutables
 
-from nrel.hive.model.energy import Charger
 import nrel.hive.model.roadnetwork.route as route
+from nrel.hive.model.energy import Charger
+from nrel.hive.model.roadnetwork.routetraversal import RouteTraversal
 from nrel.hive.model.station.station import Station
 from nrel.hive.model.vehicle.vehicle import Vehicle
-from nrel.hive.model.roadnetwork.routetraversal import RouteTraversal
 from nrel.hive.reporting.reporter import Report, ReportType
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.util import StationId, TupleOps
 from nrel.hive.util.time_helpers import time_diff
 
 if TYPE_CHECKING:
     from nrel.hive.model.request.request import Request
     from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
-    from nrel.hive.state.vehicle_state.vehicle_state_ops import MoveResult
 
 
 def vehicle_move_event(
     sim: SimulationState,
     prev_vehicle: Vehicle,
     next_vehicle: Vehicle,
     route_traversal: RouteTraversal,
@@ -47,14 +46,15 @@
     if set(prev_vehicle.energy.keys()) != set(next_vehicle.energy.keys()):
         raise ValueError(
             f"Energy types do not match: {set(prev_vehicle.energy.keys())} != {set(next_vehicle.energy.keys())}"
         )
     elif len(next_vehicle.energy.keys()) > 1:
         raise NotImplementedError("hive doesn't currently support multiple energy types")
     else:
+        # assumes one energy type per vehicle (no PHEVs)
         energy_units = list(next_vehicle.energy.keys())[0].units
 
     delta_energy = ft.reduce(
         lambda acc, e_type: acc + next_vehicle.energy[e_type] - prev_vehicle.energy[e_type],
         next_vehicle.energy.keys(),
         0.0,
     )
@@ -292,15 +292,17 @@
     # collect vehicle charge events
     reported_charge_events_accumulator: immutables.Map[StationId, Tuple[float, str]] = ft.reduce(
         _add, reports, immutables.Map()
     )
 
     # create entries for stations with no charge events reported
     reported_stations: Set[StationId] = set(reported_charge_events_accumulator.keys())
-    unreported_station_ids: Set[StationId] = set(sim.stations.keys()).difference(reported_stations)
+    unreported_station_ids: Set[StationId] = set(sim.get_station_ids()).difference(
+        reported_stations
+    )
     all_stations_accumulator = ft.reduce(
         lambda acc, id: acc.update({id: (0.0, "")}),
         unreported_station_ids,
         reported_charge_events_accumulator,
     )
 
     result = _to_reports(all_stations_accumulator)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/__pycache__/mock_lobster.cpython-310.pyc` & `nrel.hive-1.3.0/nrel/hive/resources/__pycache__/mock_lobster.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/__pycache__/mock_lobster.cpython-38.pyc` & `nrel.hive-1.3.0/nrel/hive/resources/__pycache__/mock_lobster.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/defaults/.hive.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/defaults/.hive.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 # whether or not to log the states for all entities at all timesteps; 
 # this file can get very large for big scenarios but contains detailed information; 
 log_states: True
 
 # whether or not to log events when they occur (i.e. a charging event) 
 log_events: True
 
+# whether or not to log kepler.gl inputs
+log_kepler: False
+
 # whether or not to log issued instructions 
 log_instructions: True
 
 # whether or not to log aggregate statistics like total vehicle miles traveled 
 log_stats: True
 
 # python logging level
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/defaults/hive_config.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/defaults/hive_config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 input:
   mechatronics_file: mechatronics.yaml           # default comes from nrel.hive.resources.mechatronics.mechatronics.csv
   road_network_file: null                       # default is to construct a Haversine road network
   geofence_file: null                           # default is to have no geofencing
   rate_structure_file: null                     # default is $0.00 for all services
   charging_price_file: null                     # default is $0.00 for any charging
-  demand_forecast_file: null                    # default is no demand forecasting
 sim:
   timestep_duration_seconds: 60                 # default is to advance time 1 minute between dispatcher updates
   sim_h3_resolution: 15                         # default is to store GeoIds at h3 resolution 15 (approx 1 meter hexes)
+  min_delta_energy_change: 0.0001               # default minimal step size used in time to fill to prevent iter loops
                                                 # see https://github.com/uber/h3/blob/master/docs/core-library/restable.md
   sim_h3_search_resolution: 7                   # conduct bi-level search at h3 resolution 7
   request_cancel_time_seconds: 600              # requests are cancelled by default after 10 minutes of simulation wait time
   schedule_type: "time_range"                   # finds human-driver schedules in a CSV file with start + end time ranges
 network:
   network_type: euclidean                       # default is to produce the Haversine Euclidean road newtork
   default_speed_kmph: 40.0                      # default Haversine network speeds are 40.0 kmph on each link
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/mock_lobster.py` & `nrel.hive-1.3.0/nrel/hive/resources/mock_lobster.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import tempfile
 from pathlib import Path
-from typing import Dict, Union, Callable
+from typing import Dict, FrozenSet, Optional, Tuple, Union, Callable
 
 import h3
 import immutables
 import yaml
 from pkg_resources import resource_filename
 
-
 from nrel.hive.config import HiveConfig
 from nrel.hive.dispatcher.forecaster.forecast import Forecast, ForecastType
 from nrel.hive.dispatcher.forecaster.forecaster_interface import ForecasterInterface
-from nrel.hive.dispatcher.instruction.instructions import *
 from nrel.hive.dispatcher.instruction_generator.charging_fleet_manager import ChargingFleetManager
 from nrel.hive.dispatcher.instruction_generator.dispatcher import Dispatcher
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
 from nrel.hive.model.base import Base
 from nrel.hive.model.energy.charger import Charger
 from nrel.hive.model.energy.energytype import EnergyType
 from nrel.hive.model.membership import Membership
 from nrel.hive.model.request import Request, RequestRateStructure
 from nrel.hive.model.roadnetwork.geofence import GeoFence
 from nrel.hive.model.roadnetwork.haversine_roadnetwork import HaversineRoadNetwork
 from nrel.hive.model.roadnetwork.link import Link
+from nrel.hive.model.roadnetwork.linktraversal import LinkTraversal
 from nrel.hive.model.roadnetwork.osm.osm_roadnetwork import OSMRoadNetwork
 from nrel.hive.model.roadnetwork.roadnetwork import RoadNetwork
+from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.model.station.station import Station
 from nrel.hive.model.vehicle.mechatronics.bev import BEV
 from nrel.hive.model.vehicle.mechatronics.ice import ICE
 from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
 from nrel.hive.model.vehicle.mechatronics.powercurve.tabular_powercurve import TabularPowercurve
 from nrel.hive.model.vehicle.mechatronics.powertrain.tabular_powertrain import TabularPowertrain
@@ -50,17 +50,29 @@
     HumanAvailable,
     HumanUnavailable,
 )
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.update.step_simulation import StepSimulation
 from nrel.hive.state.simulation_state.update.update import Update
+from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.vehicle_state import VehicleState
-from nrel.hive.util.typealiases import *
-from nrel.hive.util.units import *
+from nrel.hive.util.typealiases import (
+    ChargerId,
+    RequestId,
+    VehicleId,
+    StationId,
+    BaseId,
+    MechatronicsId,
+    ScheduleId,
+    MembershipId,
+    GeoId,
+    H3Resolution,
+)
+from nrel.hive.util.units import Currency, Kmph, Ratio, Seconds
 
 
 class DefaultIds:
     @classmethod
     def mock_request_id(cls) -> RequestId:
         return "r0"
 
@@ -132,14 +144,125 @@
 def mock_network(h3_res: H3Resolution = 15, geofence_res: H3Resolution = 10) -> RoadNetwork:
     return HaversineRoadNetwork(
         geofence=mock_geofence(resolution=geofence_res),
         sim_h3_resolution=h3_res,
     )
 
 
+def mock_osm_route() -> Route:
+    """A mock route taken from the mock osm network"""
+    return (
+        LinkTraversal(
+            link_id="176080957-176080956",
+            start="8f268cdacac236d",
+            end="8f268cdacace2db",
+            distance_km=0.10470500000000002,
+            speed_kmph=39.7,
+        ),
+        LinkTraversal(
+            link_id="176080956-176092324",
+            start="8f268cdacace2db",
+            end="8f268cdac375852",
+            distance_km=0.14674299999999998,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176092324-176092321",
+            start="8f268cdac375852",
+            end="8f268cdac354143",
+            distance_km=0.14593199999999998,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176092321-176092319",
+            start="8f268cdac354143",
+            end="8f268cdac2213b0",
+            distance_km=0.146583,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176092319-176092317",
+            start="8f268cdac2213b0",
+            end="8f268cdac200663",
+            distance_km=0.14668,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176092317-176092315",
+            start="8f268cdac200663",
+            end="8f268cdac21a99e",
+            distance_km=0.145991,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176092315-176084469",
+            start="8f268cdac21a99e",
+            end="8f268cdac28dc4b",
+            distance_km=0.146845,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176084469-659623106",
+            start="8f268cdac28dc4b",
+            end="8f268cda8924086",
+            distance_km=0.146254,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="659623106-3329646638",
+            start="8f268cda8924086",
+            end="8f268cda893178c",
+            distance_km=0.148035,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="3329646638-5063215690",
+            start="8f268cda893178c",
+            end="8f268cda8913d26",
+            distance_km=0.145185,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="5063215690-5313640931",
+            start="8f268cda8913d26",
+            end="8f268cda891e263",
+            distance_km=0.10451800000000001,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="5313640931-176100374",
+            start="8f268cda891e263",
+            end="8f268cda8826870",
+            distance_km=0.10771800000000001,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176100374-176104476",
+            start="8f268cda8826870",
+            end="8f268cda8821000",
+            distance_km=0.10456100000000002,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="176104476-637816565",
+            start="8f268cda8821000",
+            end="8f268cda882d781",
+            distance_km=0.10358000000000002,
+            speed_kmph=40.2,
+        ),
+        LinkTraversal(
+            link_id="637816565-279916144",
+            start="8f268cda882d781",
+            end="8f268cda8942091",
+            distance_km=0.146861,
+            speed_kmph=39.7,
+        ),
+    )
+
+
 def mock_osm_network(h3_res: H3Resolution = 15, geofence_res: H3Resolution = 10) -> OSMRoadNetwork:
     road_network_file = resource_filename(
         "nrel.hive.resources.scenarios.denver_downtown.road_network",
         "downtown_denver_network.json",
     )
     return OSMRoadNetwork.from_file(
         road_network_file=Path(road_network_file),
@@ -368,14 +491,16 @@
     driver_state: Optional[DriverState] = None,
     membership: Membership = Membership(),
     total_seats: int = 999,
 ) -> Vehicle:
     v_state = vehicle_state if vehicle_state else Idle.build(vehicle_id)
     road_network = mock_network(h3_res)
     initial_energy = mechatronics.initial_energy(soc)
+    energy_expended = mechatronics.initial_energy(0.0)
+    energy_gained = mechatronics.initial_energy(0.0)
     geoid = h3.geo_to_h3(lat, lon, road_network.sim_h3_resolution)
     d_state = (
         driver_state
         if driver_state
         else AutonomousAvailable(AutonomousDriverAttributes(vehicle_id))
     )
     position = road_network.position_from_geoid(geoid)
@@ -383,14 +508,16 @@
     if position is None:
         raise ValueError(f"geoid {geoid} is outside of boundary of road network")
 
     return Vehicle(
         id=vehicle_id,
         mechatronics_id=mechatronics.mechatronics_id,
         energy=initial_energy,
+        energy_expended=energy_expended,
+        energy_gained=energy_gained,
         position=position,
         vehicle_state=v_state,
         driver_state=d_state,
         membership=membership,
         total_seats=total_seats,
     )
 
@@ -403,28 +530,33 @@
     soc: Ratio = 1,
     driver_state: Optional[DriverState] = None,
     membership: Membership = Membership(),
     total_seats: int = 999,
 ) -> Vehicle:
     state = vehicle_state if vehicle_state else Idle.build(vehicle_id)
     initial_energy = mechatronics.initial_energy(soc)
+    energy_expended = mechatronics.initial_energy(0.0)
+    energy_gained = mechatronics.initial_energy(0.0)
+
     d_state = (
         driver_state
         if driver_state
         else AutonomousAvailable(AutonomousDriverAttributes(vehicle_id))
     )
     position = mock_network().position_from_geoid(geoid)
 
     if position is None:
         raise ValueError(f"geoid {geoid} is outside of boundary of road network")
 
     return Vehicle(
         id=vehicle_id,
         mechatronics_id=mechatronics.mechatronics_id,
         energy=initial_energy,
+        energy_expended=energy_expended,
+        energy_gained=energy_gained,
         position=position,
         vehicle_state=state,
         driver_state=d_state,
         membership=membership,
         total_seats=total_seats,
     )
 
@@ -486,15 +618,14 @@
             "bases_file": "denver_demo_bases.csv",
             "stations_file": "denver_demo_stations.csv",
             "chargers_file": "default_chargers.csv",
             "charging_price_file": "denver_charging_prices_by_geoid.csv",
             "rate_structure_file": "rate_structure.csv",
             "mechatronics_file": "mechatronics.yaml",
             "geofence_file": "downtown_denver.geojson",
-            "demand_forecast_file": "denver_demand.csv",
         }
     test_output_directory = tempfile.TemporaryDirectory()
     conf_without_temp_dir = HiveConfig.build(
         Path(
             resource_filename(
                 "nrel.hive.resources.scenarios.denver_downtown",
                 "denver_demo.yaml",
@@ -580,15 +711,15 @@
         def close(self, runner_payload: RunnerPayload):
             pass
 
     return MockReporter()
 
 
 def mock_route_from_geoids(src: GeoId, dst: GeoId, speed_kmph: Kmph = 1) -> Tuple[Link, ...]:
-    link = Link.build("1", src, dst, speed_kmph=speed_kmph)
+    link = Link.build(f"{src}-{dst}", src, dst, speed_kmph=speed_kmph)
     return (link,)
 
 
 def mock_graph_links(h3_res: int = 15, speed_kmph: Kmph = 1) -> Dict[str, Link]:
     """
     test_routetraversal is dependent on this graph topology + its attributes
     each link is approximately 1 kilometer
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/powercurve/normalized.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/powercurve/normalized.yaml`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/powertrain/normalized-electric.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/powertrain/normalized-electric.yaml`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/powertrain/normalized-gasoline.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/powertrain/normalized-gasoline.yaml`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/README.md` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Charging prices can be specified in two different ways:
+Charging prices are specified in a csv file and can be specified two different ways:
 
 1. Price per station with the following fields:
     - `time`: the time when the price becomes valid (allows for varible price schemes) 
     - `station_id`: which station this pricing applies to 
     - `charger_id`: which charger this pricing applies to 
     - `price_kwh`: the cost (in dollars) per kilowatthour of energy
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_station_id.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_station_id.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,20 @@
 
   # (required)
   stations_file: denver_demo_stations.csv
 
   # (optional) only used with `network_type: osm_network`
   road_network_file: downtown_denver_network.json
 
-  # (optional) outline a geofence for control purposes
-  geofence_file: downtown_denver.geojson
-
   # (optional) defaults to zero cost if not specified
   rate_structure_file: rate_structure.csv
 
   # (optional) defaults to zero cost if not specified
   charging_price_file: denver_charging_prices_by_geoid.csv
 
-  # (optional) default is no demand forecasting
-  demand_forecast_file: denver_demand.csv
-
 dispatcher:
 
 
   # (optional) how often should we issue dispatching instructions?  
   default_update_interval_seconds: 600
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo_constrained_charging.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo_constrained_charging.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,13 @@
   vehicles_file: denver_demo_vehicles.csv
   bases_file: denver_demo_bases.csv
   stations_file: denver_demo_stations_constrained.csv
   chargers_file: chargers_varied.csv
   mechatronics_file: mechatronics.yaml
   charging_price_file: denver_constrained_prices.csv
   rate_structure_file: rate_structure.csv
-  geofence_file: downtown_denver.geojson
-  demand_forecast_file: denver_demand.csv
   road_network_file: downtown_denver_network.json
 dispatcher:
   valid_dispatch_states:
     - Idle
     - Repositioning
   charging_search_type: nearest_shortest_queue  # "nearest_shortest_queue", or, "shortest_time_to_charge"
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_demo_fleets.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_demo_fleets.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 input:
   vehicles_file: denver_demo_vehicles.csv
   requests_file: denver_demo_fleets_requests.csv
   bases_file: denver_demo_fleets_bases.csv
   stations_file: denver_demo_fleets_stations.csv
   fleets_file: denver_duel_fleets.yaml
   road_network_file: downtown_denver_network.json
-  geofence_file: downtown_denver.geojson
   rate_structure_file: rate_structure.csv
   charging_price_file: denver_charging_prices_by_geoid.csv
-  demand_forecast_file: denver_demand.csv
 dispatcher:
   valid_dispatch_states:
     - Idle
     - Repositioning
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_no_stations.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_no_stations.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -45,26 +45,20 @@
 
   # (required)
   stations_file: denver_demo_no_stations.csv
 
   # (optional) only used with `network_type: osm_network`
   road_network_file: downtown_denver_network.json
 
-  # (optional) outline a geofence for control purposes
-  geofence_file: downtown_denver.geojson
-
   # (optional) defaults to zero cost if not specified
   rate_structure_file: rate_structure.csv
 
   # (optional) defaults to zero cost if not specified
   charging_price_file: denver_charging_prices_by_geoid.csv
 
-  # (optional) default is no demand forecasting
-  demand_forecast_file: denver_demand.csv
-
 dispatcher:
   # (optional) how often should we issue dispatching instructions?
   default_update_interval_seconds: 600
 
   # (optional) ingnore searching for any entity beyond this threshold
   max_search_radius_km: 100.0
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/denver_rl_toy.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/denver_rl_toy.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
   requests_file: denver_rl_toy_requests.csv
   vehicles_file: denver_rl_toy_vehicles.csv
   bases_file: denver_rl_toy_bases.csv
   stations_file: denver_rl_toy_stations.csv
   mechatronics_file: denver_rl_toy_mechatronics.yaml
   charging_price_file: denver_charging_prices_by_geoid.csv
   rate_structure_file: denver_rl_toy_rate_structure.csv
-  demand_forecast_file: denver_rl_toy_demand.csv
-  geofence_file: downtown_denver.geojson
 
 dispatcher:
   matching_range_km_threshold: 0
   charging_range_km_threshold: 5
   default_update_interval_seconds: 1800
   valid_dispatch_states:
     - Idle
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/fleets/README.md` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/fleets/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Fleets are specified with a yaml file.
 
 Each key represents the identifies of a fleet and then each sub key represents which entities are part of that fleet.
 
-For example, let's say we have the fleet file:
+For example, let's say we have this fleet file:
 
 ```yaml
 tnc_1:
   vehicles:
     - v1   
     - v2   
   stations:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/geofence/downtown_denver.geojson` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/geofence/downtown_denver.geojson`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_fleets_requests.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_fleets_requests.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_requests.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_requests.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/requests/denver_rl_toy_requests.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/requests/denver_rl_toy_requests.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/road_network/downtown_denver_network.json` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/road_network/downtown_denver_network.json`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/README.md` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Vehicles are specified as one vehicle per line with the following fields:
+Vehicles are specified as one vehicle per csv line with the following fields:
 
 - `vehicle_id`: a unique id for the vehicle
 - `lat`: the latitude of the vehicle starting location
 - `lon`: the longitude of the vehicle starting location
 - `mechatronics_id`: the identifier of the mechatronics that this vehicle is using
 - `initial_soc`: the initial state of charge for the vehicle
 - `schedule_id`: (optional) the schedule this vehicle should follow (human driver)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles_no_stations.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles_no_stations.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_rl_toy_vehicles.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_rl_toy_vehicles.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/charging_prices/nyc_fixed.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/charging_prices/nyc_fixed.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/geofence/nyc_single_polygon.geojson` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/geofence/nyc_single_polygon.geojson`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/manhattan.yaml` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/manhattan.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 sim:
   sim_name: manhattan_20k
   timestep_duration_seconds: 60
   request_cancel_time_seconds: 600
-  start_time: 0
-  end_time: 86400
+  start_time: "2014-12-21 00:00:00"
+  end_time: "2014-12-22 00:00:00"
   sim_h3_search_resolution: 7  # around 12ish hexes covering manhattan
 network:
   network_type: osm_network
 input:
   vehicles_file: nyc_200.csv
   requests_file: nyc_20k.csv
   bases_file: nyc_bases.csv
   stations_file: nyc_stations.csv
   road_network_file: manhattan_network.json
-  geofence_file: nyc_single_polygon.geojson
   rate_structure_file: rate_structure.csv
   charging_price_file: nyc_fixed.csv
-  demand_forecast_file: nyc_demand.csv
 dispatcher:
   valid_dispatch_states:
     - idle
     - repositioning
-    - reservebase 
-    - chargingbase 
-
-
+    - reservebase
+    - chargingbase
```

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/road_network/manhattan_network.json` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/road_network/manhattan_network.json`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/stations/nyc_stations.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/stations/nyc_stations.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_1200.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_1200.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_200.csv` & `nrel.hive-1.3.0/nrel/hive/resources/scenarios/manhattan/vehicles/nyc_200.csv`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/runner/environment.py` & `nrel.hive-1.3.0/nrel/hive/runner/environment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import NamedTuple, TYPE_CHECKING, FrozenSet, Optional
 
-from nrel.hive.reporting.reporter import Reporter
-
 import immutables
 
+from nrel.hive.reporting.reporter import Reporter
+
 if TYPE_CHECKING:
     from nrel.hive.model.energy.charger.charger import Charger
     from nrel.hive.model.vehicle.mechatronics.mechatronics_interface import MechatronicsInterface
     from nrel.hive.config import HiveConfig
     from nrel.hive.model.vehicle.schedules.schedule import ScheduleFunction
     from nrel.hive.util.typealiases import (
         ChargerId,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/runner/local_simulation_runner.py` & `nrel.hive-1.3.0/nrel/hive/runner/local_simulation_runner.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/runner/runner_payload.py` & `nrel.hive-1.3.0/nrel/hive/runner/runner_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from typing import NamedTuple, TYPE_CHECKING
 
-
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.update.update import Update
     from nrel.hive.runner.environment import Environment
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
 
 
 class RunnerPayload(NamedTuple):
```

### Comparing `nrel.hive-1.2.2/nrel/hive/runner/runner_payload_ops.py` & `nrel.hive-1.3.0/nrel/hive/runner/runner_payload_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Iterable, Tuple, Type, Union
-from returns.result import ResultE, Success, Failure
 
+from returns.result import ResultE, Success, Failure
 
+from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
+from nrel.hive.model.entity import Entity
 from nrel.hive.runner.runner_payload import RunnerPayload
 from nrel.hive.state.simulation_state.simulation_state_ops import (
     modify_entities_safe as _modify_entities_safe,
 )
-
-from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
 from nrel.hive.util.fp import throw_or_return
-from nrel.hive.model.entity import Entity
 
 
 def update_instruction_generator_safe(
     rp: RunnerPayload, ig: InstructionGenerator
 ) -> ResultE[RunnerPayload]:
     """
     Inject an updated InstructionGenerator into a runner payload
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_available.py` & `nrel.hive-1.3.0/nrel/hive/state/driver_state/autonomous_driver_state/autonomous_available.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-from multiprocessing.sharedctypes import Value
+from dataclasses import dataclass
 from typing import Tuple, Optional, TYPE_CHECKING
 
 from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.state.driver_state.autonomous_driver_state.autonomous_driver_attributes import (
     AutonomousDriverAttributes,
 )
 from nrel.hive.state.driver_state.driver_instruction_ops import (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/driver_state/driver_instruction_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/driver_state/driver_instruction_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 import logging
-from turtle import home
 from typing import Optional, TYPE_CHECKING, Tuple
 
 import h3
 
 from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.dispatcher.instruction.instructions import (
     ChargeBaseInstruction,
     DispatchBaseInstruction,
     IdleInstruction,
     RepositionInstruction,
 )
 from nrel.hive.dispatcher.instruction_generator.instruction_generator_ops import (
     instruct_vehicles_to_dispatch_to_station,
-    get_nearest_valid_station_distance,
 )
+from nrel.hive.model.energy.energytype import EnergyType
 from nrel.hive.model.entity import Entity
-from nrel.hive.util import TupleOps, H3Ops
-from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.charging_base import ChargingBase
+from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
-from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.util import TupleOps, H3Ops
+from nrel.hive.util.dict_ops import DictOps
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.runner.environment import Environment
     from nrel.hive.model.vehicle.vehicle import Vehicle
     from nrel.hive.model.base import Base
     from nrel.hive.model.energy.charger import Charger
@@ -67,22 +66,22 @@
         return None
     elif my_mechatronics.is_full(veh):
         return None
 
     chargers = tuple(
         filter(
             my_mechatronics.valid_charger,
-            [env.chargers[cid] for cid in my_station.state.keys()],
+            [env.chargers[cid] for cid in sorted(my_station.state.keys())],
         )
     )
     if not chargers:
         return None
     else:
         # take the lowest power charger
-        charger: Charger = sorted(chargers, key=lambda c: c.rate)[0]
+        charger: Charger = sorted(chargers, key=lambda c: (c.rate, c.id))[0]
         return ChargeBaseInstruction(veh.id, home_base.id, charger.id)
 
 
 def human_go_home(
     veh: Vehicle,
     home_base: Base,
     sim: SimulationState,
@@ -153,15 +152,15 @@
         if len(sim.r_search) == 0:
             # no requests in system, do nothing
             return None
         else:
             # find the most dense request search hex and sends vehicles to the center
             best_search_hex = sorted(
                 [(k, len(v)) for k, v in sim.r_search.items()],
-                key=lambda t: t[1],
+                key=lambda t: (t[1], t[0]),  # fallback to geoid (index 0) to break ties
                 reverse=True,
             )[0][0]
         destination = h3.h3_to_center_child(best_search_hex, sim.sim_h3_location_resolution)
         destination_link = sim.road_network.position_from_geoid(destination)
         return destination_link
 
     dest = _get_reposition_location()
@@ -228,23 +227,23 @@
     if not my_station:
         log.error(f"could not find station {my_base.station_id} for base {my_base.id}")
         return None
 
     chargers: Tuple[Charger, ...] = tuple(
         filter(
             my_mechatronics.valid_charger,
-            [cs.charger for cs in my_station.state.values()],
+            [cs.charger for cs in sorted(my_station.state.values(), key=lambda c: c.id)],
         )
     )
 
     if not chargers:
         return None
 
     # take the lowest power charger
-    charger: Charger = sorted(chargers, key=lambda c: c.rate)[0]
+    charger: Charger = sorted(chargers, key=lambda c: (c.rate, c.id))[0]
     return ChargeBaseInstruction(veh.id, my_base.id, charger.id)
 
 
 def av_dispatch_base_instruction(
     veh: Vehicle,
     sim: SimulationState,
     env: Environment,
@@ -269,15 +268,15 @@
 
         def valid_fn(base: Entity) -> bool:
             vehicle_has_access = base.membership.grant_access_to_membership(veh.membership)
             return vehicle_has_access
 
         best_base = H3Ops.nearest_entity_by_great_circle_distance(
             geoid=veh.geoid,
-            entities=sim.bases.values(),
+            entities=sim.get_bases(),
             entity_search=sim.b_search,
             is_valid=valid_fn,
             sim_h3_search_resolution=sim.sim_h3_search_resolution,
             max_search_distance_km=env.config.dispatcher.max_search_radius_km,
         )
 
         if best_base:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/driver_state/driver_state.py` & `nrel.hive-1.3.0/nrel/hive/state/driver_state/driver_state.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod, ABC
 from typing import Tuple, Optional, TYPE_CHECKING
 
-from nrel.hive.util import SimulationStateError
 from nrel.hive.state.simulation_state import simulation_state_ops
+from nrel.hive.util import SimulationStateError
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.runner.environment import Environment
     from nrel.hive.util.typealiases import ScheduleId, BaseId, VehicleId
     from nrel.hive.dispatcher.instruction.instruction import Instruction
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/human_driver_state.py` & `nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/human_driver_state.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
+from dataclasses import dataclass
 from typing import Tuple, Optional, TYPE_CHECKING
 
 from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.dispatcher.instruction.instructions import (
     DispatchBaseInstruction,
     ReserveBaseInstruction,
 )
@@ -26,18 +26,18 @@
 from nrel.hive.state.driver_state.human_driver_state.human_unavailable_charge_parameters import (
     HumanUnavailableChargeParameters,
 )
 from nrel.hive.state.vehicle_state.charging_base import ChargingBase
 from nrel.hive.state.vehicle_state.charging_station import ChargingStation
 from nrel.hive.state.vehicle_state.dispatch_base import DispatchBase
 from nrel.hive.state.vehicle_state.dispatch_station import DispatchStation
-from nrel.hive.state.vehicle_state.out_of_service import OutOfService
-from nrel.hive.state.vehicle_state.servicing_trip import ServicingTrip
 from nrel.hive.state.vehicle_state.idle import Idle
+from nrel.hive.state.vehicle_state.out_of_service import OutOfService
 from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
+from nrel.hive.state.vehicle_state.servicing_trip import ServicingTrip
 from nrel.hive.util import SimulationStateError, BaseId
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.runner.environment import Environment
     from nrel.hive.util.typealiases import ScheduleId
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/driver_state/human_driver_state/human_unavailable_charge_parameters.py` & `nrel.hive-1.3.0/nrel/hive/state/driver_state/human_driver_state/human_unavailable_charge_parameters.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/state/entity_state/entity_state_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/entity_state/entity_state_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import Tuple, Optional, TYPE_CHECKING
 
 from nrel.hive.util.exception import StateTransitionError
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.state.vehicle_state.vehicle_state import VehicleState
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/at_location_response.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/at_location_response.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/simulation_state_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/simulation_state_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-from typing import Iterable, Optional, TYPE_CHECKING, Tuple, cast
+from typing import Iterable, Optional, TYPE_CHECKING, Tuple
 
 import h3
-import immutables
 from returns.result import Success, Failure, ResultE
 
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.util.dict_ops import DictOps
 from nrel.hive.util.exception import SimulationStateError
 from nrel.hive.util.fp import apply_op_to_accumulator, throw_or_return
 from nrel.hive.util.typealiases import RequestId, StationId, VehicleId, BaseId
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/cancel_requests.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/cancel_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import functools as ft
-from typing import Tuple, Optional, NamedTuple
+import logging
+from dataclasses import dataclass
+from typing import Tuple, Optional
 
+from nrel.hive.reporting.reporter import Report, ReportType
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.update.simulation_update import SimulationUpdateFunction
 from nrel.hive.util.typealiases import RequestId
-from nrel.hive.reporting.reporter import Report, ReportType
-
-import logging
 
 log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class CancelRequests(SimulationUpdateFunction):
     def update(
@@ -58,15 +57,15 @@
                     return sim
                 else:
                     env.reporter.file_report(_gen_report(request_id, sim))
                     return updated_sim
 
         updated = ft.reduce(
             _remove_from_sim,
-            simulation_state.requests.keys(),
+            simulation_state.get_request_ids(),
             simulation_state,
         )
 
         return updated, None
 
 
 def _gen_report(r_id: RequestId, sim: SimulationState) -> Report:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/charging_price_update.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/charging_price_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import functools as ft
 import logging
 from csv import DictReader
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Tuple, Optional, Dict
 
-import immutables
 import h3
+import immutables
 
-from nrel.hive.model.energy.charger import Charger, build_chargers_table
+from nrel.hive.model.energy.charger import build_chargers_table
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.update.simulation_update import SimulationUpdateFunction
-from nrel.hive.util.iterators import DictReaderStepper
 from nrel.hive.util import DictOps
+from nrel.hive.util.iterators import DictReaderStepper
 from nrel.hive.util.typealiases import StationId, ChargerId
 from nrel.hive.util.units import Currency
 
 log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
@@ -127,24 +127,26 @@
 
         elif self.use_defaults:
             # we are applying the same values across all Stations
             # the default constructor creates one station_id called "default" and we
             # apply it to every station here.
             result = ft.reduce(
                 lambda sim, s_id: _update_station_prices(sim, s_id, charger_update["default"]),
-                sim_state.stations.keys(),
+                sim_state.get_station_ids(),
                 sim_state,
             )
             return result, self
 
         else:
             # apply update to all stations
             # if these updates are in the form of GeoIds, map them to StationIds
             as_station_updates = _map_to_station_ids(charger_update, sim_state)
-            station_ids_to_update = set(sim_state.stations.keys()).union(as_station_updates.keys())
+            station_ids_to_update = set(sim_state.get_station_ids()).union(
+                as_station_updates.keys()
+            )
 
             # we are applying only the updates related to valid StationIds with updates
             result = ft.reduce(
                 lambda sim, s_id: _update_station_prices(sim, s_id, as_station_updates[s_id]),
                 station_ids_to_update,
                 sim_state,
             )
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/simulation_update.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/simulation_update.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/step_simulation.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/step_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
-import logging
 import inspect
-from typing import Tuple, Optional, NamedTuple, TYPE_CHECKING, Type, Union
+import logging
+from dataclasses import dataclass, replace
+from typing import Tuple, TYPE_CHECKING, Type, Union
 
 import immutables
-
 from returns.result import ResultE, Failure, Success
-from nrel.hive.dispatcher.instruction.instruction import Instruction
 
+from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import (
     InstructionGenerator,
     InstructionGeneratorId,
 )
 from nrel.hive.dispatcher.instruction_generator.instruction_generator_ops import (
     generate_instructions,
 )
@@ -94,15 +93,15 @@
 
         i_stack, updated_i_gens = generate_instructions(
             self.ordered_instruction_generators, sim_with_drivers_updated, env
         )
 
         # pops the top instruction from the stack. this could be replaced with something like a priority queue
         final_instructions: Tuple[Instruction, ...] = ()
-        for vid in i_stack.keys():
+        for vid in sorted(i_stack.keys()):
             i, _ = DictOps.pop_from_stack_dict(i_stack, vid)
             if not i:
                 continue
             else:
                 final_instructions = (i,) + final_instructions
 
         log_instructions(final_instructions, env, simulation_state.sim_time)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/step_simulation_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/step_simulation_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from __future__ import annotations
-from dataclasses import asdict
 
 import functools as ft
 import logging
+from dataclasses import asdict
 from typing import List, Tuple, Optional, TYPE_CHECKING, Callable, NamedTuple
 
 from nrel.hive.dispatcher.instruction.instruction import Instruction
 from nrel.hive.dispatcher.instruction.instruction_result import InstructionResult
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
 from nrel.hive.state.entity_state import entity_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
-from nrel.hive.state.simulation_state.simulation_state_ops import tick
 from nrel.hive.state.vehicle_state.charge_queueing import ChargeQueueing
-from nrel.hive.util import TupleOps, SimulationStateError
+from nrel.hive.util import TupleOps
 
 if TYPE_CHECKING:
     from nrel.hive.runner.environment import Environment
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
     from nrel.hive.model.sim_time import SimTime
-    from nrel.hive.util.typealiases import VehicleId
 
 log = logging.getLogger(__name__)
 
 
 def _instruction_to_report(i: Instruction, sim_time: SimTime) -> Report:
     i_dict = asdict(i)
     i_dict["sim_time"] = sim_time
@@ -68,15 +66,15 @@
             log.error(error)
             return simulation_state
         elif not updated_sim:
             return simulation_state
         else:
             return updated_sim
 
-    next_state = ft.reduce(_step_drivers, simulation_state.vehicles.values(), simulation_state)
+    next_state = ft.reduce(_step_drivers, simulation_state.get_vehicles(), simulation_state)
     return next_state
 
 
 def perform_vehicle_state_updates(
     simulation_state: SimulationState, env: Environment
 ) -> SimulationState:
     """
@@ -99,26 +97,30 @@
         :param vs: the vehicles
         :return: the vehicles with all ChargeQueueing vehicles at the tail
         """
         charge_queueing_vehicles, other_vehicles = TupleOps.partition(
             lambda v: isinstance(v.vehicle_state, ChargeQueueing), vs
         )
 
+        # sort queueing vehicles by enqueue time followed by id as a
+        # deterministic tie-breaker via their VehicleId
         sorted_charge_queueing_vehicles = tuple(
             sorted(
                 charge_queueing_vehicles,
-                key=lambda v: v.vehicle_state.enqueue_time
+                key=lambda v: (v.vehicle_state.enqueue_time, v.id)
                 if isinstance(v.vehicle_state, ChargeQueueing)
-                else 0,
+                else (0, v.id),
             )
         )
+        sorted_other_vehicles = tuple(sorted(other_vehicles, key=lambda v: v.id))
+        return sorted_other_vehicles + sorted_charge_queueing_vehicles
 
-        return other_vehicles + sorted_charge_queueing_vehicles
-
-    # why sort here? see _sort_by_vehicle_state for an explanation
+    # why sort here? see _sort_by_vehicle_state (above) for an explanation
+    # this code doesn't use built-in sorting iterator methods because of the
+    # initial partitioning step required.
     vehicles = _sort_by_vehicle_state(tuple(simulation_state.vehicles.values()))
 
     for veh in vehicles:
         simulation_state = step_vehicle(simulation_state, env, veh)
 
     return simulation_state
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import functools as ft
-from typing import NamedTuple, Tuple, TYPE_CHECKING, Callable, Optional
+from typing import NamedTuple, Tuple, TYPE_CHECKING
 
 import immutables
 
 from nrel.hive.config import HiveConfig
 from nrel.hive.dispatcher.instruction_generator.instruction_generator import InstructionGenerator
-from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.update.cancel_requests import CancelRequests
 from nrel.hive.state.simulation_state.update.charging_price_update import ChargingPriceUpdate
 from nrel.hive.state.simulation_state.update.simulation_update import SimulationUpdateFunction
 from nrel.hive.state.simulation_state.update.step_simulation import StepSimulation
 from nrel.hive.state.simulation_state.update.update_requests_from_file import UpdateRequestsFromFile
 
 if TYPE_CHECKING:
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update_requests_from_file.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update_requests_from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import functools as ft
 import logging
 from csv import DictReader
+from dataclasses import dataclass
 from pathlib import Path
-from typing import NamedTuple, Tuple, Optional, Iterator, Dict
+from typing import Tuple, Optional, Iterator, Dict
 
 from returns.result import Failure
 
 from nrel.hive.model.request import Request, RequestRateStructure
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.reporting.reporter import Report, ReportType
 from nrel.hive.runner.environment import Environment
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/simulation_state/update/update_requests_sampling.py` & `nrel.hive-1.3.0/nrel/hive/state/simulation_state/update/update_requests_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import functools as ft
 import logging
 from csv import DictReader
+from dataclasses import dataclass
 from pathlib import Path
-from typing import NamedTuple, Tuple, Optional
+from typing import Tuple, Optional
 
 from returns.result import Failure
 
 from nrel.hive.model.request import RequestRateStructure, Request
 from nrel.hive.reporting.report_type import ReportType
 from nrel.hive.reporting.reporter import Report
 from nrel.hive.runner.environment import Environment
-from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state import simulation_state_ops
+from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.update.simulation_update import SimulationUpdateFunction
 from nrel.hive.util.iterators import ObjectIterator
 
 log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charge_queueing.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charge_queueing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
+from dataclasses import dataclass
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.model.sim_time import SimTime
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.charging_station import ChargingStation
 from nrel.hive.state.vehicle_state.vehicle_state import (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charging_base.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charging_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-from typing import Tuple, Optional, NamedTuple, TYPE_CHECKING
+from dataclasses import dataclass
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/charging_station.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/charging_station.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
-from typing import Tuple, Optional, NamedTuple, TYPE_CHECKING
 import uuid
+from dataclasses import dataclass, replace
+from typing import Tuple, Optional, TYPE_CHECKING
 
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_base.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
+
 import logging
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
+from dataclasses import dataclass, replace
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_cooresponds_with_entities,
 )
 from nrel.hive.runner.environment import Environment
+from nrel.hive.state.vehicle_state import vehicle_state_ops
+from nrel.hive.state.vehicle_state.idle import Idle
+from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
 )
-from nrel.hive.state.vehicle_state import vehicle_state_ops
-from nrel.hive.state.vehicle_state.idle import Idle
-from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
 from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
 from nrel.hive.util.exception import SimulationStateError
 from nrel.hive.util.typealiases import BaseId, VehicleId
 
 if TYPE_CHECKING:
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_ops.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools as ft
 from typing import Tuple, Optional
 
-from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.model.entity_position import EntityPosition
+from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.model.vehicle.trip_phase import TripPhase
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.vehicle_state.dispatch_pooling_trip import DispatchPoolingTrip
 from nrel.hive.state.vehicle_state.servicing_pooling_trip import ServicingPoolingTrip
 from nrel.hive.util import (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_pooling_trip.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_pooling_trip.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
+from dataclasses import dataclass, replace
 from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 import immutables
 
 from nrel.hive.model.request import Request
 from nrel.hive.model.roadnetwork.route import (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_station.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_station.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
+from dataclasses import dataclass, replace
 from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_cooresponds_with_entities,
 )
 from nrel.hive.runner.environment import Environment
+from nrel.hive.state.vehicle_state import vehicle_state_ops
 from nrel.hive.state.vehicle_state.charge_queueing import ChargeQueueing
 from nrel.hive.state.vehicle_state.charging_station import ChargingStation
-from nrel.hive.state.vehicle_state import vehicle_state_ops
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
 )
 from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
 from nrel.hive.util.exception import SimulationStateError
 from nrel.hive.util.typealiases import StationId, VehicleId, ChargerId
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/dispatch_trip.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/dispatch_trip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
+from dataclasses import dataclass, replace
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 import immutables
 
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_cooresponds_with_entities,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/idle.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/idle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
-
+from dataclasses import dataclass, replace
 from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.out_of_service import OutOfService
 from nrel.hive.state.vehicle_state.vehicle_state import (
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/out_of_service.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/out_of_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass
-
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
 
+from dataclasses import dataclass
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
 )
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/repositioning.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/repositioning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
+
 from dataclasses import dataclass, replace
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_cooresponds_with_entities,
 )
 from nrel.hive.runner.environment import Environment
-from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state import vehicle_state_ops
 from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
 )
 from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/reserve_base.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/reserve_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass
 
 import logging
-from typing import NamedTuple, Tuple, Optional, TYPE_CHECKING
+from dataclasses import dataclass
+from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.runner.environment import Environment
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.vehicle_state import (
     VehicleState,
     VehicleStateInstanceId,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_ops.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
-from dataclasses import replace
 
+from dataclasses import replace
 from typing import Optional, Tuple, TYPE_CHECKING, NamedTuple
 
 from nrel.hive.model.request import Request
 from nrel.hive.model.roadnetwork.route import Route
 from nrel.hive.model.vehicle.trip_phase import TripPhase
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.vehicle_event_ops import (
     report_pickup_request,
     report_dropoff_request,
 )
 from nrel.hive.runner import Environment
-from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.simulation_state import SimulationState
 from nrel.hive.state.simulation_state.simulation_state_ops import modify_vehicle
+from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
 from nrel.hive.util import RequestId, TupleOps, SimulationStateError, VehicleId
 
 if TYPE_CHECKING:
     from nrel.hive.state.vehicle_state.servicing_pooling_trip import ServicingPoolingTrip
 
 
 class ActivePoolingTrip(NamedTuple):
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_pooling_trip.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_pooling_trip.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
+from dataclasses import dataclass, replace
 from typing import Tuple, TYPE_CHECKING, Optional
 from uuid import uuid4
 
 import immutables
 
 from nrel.hive.model.request import Request
 from nrel.hive.model.roadnetwork.route import Route
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/servicing_trip.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/servicing_trip.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from dataclasses import dataclass, replace
 
 import logging
+from dataclasses import dataclass, replace
 from typing import Tuple, Optional, TYPE_CHECKING
 from uuid import uuid4
 
 from nrel.hive.model.request import Request
 from nrel.hive.model.roadnetwork.route import (
     Route,
     route_cooresponds_with_entities,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/vehicle_state.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/vehicle_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
-from dataclasses import dataclass
-
-from uuid import UUID
 
+import logging
 from abc import abstractmethod, ABC
+from dataclasses import dataclass
 from typing import Tuple, Optional, TYPE_CHECKING
+from uuid import UUID
 
 from nrel.hive.state.entity_state import entity_state_ops
 from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.vehicle_state_type import VehicleStateType
 from nrel.hive.util.exception import SimulationStateError, StateTransitionError
 from nrel.hive.util.typealiases import VehicleId
 
-import logging
-
 if TYPE_CHECKING:
     from nrel.hive.runner.environment import Environment
     from nrel.hive.state.simulation_state.simulation_state import SimulationState
 
 log = logging.getLogger(__name__)
 
 VehicleStateInstanceId = UUID
```

### Comparing `nrel.hive-1.2.2/nrel/hive/state/vehicle_state/vehicle_state_ops.py` & `nrel.hive-1.3.0/nrel/hive/state/vehicle_state/vehicle_state_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Tuple, Optional, NamedTuple, TYPE_CHECKING
-
+import immutables
 from nrel.hive.model.entity_position import EntityPosition
-from nrel.hive.model.roadnetwork.route import Route, empty_route
+from nrel.hive.model.roadnetwork.route import empty_route
 from nrel.hive.model.roadnetwork.routetraversal import traverse, RouteTraversal
 from nrel.hive.model.vehicle.vehicle import Vehicle
 from nrel.hive.reporting.vehicle_event_ops import (
     vehicle_move_event,
     vehicle_charge_event,
 )
 from nrel.hive.state.simulation_state import simulation_state_ops
@@ -34,15 +34,17 @@
     :param sim: the simulation state
     :param env: the simulation environment
     :param vehicle_id: the vehicle transitioning
     :param station_id: the station where we are charging
     :param charger_id: the charger_id we are using
     :return: an exception due to failure or an optional updated simulation
     """
-    context = f"vehicle {vehicle_id} attempting to charge at station {station_id} with charger {charger_id}"
+    context = f"""
+    vehicle {vehicle_id} attempting to charge at station {station_id} with charger {charger_id}"
+    """
 
     vehicle = sim.vehicles.get(vehicle_id)
     mechatronics = env.mechatronics.get(vehicle.mechatronics_id) if vehicle else None
     station = sim.stations.get(station_id)
     if station is None:
         return (
             SimulationStateError(f"station not found; context {context}"),
@@ -93,14 +95,17 @@
         )  # kwh
         charger_price = station.get_price(charger_id)  # Currency
         charging_price = kwh_transacted * charger_price if charger_price else 0.0
 
         # perform updates
         updated_vehicle = charged_vehicle.send_payment(charging_price)
         updated_station = station.receive_payment(charging_price)
+        updated_station = updated_station.tick_energy_dispensed(
+            immutables.Map({charger.energy_type: kwh_transacted})
+        )
 
         veh_error, sim_with_vehicle = simulation_state_ops.modify_vehicle(sim, updated_vehicle)
         if veh_error:
             response = SimulationStateError(f"failure during charge for vehicle {vehicle.id}")
             response.__cause__ = veh_error
             return response, None
         elif sim_with_vehicle is None:
@@ -135,15 +140,16 @@
 
     :param sim: the sim before the move event
     :param env: the sim environment
     :param vehicle_id: the vehicle that moved and ran out of energy
     :return: an optional error, or an optional sim with the out of service vehicle
     """
     # TODO: ways we can improve this:
-    # - find the exact point in the route where a vehicle runs out of energy and move it there before transitioning
+    # - find the exact point in the route where a vehicle runs out of
+    #   energy and move it there before transitioning
     #   to out of service.
     # - report stranded passengers if we're servicing a trip when this happens.
     next_state = OutOfService.build(vehicle_id)
     return next_state.enter(sim, env)
 
 
 def move(
@@ -175,38 +181,40 @@
         )
 
     if not hasattr(vehicle.vehicle_state, "route"):
         return (
             SimulationStateError(f"vehicle state does not have route; context {context}"),
             None,
         )
-    elif not hasattr(vehicle.vehicle_state, "update_route"):
-        return (
-            SimulationStateError(
-                f"vehicle state does not have update_route method; context {context}"
-            ),
-            None,
-        )
     else:
         route = vehicle.vehicle_state.route
 
     error, traverse_result = traverse(
         route_estimate=route,
         duration_seconds=int(sim.sim_timestep_duration_seconds),
+        road_network=sim.road_network,
     )
     if error:
         return error, None
     elif traverse_result is None:
         return None, None
 
     if not traverse_result.experienced_route:
         # vehicle did not traverse so we set an empty route
-        # ignore mypy error since we explicitly check for attribute above
-        updated_vehicle_state = vehicle.vehicle_state.update_route(route=empty_route())  # type: ignore
-        updated_vehicle = vehicle.modify_vehicle_state(updated_vehicle_state)
+        if not hasattr(vehicle.vehicle_state, "update_route"):
+            return (
+                SimulationStateError(
+                    f"vehicle state does not have update_route method; context {context}"
+                ),
+                None,
+            )
+        else:
+            er = empty_route()
+            updated_vehicle_state = vehicle.vehicle_state.update_route(route=er)
+            updated_vehicle = vehicle.modify_vehicle_state(updated_vehicle_state)
     else:
         experienced_route = traverse_result.experienced_route
         remaining_route = traverse_result.remaining_route
         less_energy_vehicle = mechatronics.consume_energy(vehicle, experienced_route)
         if mechatronics.is_empty(less_energy_vehicle):
             # impossible to move, let's transition to OutOfService
             return _go_out_of_service_on_empty(sim, env, vehicle_id)
@@ -215,20 +223,27 @@
         last_link_traversed = experienced_route[-1]
 
         vehicle_position = EntityPosition(last_link_traversed.link_id, last_link_traversed.end)
         new_position_vehicle = less_energy_vehicle.modify_position(
             position=vehicle_position
         ).tick_distance_traveled_km(step_distance_km)
 
-        # ignore mypy error since we explicitly check for attribute above
-        new_route_state = new_position_vehicle.vehicle_state.update_route(route=remaining_route)  # type: ignore
-        updated_vehicle = new_position_vehicle.modify_vehicle_state(new_route_state)
+        if not hasattr(new_position_vehicle.vehicle_state, "update_route"):
+            return (
+                SimulationStateError(
+                    f"vehicle state does not have update_route method; context {context}"
+                ),
+                None,
+            )
+        else:
+            new_route_state = new_position_vehicle.vehicle_state.update_route(route=remaining_route)
+            updated_vehicle = new_position_vehicle.modify_vehicle_state(new_route_state)
 
-        report = vehicle_move_event(sim, vehicle, updated_vehicle, traverse_result, env)
-        env.reporter.file_report(report)
+            report = vehicle_move_event(sim, vehicle, updated_vehicle, traverse_result, env)
+            env.reporter.file_report(report)
 
     error, moved_sim = simulation_state_ops.modify_vehicle(sim, updated_vehicle)
     if error:
         response = SimulationStateError(
             f"failure during _apply_route_traversal for vehicle {vehicle.id}"
         )
         response.__cause__ = error
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/__init__.py` & `nrel.hive-1.3.0/nrel/hive/util/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from nrel.hive.util.iterators import DictReaderStepper
+from nrel.hive.util.dict_ops import DictOps
 from nrel.hive.util.exception import (
     StateOfChargeError,
     StateTransitionError,
     SimulationStateError,
     RouteStepError,
     EntityError,
     UnitError,
     H3Error,
 )
 from nrel.hive.util.h3_ops import H3Ops
-from nrel.hive.util.dict_ops import DictOps
+from nrel.hive.util.iterators import DictReaderStepper
 from nrel.hive.util.tuple_ops import TupleOps
 from nrel.hive.util.typealiases import (
     RequestId,
     VehicleId,
     StationId,
     BaseId,
     PowertrainId,
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/exception.py` & `nrel.hive-1.3.0/nrel/hive/util/exception.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/util/fp.py` & `nrel.hive-1.3.0/nrel/hive/util/fp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import functools as ft
 from typing import Any, Callable, Iterable, TypeVar
-from returns.io import IOResult
+
 from returns.result import ResultE, Success, Failure
 from returns.unsafe import unsafe_perform_io
 
-import functools as ft
-
 
 def throw_on_failure(io_result):
     """
     helper that throws an io result if it contains a Failure
 
     should only be used in the hive.app module (at the "end-of-the-world").
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/fs.py` & `nrel.hive-1.3.0/nrel/hive/util/fs.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/util/geo.py` & `nrel.hive-1.3.0/nrel/hive/util/geo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import h3
 
-from nrel.hive.util import GeoId, SimulationStateError
+from nrel.hive.util import GeoId
 
 
 def same_simulation_location(
     a: GeoId,
     b: GeoId,
     sim_h3_resolution: int,
     override_resolution: Optional[int],
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/h3_ops.py` & `nrel.hive-1.3.0/nrel/hive/util/h3_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
-from math import radians, cos, sin, asin, sqrt, ceil
 from typing import Any, Dict, Optional, TYPE_CHECKING, FrozenSet, Iterable, Callable, Tuple
 
 import h3
 import immutables
+from math import radians, cos, sin, asin, sqrt, ceil
+from nrel.hive.util.dict_ops import DictOps
 
 from nrel.hive.util.exception import H3Error
 from nrel.hive.util.typealiases import EntityId, GeoId
 from nrel.hive.util.units import Kilometers, Seconds, SECONDS_TO_HOURS
 
 if TYPE_CHECKING:
     from nrel.hive.model.entity import Entity
@@ -144,15 +145,15 @@
             return found
 
     @classmethod
     def nearest_entity_point_to_point(
         cls,
         geoid: GeoId,
         entities: Dict[EntityId, Entity],
-        entity_locations: Dict[GeoId, Tuple[EntityId, ...]],
+        entity_locations: immutables.Map[GeoId, Tuple[EntityId, ...]],
         is_valid: Callable = lambda x: True,
     ) -> Optional[Entity]:
         """
         A nearest neighbor search that scans all entities and returns the one with the lowest distance to the geoid.
 
 
         :param geoid: GeoId to match to
@@ -160,15 +161,15 @@
         :param entity_locations: Location of entities
         :param is_valid: Optional function to filter for valid entities
         :return: an optional entity if found
         """
 
         best_dist_km = 1000000.0
         best_e = None
-        for e_geoid, e_ids in entity_locations.items():
+        for e_geoid, e_ids in DictOps.iterate_items(entity_locations):
             dist_km = cls.great_circle_distance(geoid, e_geoid)
             for e_id in e_ids:
                 if e_id not in entities:
                     continue
                 e = entities[e_id]
                 if dist_km < best_dist_km and is_valid(e):
                     best_dist_km = dist_km
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/iterators.py` & `nrel.hive-1.3.0/nrel/hive/util/iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from __future__ import annotations
 
 import csv
 import logging
+from itertools import islice, tee
 from pathlib import Path
 from typing import (
     Iterator,
     Dict,
     TextIO,
     Optional,
     Callable,
     Tuple,
     Any,
-    NamedTuple,
     Iterable,
     Generator,
     Union,
 )
 
-from itertools import islice, tee
-
 log = logging.getLogger(__name__)
 
 
 class ObjectIterator:
     """
     iterator that deals with a set of named tuples
     """
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/time_helpers.py` & `nrel.hive-1.3.0/nrel/hive/util/time_helpers.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/util/tuple_ops.py` & `nrel.hive-1.3.0/nrel/hive/util/tuple_ops.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/util/typealiases.py` & `nrel.hive-1.3.0/nrel/hive/util/typealiases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Tuple, FrozenSet
 
 from immutables import Map
 
-
 # MODEL ID TYPES
 RequestId = str
 VehicleId = str
 StationId = str
 PowertrainId = str
 PowercurveId = str
 BaseId = str
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/units.py` & `nrel.hive-1.3.0/nrel/hive/util/units.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from typing import Dict
 from enum import Enum, auto
+from typing import Dict
 
 
 class Unit(Enum):
     MPH = auto()
     KMPH = auto()
     MILES = auto()
     KILOMETERS = auto()
```

### Comparing `nrel.hive-1.2.2/nrel/hive/util/validation.py` & `nrel.hive-1.3.0/nrel/hive/util/validation.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/nrel/hive/util/wkt.py` & `nrel.hive-1.3.0/nrel/hive/util/wkt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Tuple
-
 import functools as ft
+from typing import Tuple
 
 
 def polygon_empty() -> str:
     return "POLYGON EMPTY"
 
 
 def _point_to_string(point: Tuple[float, float], x_y_ordering: bool) -> str:
```

### Comparing `nrel.hive-1.2.2/nrel.hive.egg-info/SOURCES.txt` & `nrel.hive-1.3.0/nrel.hive.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 nrel/hive/__init__.py
 nrel/hive/__main__.py
 nrel/hive/py.typed
 nrel/hive/app/__init__.py
 nrel/hive/app/hive_cosim.py
 nrel/hive/app/run.py
 nrel/hive/app/run_batch.py
-nrel/hive/app/run_tune.py
 nrel/hive/config/__init__.py
 nrel/hive/config/config_builder.py
 nrel/hive/config/dispatcher_config.py
 nrel/hive/config/global_config.py
 nrel/hive/config/hive_config.py
 nrel/hive/config/input.py
 nrel/hive/config/network.py
@@ -37,14 +36,15 @@
 nrel/hive/dispatcher/instruction/instruction_result.py
 nrel/hive/dispatcher/instruction/instructions.py
 nrel/hive/dispatcher/instruction_generator/__init__.py
 nrel/hive/dispatcher/instruction_generator/assignment_ops.py
 nrel/hive/dispatcher/instruction_generator/charging_fleet_manager.py
 nrel/hive/dispatcher/instruction_generator/charging_search_type.py
 nrel/hive/dispatcher/instruction_generator/dispatcher.py
+nrel/hive/dispatcher/instruction_generator/instruction_function.py
 nrel/hive/dispatcher/instruction_generator/instruction_generator.py
 nrel/hive/dispatcher/instruction_generator/instruction_generator_ops.py
 nrel/hive/initialization/__init__.py
 nrel/hive/initialization/initialize_ops.py
 nrel/hive/initialization/initialize_simulation.py
 nrel/hive/initialization/initialize_simulation_with_sampling.py
 nrel/hive/initialization/load.py
@@ -108,28 +108,30 @@
 nrel/hive/reporting/reporter.py
 nrel/hive/reporting/reporter_ops.py
 nrel/hive/reporting/vehicle_event_ops.py
 nrel/hive/reporting/handler/__init__.py
 nrel/hive/reporting/handler/eventful_handler.py
 nrel/hive/reporting/handler/handler.py
 nrel/hive/reporting/handler/instruction_handler.py
+nrel/hive/reporting/handler/kepler_feature.py
+nrel/hive/reporting/handler/kepler_handler.py
 nrel/hive/reporting/handler/stateful_handler.py
 nrel/hive/reporting/handler/stats_handler.py
 nrel/hive/reporting/handler/summary_stats.py
 nrel/hive/reporting/handler/time_step_stats_handler.py
 nrel/hive/reporting/handler/vehicle_charge_events_handler.py
-nrel/hive/resources/.DS_Store
 nrel/hive/resources/__init__.py
 nrel/hive/resources/mock_lobster.py
 nrel/hive/resources/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/__pycache__/__init__.cpython-37.pyc
 nrel/hive/resources/__pycache__/__init__.cpython-38.pyc
 nrel/hive/resources/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/__pycache__/mock_lobster.cpython-310.pyc
 nrel/hive/resources/__pycache__/mock_lobster.cpython-38.pyc
+nrel/hive/resources/__pycache__/mock_lobster.cpython-39.pyc
 nrel/hive/resources/chargers/__init__.py
 nrel/hive/resources/chargers/default_chargers.csv
 nrel/hive/resources/chargers/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/chargers/__pycache__/__init__.cpython-37.pyc
 nrel/hive/resources/chargers/__pycache__/__init__.cpython-38.pyc
 nrel/hive/resources/chargers/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/defaults/.hive.yaml
@@ -154,21 +156,19 @@
 nrel/hive/resources/powertrain/__init__.py
 nrel/hive/resources/powertrain/normalized-electric.yaml
 nrel/hive/resources/powertrain/normalized-gasoline.yaml
 nrel/hive/resources/powertrain/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/powertrain/__pycache__/__init__.cpython-37.pyc
 nrel/hive/resources/powertrain/__pycache__/__init__.cpython-38.pyc
 nrel/hive/resources/powertrain/__pycache__/__init__.cpython-39.pyc
-nrel/hive/resources/scenarios/.DS_Store
 nrel/hive/resources/scenarios/__init__.py
 nrel/hive/resources/scenarios/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/__pycache__/__init__.cpython-37.pyc
 nrel/hive/resources/scenarios/__pycache__/__init__.cpython-38.pyc
 nrel/hive/resources/scenarios/__pycache__/__init__.cpython-39.pyc
-nrel/hive/resources/scenarios/denver_downtown/.DS_Store
 nrel/hive/resources/scenarios/denver_downtown/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/denver_demo.yaml
 nrel/hive/resources/scenarios/denver_downtown/denver_demo_constrained_charging.yaml
 nrel/hive/resources/scenarios/denver_downtown/denver_demo_fleets.yaml
 nrel/hive/resources/scenarios/denver_downtown/denver_no_stations.yaml
 nrel/hive/resources/scenarios/denver_downtown/denver_rl_toy.yaml
 nrel/hive/resources/scenarios/denver_downtown/__pycache__/__init__.cpython-310.pyc
@@ -188,71 +188,70 @@
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_geoid.csv
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_charging_prices_by_station_id.csv
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_constrained_prices.csv
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/denver_rl_toy_charging_prices.csv
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-38.pyc
-nrel/hive/resources/scenarios/denver_downtown/demand_forecast/__init__.py
-nrel/hive/resources/scenarios/denver_downtown/demand_forecast/denver_demand.csv
-nrel/hive/resources/scenarios/denver_downtown/demand_forecast/denver_rl_toy_demand.csv
+nrel/hive/resources/scenarios/denver_downtown/charging_prices/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/denver_downtown/fleets/README.md
 nrel/hive/resources/scenarios/denver_downtown/fleets/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/fleets/denver_duel_fleets.yaml
 nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-38.pyc
+nrel/hive/resources/scenarios/denver_downtown/fleets/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/denver_downtown/geofence/README.md
 nrel/hive/resources/scenarios/denver_downtown/geofence/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/geofence/downtown_denver.geojson
 nrel/hive/resources/scenarios/denver_downtown/mechatronics/README.md
 nrel/hive/resources/scenarios/denver_downtown/mechatronics/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/mechatronics/denver_rl_toy_mechatronics.yaml
 nrel/hive/resources/scenarios/denver_downtown/requests/README.md
 nrel/hive/resources/scenarios/denver_downtown/requests/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_fleets_requests.csv
 nrel/hive/resources/scenarios/denver_downtown/requests/denver_demo_requests.csv
 nrel/hive/resources/scenarios/denver_downtown/requests/denver_rl_toy_requests.csv
 nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-38.pyc
+nrel/hive/resources/scenarios/denver_downtown/requests/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/denver_downtown/road_network/README.md
 nrel/hive/resources/scenarios/denver_downtown/road_network/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/road_network/downtown_denver_network.json
 nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-38.pyc
+nrel/hive/resources/scenarios/denver_downtown/road_network/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/denver_downtown/service_prices/README.md
 nrel/hive/resources/scenarios/denver_downtown/service_prices/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/service_prices/denver_rl_toy_rate_structure.csv
 nrel/hive/resources/scenarios/denver_downtown/service_prices/rate_structure.csv
 nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-38.pyc
+nrel/hive/resources/scenarios/denver_downtown/service_prices/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/denver_downtown/stations/README.md
 nrel/hive/resources/scenarios/denver_downtown/stations/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_fleets_stations.csv
 nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_no_stations.csv
 nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations.csv
 nrel/hive/resources/scenarios/denver_downtown/stations/denver_demo_stations_constrained.csv
 nrel/hive/resources/scenarios/denver_downtown/stations/denver_rl_toy_stations.csv
 nrel/hive/resources/scenarios/denver_downtown/vehicles/README.md
 nrel/hive/resources/scenarios/denver_downtown/vehicles/__init__.py
 nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles.csv
 nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_demo_vehicles_no_stations.csv
 nrel/hive/resources/scenarios/denver_downtown/vehicles/denver_rl_toy_vehicles.csv
-nrel/hive/resources/scenarios/manhattan/.DS_Store
 nrel/hive/resources/scenarios/manhattan/__init__.py
 nrel/hive/resources/scenarios/manhattan/manhattan.yaml
 nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-310.pyc
 nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-37.pyc
 nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-38.pyc
 nrel/hive/resources/scenarios/manhattan/__pycache__/__init__.cpython-39.pyc
 nrel/hive/resources/scenarios/manhattan/bases/__init__.py
 nrel/hive/resources/scenarios/manhattan/bases/nyc_bases.csv
 nrel/hive/resources/scenarios/manhattan/charging_prices/__init__.py
 nrel/hive/resources/scenarios/manhattan/charging_prices/nyc_fixed.csv
-nrel/hive/resources/scenarios/manhattan/demand_forecast/__init__.py
-nrel/hive/resources/scenarios/manhattan/demand_forecast/nyc_demand.csv
 nrel/hive/resources/scenarios/manhattan/geofence/__init__.py
 nrel/hive/resources/scenarios/manhattan/geofence/nyc_single_polygon.geojson
 nrel/hive/resources/scenarios/manhattan/requests/__init__.py
 nrel/hive/resources/scenarios/manhattan/requests/nyc_20k.csv
 nrel/hive/resources/scenarios/manhattan/road_network/__init__.py
 nrel/hive/resources/scenarios/manhattan/road_network/manhattan_network.json
 nrel/hive/resources/scenarios/manhattan/service_prices/__init__.py
@@ -322,14 +321,15 @@
 nrel/hive/util/dict_ops.py
 nrel/hive/util/error_or_result.py
 nrel/hive/util/exception.py
 nrel/hive/util/fp.py
 nrel/hive/util/fs.py
 nrel/hive/util/geo.py
 nrel/hive/util/h3_ops.py
+nrel/hive/util/io.py
 nrel/hive/util/iterators.py
 nrel/hive/util/time_helpers.py
 nrel/hive/util/tuple_ops.py
 nrel/hive/util/typealiases.py
 nrel/hive/util/units.py
 nrel/hive/util/validation.py
 nrel/hive/util/wkt.py
@@ -348,16 +348,18 @@
 tests/test_haversine_roadnetwork.py
 tests/test_human_driver_state.py
 tests/test_ice_mechatronics.py
 tests/test_initialize_ops.py
 tests/test_initialize_simulation.py
 tests/test_instruction_generator_ops.py
 tests/test_instruction_generators.py
+tests/test_kepler_feature.py
 tests/test_local_simulation_runner.py
 tests/test_osm_roadnetwork.py
+tests/test_powercurve_ops.py
 tests/test_request.py
 tests/test_routetraversal.py
 tests/test_run_cosim.py
 tests/test_sample_functions.py
 tests/test_schedules.py
 tests/test_simulation_state_ops.py
 tests/test_simulationstate.py
```

### Comparing `nrel.hive-1.2.2/pyproject.toml` & `nrel.hive-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nrel.hive"
-version = "1.2.2"
+version = "1.3.0"
 description = "HIVE is a mobility services research platform developed by the Mobility and Advanced Powertrains (MBAP) group at the National Renewable Energy Laboratory in Golden, Colorado, USA."
 readme = "README.md"
 authors = [{ name = "National Renewable Energy Laboratory" }]
 license = { text = "BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
@@ -18,24 +18,23 @@
     "Programming Language :: Python :: 3.8",
     "Topic :: Scientific/Engineering",
 ]
 keywords = ["simulation", "transportation", "ride-sharing", "agent-based"]
 dependencies = [
     "immutables",
     "numpy",
-    "pandas",
     "networkx",
     "PyYAML",
     "tqdm",
     "rich",
     "h3 < 4",
     "scipy",
     "returns",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 docs = [
     "sphinx",
     "sphinx-autoapi",
     "sphinx-rtd-theme",
     "sphinxemoji",
@@ -46,26 +45,30 @@
     "nrel.hive[docs]",
     "pytest",
     "black==23.1.0",
     "mypy",
     "twine",
     "types-PyYAML",
     "types-setuptools",
+    "pre-commit",
 ]
 
 [project.urls]
 Homepage = "https://github.com/NREL/hive"
 
 [project.scripts]
 hive = "nrel.hive.app.run:run"
 hive-batch = "nrel.hive.app.run_batch:run"
 
 [tool.black]
 line-length = 100
 
+[tool.ruff]
+line-length = 100
+
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["nrel*"]  # package names should match these glob patterns (["*"] by default)
-exclude = ["rust*"] 
+exclude = ["rust*"]
 
 [tool.setuptools.package-data]
-"*" = ["py.typed"]
+"*" = ["py.typed"]
```

### Comparing `nrel.hive-1.2.2/tests/test_base.py` & `nrel.hive-1.3.0/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from csv import DictReader
 from unittest import TestCase
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+import pytest
+
+from nrel.hive.resources.mock_lobster import mock_base, mock_network
+from nrel.hive.model.base import Base
 
 
 class TestBase(TestCase):
     def test_from_row(self):
         source = """base_id,lat,lon,stall_count,station_id
                     b1,37,122,10,s1"""
 
@@ -86,7 +90,19 @@
         base = base.set_membership(("fleet_1", "fleet_3"))
 
         self.assertEqual(
             base.membership.memberships,
             frozenset(["fleet_1", "fleet_3"]),
             "should have membership for fleet_1 and fleet_3",
         )
+
+    def test_parse_error_raises(self):
+        source = """base_id,lat,lon,stall_count,station_id
+                            b1,thirtyseven,122,10,s1"""
+
+        network = mock_network()
+        row = next(DictReader(source.split()))
+
+        with pytest.raises(IOError, match="unable to parse id") as exc_info:
+            Base.from_row(row, network)
+
+        assert isinstance(exc_info.value.__cause__, ValueError)
```

### Comparing `nrel.hive-1.2.2/tests/test_bev_mechatronics.py` & `nrel.hive-1.3.0/tests/test_bev_mechatronics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from unittest import TestCase
+from nrel.hive.model.energy.energytype import EnergyType
 
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import (
+    mock_bev,
+    mock_dcfc_charger,
+    mock_l2_charger,
+    mock_route,
+    mock_vehicle,
+)
+from nrel.hive.util.units import KM_TO_MILE, MILE_TO_KM, hours_to_seconds
 
 
 class TestBEV(TestCase):
     def test_leaf_energy_gain_0_soc(self):
         bev = mock_bev(battery_capacity_kwh=50)
         vehicle = mock_vehicle(soc=0)
```

### Comparing `nrel.hive-1.2.2/tests/test_build_mechatronics_table.py` & `nrel.hive-1.3.0/tests/test_build_mechatronics_table.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/tests/test_cancel_requests.py` & `nrel.hive-1.3.0/tests/test_cancel_requests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest import TestCase
 
 from returns.result import Success
+from nrel.hive.resources.mock_lobster import mock_env, mock_request, mock_sim
+from nrel.hive.state.simulation_state import simulation_state_ops
 
 from nrel.hive.state.simulation_state.update.cancel_requests import CancelRequests
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestCancelRequests(TestCase):
     def test_update_cancellable(self):
         req = mock_request()
         sim_or_err = simulation_state_ops.add_request_safe(mock_sim(sim_time=600), req)
         self.assertIsInstance(sim_or_err, Success)
```

### Comparing `nrel.hive-1.2.2/tests/test_charging_price_update.py` & `nrel.hive-1.3.0/tests/test_charging_price_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 from unittest import TestCase
+import immutables
+
+from pkg_resources import resource_filename
+from nrel.hive.resources.mock_lobster import (
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_l1_charger_id,
+    mock_l2_charger_id,
+    mock_sim,
+    mock_station,
+    mock_station_from_geoid,
+)
 
 from nrel.hive.state.simulation_state.update.charging_price_update import ChargingPriceUpdate
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestChargingPriceUpdate(TestCase):
     def test_charge_price_update_from_station_id_file(self):
         # prices are set to bump at 28800 (8 am)
         sim = mock_sim(
             stations=(
```

### Comparing `nrel.hive-1.2.2/tests/test_config_builder.py` & `nrel.hive-1.3.0/tests/test_config_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         test_class = ConfigBuilder.build(
             default_config=defaults,
             required_config=(),
             config_constructor=TestConfigBuilderAssets.constructor,
             config=None,
         )
 
-        self.assertIsInstance(test_class, TestConfigBuilderAssets.TestClass)
+        self.assertIsInstance(test_class, TestConfigBuilderAssets.SampleClass)
         self.assertEqual(test_class.a, defaults["a"])
         self.assertEqual(test_class.b, defaults["b"])
 
     def test_build_has_required_fields(self):
         required = (
             "a",
             "b",
@@ -36,30 +36,30 @@
         test_class = ConfigBuilder.build(
             default_config={},
             required_config=required,
             config_constructor=TestConfigBuilderAssets.constructor,
             config=config,
         )
 
-        self.assertIsInstance(test_class, TestConfigBuilderAssets.TestClass)
+        self.assertIsInstance(test_class, TestConfigBuilderAssets.SampleClass)
         self.assertEqual(test_class.a, config["a"])
         self.assertEqual(test_class.b, config["b"])
 
     def test_build_missing_required_field(self):
         required = (
             "a",
             "b",
         )
 
         config = {
             "a": 6,
         }
 
         with self.assertRaises(AttributeError):
-            test_class = ConfigBuilder.build(
+            ConfigBuilder.build(
                 default_config={},
                 required_config=required,
                 config_constructor=TestConfigBuilderAssets.constructor,
                 config=config,
             )
 
     def test_build_ignores_extra_fields(self):
@@ -73,20 +73,20 @@
         test_class = ConfigBuilder.build(
             default_config={},
             required_config=(),
             config_constructor=TestConfigBuilderAssets.constructor,
             config=config,
         )
 
-        self.assertIsInstance(test_class, TestConfigBuilderAssets.TestClass)
+        self.assertIsInstance(test_class, TestConfigBuilderAssets.SampleClass)
         self.assertEqual(test_class.a, config["a"])
         self.assertEqual(test_class.b, config["b"])
 
 
 class TestConfigBuilderAssets:
-    class TestClass(NamedTuple):
+    class SampleClass(NamedTuple):
         a: int
         b: str
 
     @classmethod
     def constructor(cls, d: Dict):
-        return TestConfigBuilderAssets.TestClass(d["a"], d["b"])
+        return TestConfigBuilderAssets.SampleClass(d["a"], d["b"])
```

### Comparing `nrel.hive-1.2.2/tests/test_dict_ops.py` & `nrel.hive-1.3.0/tests/test_dict_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from unittest import TestCase
 
 import immutables
-from typing import FrozenSet
 
 from nrel.hive.util import DictOps
 
 
 class TestDictOps(TestCase):
     def test_add_to_dict(self):
         m = immutables.Map()
```

### Comparing `nrel.hive-1.2.2/tests/test_dict_reader_stepper.py` & `nrel.hive-1.3.0/tests/test_dict_reader_stepper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from typing import Callable
 from unittest import TestCase
 
 from pkg_resources import resource_filename
 
 from nrel.hive.model.sim_time import SimTime
-from nrel.hive.util.iterators import *
+from nrel.hive.util.iterators import DictReaderStepper
 
 
 class TestDictReaderStepper(TestCase):
     def _generate_stop_condition(self, stop_time: SimTime) -> Callable:
         def stop_condition(value: SimTime) -> bool:
             r = value < stop_time
             return r
```

### Comparing `nrel.hive-1.2.2/tests/test_driver_instruction_ops.py` & `nrel.hive-1.3.0/tests/test_driver_instruction_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from unittest import TestCase
+from nrel.hive.dispatcher.instruction.instructions import (
+    DispatchBaseInstruction,
+    DispatchStationInstruction,
+)
 
 from nrel.hive.state.driver_state.driver_instruction_ops import human_go_home
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import (
+    mock_base,
+    mock_env,
+    mock_sim,
+    mock_station,
+    mock_vehicle,
+)
 
 
 class TestDriverInstructionOps(TestCase):
     def test_human_go_home_with_enough_range(self):
         veh = mock_vehicle(soc=0.8, lat=0, lon=0)
         base = mock_base(lat=1, lon=1, station_id="hb1")  # 141-ish km away
         station = mock_station(lat=0.01, lon=0.01)  # 1.41km-ish away
```

### Comparing `nrel.hive-1.2.2/tests/test_fs.py` & `nrel.hive-1.3.0/tests/test_fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class TestDictReaderStepper(TestCase):
     def test_global_hive_config_search_finds_default(self):
         result = global_hive_config_search()
         self.assertIsInstance(result, GlobalConfig, "should be a GlobalConfig class instance")
 
     def test_global_hive_config_search_finds_parent(self):
+        original_dir = os.getcwd()
         with tempfile.TemporaryDirectory() as parent:
             root_path = Path(parent)
             parent_hive_file = root_path.joinpath(".hive.yaml")
             with open(parent_hive_file, "w") as file:
                 yaml.safe_dump({"log_states": False}, file)
             with tempfile.TemporaryDirectory(dir=parent) as child:
                 os.chdir(child)
@@ -32,7 +33,8 @@
                     result.log_states,
                     "should have found the modified config in the parent directory",
                 )  # default is "True"
                 self.assertTrue(
                     result.log_run,
                     "should also contain keys from the default config",
                 )
+                os.chdir(original_dir)
```

### Comparing `nrel.hive-1.2.2/tests/test_h3_ops.py` & `nrel.hive-1.3.0/tests/test_h3_ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from unittest import TestCase
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+import immutables
+from nrel.hive.model.roadnetwork.link import Link
+from nrel.hive.resources.mock_lobster import mock_request_from_geoids, mock_sim
+from nrel.hive.state.simulation_state import simulation_state_ops
+
 from nrel.hive.util.h3_ops import H3Ops
 from nrel.hive.util.fp import throw_or_return
+from nrel.hive.util.units import hours_to_seconds
 
 
 class TestH3Ops(TestCase):
     def test_point_along_link(self):
         # endpoints are about 1km apart
         start = h3.geo_to_h3(37, 122, 15)
         end = h3.geo_to_h3(37.008994, 122, 15)
@@ -58,15 +64,15 @@
         sim_with_req1 = throw_or_return(simulation_state_ops.add_request_safe(sim, req_near))
         sim_with_reqs = throw_or_return(
             simulation_state_ops.add_request_safe(sim_with_req1, req_far)
         )
 
         nearest = H3Ops.nearest_entity_by_great_circle_distance(
             geoid=somewhere,
-            entities=tuple(sim_with_reqs.requests.values()),
+            entities=tuple(sim_with_reqs.get_requests()),
             entity_search=sim_with_reqs.r_search,
             sim_h3_search_resolution=sim_with_reqs.sim_h3_search_resolution,
         )
 
         self.assertEqual(nearest.geoid, req_near.geoid)
 
     def test_great_circle_distance(self):
```

### Comparing `nrel.hive-1.2.2/tests/test_haversine_roadnetwork.py` & `nrel.hive-1.3.0/tests/test_haversine_roadnetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from unittest import TestCase, skip
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+
+from nrel.hive.resources.mock_lobster import mock_network
 
 
 class TestHaversineRoadNetwork(TestCase):
     @skip("")
     def test_geoid_within_geofence(self):
         somewhere_out_of_geofence = h3.geo_to_h3(0, 0, 15)
         somewhere_within_geofence = h3.geo_to_h3(39.76138151, -104.982001, 15)
```

### Comparing `nrel.hive-1.2.2/tests/test_human_driver_state.py` & `nrel.hive-1.3.0/tests/test_human_driver_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,41 @@
 from unittest import TestCase
+from nrel.hive.dispatcher.instruction.instructions import (
+    ChargeBaseInstruction,
+    DispatchBaseInstruction,
+    IdleInstruction,
+    RepositionInstruction,
+    ReserveBaseInstruction,
+)
+from nrel.hive.state.driver_state.human_driver_state.human_driver_state import (
+    HumanAvailable,
+    HumanUnavailable,
+)
+from nrel.hive.state.simulation_state import simulation_state_ops
+from nrel.hive.state.vehicle_state.charging_station import ChargingStation
+from nrel.hive.state.vehicle_state.idle import Idle
+from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
 
-from nrel.hive.resources.mock_lobster import *
 from nrel.hive.util.fp import throw_or_return
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_base,
+    mock_base_from_geoid,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_human_driver,
+    mock_request_from_geoids,
+    mock_sim,
+    mock_station,
+    mock_station_from_geoid,
+    mock_vehicle,
+    mock_vehicle_from_geoid,
+    somewhere,
+    somewhere_else,
+)
 
 
 def on_schedule(a, b):
     return True
 
 
 def off_schedule(a, b):
@@ -198,15 +228,16 @@
                 charger_id=mock_dcfc_charger_id(),
             ),
             soc=0.9,
         )
         sim = mock_sim(vehicles=(veh,))
         env = mock_env()
 
-        # the default soc limit for charging at a station is 0.8 so we should generate an idle instruction.
+        # the default soc limit for charging at a station is 0.8
+        # so we should generate an idle instruction.
         i = veh.driver_state.generate_instruction(sim, env)
 
         self.assertIsInstance(i, IdleInstruction)
 
     def test_turn_off_at_home(self):
         state = mock_human_driver(available=False, schedule_id="off")
         veh = mock_vehicle_from_geoid(
@@ -214,11 +245,12 @@
             vehicle_state=Idle.build(vehicle_id=DefaultIds.mock_vehicle_id()),
             geoid=somewhere(),
         )
         base = mock_base_from_geoid(geoid=somewhere())
         sim = mock_sim(vehicles=(veh,), bases=(base,))
         env = mock_env()
 
-        # the driver is at home and idle so it should try to turn off (i.e. transition to ReserveBase).
+        # the driver is at home and idle so it should try to turn off
+        # (i.e. transition to ReserveBase).
         i = veh.driver_state.generate_instruction(sim, env)
 
         self.assertIsInstance(i, ReserveBaseInstruction)
```

### Comparing `nrel.hive-1.2.2/tests/test_ice_mechatronics.py` & `nrel.hive-1.3.0/tests/test_ice_mechatronics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from unittest import TestCase
+from nrel.hive.model.energy.energytype import EnergyType
 
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import mock_gasoline_pump, mock_ice, mock_route, mock_vehicle
+from nrel.hive.util.units import KM_TO_MILE, MILE_TO_KM, hours_to_seconds
 
 
 class TestICE(TestCase):
     def test_energy_gain(self):
         ice = mock_ice(tank_capacity_gallons=10)
         vehicle = mock_vehicle(soc=0, mechatronics=ice)
```

### Comparing `nrel.hive-1.2.2/tests/test_initialize_ops.py` & `nrel.hive-1.3.0/tests/test_initialize_ops.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/tests/test_instruction_generator_ops.py` & `nrel.hive-1.3.0/tests/test_instruction_generator_ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from unittest import TestCase
 
 from nrel.hive.dispatcher.instruction_generator.instruction_generator_ops import (
     instruct_vehicles_to_dispatch_to_station,
 )
 from nrel.hive.dispatcher.instruction_generator.charging_search_type import ChargingSearchType
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import (
+    mock_env,
+    mock_ice,
+    mock_sim,
+    mock_station,
+    mock_vehicle,
+)
 
 
 class TestInstructionGenerators(TestCase):
     def test_dispatch_station_ops_mismatch_charger_queue(self):
         """
         this tests the helper function instruct_vehicles_to_dispatch_to_station.
 
         here we create a simulation in which the chargers that exist in the sim can't be used by the
         vehicle; this edge case should not fail but rather result in zero instructions; given the
-        logic splits for each ChargingSearchType, we test ChargingSearchType.NEAREST_SHORTEST_QUEUE here
+        logic splits for each ChargingSearchType, we test ChargingSearchType.NEAREST_SHORTEST_QUEUE
         """
         station = mock_station()
         ice_mechatronics = mock_ice()
         vehicle = mock_vehicle(
             mechatronics=ice_mechatronics,
             soc=0.1,
         )
@@ -43,15 +49,15 @@
 
     def test_dispatch_station_ops_mismatch_charger_shortest_time(self):
         """
         this tests the helper function instruct_vehicles_to_dispatch_to_station.
 
         here we create a simulation in which the chargers that exist in the sim can't be used by the
         vehicle; this edge case should not fail but rather result in zero instructions; given the
-        logic splits for each ChargingSearchType, we test ChargingSearchType.SHORTEST_TIME_TO_CHARGE here
+        logic splits for each ChargingSearchType, we test ChargingSearchType.SHORTEST_TIME_TO_CHARGE
         """
         station = mock_station()
         mechatronics = mock_ice()
         vehicle = mock_vehicle(
             mechatronics=mechatronics,
             soc=0.1,
         )
```

### Comparing `nrel.hive-1.2.2/tests/test_instruction_generators.py` & `nrel.hive-1.3.0/tests/test_instruction_generators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 from unittest import TestCase
+import h3
 
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.dispatcher.instruction.instructions import (
+    DispatchStationInstruction,
+    DispatchTripInstruction,
+)
+from nrel.hive.dispatcher.instruction_generator.charging_fleet_manager import ChargingFleetManager
+from nrel.hive.dispatcher.instruction_generator.dispatcher import Dispatcher
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_config,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_membership,
+    mock_request_from_geoids,
+    mock_sim,
+    mock_station_from_geoid,
+    mock_vehicle_from_geoid,
+)
+from nrel.hive.state.simulation_state import simulation_state_ops
 
 
 class TestInstructionGenerators(TestCase):
     def test_dispatcher_match_vehicle(self):
         dispatcher = Dispatcher(mock_config().dispatcher)
 
         somewhere = h3.geo_to_h3(39.7539, -104.974, 15)
@@ -101,15 +119,16 @@
 
         v_geoid = h3.geo_to_h3(39.0, -104.0, 15)
         veh_low_battery = mock_vehicle_from_geoid(geoid=v_geoid, soc=0.01)
 
         s1_geoid = h3.geo_to_h3(39.01, -104.0, 15)
         s2_geoid = h3.geo_to_h3(39.015, -104.0, 15)  # slightly further away
 
-        # prepare the scenario where the closer station has no available chargers and one enqueued vehicle
+        # prepare the scenario where the closer station has no
+        # available chargers and one enqueued vehicle
         s1 = mock_station_from_geoid(
             station_id="s1",
             geoid=s1_geoid,
             chargers={mock_dcfc_charger_id(): 1},
         )
         e, s1 = s1.checkout_charger(mock_dcfc_charger_id())
         self.assertIsNone(e, "test invariant failed (unable to check out charger at station")
```

### Comparing `nrel.hive-1.2.2/tests/test_osm_roadnetwork.py` & `nrel.hive-1.3.0/tests/test_osm_roadnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from unittest import TestCase, skip
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+
+from nrel.hive.resources.mock_lobster import mock_osm_network
 
 
 class TestOSMRoadNetwork(TestCase):
     @skip("")
     def test_geoid_within_geofence(self):
         somewhere_out_of_geofence = h3.geo_to_h3(0, 0, 15)
         somewhere_within_geofence = h3.geo_to_h3(39.76138151, -104.982001, 15)
```

### Comparing `nrel.hive-1.2.2/tests/test_request.py` & `nrel.hive-1.3.0/tests/test_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from unittest import TestCase
 from csv import DictReader
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+from nrel.hive.model.request.request import Request
+from nrel.hive.model.sim_time import SimTime
+from nrel.hive.resources.mock_lobster import mock_config, mock_env, mock_network, mock_request
 
 from nrel.hive.util.exception import TimeParseError
 
 
 class TestRequest(TestCase):
     request_id = "test"
     origin = h3.geo_to_h3(0, 0, resolution=11)
@@ -52,15 +55,16 @@
             h3.geo_to_h3(31.2109091, 121.4532226, env.config.sim.sim_h3_resolution),
         )
         self.assertEqual(req.departure_time, 61200)
         self.assertEqual(len(req.passengers), 4)
         self.assertTrue(req.membership.public)
 
     def test_from_row_with_fleet_id(self):
-        source = """request_id,o_lat,o_lon,d_lat,d_lon,departure_time,cancel_time,passengers,fleet_id
+        source = """
+        request_id,o_lat,o_lon,d_lat,d_lon,departure_time,cancel_time,passengers,fleet_id
         1_a,31.2074449,121.4294263,31.2109091,121.4532226,61200,61800,4,uber
         """
         row = next(DictReader(source.split()))
         env = mock_env()
         network = mock_network()
         _, req = Request.from_row(row, env, network)
         self.assertEqual(req.id, "1_a")
```

### Comparing `nrel.hive-1.2.2/tests/test_routetraversal.py` & `nrel.hive-1.3.0/tests/test_routetraversal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 from unittest import TestCase
 
 from nrel.hive.model.roadnetwork.linktraversal import traverse_up_to
 from nrel.hive.model.roadnetwork.routetraversal import traverse
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import mock_osm_network, mock_osm_route, mock_route
+from nrel.hive.util.units import hours_to_seconds
 
 
 class TestRouteTraversal(TestCase):
     def test_traverse_with_enough_time(self):
         """
         the mock problem is tuned to complete the route with a time step of just beyond 3 time units
         """
-        links = mock_route()
+        rn = mock_osm_network()
+        route = mock_osm_route()
 
-        _, result = traverse(route_estimate=links, duration_seconds=hours_to_seconds(4))
+        _, result = traverse(
+            route_estimate=route, duration_seconds=hours_to_seconds(4), road_network=rn
+        )
         self.assertGreater(result.remaining_time_seconds, 0, "should have more time left")
         self.assertEqual(len(result.remaining_route), 0, "should have no more route")
-        self.assertEqual(len(result.experienced_route), 3, "should have hit all 3 links")
+        self.assertEqual(len(result.experienced_route), len(route), "should have hit all links")
 
     def test_traverse_without_enough_time(self):
         """
-        the mock problem needs more than 1.5 time to complete the route. should end
-        up somewhere in the middle
+        should end up somewhere in the middle
         """
-        links = mock_route()
+        rn = mock_osm_network()
+        route = mock_osm_route()
+        midway = int(len(route) / 2)
+        midway_travel_time_seconds = sum([link.travel_time_seconds for link in route[:midway]])
+
         _, result = traverse(
-            route_estimate=links,
-            duration_seconds=hours_to_seconds(1.5),  # 1.5 hours at 1kmph, 1km per link, 3 links
+            route_estimate=route,
+            duration_seconds=midway_travel_time_seconds,
+            road_network=rn,
         )
         self.assertEqual(result.remaining_time_seconds, 0, "should have no more time left")
-        self.assertEqual(len(result.remaining_route), 2, "should have 2 links remaining")
-        self.assertEqual(len(result.experienced_route), 2, "should have traversed 2 links")
+        self.assertEqual(
+            len(result.remaining_route), len(route[midway:]), "should have some route left"
+        )
+        self.assertEqual(len(result.experienced_route), midway, "should have hit half the links")
 
     def test_traverse_up_to_split(self):
         links = mock_route()
         test_link = links[0]
 
         error, result = traverse_up_to(
             link=test_link,
```

### Comparing `nrel.hive-1.2.2/tests/test_run_cosim.py` & `nrel.hive-1.3.0/tests/test_run_cosim.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+from pkg_resources import resource_filename
 from unittest import TestCase
 
 from nrel.hive.app import hive_cosim
 from nrel.hive.reporting.handler.vehicle_charge_events_handler import VehicleChargeEventsHandler
 from nrel.hive.resources.mock_lobster import mock_env, mock_sim, mock_update
 from nrel.hive.runner.runner_payload import RunnerPayload
```

### Comparing `nrel.hive-1.2.2/tests/test_sample_functions.py` & `nrel.hive-1.3.0/tests/test_sample_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from unittest import TestCase
 
 from returns.primitives.exceptions import UnwrapFailedError
-from returns.result import Result
 
 from nrel.hive.initialization.sample_requests import default_request_sampler
 from nrel.hive.initialization.sample_vehicles import (
     sample_vehicles,
     build_default_location_sampling_fn,
     build_default_soc_sampling_fn,
 )
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.model.roadnetwork.link import Link
+from nrel.hive.model.vehicle.vehicle import Vehicle
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_base,
+    mock_env,
+    mock_osm_network,
+    mock_sim,
+)
 
 
 class TestSampleVehicles(TestCase):
     def test_sample_n_requests_default(self):
         n = 100
         sim = mock_sim(road_network=mock_osm_network())
         env = mock_env()
 
         sample_requests = default_request_sampler(n, sim, env)
 
-        self.assertEquals(len(sample_requests), n, f"should have sampled {n} requests")
+        self.assertEqual(len(sample_requests), n, f"should have sampled {n} requests")
 
         for r in sample_requests:
             self.assertNotEqual(
                 r.origin,
                 r.destination,
-                f"request should not have equal origin and destination",
+                "request should not have equal origin and destination",
             )
 
     def test_sample_n_vehicles_default(self):
         """
-        samples 10 vehicles and expects them to be instantiated with full charge at the same base location
+        samples 10 vehicles and expects them to be instantiated
+        with full charge at the same base location
         """
         n = 10
         base = mock_base()
         bases = (base,)
         sim = mock_sim(bases=bases, road_network=mock_osm_network())
         env = mock_env()
         mechatronics_id = DefaultIds.mock_mechatronics_bev_id()
@@ -47,23 +56,23 @@
             sim=sim,
             env=env,
             location_sampling_function=loc_fn,
             soc_sampling_function=soc_fn,
         )
 
         def check_vehicle(v: Vehicle):
-            self.assertEquals(v.mechatronics_id, DefaultIds.mock_mechatronics_bev_id())
-            self.assertEquals(
+            self.assertEqual(v.mechatronics_id, DefaultIds.mock_mechatronics_bev_id())
+            self.assertEqual(
                 v.energy.get(EnergyType.ELECTRIC),
                 env.mechatronics.get(mechatronics_id).battery_capacity_kwh,
             )
             self.assertEquals(v.position, base.position)
 
         self.assertEqual(len(result.unwrap().vehicles), n, f"should have {n} vehicles")
-        map(check_vehicle, result.unwrap().vehicles.values())
+        map(check_vehicle, result.unwrap().get_vehicles())
 
     def test_sample_n_with_failure(self):
         """
         this test is really just here to help demonstrate the Returns library.
         instead of blowing up in the sample_vehicles reduce loop, we get the first
         error result after 4 items succeed. this is because of the "railway" programming
         aka fail-fast feature of Monads, where we only call "bind" when in the Success path.
@@ -93,8 +102,8 @@
             env=env,
             location_sampling_function=wonky_loc_fn,
             soc_sampling_function=soc_fn,
         )
 
         with self.assertRaises(UnwrapFailedError):
             result.unwrap()
-        self.assertEquals(result._inner_value.args[0], failure_msg)
+        self.assertEqual(result._inner_value.args[0], failure_msg)
```

### Comparing `nrel.hive-1.2.2/tests/test_schedules.py` & `nrel.hive-1.3.0/tests/test_schedules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 
 from nrel.hive.model.vehicle.schedules.time_range_schedule import time_range_schedules_from_string
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import DefaultIds, mock_sim
 
 
 class TestSchedules(TestCase):
     def test_time_range_schedule(self):
         schedules_input = """schedule_id,start_time,end_time
                              first,"09:00:00","17:00:00"
                              second,"17:00:00","01:00:00"
```

### Comparing `nrel.hive-1.2.2/tests/test_simulation_state_ops.py` & `nrel.hive-1.3.0/tests/test_simulation_state_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from dataclasses import replace
 from unittest import TestCase
 
 from returns.result import Success
+from nrel.hive.model.entity_position import EntityPosition
 
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import (
+    mock_base,
+    mock_request,
+    mock_sim,
+    mock_station,
+    mock_vehicle,
+)
+from nrel.hive.state.simulation_state import simulation_state_ops
 
 
 class TestSimulationStateOps(TestCase):
     def test_add_entity(self):
         sim = mock_sim()
         req = mock_request()
         station = mock_station()
@@ -27,27 +35,27 @@
         self.assertEqual(sim_w_vehicle.vehicles[vehicle.id], vehicle)
 
     def test_add_entities(self):
         sim = mock_sim()
 
         reqs = [mock_request(i) for i in range(10)]
         sim_with_reqs = simulation_state_ops.add_entities_safe(sim, reqs).unwrap()
-        self.assertEqual(len(sim_with_reqs.requests.values()), 10)
+        self.assertEqual(len(sim_with_reqs.get_requests()), 10)
 
         vehicles = [mock_vehicle(i) for i in range(10)]
         sim_with_vehicles = simulation_state_ops.add_entities_safe(sim, vehicles).unwrap()
-        self.assertEqual(len(sim_with_vehicles.vehicles.values()), 10)
+        self.assertEqual(len(sim_with_vehicles.get_vehicles()), 10)
 
         stations = [mock_station(i) for i in range(10)]
         sim_with_stations = simulation_state_ops.add_entities_safe(sim, stations).unwrap()
-        self.assertEqual(len(sim_with_stations.stations.values()), 10)
+        self.assertEqual(len(sim_with_stations.get_stations()), 10)
 
         bases = [mock_base(i) for i in range(10)]
         sim_with_bases = simulation_state_ops.add_entities_safe(sim, bases).unwrap()
-        self.assertEqual(len(sim_with_bases.bases.values()), 10)
+        self.assertEqual(len(sim_with_bases.get_bases()), 10)
 
     def test_modify_entity(self):
         sim = mock_sim()
         station = mock_station()
         sim_w_station = simulation_state_ops.add_entity(sim, station)
 
         station2 = sim_w_station.stations.get(station.id)
@@ -60,20 +68,20 @@
         self.assertTrue("test!" in updated_station2.membership.memberships)
 
     def test_modify_entities(self):
         sim = mock_sim()
         stations = [mock_station(i) for i in range(10)]
         sim_w_stations = simulation_state_ops.add_entities(sim, stations)
 
-        updated_stations = [s.add_membership("test!") for s in sim_w_stations.stations.values()]
+        updated_stations = [s.add_membership("test!") for s in sim_w_stations.get_stations()]
 
         sim_w_new_stations = simulation_state_ops.modify_entities(sim_w_stations, updated_stations)
 
         self.assertTrue(
-            all(["test!" in s.membership.memberships for s in sim_w_new_stations.stations.values()])
+            all(["test!" in s.membership.memberships for s in sim_w_new_stations.get_stations()])
         )
 
     def test_add_request(self):
         req = mock_request()
         sim = mock_sim()
         sim_with_req = simulation_state_ops.add_request_safe(sim, req).unwrap()
         self.assertEqual(
```

### Comparing `nrel.hive-1.2.2/tests/test_simulationstate.py` & `nrel.hive-1.3.0/tests/test_simulationstate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,46 @@
 from unittest import TestCase
 
+import h3
+import immutables
+from nrel.hive.dispatcher.instruction.instructions import (
+    ChargeBaseInstruction,
+    ChargeStationInstruction,
+    DispatchBaseInstruction,
+    DispatchStationInstruction,
+    DispatchTripInstruction,
+    RepositionInstruction,
+    ReserveBaseInstruction,
+)
+from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.model.station.station import Station
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_base,
+    mock_base_from_geoid,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_l2_charger_id,
+    mock_request,
+    mock_request_from_geoids,
+    mock_sim,
+    mock_station,
+    mock_station_from_geoid,
+    mock_vehicle,
+    mock_vehicle_from_geoid,
+)
+
 from nrel.hive.state.entity_state import entity_state_ops
+from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.simulation_state.update.step_simulation import perform_vehicle_state_updates
+from nrel.hive.state.vehicle_state.charging_station import ChargingStation
+from nrel.hive.state.vehicle_state.idle import Idle
 from nrel.hive.state.vehicle_state.out_of_service import OutOfService
+from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
 from nrel.hive.state.vehicle_state.servicing_trip import ServicingTrip
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestSimulationState(TestCase):
     def test_at_vehicle_geoid(self):
         somewhere = h3.geo_to_h3(39.7539, -104.974, 15)
         somewhere_else = h3.geo_to_h3(39.755, -104.976, 15)
         veh = mock_vehicle_from_geoid(geoid=somewhere)
@@ -349,15 +381,16 @@
             sim,
             env,
             instruction_result.prev_state,
             instruction_result.next_state,
         )
         self.assertIsNotNone(sim, "Vehicle should have set instruction.")
 
-        # 1000 seconds should get us there, and 1 more sim step of any size to transition vehicle state
+        # 1000 seconds should get us there, and 1 more sim step
+        # of any size to transition vehicle state
         sim_at_base = perform_vehicle_state_updates(
             sim_updated._replace(sim_timestep_duration_seconds=1000), env
         )
         sim_in_base = perform_vehicle_state_updates(
             sim_at_base._replace(sim_timestep_duration_seconds=1), env
         )
 
@@ -389,15 +422,16 @@
         self.assertIsNotNone(sim, "Vehicle should have set instruction.")
         sim_error, sim_updated = entity_state_ops.transition_previous_to_next(
             sim,
             env,
             instruction_result.prev_state,
             instruction_result.next_state,
         )
-        # 1000 seconds should get us there, and 1 more sim step of any size to transition vehicle state
+        # 1000 seconds should get us there, and 1 more sim step of
+        # any size to transition vehicle state
         sim_at_new_pos = perform_vehicle_state_updates(
             sim_updated._replace(sim_timestep_duration_seconds=1000), env
         )
         sim_in_new_state = perform_vehicle_state_updates(
             sim_at_new_pos._replace(sim_timestep_duration_seconds=1), env
         )
 
@@ -432,15 +466,16 @@
         self.assertIsNotNone(sim, "Vehicle should have set instruction.")
         sim_error, sim_updated = entity_state_ops.transition_previous_to_next(
             sim,
             env,
             instruction_result.prev_state,
             instruction_result.next_state,
         )
-        # 10 hours should get us charged , and 1 more sim step of any size to transition vehicle state
+        # 10 hours should get us charged , and 1 more sim step
+        # of any size to transition vehicle state
         sim_charged = perform_vehicle_state_updates(
             sim_updated._replace(sim_timestep_duration_seconds=36000), env
         )
         sim_in_new_state = perform_vehicle_state_updates(
             sim_charged._replace(sim_timestep_duration_seconds=1), env
         )
 
@@ -471,15 +506,16 @@
         self.assertIsNotNone(sim, "Vehicle should have set instruction.")
         sim_error, sim_updated = entity_state_ops.transition_previous_to_next(
             sim,
             env,
             instruction_result.prev_state,
             instruction_result.next_state,
         )
-        # 10 hours should get us charged, and 1 more sim step of any size to transition vehicle state
+        # 10 hours should get us charged, and 1 more sim step
+        # of any size to transition vehicle state
         sim_charged = perform_vehicle_state_updates(
             sim_updated._replace(sim_timestep_duration_seconds=36000), env
         )
         sim_in_new_state = perform_vehicle_state_updates(
             sim_charged._replace(sim_timestep_duration_seconds=1), env
         )
 
@@ -592,17 +628,15 @@
             bases=(
                 mock_base("b1", lat=0, lon=0, stall_count=0),
                 mock_base("b2", lat=1, lon=1, stall_count=2),
                 mock_base("b3", lat=2, lon=2, stall_count=1),
             )
         )
 
-        sorted_bases = sim.get_bases(
-            sort=True, sort_reversed=True, sort_key=lambda b: b.total_stalls
-        )
+        sorted_bases = sim.get_bases(sort_key=lambda b: -b.total_stalls)
 
         self.assertEqual(sorted_bases[0].id, "b2", "base 2 has the most stalls")
 
     def test_get_bases_at_same_geoid(self):
         sim = mock_sim(
             bases=(
                 mock_base("b1", lat=0, lon=0, stall_count=0),
@@ -624,26 +658,24 @@
                 mock_vehicle("v2", soc=0.5),
                 mock_vehicle("v3", soc=0.2),
                 mock_vehicle("v4", soc=0.1),
             )
         )
 
         sorted_and_filtered_vehicles = sim.get_vehicles(
-            sort=True,
-            sort_key=lambda v: v.energy[EnergyType.ELECTRIC],
-            sort_reversed=True,
+            sort_key=lambda v: -v.energy[EnergyType.ELECTRIC],
         )
 
         self.assertEqual(sorted_and_filtered_vehicles[0].id, "v1", "v1 has highest soc")
 
     def test_get_requests(self):
         sim = mock_sim()
         r1 = mock_request("r1", departure_time=0)
         r2 = mock_request("r2", departure_time=10)
         r3 = mock_request("r3", departure_time=20)
         sim = simulation_state_ops.add_request_safe(sim, r3).unwrap()
         sim = simulation_state_ops.add_request_safe(sim, r2).unwrap()
         sim = simulation_state_ops.add_request_safe(sim, r1).unwrap()
 
-        sorted_requests = sim.get_requests(sort=True, sort_key=lambda r: r.departure_time)
+        sorted_requests = sim.get_requests(sort_key=lambda r: r.departure_time)
 
         self.assertEqual(sorted_requests[0].id, "r1", "r1 has lowest departure time")
```

### Comparing `nrel.hive-1.2.2/tests/test_station.py` & `nrel.hive-1.3.0/tests/test_station.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from csv import DictReader
 from unittest import TestCase
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+import immutables
+
 
 from returns.result import Failure
+from nrel.hive.model.station.station import Station
+
+from nrel.hive.resources.mock_lobster import (
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_l1_charger_id,
+    mock_l2_charger_id,
+    mock_network,
+    mock_station,
+)
 
 
 class TestStation(TestCase):
     def test_from_row(self):
         source = """station_id,lat,lon,charger_id,charger_count,on_shift_access
                  s1,37,122,DCFC,10,true
                  """
```

### Comparing `nrel.hive-1.2.2/tests/test_station_load_handler.py` & `nrel.hive-1.3.0/tests/test_station_load_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 from unittest import TestCase
 
 from nrel.hive.reporting import vehicle_event_ops
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_bev,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_sim,
+    mock_station,
+    mock_vehicle,
+)
+from nrel.hive.state.vehicle_state.charging_station import ChargingStation
 
 
 class TestStationLoadHandler(TestCase):
     def test_correctly_reads_one_vehicle_charge_event(self):
         """
         this test is mostly here just to make sure we don't mess with
         the structure of vehicle charge events in a way that would
```

### Comparing `nrel.hive-1.2.2/tests/test_step_simulation_ops.py` & `nrel.hive-1.3.0/tests/test_step_simulation_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
+from nrel.hive.resources.mock_lobster import mock_env, mock_sim, mock_vehicle
 from nrel.hive.state.simulation_state.update.step_simulation_ops import (
     perform_vehicle_state_updates,
 )
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestStepSimulationOps(TestCase):
     def test_step_vehicle(self):
         """
         build a sim with two idle vehicles and only step one of them for 10 time steps (600 seconds)
```

### Comparing `nrel.hive-1.2.2/tests/test_time.py` & `nrel.hive-1.3.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `nrel.hive-1.2.2/tests/test_update_requests.py` & `nrel.hive-1.3.0/tests/test_update_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from unittest import TestCase
 
+from pkg_resources import resource_filename
+from nrel.hive.model.sim_time import SimTime
+from nrel.hive.resources.mock_lobster import mock_config, mock_env, mock_sim
+
 from nrel.hive.state.simulation_state.update.update_requests_from_file import UpdateRequestsFromFile
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestUpdateRequests(TestCase):
     def test_update(self):
         """
         test invariant: the below file resource exists
         """
@@ -25,15 +28,15 @@
         rate_structure_file = resource_filename(
             "nrel.hive.resources.scenarios.denver_downtown.service_prices",
             "rate_structure.csv",
         )
         fn = UpdateRequestsFromFile.build(req_file, rate_structure_file)
         result, _ = fn.update(sim, env)
         self.assertEqual(len(result.requests), 2, "should have added the reqs")
-        for req in result.requests.values():
+        for req in result.get_requests():
             self.assertLess(req.departure_time, sim_time, f"should be less than {sim_time}")
 
     def test_update_some_aready_cancelled(self):
         """
         won't add requests whos cancel_time has already been exceeded, will instead report them
         test invariant: the below file resource exists
         """
@@ -54,15 +57,15 @@
         rate_structure_file = resource_filename(
             "nrel.hive.resources.scenarios.denver_downtown.service_prices",
             "rate_structure.csv",
         )
         fn = UpdateRequestsFromFile.build(req_file, rate_structure_file)
         result, _ = fn.update(sim, env)
         self.assertEqual(expected_reqs, len(result.requests), "should have added the reqs")
-        for req in result.requests.values():
+        for req in result.get_requests():
             self.assertLess(req.departure_time, sim_time, f"should be less than {sim_time}")
 
     def test_update_rate_structure(self):
         """
         won't add requests whos cancel_time has already been exceeded, will instead report them
         test invariant: the below file resource exists
         """
@@ -81,20 +84,20 @@
         )
         rate_structure_file = resource_filename(
             "nrel.hive.resources.scenarios.denver_downtown.service_prices",
             "rate_structure.csv",
         )
         fn = UpdateRequestsFromFile.build(req_file, rate_structure_file)
         result, _ = fn.update(sim, env)
-        for req in result.requests.values():
+        for req in result.get_requests():
             print(req)
             self.assertGreaterEqual(
                 req.value,
                 5,
-                f"should be greater/equal than minimum price of 5",
+                "should be greater/equal than minimum price of 5",
             )
 
     def test_update_lazy_file_reading(self):
         """
         test invariant: the below file resource exists
         """
         sim_time = SimTime.build(
@@ -113,9 +116,9 @@
         rate_structure_file = resource_filename(
             "nrel.hive.resources.scenarios.denver_downtown.service_prices",
             "rate_structure.csv",
         )
         fn = UpdateRequestsFromFile.build(req_file, rate_structure_file, lazy_file_reading=True)
         result, _ = fn.update(sim, env)
         self.assertEqual(len(result.requests), 2, "should have added the reqs")
-        for req in result.requests.values():
+        for req in result.get_requests():
             self.assertLess(req.departure_time, sim_time, f"should be less than {sim_time}")
```

### Comparing `nrel.hive-1.2.2/tests/test_vehicle.py` & `nrel.hive-1.3.0/tests/test_vehicle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from csv import DictReader
 from unittest import TestCase
 
-from nrel.hive.resources.mock_lobster import *
+import h3
+from nrel.hive.model.vehicle.vehicle import Vehicle
+
+from nrel.hive.resources.mock_lobster import mock_env, mock_network
+from nrel.hive.state.vehicle_state.idle import Idle
 
 
 class TestVehicle(TestCase):
     def test_from_row(self):
         source = """vehicle_id,lat,lon,mechatronics_id,initial_soc,schedule_id,home_base_id
                     v1,39.7539,-104.976,bev,1.0,schedule0,b0"""
```

### Comparing `nrel.hive-1.2.2/tests/test_vehicle_state.py` & `nrel.hive-1.3.0/tests/test_vehicle_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,52 @@
 from dataclasses import replace
 from unittest import TestCase
 
+import immutables
+import h3
+
+from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.model.membership import Membership
+from nrel.hive.model.sim_time import SimTime
+from nrel.hive.model.vehicle.trip_phase import TripPhase
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_base,
+    mock_base_from_geoid,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_ice,
+    mock_l2_charger_id,
+    mock_request,
+    mock_request_from_geoids,
+    mock_route_from_geoids,
+    mock_sim,
+    mock_station,
+    mock_station_from_geoid,
+    mock_vehicle,
+    mock_vehicle_from_geoid,
+)
 from nrel.hive.state.entity_state import entity_state_ops
+from nrel.hive.state.simulation_state import simulation_state_ops
 from nrel.hive.state.vehicle_state.charge_queueing import ChargeQueueing
+from nrel.hive.state.vehicle_state.charging_base import ChargingBase
+from nrel.hive.state.vehicle_state.charging_station import ChargingStation
+from nrel.hive.state.vehicle_state.dispatch_base import DispatchBase
 from nrel.hive.state.vehicle_state.dispatch_pooling_trip import DispatchPoolingTrip
+from nrel.hive.state.vehicle_state.dispatch_station import DispatchStation
+from nrel.hive.state.vehicle_state.dispatch_trip import DispatchTrip
+from nrel.hive.state.vehicle_state.idle import Idle
+from nrel.hive.state.vehicle_state.repositioning import Repositioning
+from nrel.hive.state.vehicle_state.reserve_base import ReserveBase
+from nrel.hive.state.vehicle_state.servicing_pooling_trip import ServicingPoolingTrip
 from nrel.hive.state.vehicle_state.servicing_trip import ServicingTrip
 from nrel.hive.state.vehicle_state.out_of_service import OutOfService
-from nrel.hive.resources.mock_lobster import *
 
 
 class TestVehicleState(TestCase):
-    ####################################################################################################################
-    # ChargingStation ##################################################################################################
-    ####################################################################################################################
-
     def test_charging_station_enter(self):
         vehicle = mock_vehicle()
         station = mock_station()
         charger = mock_dcfc_charger_id()
         sim = mock_sim(vehicles=(vehicle,), stations=(station,))
         env = mock_env()
 
@@ -30,15 +59,15 @@
         updated_station = updated_sim.stations.get(station.id)
         available_chargers = updated_station.get_available_chargers(charger)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ChargingStation,
             "should be in a charging state",
         )
-        self.assertEquals(
+        self.assertEqual(
             available_chargers,
             0,
             "should have claimed the only DCFC charger_id",
         )
 
     def test_charging_station_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
@@ -72,15 +101,15 @@
         updated_station = updated_sim.stations.get(station.id)
         available_chargers = updated_station.get_available_chargers(charger)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ChargingStation,
             "should still be in a charging state",
         )
-        self.assertEquals(
+        self.assertEqual(
             available_chargers,
             1,
             "should have returned the only DCFC charger_id",
         )
 
     def test_charging_station_update(self):
         vehicle = mock_vehicle(soc=0.5)
@@ -128,15 +157,15 @@
         updated_vehicle = sim_updated.vehicles.get(vehicle.id)
         updated_station = sim_updated.stations.get(station.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             Idle,
             "vehicle should be in idle state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_station.get_available_chargers(charger),
             1,
             "should have returned the charger_id",
         )
 
     def test_charging_station_enter_with_no_station(self):
         vehicle = mock_vehicle(soc=0.99)
@@ -225,18 +254,14 @@
         )
         self.assertEqual(
             l2_available,
             0,
             "second instruction should have claimed the only L2 charger_id",
         )
 
-    ####################################################################################################################
-    # ChargingBase #####################################################################################################
-    ####################################################################################################################
-
     def test_charging_base_enter(self):
         vehicle = mock_vehicle()
         station = mock_station()
         base = mock_base(station_id=DefaultIds.mock_station_id())
         charger = mock_dcfc_charger_id()
         sim = mock_sim(vehicles=(vehicle,), stations=(station,), bases=(base,))
         env = mock_env()
@@ -250,15 +275,15 @@
         updated_station = updated_sim.stations.get(station.id)
         available_chargers = updated_station.get_available_chargers(charger)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ChargingBase,
             "should be in a charging state",
         )
-        self.assertEquals(
+        self.assertEqual(
             available_chargers,
             0,
             "should have claimed the only DCFC charger_id",
         )
 
     def test_charging_base_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
@@ -315,15 +340,15 @@
         updated_station = updated_sim.stations.get(station.id)
         available_chargers = updated_station.get_available_chargers(charger)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ChargingBase,
             "should still be in a charging state",
         )
-        self.assertEquals(
+        self.assertEqual(
             available_chargers,
             1,
             "should have returned the only DCFC charger_id",
         )
 
     def test_charging_base_update(self):
         vehicle = mock_vehicle(soc=0.5)
@@ -373,15 +398,15 @@
         updated_vehicle = sim_updated.vehicles.get(vehicle.id)
         updated_base = sim_updated.bases.get(base.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ReserveBase,
             "vehicle should be in ReserveBase state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_base.available_stalls,
             0,
             "should have taken the only available stall",
         )
 
     def test_charging_base_enter_with_no_base(self):
         vehicle = mock_vehicle(soc=1.0)
@@ -470,18 +495,14 @@
         )
         self.assertEqual(
             l2_available,
             0,
             "second instruction should have claimed the only L2 charger_id",
         )
 
-    ####################################################################################################################
-    # DispatchBase #####################################################################################################
-    ####################################################################################################################
-
     def test_dispatch_base_enter(self):
         vehicle = mock_vehicle()
         base = mock_base()
         sim = mock_sim(vehicles=(vehicle,), bases=(base,))
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, base.geoid)
 
@@ -492,15 +513,15 @@
 
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchBase,
             "should be in a dispatch to base state",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_dispatch_base_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
         base = mock_base(membership=Membership.single_membership("lyft"))
 
         sim = mock_sim(vehicles=(vehicle,), bases=(base,))
         env = mock_env()
@@ -522,15 +543,15 @@
         enter_error, entered_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "test precondition (enter works correctly) not met")
 
         # begin test
         error, exited_sim = state.exit(Idle.build(vehicle.id), entered_sim, env)
 
         self.assertIsNone(error, "should have no errors")
-        self.assertEquals(entered_sim, exited_sim, "should see no change due to exit")
+        self.assertEqual(entered_sim, exited_sim, "should see no change due to exit")
 
     def test_dispatch_base_update(self):
         near = h3.geo_to_h3(39.7539, -104.974, 15)
         omf_brewing = h3.geo_to_h3(39.7608873, -104.9845391, 15)
         vehicle = mock_vehicle_from_geoid(geoid=near)
         base = mock_base_from_geoid(geoid=omf_brewing)
         sim = mock_sim(vehicles=(vehicle,), bases=(base,))
@@ -581,15 +602,15 @@
         updated_vehicle = sim_updated.vehicles.get(vehicle.id)
         updated_base = sim_updated.bases.get(base.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ReserveBase,
             "vehicle should be in ReserveBase state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_base.available_stalls,
             0,
             "should have taken the only available stall",
         )
 
     def test_dispatch_base_enter_no_base(self):
         vehicle = mock_vehicle()
@@ -645,18 +666,14 @@
         route = mock_route_from_geoids(vehicle.geoid, omf_brewing)
 
         state = DispatchBase.build(vehicle.id, base.id, route)
         enter_error, enter_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "should be no error")
         self.assertIsNone(enter_sim, "invalid route should have not changed sim state")
 
-    ####################################################################################################################
-    # DispatchStation ##################################################################################################
-    ####################################################################################################################
-
     def test_dispatch_station_enter(self):
         outer_range_brewing = h3.geo_to_h3(39.5892193, -106.1011423, 15)
         vehicle = mock_vehicle()
         station = mock_station_from_geoid(geoid=outer_range_brewing)
         charger = mock_dcfc_charger_id()
         sim = mock_sim(vehicles=(vehicle,), stations=(station,))
         env = mock_env()
@@ -669,15 +686,15 @@
 
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchStation,
             "should be in a dispatch to station state",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_dispatch_station_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
         station = mock_station(membership=Membership.single_membership("lyft"))
         charger = mock_dcfc_charger_id()
 
         sim = mock_sim(
@@ -725,15 +742,15 @@
         enter_error, entered_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "test precondition (enter works correctly) not met")
 
         # begin test
         error, exited_sim = state.exit(Idle.build(vehicle.id), entered_sim, env)
 
         self.assertIsNone(error, "should have no errors")
-        self.assertEquals(entered_sim, exited_sim, "should see no change due to exit")
+        self.assertEqual(entered_sim, exited_sim, "should see no change due to exit")
 
     def test_dispatch_station_update(self):
         near = h3.geo_to_h3(39.7539, -104.974, 15)
         omf_brewing = h3.geo_to_h3(39.7608873, -104.9845391, 15)
         vehicle = mock_vehicle_from_geoid(geoid=near)
         station = mock_station_from_geoid(geoid=omf_brewing)
         charger = mock_dcfc_charger_id()
@@ -795,15 +812,15 @@
             updated_vehicle
         )
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ChargingStation,
             "vehicle should be in ChargingStation state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_station.get_available_chargers(charger),
             0,
             "should have taken the only available charger_id",
         )
         self.assertGreater(new_soc, initial_soc, "should have charged for one time step")
 
     def test_dispatch_station_enter_no_station(self):
@@ -863,21 +880,18 @@
         route = mock_route_from_geoids(vehicle.geoid, outer_range_brewing)
 
         state = DispatchStation.build(vehicle.id, station.id, route, charger)
         enter_error, enter_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "should be no error")
         self.assertIsNone(
             enter_sim,
-            "invalid route should have not changed sim state - station and route destination do not match",
+            "invalid route should have not changed sim state"
+            " - station and route destination do not match",
         )
 
-    ####################################################################################################################
-    # DispatchTrip #####################################################################################################
-    ####################################################################################################################
-
     def test_dispatch_trip_enter(self):
         vehicle = mock_vehicle()
         request = mock_request()
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, request.geoid)
 
@@ -889,20 +903,20 @@
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         updated_request = updated_sim.requests.get(request.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchTrip,
             "should be in a dispatch to request state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_request.dispatched_vehicle,
             vehicle.id,
             "request should be assigned this vehicle",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_dispatch_trip_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
         request = mock_request(fleet_id="lyft")
 
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
@@ -996,15 +1010,15 @@
         updated_vehicle = sim_updated.vehicles.get(vehicle.id)
         updated_request = sim_updated.requests.get(request.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ServicingTrip,
             "vehicle should be in ServicingTrip state",
         )
-        self.assertEquals(
+        self.assertEqual(
             request,
             updated_vehicle.vehicle_state.request,
             "passengers not picked up",
         )
         self.assertIsNone(
             updated_request,
             "request should no longer exist as it has been picked up",
@@ -1061,18 +1075,14 @@
         route = mock_route_from_geoids(vehicle.geoid, omf_brewing)
 
         state = DispatchTrip.build(vehicle.id, request.id, route)
         enter_error, enter_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "should be no error")
         self.assertIsNone(enter_sim, "invalid route should have not changed sim state")
 
-    ####################################################################################################################
-    # Idle #############################################################################################################
-    ####################################################################################################################
-
     def test_idle_enter(self):
         # should intially not be in an Idle state
         vehicle = mock_vehicle().modify_vehicle_state(
             DispatchBase.build(DefaultIds.mock_vehicle_id(), DefaultIds.mock_base_id(), ())
         )
         sim = mock_sim(vehicles=(vehicle,))
         env = mock_env()
@@ -1101,15 +1111,15 @@
         enter_error, entered_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "test precondition (enter works correctly) not met")
 
         # begin test
         error, exited_sim = state.exit(Idle.build(vehicle.id), entered_sim, env)
 
         self.assertIsNone(error, "should have no errors")
-        self.assertEquals(entered_sim, exited_sim, "should see no change due to exit")
+        self.assertEqual(entered_sim, exited_sim, "should see no change due to exit")
 
     def test_idle_update(self):
         # should intially not be in an Idle state
         vehicle = mock_vehicle().modify_vehicle_state(
             DispatchBase.build(DefaultIds.mock_vehicle_id(), DefaultIds.mock_base_id(), ())
         )
         sim = mock_sim(vehicles=(vehicle,))
@@ -1167,18 +1177,14 @@
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             OutOfService,
             "vehicle should be OutOfService",
         )
         self.assertTrue(is_empty, "vehicle should have no energy")
 
-    ####################################################################################################################
-    # OutOfService #####################################################################################################
-    ####################################################################################################################
-
     def test_out_of_service_enter(self):
         # should intially not be in an Idle state
         vehicle = mock_vehicle(soc=0.0)
         sim = mock_sim(vehicles=(vehicle,))
         env = mock_env()
 
         state = OutOfService.build(vehicle.id)
@@ -1203,15 +1209,15 @@
         enter_error, entered_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "test precondition (enter works correctly) not met")
 
         # begin test
         error, exited_sim = state.exit(Idle.build(vehicle.id), entered_sim, env)
 
         self.assertIsNone(error, "should have no errors")
-        self.assertEquals(entered_sim, exited_sim, "should see no change due to exit")
+        self.assertEqual(entered_sim, exited_sim, "should see no change due to exit")
 
     def test_out_of_service_update(self):
         # should intially not be in an Idle state
         vehicle = mock_vehicle(soc=0.0)
         sim = mock_sim(vehicles=(vehicle,))
         env = mock_env()
 
@@ -1239,18 +1245,14 @@
             entered_state.instance_id,
             updated_vehicle.vehicle_state.instance_id,
             "should be the same instance",
         )
 
     # def test_out_of_service_update_terminal(self):  # there is no terminal state for OutOfService
 
-    ####################################################################################################################
-    # Repositioning ####################################################################################################
-    ####################################################################################################################
-
     def test_repositioning_enter(self):
         vehicle = mock_vehicle()
         sim = mock_sim(
             vehicles=(vehicle,),
         )
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, vehicle.geoid)
@@ -1262,15 +1264,15 @@
 
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             Repositioning,
             "should be in a repositioning state",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_repositioning_exit(self):
         vehicle = mock_vehicle()
         sim = mock_sim(
             vehicles=(vehicle,),
         )
         env = mock_env()
@@ -1280,15 +1282,15 @@
         enter_error, entered_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "test precondition (enter works correctly) not met")
 
         # begin test
         error, exited_sim = state.exit(Idle.build(vehicle.id), entered_sim, env)
 
         self.assertIsNone(error, "should have no errors")
-        self.assertEquals(entered_sim, exited_sim, "should see no change due to exit")
+        self.assertEqual(entered_sim, exited_sim, "should see no change due to exit")
 
     def test_repositioning_update(self):
         near = h3.geo_to_h3(39.7539, -104.974, 15)
         omf_brewing = h3.geo_to_h3(39.7608873, -104.9845391, 15)
         vehicle = mock_vehicle()
         sim = mock_sim(
             vehicles=(vehicle,),
@@ -1363,20 +1365,15 @@
         env = mock_env()
         route = mock_route_from_geoids(omf_brewing, vehicle.geoid)
 
         state = Repositioning.build(vehicle.id, route)
         enter_error, enter_sim = state.enter(sim, env)
 
         self.assertIsNone(enter_error, "should be no error")
-        self.assertIsNone(
-            enter_sim, "invalid route should have not changed sim state"
-        )  ####################################################################################################################
-
-    # ReserveBase ######################################################################################################
-    ####################################################################################################################
+        self.assertIsNone(enter_sim, "invalid route should have not changed sim state")
 
     def test_reserve_base_enter(self):
         vehicle = mock_vehicle()
         base = mock_base()
         sim = mock_sim(vehicles=(vehicle,), bases=(base,))
         env = mock_env()
 
@@ -1467,27 +1464,25 @@
 
     def test_reserve_base_enter_no_base(self):
         vehicle = mock_vehicle()
         sim = mock_sim(
             vehicles=(vehicle,),
         )
         env = mock_env()
-        route = ()
 
         state = ReserveBase.build(vehicle.id, DefaultIds.mock_base_id())
         enter_error, _ = state.enter(sim, env)
         self.assertIsInstance(enter_error, Exception, "should have exception")
 
     def test_reserve_base_enter_no_vehicle(self):
         base = mock_base()
         sim = mock_sim(
             bases=(base,),
         )
         env = mock_env()
-        route = ()
 
         state = ReserveBase.build(DefaultIds.mock_vehicle_id(), base.id)
         enter_error, _ = state.enter(sim, env)
         self.assertIsInstance(enter_error, Exception, "should have exception")
 
     def test_reserve_base_no_stalls_available(self):
         vehicle = mock_vehicle()
@@ -1502,20 +1497,14 @@
             "no stall failure should not result in an exception (fail silently)",
         )
         self.assertIsNone(
             entered_sim,
             "no stall failure should result in no SimulationState result",
         )
 
-    # def test_reserve_base_update_terminal(self):  # there is no terminal state for OutOfService
-
-    ####################################################################################################################
-    # ServicingTrip ####################################################################################################
-    ####################################################################################################################
-
     def test_servicing_trip_enter(self):
         prev_state = DispatchTrip.build(
             DefaultIds.mock_vehicle_id(), DefaultIds.mock_request_id(), ()
         )
         vehicle = mock_vehicle(vehicle_state=prev_state)
         request = mock_request_from_geoids(origin=vehicle.geoid)
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
@@ -1529,15 +1518,15 @@
 
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ServicingTrip,
             "should be in a ServicingTrip state",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_servicing_trip_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
         request = mock_request(fleet_id="lyft")
 
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
@@ -1619,16 +1608,14 @@
             error, "should have no errors"
         )  # errors due to passengers not being at destination
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             OutOfService,
             "vehicle should be out of service",
         )
-        # self.assertIsNotNone(updated_sim,
-        #                      "should have allowed exit of ServicingTrip because out of fuel allows transition to OutOfService")
 
     def test_servicing_trip_update(self):
         near = h3.geo_to_h3(39.7539, -104.974, 15)
         omf_brewing = h3.geo_to_h3(39.7608873, -104.9845391, 15)
         prev_state = DispatchTrip.build(
             DefaultIds.mock_vehicle_id(), DefaultIds.mock_request_id(), ()
         )
@@ -1757,18 +1744,14 @@
             vehicle.geoid, omf_brewing
         )  # request.destination should not be omf brewing co
 
         state = ServicingTrip.build(vehicle.id, request, sim.sim_time, route)
         enter_error, enter_sim = state.enter(sim, env)
         self.assertIsNotNone(enter_error, "bad destination is a good reason to bork this sim")
 
-    ####################################################################################################################
-    # ChargeQueueing ###################################################################################################
-    ####################################################################################################################
-
     def test_charge_queueing_enter(self):
         vehicle = mock_vehicle()
         s0 = mock_station()
         err, station = s0.checkout_charger(mock_dcfc_charger_id())
         self.assertIsNone(
             err,
             "test invariant failed (station should have charger checked out)",
@@ -1922,18 +1905,14 @@
 
         state = ChargeQueueing.build(vehicle_queueing.id, station.id, mock_dcfc_charger_id(), 0)
         error, updated_sim = state.enter(sim1, env)
 
         self.assertIsNone(error, "should have no errors")
         self.assertIsNone(updated_sim, "should not have entered a queueing state")
 
-    ####################################################################################################################
-    # DispatchPoolingTrip ##############################################################################################
-    ####################################################################################################################
-
     def test_dispatch_pooling_trip_enter(self):
         vehicle = mock_vehicle()
         request = mock_request()
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, request.geoid)
         trip_plan = (
@@ -1949,20 +1928,20 @@
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         updated_request = updated_sim.requests.get(request.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchPoolingTrip,
             "should be in a dispatch to request state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_request.dispatched_vehicle,
             vehicle.id,
             "request should be assigned this vehicle",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_dispatch_pooling_trip_enter_two_requests(self):
         vehicle = mock_vehicle()
         r1 = mock_request("r1", 39.70, -104.97, 39.85, -104.97)  # pickup 1, dropoff 2
         r2 = mock_request("r2", 39.75, -104.97, 39.80, -104.97)  # pickup 2, dropoff 1
         s0 = mock_sim(vehicles=(vehicle,))
         env = mock_env()
@@ -1986,25 +1965,25 @@
         updated_r1 = updated_sim.requests.get(r1.id)
         updated_r2 = updated_sim.requests.get(r2.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchPoolingTrip,
             "should be in a dispatch to request state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_r1.dispatched_vehicle,
             vehicle.id,
             "r1 should be assigned this vehicle",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_r2.dispatched_vehicle,
             vehicle.id,
             "r2 should be assigned this vehicle",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
 
     def test_dispatch_pooling_trip_bad_membership(self):
         vehicle = mock_vehicle(membership=Membership.single_membership("uber"))
         request = mock_request(fleet_id="lyft")
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, request.geoid)
@@ -2115,18 +2094,19 @@
             updated_request,
             "request should no longer exist as it has been picked up",
         )
         self.assertIsNotNone(
             boarded_request,
             f"request {request.id} should have boarded the vehicle",
         )
-        self.assertEquals(
+        self.assertEqual(
             boarded_request.id,
             request.id,
-            f"request {request.id} should have boarded the vehicle, found {boarded_request.id} instead",
+            f"request {request.id} should have boarded the vehicle, "
+            f"found {boarded_request.id} instead",
         )
 
     def test_dispatch_pooling_trip_enter_no_request(self):
         vehicle = mock_vehicle()
         request = mock_request()
         sim = mock_sim(vehicles=(vehicle,))  # request not added to sim
         env = mock_env()
@@ -2176,18 +2156,14 @@
         route = mock_route_from_geoids(vehicle.geoid, omf_brewing)
 
         state = DispatchTrip.build(vehicle.id, request.id, route)
         enter_error, enter_sim = state.enter(sim, env)
         self.assertIsNone(enter_error, "should be no error")
         self.assertIsNone(enter_sim, "invalid route should have not changed sim state")
 
-    ####################################################################################################################
-    # ServicingPoolingTrip #############################################################################################
-    ####################################################################################################################
-
     def test_servicing_pooling_trip_enter(self):
         vehicle = mock_vehicle()
         request = mock_request()
         sim = simulation_state_ops.add_request_safe(mock_sim(vehicles=(vehicle,)), request).unwrap()
         env = mock_env()
         route = mock_route_from_geoids(vehicle.geoid, request.geoid)
         trip_plan = (
@@ -2220,15 +2196,15 @@
 
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             ServicingPoolingTrip,
             "should be in a ServicingPoolingTrip state",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.routes), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.routes), 1, "should have a route")
 
     def test_servicing_pooling_trip_update_terminal(self):
         # 3 adjacent h3 cells, total trip distance is ~ 2 meters
         vehicle = mock_vehicle_from_geoid(geoid="8f268cd9601daa1")
         request = mock_request_from_geoids(origin="8f268cd9601daac", destination="8f268cd9601da10")
         sim0 = mock_sim(vehicles=(vehicle,), sim_timestep_duration_seconds=60)
 
@@ -2420,20 +2396,20 @@
         updated_vehicle = updated_sim.vehicles.get(vehicle.id)
         updated_request = updated_sim.requests.get(request.id)
         self.assertIsInstance(
             updated_vehicle.vehicle_state,
             DispatchPoolingTrip,
             "should be in a dispatch to request state",
         )
-        self.assertEquals(
+        self.assertEqual(
             updated_request.dispatched_vehicle,
             vehicle.id,
             "request should be assigned this vehicle",
         )
-        self.assertEquals(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
+        self.assertEqual(len(updated_vehicle.vehicle_state.route), 1, "should have a route")
         self.assertEqual(
             entered_state.instance_id,
             updated_vehicle.vehicle_state.instance_id,
             "should be the same instance",
         )
 
     def test_servicing_pooling_trip_exit(self):
```

### Comparing `nrel.hive-1.2.2/tests/test_vehicle_state_ops.py` & `nrel.hive-1.3.0/tests/test_vehicle_state_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 from unittest import TestCase
 
+import h3
+
 from returns.result import Success
+from nrel.hive.model.energy.energytype import EnergyType
+from nrel.hive.resources.mock_lobster import (
+    DefaultIds,
+    mock_base_from_geoid,
+    mock_dcfc_charger_id,
+    mock_env,
+    mock_sim,
+    mock_station_from_geoid,
+    mock_vehicle_from_geoid,
+)
+from nrel.hive.state.simulation_state import simulation_state_ops
 
 from nrel.hive.state.vehicle_state import vehicle_state_ops
-from nrel.hive.resources.mock_lobster import *
+from nrel.hive.state.vehicle_state.charging_base import ChargingBase
+from nrel.hive.state.vehicle_state.repositioning import Repositioning
 
 
 class TestVehicleStateOps(TestCase):
     def test_move(self):
         somewhere = h3.geo_to_h3(39.7539, -104.974, 15)
         somewhere_else = h3.geo_to_h3(39.7579, -104.978, 15)
         sim = mock_sim(sim_timestep_duration_seconds=10)
```

