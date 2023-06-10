# Comparing `tmp/isar-1.9.1.tar.gz` & `tmp/isar-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isar-1.9.1.tar", last modified: Fri Jun 24 06:25:27 2022, max compression
+gzip compressed data, was "isar-1.9.2.tar", last modified: Tue Jul  5 08:29:35 2022, max compression
```

## Comparing `isar-1.9.1.tar` & `isar-1.9.2.tar`

### file list

```diff
@@ -1,255 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.493464 isar-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-24 06:25:05.000000 isar-1.9.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.457483 isar-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.457483 isar-1.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-24 06:25:05.000000 isar-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-06-24 06:25:05.000000 isar-1.9.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-06-24 06:25:05.000000 isar-1.9.1/.github/ISSUE_TEMPLATE/improvement.md
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-06-24 06:25:05.000000 isar-1.9.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.457483 isar-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-06-24 06:25:05.000000 isar-1.9.1/.github/workflows/project_automations.yml
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-06-24 06:25:05.000000 isar-1.9.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-06-24 06:25:05.000000 isar-1.9.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-06-24 06:25:05.000000 isar-1.9.1/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-06-24 06:25:05.000000 isar-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-06-24 06:25:05.000000 isar-1.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    14058 2022-06-24 06:25:05.000000 isar-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10873 2022-06-24 06:25:27.493464 isar-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10213 2022-06-24 06:25:05.000000 isar-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-06-24 06:25:05.000000 isar-1.9.1/docker-compose-turtlebot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-06-24 06:25:05.000000 isar-1.9.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.457483 isar-1.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-06-24 06:25:05.000000 isar-1.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-24 06:25:05.000000 isar-1.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-06-24 06:25:05.000000 isar-1.9.1/docs/rst_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-06-24 06:25:05.000000 isar-1.9.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-06-24 06:25:05.000000 isar-1.9.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-24 06:25:05.000000 isar-1.9.1/docs/source/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-06-24 06:25:05.000000 isar-1.9.1/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-24 06:25:05.000000 isar-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-24 06:25:05.000000 isar-1.9.1/radixconfig.yml
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-24 06:25:27.493464 isar-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-06-24 06:25:05.000000 isar-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.453485 isar-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar/apis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7714 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar/apis/models/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar/apis/schedule/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11307 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/schedule/scheduling_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar/apis/security/
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/apis/security/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.465479 isar-1.9.1/src/isar/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/configuration_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.465479 isar-1.9.1/src/isar/config/keyvault/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/keyvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/keyvault/keyvault_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/keyvault/keyvault_service.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.465479 isar-1.9.1/src/isar/config/maps/
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/JSP1_intermediate_deck.json
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/JSP1_weather_deck.json
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/default_map.json
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/klab_b.json
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/klab_compressor.json
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/klab_turtlebot.json
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/maps/turtleworld.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.465479 isar-1.9.1/src/isar/config/predefined_missions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/predefined_missions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/predefined_missions/default.json
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/predefined_missions/default_turtlebot.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.465479 isar-1.9.1/src/isar/config/predefined_poses/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/predefined_poses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24720 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/predefined_poses/predefined_poses.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/settings.env
--rw-r--r--   0 runner    (1001) docker     (121)     8568 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/mission_planner/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/mission_planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5680 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/mission_planner/echo_planner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/mission_planner/local_planner.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/mission_planner/mission_planner_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/mission_planner/mission_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/models/communication/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/models/communication/queues/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/queues/queue_io.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/queues/queue_timeout_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/queues/queues.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/communication/queues/status_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/models/mission/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/mission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/mission/mission.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/mission/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/models/mission_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/mission_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/models/mission_metadata/mission_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.469477 isar-1.9.1/src/isar/services/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/auth/azure_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/services/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/readers/base_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/services/service_connections/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/services/service_connections/mqtt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/mqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/services/service_connections/stid/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/stid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/service_connections/stid/stid_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/services/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/utilities/queue_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/utilities/scheduling_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/services/utilities/threaded_request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.473474 isar-1.9.1/src/isar/state_machine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17658 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/isar/state_machine/states/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/idle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/initialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/initiate_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/off.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/paused.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states/stop_step.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/state_machine/states_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/isar/storage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/slimm_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-06-24 06:25:05.000000 isar-1.9.1/src/isar/storage/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.461481 isar-1.9.1/src/isar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10873 2022-06-24 06:25:26.000000 isar-1.9.1/src/isar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7165 2022-06-24 06:25:27.000000 isar-1.9.1/src/isar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 06:25:26.000000 isar-1.9.1/src/isar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-06-24 06:25:27.000000 isar-1.9.1/src/isar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-24 06:25:27.000000 isar-1.9.1/src/isar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/robot_interface/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/robot_interface/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/robot_interface/models/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/exceptions/robot_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/robot_interface/models/initialize/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/initialize/initialize_params.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.477472 isar-1.9.1/src/robot_interface/models/inspection/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/inspection/inspection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/src/robot_interface/models/mission/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/mission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/mission/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/models/mission/step.py
--rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/robot_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/src/robot_interface/telemetry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/telemetry/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/telemetry/payloads.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/test_robot_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/src/robot_interface/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-06-24 06:25:05.000000 isar-1.9.1/src/robot_interface/utilities/json_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-06-24 06:25:05.000000 isar-1.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/integration/turtlebot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/integration/turtlebot/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/integration/turtlebot/config/maps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/config/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/config/maps/turtleworld.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/integration/turtlebot/config/missions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/config/missions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/config/missions/default.json
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-06-24 06:25:05.000000 isar-1.9.1/tests/integration/turtlebot/test_successful_mission.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/isar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.481470 isar-1.9.1/tests/isar/apis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/apis/scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/apis/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/apis/scheduler/test_scheduler_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/apis/security/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/apis/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/apis/security/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/mission_planner/
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/mission_planner/test_mission_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/models/communication/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/models/communication/test_queues.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/readers/test_base_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/readers/test_mission_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/service_connections/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/service_connections/echo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/echo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/echo/test_echo_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/service_connections/stid/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/stid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/stid/test_stid_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/service_connections/test_base_request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.485468 isar-1.9.1/tests/isar/services/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/utilities/test_queue_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/services/utilities/test_scheduling_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.489466 isar-1.9.1/tests/isar/state_machine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/state_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.489466 isar-1.9.1/tests/isar/state_machine/states/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/state_machine/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/state_machine/states/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6243 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/state_machine/test_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.489466 isar-1.9.1/tests/isar/storage/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/storage/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-06-24 06:25:05.000000 isar-1.9.1/tests/isar/storage/test_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.489466 isar-1.9.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/mission_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/pose.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/robot_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/status.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/step.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/task.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-24 06:25:05.000000 isar-1.9.1/tests/mocks/token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.489466 isar-1.9.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_json_file.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 06:25:27.493464 isar-1.9.1/tests/test_data/test_map_config/
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_map_config/test_map_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_mission_not_working.json
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_mission_working.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_mission_working_no_tasks.json
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_data/test_thermal_image_mission.json
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-06-24 06:25:05.000000 isar-1.9.1/tests/test_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.248777 isar-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-07-05 08:29:10.000000 isar-1.9.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.216776 isar-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.216776 isar-1.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-05 08:29:10.000000 isar-1.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-05 08:29:10.000000 isar-1.9.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-07-05 08:29:10.000000 isar-1.9.2/.github/ISSUE_TEMPLATE/improvement.md
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-05 08:29:10.000000 isar-1.9.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-07-05 08:29:10.000000 isar-1.9.2/.github/workflows/project_automations.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-07-05 08:29:10.000000 isar-1.9.2/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-07-05 08:29:10.000000 isar-1.9.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-07-05 08:29:10.000000 isar-1.9.2/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-07-05 08:29:10.000000 isar-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-07-05 08:29:10.000000 isar-1.9.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)    14058 2022-07-05 08:29:10.000000 isar-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-07-05 08:29:35.248777 isar-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10213 2022-07-05 08:29:10.000000 isar-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-07-05 08:29:10.000000 isar-1.9.2/docker-compose-turtlebot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-05 08:29:10.000000 isar-1.9.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-07-05 08:29:10.000000 isar-1.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-07-05 08:29:10.000000 isar-1.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-07-05 08:29:10.000000 isar-1.9.2/docs/rst_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-07-05 08:29:10.000000 isar-1.9.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-07-05 08:29:10.000000 isar-1.9.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-05 08:29:10.000000 isar-1.9.2/docs/source/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-07-05 08:29:10.000000 isar-1.9.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-05 08:29:10.000000 isar-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-07-05 08:29:10.000000 isar-1.9.2/radixconfig.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-05 08:29:35.252777 isar-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-07-05 08:29:10.000000 isar-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.212776 isar-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7714 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar/apis/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar/apis/schedule/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11307 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/schedule/scheduling_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar/apis/security/
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/apis/security/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/certs/
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/certs/ca-cert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/configuration_error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/keyvault/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/keyvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/keyvault/keyvault_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/keyvault/keyvault_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/maps/
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/JSP1_intermediate_deck.json
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/JSP1_weather_deck.json
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/default_map.json
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/klab_b.json
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/klab_compressor.json
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/klab_turtlebot.json
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/maps/turtleworld.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/predefined_missions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/predefined_missions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/predefined_missions/default.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/predefined_missions/default_turtlebot.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.224776 isar-1.9.2/src/isar/config/predefined_poses/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/predefined_poses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24720 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/predefined_poses/predefined_poses.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/settings.env
+-rw-r--r--   0 runner    (1001) docker     (121)     8568 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/mission_planner/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/mission_planner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5680 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/mission_planner/echo_planner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/mission_planner/local_planner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/mission_planner/mission_planner_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/mission_planner/mission_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/models/communication/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/message.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/models/communication/queues/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/queues/queue_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/queues/queue_timeout_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/queues/queues.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/communication/queues/status_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/models/mission/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/mission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/mission/mission.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/mission/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/models/mission_metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/mission_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/models/mission_metadata/mission_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/auth/azure_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/readers/base_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/service_connections/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/service_connections/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3571 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/mqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.228776 isar-1.9.2/src/isar/services/service_connections/stid/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/stid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/service_connections/stid/stid_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.232776 isar-1.9.2/src/isar/services/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/utilities/queue_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/utilities/scheduling_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/services/utilities/threaded_request.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.232776 isar-1.9.2/src/isar/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17658 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.232776 isar-1.9.2/src/isar/state_machine/states/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/idle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/initiate_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/off.py
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/paused.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states/stop_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/state_machine/states_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.232776 isar-1.9.2/src/isar/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/slimm_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-07-05 08:29:10.000000 isar-1.9.2/src/isar/storage/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.220776 isar-1.9.2/src/isar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-07-05 08:29:35.000000 isar-1.9.2/src/isar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7199 2022-07-05 08:29:35.000000 isar-1.9.2/src/isar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 08:29:35.000000 isar-1.9.2/src/isar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-05 08:29:35.000000 isar-1.9.2/src/isar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-05 08:29:35.000000 isar-1.9.2/src/isar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/models/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/exceptions/robot_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/models/initialize/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/initialize/initialize_params.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/models/inspection/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/inspection/inspection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/models/mission/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/mission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/mission/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/models/mission/step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/robot_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/telemetry/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/telemetry/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/test_robot_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.236776 isar-1.9.2/src/robot_interface/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-07-05 08:29:10.000000 isar-1.9.2/src/robot_interface/utilities/json_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-07-05 08:29:10.000000 isar-1.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/integration/turtlebot/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/integration/turtlebot/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/integration/turtlebot/config/maps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/config/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/config/maps/turtleworld.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/integration/turtlebot/config/missions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/config/missions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/config/missions/default.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-07-05 08:29:10.000000 isar-1.9.2/tests/integration/turtlebot/test_successful_mission.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/apis/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/apis/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/apis/scheduler/test_scheduler_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/apis/security/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/apis/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/apis/security/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/mission_planner/
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/mission_planner/test_mission_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/models/communication/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/models/communication/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.240776 isar-1.9.2/tests/isar/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/services/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/readers/test_base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/readers/test_mission_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/services/service_connections/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/services/service_connections/echo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/echo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/echo/test_echo_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/services/service_connections/stid/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/stid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/stid/test_stid_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/service_connections/test_base_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/services/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/utilities/test_queue_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/services/utilities/test_scheduling_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/state_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/state_machine/states/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/state_machine/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/state_machine/states/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6243 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/state_machine/test_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.244777 isar-1.9.2/tests/isar/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/storage/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-07-05 08:29:10.000000 isar-1.9.2/tests/isar/storage/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.248777 isar-1.9.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/mission_definition.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/pose.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/robot_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/step.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-05 08:29:10.000000 isar-1.9.2/tests/mocks/token.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.248777 isar-1.9.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_json_file.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 08:29:35.248777 isar-1.9.2/tests/test_data/test_map_config/
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_map_config/test_map_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_mission_not_working.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_mission_working.json
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_mission_working_no_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_data/test_thermal_image_mission.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-07-05 08:29:10.000000 isar-1.9.2/tests/test_modules.py
```

### Comparing `isar-1.9.1/.github/workflows/project_automations.yml` & `isar-1.9.2/.github/workflows/project_automations.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/.github/workflows/pythonpackage.yml` & `isar-1.9.2/.github/workflows/pythonpackage.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       - main
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.9", "3.10"]
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `isar-1.9.1/.github/workflows/pythonpublish.yml` & `isar-1.9.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/.github/workflows/stale.yml` & `isar-1.9.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/.gitignore` & `isar-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/Dockerfile` & `isar-1.9.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/LICENSE` & `isar-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/PKG-INFO` & `isar-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: isar
-Version: 1.9.1
+Version: 1.9.2
 Summary: Integration and Supervisory control of Autonomous Robots
 Home-page: https://github.com/equinor/isar
 Author: Equinor ASA
 Author-email: fg_robots_dev@equinor.com
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ISAR
 
 [![Python package](https://github.com/equinor/isar/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/equinor/isar/actions/workflows/pythonpackage.yml)
```

### Comparing `isar-1.9.1/README.md` & `isar-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/docker-compose-turtlebot.yml` & `isar-1.9.2/docker-compose-turtlebot.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/docker-compose.yml` & `isar-1.9.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/docs/Makefile` & `isar-1.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/docs/make.bat` & `isar-1.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/docs/source/conf.py` & `isar-1.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/main.py` & `isar-1.9.2/main.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/radixconfig.yml` & `isar-1.9.2/radixconfig.yml`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/setup.cfg` & `isar-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/setup.py` & `isar-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,9 +52,9 @@
             "pytest-mock",
             "pytest-xdist",
             "pytest",
             "requests-mock",
             "sphinx",
         ]
     },
-    python_requires=">=3.10",
+    python_requires=">=3.9",
 )
```

### Comparing `isar-1.9.1/src/isar/apis/api.py` & `isar-1.9.2/src/isar/apis/api.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/apis/schedule/scheduling_controller.py` & `isar-1.9.2/src/isar/apis/schedule/scheduling_controller.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/apis/security/authentication.py` & `isar-1.9.2/src/isar/apis/security/authentication.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/keyvault/keyvault_service.py` & `isar-1.9.2/src/isar/config/keyvault/keyvault_service.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/log.py` & `isar-1.9.2/src/isar/config/log.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/logging.conf` & `isar-1.9.2/src/isar/config/logging.conf`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/JSP1_intermediate_deck.json` & `isar-1.9.2/src/isar/config/maps/JSP1_intermediate_deck.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/JSP1_weather_deck.json` & `isar-1.9.2/src/isar/config/maps/JSP1_weather_deck.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/default_map.json` & `isar-1.9.2/src/isar/config/maps/default_map.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/klab_b.json` & `isar-1.9.2/src/isar/config/maps/klab_b.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/klab_compressor.json` & `isar-1.9.2/src/isar/config/maps/klab_compressor.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/klab_turtlebot.json` & `isar-1.9.2/src/isar/config/maps/klab_turtlebot.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/maps/turtleworld.json` & `isar-1.9.2/src/isar/config/maps/turtleworld.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/predefined_missions/default.json` & `isar-1.9.2/src/isar/config/predefined_missions/default.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/predefined_missions/default_turtlebot.json` & `isar-1.9.2/src/isar/config/predefined_missions/default_turtlebot.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/predefined_poses/predefined_poses.py` & `isar-1.9.2/src/isar/config/predefined_poses/predefined_poses.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/config/settings.py` & `isar-1.9.2/src/isar/config/settings.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/mission_planner/echo_planner.py` & `isar-1.9.2/src/isar/mission_planner/echo_planner.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/mission_planner/local_planner.py` & `isar-1.9.2/src/isar/mission_planner/local_planner.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/models/communication/queues/queues.py` & `isar-1.9.2/src/isar/models/communication/queues/queues.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/models/mission/mission.py` & `isar-1.9.2/src/isar/models/mission/mission.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/models/mission/status.py` & `isar-1.9.2/src/isar/models/mission/status.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/models/mission_metadata/mission_metadata.py` & `isar-1.9.2/src/isar/models/mission_metadata/mission_metadata.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/modules.py` & `isar-1.9.2/src/isar/modules.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/readers/base_reader.py` & `isar-1.9.2/src/isar/services/readers/base_reader.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/service_connections/mqtt/mqtt_client.py` & `isar-1.9.2/src/isar/services/service_connections/mqtt/mqtt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
         self.port: int = settings.MQTT_PORT
 
         self.client: Client = Client()
 
         self.client.enable_logger(logger=self.logger)
 
+        dirname = os.path.dirname(__file__)
+        cert_path = os.path.join(dirname, "../../../config/certs/ca-cert.pem")
+        self.client.tls_set(ca_certs=cert_path)
         self.client.on_connect = self.on_connect
         self.client.on_disconnect = self.on_disconnect
 
         self.client.username_pw_set(username=username, password=password)
 
     def run(self) -> None:
         self.connect(host=self.host, port=self.port)
```

### Comparing `isar-1.9.1/src/isar/services/service_connections/request_handler.py` & `isar-1.9.2/src/isar/services/service_connections/request_handler.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/service_connections/stid/stid_service.py` & `isar-1.9.2/src/isar/services/service_connections/stid/stid_service.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/utilities/queue_utilities.py` & `isar-1.9.2/src/isar/services/utilities/queue_utilities.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/utilities/scheduling_utilities.py` & `isar-1.9.2/src/isar/services/utilities/scheduling_utilities.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/services/utilities/threaded_request.py` & `isar-1.9.2/src/isar/services/utilities/threaded_request.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/state_machine.py` & `isar-1.9.2/src/isar/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/idle.py` & `isar-1.9.2/src/isar/state_machine/states/idle.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/initialize.py` & `isar-1.9.2/src/isar/state_machine/states/initialize.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/initiate_step.py` & `isar-1.9.2/src/isar/state_machine/states/initiate_step.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/monitor.py` & `isar-1.9.2/src/isar/state_machine/states/monitor.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/off.py` & `isar-1.9.2/src/isar/state_machine/states/off.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/paused.py` & `isar-1.9.2/src/isar/state_machine/states/paused.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/state_machine/states/stop_step.py` & `isar-1.9.2/src/isar/state_machine/states/stop_step.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/blob_storage.py` & `isar-1.9.2/src/isar/storage/blob_storage.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/local_storage.py` & `isar-1.9.2/src/isar/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/slimm_storage.py` & `isar-1.9.2/src/isar/storage/slimm_storage.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/storage_interface.py` & `isar-1.9.2/src/isar/storage/storage_interface.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/uploader.py` & `isar-1.9.2/src/isar/storage/uploader.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar/storage/utilities.py` & `isar-1.9.2/src/isar/storage/utilities.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/isar.egg-info/PKG-INFO` & `isar-1.9.2/src/isar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: isar
-Version: 1.9.1
+Version: 1.9.2
 Summary: Integration and Supervisory control of Autonomous Robots
 Home-page: https://github.com/equinor/isar
 Author: Equinor ASA
 Author-email: fg_robots_dev@equinor.com
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ISAR
 
 [![Python package](https://github.com/equinor/isar/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/equinor/isar/actions/workflows/pythonpackage.yml)
```

### Comparing `isar-1.9.1/src/isar.egg-info/SOURCES.txt` & `isar-1.9.2/src/isar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/isar/apis/security/authentication.py
 src/isar/config/__init__.py
 src/isar/config/configuration_error.py
 src/isar/config/log.py
 src/isar/config/logging.conf
 src/isar/config/settings.env
 src/isar/config/settings.py
+src/isar/config/certs/ca-cert.pem
 src/isar/config/keyvault/__init__.py
 src/isar/config/keyvault/keyvault_error.py
 src/isar/config/keyvault/keyvault_service.py
 src/isar/config/maps/JSP1_intermediate_deck.json
 src/isar/config/maps/JSP1_weather_deck.json
 src/isar/config/maps/default_map.json
 src/isar/config/maps/klab_b.json
```

### Comparing `isar-1.9.1/src/robot_interface/models/inspection/inspection.py` & `isar-1.9.2/src/robot_interface/models/inspection/inspection.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/robot_interface/models/mission/step.py` & `isar-1.9.2/src/robot_interface/models/mission/step.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/robot_interface/robot_interface.py` & `isar-1.9.2/src/robot_interface/robot_interface.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/robot_interface/telemetry/mqtt_client.py` & `isar-1.9.2/src/robot_interface/telemetry/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/robot_interface/test_robot_interface.py` & `isar-1.9.2/src/robot_interface/test_robot_interface.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/src/robot_interface/utilities/json_service.py` & `isar-1.9.2/src/robot_interface/utilities/json_service.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/conftest.py` & `isar-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/integration/turtlebot/config/maps/turtleworld.json` & `isar-1.9.2/tests/integration/turtlebot/config/maps/turtleworld.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/integration/turtlebot/config/missions/default.json` & `isar-1.9.2/tests/integration/turtlebot/config/missions/default.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/integration/turtlebot/test_successful_mission.py` & `isar-1.9.2/tests/integration/turtlebot/test_successful_mission.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/apis/scheduler/test_scheduler_routes.py` & `isar-1.9.2/tests/isar/apis/scheduler/test_scheduler_routes.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/apis/security/test_authentication.py` & `isar-1.9.2/tests/isar/apis/security/test_authentication.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/mission_planner/test_mission_validator.py` & `isar-1.9.2/tests/isar/mission_planner/test_mission_validator.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/models/communication/test_queues.py` & `isar-1.9.2/tests/isar/models/communication/test_queues.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/readers/test_base_reader.py` & `isar-1.9.2/tests/isar/services/readers/test_base_reader.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/readers/test_mission_reader.py` & `isar-1.9.2/tests/isar/services/readers/test_mission_reader.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/service_connections/echo/test_echo_service.py` & `isar-1.9.2/tests/isar/services/service_connections/echo/test_echo_service.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/service_connections/stid/test_stid_service.py` & `isar-1.9.2/tests/isar/services/service_connections/stid/test_stid_service.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/service_connections/test_base_request_handler.py` & `isar-1.9.2/tests/isar/services/service_connections/test_base_request_handler.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/utilities/test_queue_utilities.py` & `isar-1.9.2/tests/isar/services/utilities/test_queue_utilities.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/services/utilities/test_scheduling_utilities.py` & `isar-1.9.2/tests/isar/services/utilities/test_scheduling_utilities.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/state_machine/states/test_monitor.py` & `isar-1.9.2/tests/isar/state_machine/states/test_monitor.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/state_machine/test_state_machine.py` & `isar-1.9.2/tests/isar/state_machine/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/storage/test_blob_storage.py` & `isar-1.9.2/tests/isar/storage/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/isar/storage/test_uploader.py` & `isar-1.9.2/tests/isar/storage/test_uploader.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/mocks/blob_storage.py` & `isar-1.9.2/tests/mocks/blob_storage.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/mocks/mission_definition.py` & `isar-1.9.2/tests/mocks/mission_definition.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/mocks/robot_interface.py` & `isar-1.9.2/tests/mocks/robot_interface.py`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/test_data/test_json_file.json` & `isar-1.9.2/tests/test_data/test_json_file.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/test_data/test_map_config/test_map_config.json` & `isar-1.9.2/tests/test_data/test_map_config/test_map_config.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/test_data/test_mission_not_working.json` & `isar-1.9.2/tests/test_data/test_mission_not_working.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/test_data/test_mission_working.json` & `isar-1.9.2/tests/test_data/test_mission_working.json`

 * *Files identical despite different names*

### Comparing `isar-1.9.1/tests/test_modules.py` & `isar-1.9.2/tests/test_modules.py`

 * *Files identical despite different names*

