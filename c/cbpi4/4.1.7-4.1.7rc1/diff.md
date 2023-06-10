# Comparing `tmp/cbpi4-4.1.7.tar.gz` & `tmp/cbpi4-4.1.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-4.1.7.tar", last modified: Thu Mar 30 05:12:19 2023, max compression
+gzip compressed data, was "cbpi4-4.1.7rc1.tar", last modified: Sun Mar 26 14:42:18 2023, max compression
```

## Comparing `cbpi4-4.1.7.tar` & `cbpi4-4.1.7rc1.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.154069 cbpi4-4.1.7/
--rw-rw-rw-   0        0        0    35823 2021-12-30 07:59:04.000000 cbpi4-4.1.7/LICENSE
--rw-rw-rw-   0        0        0      100 2021-12-30 07:59:04.000000 cbpi4-4.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2770 2023-03-30 05:12:19.152065 cbpi4-4.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-03-10 14:45:36.000000 cbpi4-4.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.451407 cbpi4-4.1.7/cbpi/
--rw-rw-rw-   0        0        0       57 2023-03-29 04:53:34.000000 cbpi4-4.1.7/cbpi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.533411 cbpi4-4.1.7/cbpi/api/
--rw-rw-rw-   0        0        0      841 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/__init__.py
--rw-rw-rw-   0        0        0     2248 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/actor.py
--rw-rw-rw-   0        0        0     2553 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/api/base.py
--rw-rw-rw-   0        0        0      238 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/config.py
--rw-rw-rw-   0        0        0     6694 2023-03-08 17:51:21.000000 cbpi4-4.1.7/cbpi/api/dataclasses.py
--rw-rw-rw-   0        0        0     2384 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/api/decorator.py
--rw-rw-rw-   0        0        0      356 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/exceptions.py
--rw-rw-rw-   0        0        0     1194 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/api/extension.py
--rw-rw-rw-   0        0        0     1071 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/fermenter_logic.py
--rw-rw-rw-   0        0        0     1068 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/api/kettle_logic.py
--rw-rw-rw-   0        0        0     3821 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/property.py
--rw-rw-rw-   0        0        0     1847 2023-03-08 17:51:54.000000 cbpi4-4.1.7/cbpi/api/sensor.py
--rw-rw-rw-   0        0        0     5926 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/step.py
--rw-rw-rw-   0        0        0     2508 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/api/timer.py
--rw-rw-rw-   0        0        0    12806 2023-02-07 18:06:09.000000 cbpi4-4.1.7/cbpi/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.573516 cbpi4-4.1.7/cbpi/config/
--rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/actor.json
--rw-rw-rw-   0        0        0      264 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/config/chromium.desktop
--rw-rw-rw-   0        0        0     4038 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/config.json
--rw-rw-rw-   0        0        0      243 2022-11-17 18:42:08.000000 cbpi4-4.1.7/cbpi/config/config.yaml
--rw-rw-rw-   0        0        0      152 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/craftbeerpi.service
--rw-rw-rw-   0        0        0     1676 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/craftbeerpiboot
--rw-rw-rw-   0        0        0     2711 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/create_database.sql
--rw-rw-rw-   0        0        0       35 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/config/fermenter_data.json
--rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/kettle.json
--rw-rw-rw-   0        0        0       73 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/plugin_list.txt
--rw-rw-rw-   0        0        0       36 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/sensor.json
--rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/splash.png
--rw-rw-rw-   0        0        0       81 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/config/step_data.json
--rw-rw-rw-   0        0        0    11053 2023-01-26 16:36:52.000000 cbpi4-4.1.7/cbpi/configFolder.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.627300 cbpi4-4.1.7/cbpi/controller/
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/controller/__init__.py
--rw-rw-rw-   0        0        0     3418 2022-11-17 18:47:01.000000 cbpi4-4.1.7/cbpi/controller/actor_controller.py
--rw-rw-rw-   0        0        0     6177 2023-03-08 18:12:15.000000 cbpi4-4.1.7/cbpi/controller/basic_controller2.py
--rw-rw-rw-   0        0        0     2322 2022-11-17 18:47:01.000000 cbpi4-4.1.7/cbpi/controller/config_controller.py
--rw-rw-rw-   0        0        0     2797 2023-01-22 15:33:23.000000 cbpi4-4.1.7/cbpi/controller/dashboard_controller.py
--rw-rw-rw-   0        0        0    23493 2023-01-26 16:40:07.000000 cbpi4-4.1.7/cbpi/controller/fermentation_controller.py
--rw-rw-rw-   0        0        0     2807 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/controller/fermenter_recipe_controller.py
--rw-rw-rw-   0        0        0     1662 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/controller/job_controller.py
--rw-rw-rw-   0        0        0     1722 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/controller/kettle_controller.py
--rw-rw-rw-   0        0        0     9533 2023-03-24 21:18:30.000000 cbpi4-4.1.7/cbpi/controller/log_file_controller.py
--rw-rw-rw-   0        0        0     3336 2023-01-22 15:30:15.000000 cbpi4-4.1.7/cbpi/controller/notification_controller.py
--rw-rw-rw-   0        0        0     9768 2023-01-27 10:53:55.000000 cbpi4-4.1.7/cbpi/controller/plugin_controller.py
--rw-rw-rw-   0        0        0     2849 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/controller/recipe_controller.py
--rw-rw-rw-   0        0        0     8030 2023-03-26 13:21:40.000000 cbpi4-4.1.7/cbpi/controller/satellite_controller.py
--rw-rw-rw-   0        0        0     1040 2023-03-08 18:10:16.000000 cbpi4-4.1.7/cbpi/controller/sensor_controller.py
--rw-rw-rw-   0        0        0    13578 2023-01-26 16:39:43.000000 cbpi4-4.1.7/cbpi/controller/step_controller.py
--rw-rw-rw-   0        0        0    12802 2022-11-17 18:47:01.000000 cbpi4-4.1.7/cbpi/controller/system_controller.py
--rw-rw-rw-   0        0        0    54504 2022-11-19 11:46:41.000000 cbpi4-4.1.7/cbpi/controller/upload_controller.py
--rw-rw-rw-   0        0        0    12388 2023-01-20 16:30:21.000000 cbpi4-4.1.7/cbpi/craftbeerpi.py
--rw-rw-rw-   0        0        0     7029 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/eventbus.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.630299 cbpi4-4.1.7/cbpi/extension/
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.636304 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/
--rw-rw-rw-   0        0        0    20211 2023-03-24 06:10:43.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.646654 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/
--rw-rw-rw-   0        0        0     8582 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    22659 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     7583 2022-02-16 16:13:43.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     9326 2023-03-24 17:11:00.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       47 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/ConfigUpdate/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.653650 cbpi4-4.1.7/cbpi/extension/FermentationStep/
--rw-rw-rw-   0        0        0    20143 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.667647 cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/
--rw-rw-rw-   0        0        0    14091 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    34360 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    11626 2022-02-25 13:23:11.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    14328 2022-05-09 15:22:15.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       48 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/FermentationStep/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.674644 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/
--rw-rw-rw-   0        0        0    12519 2023-01-27 16:09:06.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.688645 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/
--rw-rw-rw-   0        0        0     7807 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    17903 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     4843 2022-01-03 11:51:56.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     8266 2023-01-27 16:59:06.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       51 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/config.yaml
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.701808 cbpi4-4.1.7/cbpi/extension/__pycache__/
--rw-rw-rw-   0        0        0      130 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      155 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      159 2022-02-26 13:38:02.000000 cbpi4-4.1.7/cbpi/extension/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.707644 cbpi4-4.1.7/cbpi/extension/dummyactor/
--rw-rw-rw-   0        0        0     1281 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.721645 cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/
--rw-rw-rw-   0        0        0     2167 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3282 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2181 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2202 2022-02-26 13:38:02.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       42 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/dummyactor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.726645 cbpi4-4.1.7/cbpi/extension/dummysensor/
--rw-rw-rw-   0        0        0     2728 2023-03-07 19:37:46.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.760648 cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/
--rw-rw-rw-   0        0        0     2871 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     5500 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1359 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2971 2023-03-07 19:55:17.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/dummysensor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.770646 cbpi4-4.1.7/cbpi/extension/gpioactor/
--rw-rw-rw-   0        0        0     6111 2023-03-10 17:08:18.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.789646 cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/
--rw-rw-rw-   0        0        0     5776 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    11052 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     5823 2022-02-16 16:13:43.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     5737 2023-03-10 17:08:23.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       41 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/gpioactor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.794644 cbpi4-4.1.7/cbpi/extension/httpsensor/
--rw-rw-rw-   0        0        0     7781 2023-03-28 04:58:15.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.806053 cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/
--rw-rw-rw-   0        0        0     3249 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7516 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3212 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     6170 2023-03-27 18:06:10.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/httpsensor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.811053 cbpi4-4.1.7/cbpi/extension/hysteresis/
--rw-rw-rw-   0        0        0     2210 2023-03-02 05:51:03.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.823054 cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/
--rw-rw-rw-   0        0        0     1905 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4025 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1798 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2012 2023-03-04 10:48:54.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       48 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/hysteresis/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.829053 cbpi4-4.1.7/cbpi/extension/mashstep/
--rw-rw-rw-   0        0        0    26901 2023-02-11 14:27:45.000000 cbpi4-4.1.7/cbpi/extension/mashstep/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.840053 cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/
--rw-rw-rw-   0        0        0    19082 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    46297 2023-03-09 06:14:16.000000 cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    20852 2022-01-04 06:30:42.000000 cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    21087 2023-02-11 14:27:52.000000 cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       40 2022-01-04 06:30:19.000000 cbpi4-4.1.7/cbpi/extension/mashstep/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.853053 cbpi4-4.1.7/cbpi/extension/mqtt_actor/
--rw-rw-rw-   0        0        0      650 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.900052 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/
--rw-rw-rw-   0        0        0      804 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1278 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      819 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      837 2022-03-21 11:27:58.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2164 2023-01-07 21:29:06.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     3552 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2148 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0     2173 2022-11-27 13:47:03.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0     2396 2023-01-07 21:29:05.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     4334 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2338 2022-01-25 10:19:18.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0     2397 2022-11-27 13:47:03.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0      869 2023-01-07 21:29:06.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     1267 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0      874 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0      902 2022-03-21 11:27:58.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/config.yaml
--rw-rw-rw-   0        0        0     1702 2022-11-17 18:47:01.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/generic_mqtt_actor.py
--rw-rw-rw-   0        0        0     1922 2022-11-17 18:47:01.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/mqtt_actor.py
--rw-rw-rw-   0        0        0      442 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/mqtt_actor/tasmota_mqtt_actor.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.906054 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/
--rw-rw-rw-   0        0        0     7318 2023-03-28 04:55:57.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.917054 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/
--rw-rw-rw-   0        0        0     2481 2023-01-07 21:29:06.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7045 2023-03-09 06:14:17.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2438 2021-12-30 07:59:45.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     5647 2023-03-27 17:56:03.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/mqtt_sensor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.922052 cbpi4-4.1.7/cbpi/extension/mqtt_util/
--rw-rw-rw-   0        0        0     2618 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.932597 cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/
--rw-rw-rw-   0        0        0     2130 2023-01-07 21:29:06.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4059 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2117 2022-02-16 16:13:43.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2143 2022-03-21 11:27:58.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       42 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/extension/mqtt_util/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.938596 cbpi4-4.1.7/cbpi/extension/onewire/
--rw-rw-rw-   0        0        0     7292 2023-03-28 04:56:56.000000 cbpi4-4.1.7/cbpi/extension/onewire/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.949593 cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/
--rw-rw-rw-   0        0        0     3813 2023-01-07 21:29:06.000000 cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7131 2023-01-15 12:43:43.000000 cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3737 2022-01-25 10:19:18.000000 cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     6059 2023-03-27 17:56:03.000000 cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/extension/onewire/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.955593 cbpi4-4.1.7/cbpi/extension/timer/
--rw-rw-rw-   0        0        0     3267 2023-03-08 18:19:14.000000 cbpi4-4.1.7/cbpi/extension/timer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.959591 cbpi4-4.1.7/cbpi/extension/timer/__pycache__/
--rw-rw-rw-   0        0        0     6763 2023-03-09 06:14:17.000000 cbpi4-4.1.7/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3644 2023-03-08 18:19:20.000000 cbpi4-4.1.7/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       37 2023-03-07 19:56:41.000000 cbpi4-4.1.7/cbpi/extension/timer/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.008426 cbpi4-4.1.7/cbpi/http_endpoints/
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/http_endpoints/__init__.py
--rw-rw-rw-   0        0        0     8004 2023-03-04 14:02:12.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_actor.py
--rw-rw-rw-   0        0        0     2381 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_config.py
--rw-rw-rw-   0        0        0     5283 2023-01-22 15:33:56.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_dashboard.py
--rw-rw-rw-   0        0        0    20118 2022-05-09 15:06:48.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_fermentation.py
--rw-rw-rw-   0        0        0     5003 2023-01-22 15:34:10.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_fermenterrecipe.py
--rw-rw-rw-   0        0        0     8170 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_kettle.py
--rw-rw-rw-   0        0        0     7193 2023-03-08 20:36:09.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_log.py
--rw-rw-rw-   0        0        0     1064 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_login.py
--rw-rw-rw-   0        0        0     1162 2023-01-22 15:34:36.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_notification.py
--rw-rw-rw-   0        0        0     2756 2023-01-27 10:47:00.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_plugin.py
--rw-rw-rw-   0        0        0     4699 2023-01-22 15:34:55.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_recipe.py
--rw-rw-rw-   0        0        0     6512 2023-03-08 17:52:22.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_sensor.py
--rw-rw-rw-   0        0        0     7670 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_step.py
--rw-rw-rw-   0        0        0     7938 2023-01-27 11:25:48.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_system.py
--rw-rw-rw-   0        0        0     5561 2022-03-21 11:22:35.000000 cbpi4-4.1.7/cbpi/http_endpoints/http_upload.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.020855 cbpi4-4.1.7/cbpi/job/
--rw-rw-rw-   0        0        0      851 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/job/__init__.py
--rw-rw-rw-   0        0        0     4428 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/job/_job.py
--rw-rw-rw-   0        0        0     4681 2022-11-27 09:48:32.000000 cbpi4-4.1.7/cbpi/job/_scheduler.py
--rw-rw-rw-   0        0        0     1252 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/job/aiohttp.py
--rw-rw-rw-   0        0        0     2948 2023-01-07 16:16:24.000000 cbpi4-4.1.7/cbpi/satellite.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.095938 cbpi4-4.1.7/cbpi/static/
--rw-rw-rw-   0        0        0     3329 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/beer_icon.svg
--rw-rw-rw-   0        0        0     2512 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/calculator_icon.svg
--rw-rw-rw-   0        0        0     8711 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/cbpi_icon.svg
--rw-rw-rw-   0        0        0      857 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/control_icon.svg
--rw-rw-rw-   0        0        0     2755 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/glass_icon.svg
--rw-rw-rw-   0        0        0     2931 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/grain.svg
--rw-rw-rw-   0        0        0     4158 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/hops_icon.svg
--rw-rw-rw-   0        0        0     3654 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/kettle2_icon.svg
--rw-rw-rw-   0        0        0      509 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/kettle_icon.svg
--rw-rw-rw-   0        0        0     9743 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/led.svg
--rw-rw-rw-   0        0        0     2499 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/liquid_icon.svg
--rw-rw-rw-   0        0        0     5613 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/paddle_icon.svg
--rw-rw-rw-   0        0        0     3040 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/pipe_icon.svg
--rw-rw-rw-   0        0        0     1746 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/sensor_icon.svg
--rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/splash.png
--rw-rw-rw-   0        0        0     2615 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/svg_icon.svg
--rw-rw-rw-   0        0        0      713 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/tank_icon.svg
--rw-rw-rw-   0        0        0     1834 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/target_temp.svg
--rw-rw-rw-   0        0        0      258 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/test.html
--rw-rw-rw-   0        0        0     1338 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/thermomenter.svg
--rw-rw-rw-   0        0        0     2946 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/static/yeast.svg
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.106939 cbpi4-4.1.7/cbpi/utils/
--rw-rw-rw-   0        0        0       32 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/utils/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-22 15:35:22.000000 cbpi4-4.1.7/cbpi/utils/encoder.py
--rw-rw-rw-   0        0        0      398 2021-12-30 07:59:04.000000 cbpi4-4.1.7/cbpi/utils/utils.py
--rw-rw-rw-   0        0        0     3314 2023-01-07 16:16:17.000000 cbpi4-4.1.7/cbpi/websocket.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:18.489413 cbpi4-4.1.7/cbpi4.egg-info/
--rw-rw-rw-   0        0        0     2770 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8957 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      439 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-30 05:12:18.000000 cbpi4-4.1.7/cbpi4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 05:12:19.154069 cbpi4-4.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2404 2023-03-24 17:09:07.000000 cbpi4-4.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:12:19.148061 cbpi4-4.1.7/tests/
--rw-rw-rw-   0        0        0        0 2021-11-08 11:20:02.000000 cbpi4-4.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0      900 2022-11-17 18:47:01.000000 cbpi4-4.1.7/tests/cbpi_config_fixture.py
--rw-rw-rw-   0        0        0     2713 2023-01-15 14:28:19.000000 cbpi4-4.1.7/tests/test_actor.py
--rw-rw-rw-   0        0        0      462 2022-11-17 18:47:01.000000 cbpi4-4.1.7/tests/test_cli.py
--rw-rw-rw-   0        0        0     1047 2023-01-15 14:33:37.000000 cbpi4-4.1.7/tests/test_config.py
--rw-rw-rw-   0        0        0      819 2023-01-15 14:33:47.000000 cbpi4-4.1.7/tests/test_dashboard.py
--rw-rw-rw-   0        0        0      918 2022-05-09 15:06:48.000000 cbpi4-4.1.7/tests/test_gpio.py
--rw-rw-rw-   0        0        0     1034 2023-01-15 14:34:07.000000 cbpi4-4.1.7/tests/test_index.py
--rw-rw-rw-   0        0        0     1402 2023-01-15 14:33:11.000000 cbpi4-4.1.7/tests/test_kettle.py
--rw-rw-rw-   0        0        0      980 2023-01-15 14:34:18.000000 cbpi4-4.1.7/tests/test_logger.py
--rw-rw-rw-   0        0        0      245 2023-01-15 14:34:26.000000 cbpi4-4.1.7/tests/test_notification_controller.py
--rw-rw-rw-   0        0        0     1026 2022-05-09 15:06:48.000000 cbpi4-4.1.7/tests/test_sensor.py
--rw-rw-rw-   0        0        0     1427 2022-05-09 15:06:48.000000 cbpi4-4.1.7/tests/test_step.py
--rw-rw-rw-   0        0        0      447 2022-05-09 15:06:48.000000 cbpi4-4.1.7/tests/test_system.py
--rw-rw-rw-   0        0        0     1814 2022-05-09 15:06:48.000000 cbpi4-4.1.7/tests/test_ws.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.835940 cbpi4-4.1.7rc1/
+-rw-rw-rw-   0        0        0    35823 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/LICENSE
+-rw-rw-rw-   0        0        0      100 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2773 2023-03-26 14:42:18.832947 cbpi4-4.1.7rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-03-10 14:45:36.000000 cbpi4-4.1.7rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.554484 cbpi4-4.1.7rc1/cbpi/
+-rw-rw-rw-   0        0        0       61 2023-03-26 14:41:30.000000 cbpi4-4.1.7rc1/cbpi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.705485 cbpi4-4.1.7rc1/cbpi/api/
+-rw-rw-rw-   0        0        0      841 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/__init__.py
+-rw-rw-rw-   0        0        0     2248 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/actor.py
+-rw-rw-rw-   0        0        0     2553 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/api/base.py
+-rw-rw-rw-   0        0        0      238 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/config.py
+-rw-rw-rw-   0        0        0     6694 2023-03-08 17:51:21.000000 cbpi4-4.1.7rc1/cbpi/api/dataclasses.py
+-rw-rw-rw-   0        0        0     2384 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/api/decorator.py
+-rw-rw-rw-   0        0        0      356 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/exceptions.py
+-rw-rw-rw-   0        0        0     1194 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/api/extension.py
+-rw-rw-rw-   0        0        0     1071 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/fermenter_logic.py
+-rw-rw-rw-   0        0        0     1068 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/api/kettle_logic.py
+-rw-rw-rw-   0        0        0     3821 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/property.py
+-rw-rw-rw-   0        0        0     1847 2023-03-08 17:51:54.000000 cbpi4-4.1.7rc1/cbpi/api/sensor.py
+-rw-rw-rw-   0        0        0     5926 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/step.py
+-rw-rw-rw-   0        0        0     2508 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/api/timer.py
+-rw-rw-rw-   0        0        0    12806 2023-02-07 18:06:09.000000 cbpi4-4.1.7rc1/cbpi/cli.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.844479 cbpi4-4.1.7rc1/cbpi/config/
+-rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/actor.json
+-rw-rw-rw-   0        0        0      264 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/config/chromium.desktop
+-rw-rw-rw-   0        0        0     4038 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/config.json
+-rw-rw-rw-   0        0        0      243 2022-11-17 18:42:08.000000 cbpi4-4.1.7rc1/cbpi/config/config.yaml
+-rw-rw-rw-   0        0        0      152 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/craftbeerpi.service
+-rw-rw-rw-   0        0        0     1676 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/craftbeerpiboot
+-rw-rw-rw-   0        0        0     2711 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/create_database.sql
+-rw-rw-rw-   0        0        0       35 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/config/fermenter_data.json
+-rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/kettle.json
+-rw-rw-rw-   0        0        0       73 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/plugin_list.txt
+-rw-rw-rw-   0        0        0       36 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/sensor.json
+-rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/splash.png
+-rw-rw-rw-   0        0        0       81 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/config/step_data.json
+-rw-rw-rw-   0        0        0    11053 2023-01-26 16:36:52.000000 cbpi4-4.1.7rc1/cbpi/configFolder.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.894482 cbpi4-4.1.7rc1/cbpi/controller/
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3418 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/cbpi/controller/actor_controller.py
+-rw-rw-rw-   0        0        0     6177 2023-03-08 18:12:15.000000 cbpi4-4.1.7rc1/cbpi/controller/basic_controller2.py
+-rw-rw-rw-   0        0        0     2322 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/cbpi/controller/config_controller.py
+-rw-rw-rw-   0        0        0     2797 2023-01-22 15:33:23.000000 cbpi4-4.1.7rc1/cbpi/controller/dashboard_controller.py
+-rw-rw-rw-   0        0        0    23493 2023-01-26 16:40:07.000000 cbpi4-4.1.7rc1/cbpi/controller/fermentation_controller.py
+-rw-rw-rw-   0        0        0     2807 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/controller/fermenter_recipe_controller.py
+-rw-rw-rw-   0        0        0     1662 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/controller/job_controller.py
+-rw-rw-rw-   0        0        0     1722 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/controller/kettle_controller.py
+-rw-rw-rw-   0        0        0     9533 2023-03-24 21:18:30.000000 cbpi4-4.1.7rc1/cbpi/controller/log_file_controller.py
+-rw-rw-rw-   0        0        0     3336 2023-01-22 15:30:15.000000 cbpi4-4.1.7rc1/cbpi/controller/notification_controller.py
+-rw-rw-rw-   0        0        0     9768 2023-01-27 10:53:55.000000 cbpi4-4.1.7rc1/cbpi/controller/plugin_controller.py
+-rw-rw-rw-   0        0        0     2849 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/controller/recipe_controller.py
+-rw-rw-rw-   0        0        0     8030 2023-03-26 13:21:40.000000 cbpi4-4.1.7rc1/cbpi/controller/satellite_controller.py
+-rw-rw-rw-   0        0        0     1040 2023-03-08 18:10:16.000000 cbpi4-4.1.7rc1/cbpi/controller/sensor_controller.py
+-rw-rw-rw-   0        0        0    13578 2023-01-26 16:39:43.000000 cbpi4-4.1.7rc1/cbpi/controller/step_controller.py
+-rw-rw-rw-   0        0        0    12802 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/cbpi/controller/system_controller.py
+-rw-rw-rw-   0        0        0    54504 2022-11-19 11:46:41.000000 cbpi4-4.1.7rc1/cbpi/controller/upload_controller.py
+-rw-rw-rw-   0        0        0    12388 2023-01-20 16:30:21.000000 cbpi4-4.1.7rc1/cbpi/craftbeerpi.py
+-rw-rw-rw-   0        0        0     7029 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/eventbus.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.898482 cbpi4-4.1.7rc1/cbpi/extension/
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.905493 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/
+-rw-rw-rw-   0        0        0    20211 2023-03-24 06:10:43.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.944484 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/
+-rw-rw-rw-   0        0        0     8582 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    22659 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7583 2022-02-16 16:13:43.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     9326 2023-03-24 17:11:00.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       47 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.950484 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/
+-rw-rw-rw-   0        0        0    20143 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.997578 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/
+-rw-rw-rw-   0        0        0    14091 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    34360 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11626 2022-02-25 13:23:11.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    14328 2022-05-09 15:22:15.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       48 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.006569 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/
+-rw-rw-rw-   0        0        0    12519 2023-01-27 16:09:06.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.060568 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/
+-rw-rw-rw-   0        0        0     7807 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17903 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4843 2022-01-03 11:51:56.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     8266 2023-01-27 16:59:06.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       51 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/config.yaml
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.122572 cbpi4-4.1.7rc1/cbpi/extension/__pycache__/
+-rw-rw-rw-   0        0        0      130 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      155 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      159 2022-02-26 13:38:02.000000 cbpi4-4.1.7rc1/cbpi/extension/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.136576 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/
+-rw-rw-rw-   0        0        0     1281 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.188570 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/
+-rw-rw-rw-   0        0        0     2167 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3282 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2181 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2202 2022-02-26 13:38:02.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       42 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/dummyactor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.194568 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/
+-rw-rw-rw-   0        0        0     2728 2023-03-07 19:37:46.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.245568 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/
+-rw-rw-rw-   0        0        0     2871 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5500 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1359 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2971 2023-03-07 19:55:17.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/dummysensor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.256576 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/
+-rw-rw-rw-   0        0        0     6111 2023-03-10 17:08:18.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.312566 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/
+-rw-rw-rw-   0        0        0     5776 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11052 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5823 2022-02-16 16:13:43.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5737 2023-03-10 17:08:23.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       41 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/gpioactor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.321580 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/
+-rw-rw-rw-   0        0        0     7547 2023-03-25 13:55:01.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.381084 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/
+-rw-rw-rw-   0        0        0     3249 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7516 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3212 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6114 2023-03-25 16:24:03.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/httpsensor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.389080 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/
+-rw-rw-rw-   0        0        0     2210 2023-03-02 05:51:03.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.441077 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/
+-rw-rw-rw-   0        0        0     1905 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4025 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1798 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2012 2023-03-04 10:48:54.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       48 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/hysteresis/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.446075 cbpi4-4.1.7rc1/cbpi/extension/mashstep/
+-rw-rw-rw-   0        0        0    26901 2023-02-11 14:27:45.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.507507 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/
+-rw-rw-rw-   0        0        0    19082 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    46297 2023-03-09 06:14:16.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    20852 2022-01-04 06:30:42.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    21087 2023-02-11 14:27:52.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       40 2022-01-04 06:30:19.000000 cbpi4-4.1.7rc1/cbpi/extension/mashstep/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.526507 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/
+-rw-rw-rw-   0        0        0      650 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.824856 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/
+-rw-rw-rw-   0        0        0      804 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1278 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      819 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      837 2022-03-21 11:27:58.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2164 2023-01-07 21:29:06.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3552 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2148 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2173 2022-11-27 13:47:03.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2396 2023-01-07 21:29:05.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4334 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2338 2022-01-25 10:19:18.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2397 2022-11-27 13:47:03.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0      869 2023-01-07 21:29:06.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1267 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0      874 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0      902 2022-03-21 11:27:58.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/config.yaml
+-rw-rw-rw-   0        0        0     1702 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/generic_mqtt_actor.py
+-rw-rw-rw-   0        0        0     1922 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/mqtt_actor.py
+-rw-rw-rw-   0        0        0      442 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/tasmota_mqtt_actor.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.831878 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/
+-rw-rw-rw-   0        0        0     7065 2023-03-25 18:14:44.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.924248 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/
+-rw-rw-rw-   0        0        0     2481 2023-01-07 21:29:06.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7045 2023-03-09 06:14:17.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2438 2021-12-30 07:59:45.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5630 2023-03-26 07:26:10.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:17.930238 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/
+-rw-rw-rw-   0        0        0     2618 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.028130 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/
+-rw-rw-rw-   0        0        0     2130 2023-01-07 21:29:06.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4059 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2117 2022-02-16 16:13:43.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2143 2022-03-21 11:27:58.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       42 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.040132 cbpi4-4.1.7rc1/cbpi/extension/onewire/
+-rw-rw-rw-   0        0        0     7011 2023-03-25 13:23:10.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.125132 cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/
+-rw-rw-rw-   0        0        0     3813 2023-01-07 21:29:06.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7131 2023-01-15 12:43:43.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3737 2022-01-25 10:19:18.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6042 2023-03-25 16:24:03.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/extension/onewire/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.133138 cbpi4-4.1.7rc1/cbpi/extension/timer/
+-rw-rw-rw-   0        0        0     3267 2023-03-08 18:19:14.000000 cbpi4-4.1.7rc1/cbpi/extension/timer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.159950 cbpi4-4.1.7rc1/cbpi/extension/timer/__pycache__/
+-rw-rw-rw-   0        0        0     6763 2023-03-09 06:14:17.000000 cbpi4-4.1.7rc1/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3644 2023-03-08 18:19:20.000000 cbpi4-4.1.7rc1/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       37 2023-03-07 19:56:41.000000 cbpi4-4.1.7rc1/cbpi/extension/timer/config.yaml
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.228951 cbpi4-4.1.7rc1/cbpi/http_endpoints/
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/__init__.py
+-rw-rw-rw-   0        0        0     8004 2023-03-04 14:02:12.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_actor.py
+-rw-rw-rw-   0        0        0     2381 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_config.py
+-rw-rw-rw-   0        0        0     5283 2023-01-22 15:33:56.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_dashboard.py
+-rw-rw-rw-   0        0        0    20118 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_fermentation.py
+-rw-rw-rw-   0        0        0     5003 2023-01-22 15:34:10.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_fermenterrecipe.py
+-rw-rw-rw-   0        0        0     8170 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_kettle.py
+-rw-rw-rw-   0        0        0     7193 2023-03-08 20:36:09.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_log.py
+-rw-rw-rw-   0        0        0     1064 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_login.py
+-rw-rw-rw-   0        0        0     1162 2023-01-22 15:34:36.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_notification.py
+-rw-rw-rw-   0        0        0     2756 2023-01-27 10:47:00.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_plugin.py
+-rw-rw-rw-   0        0        0     4699 2023-01-22 15:34:55.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_recipe.py
+-rw-rw-rw-   0        0        0     6512 2023-03-08 17:52:22.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_sensor.py
+-rw-rw-rw-   0        0        0     7670 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_step.py
+-rw-rw-rw-   0        0        0     7938 2023-01-27 11:25:48.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_system.py
+-rw-rw-rw-   0        0        0     5561 2022-03-21 11:22:35.000000 cbpi4-4.1.7rc1/cbpi/http_endpoints/http_upload.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.277952 cbpi4-4.1.7rc1/cbpi/job/
+-rw-rw-rw-   0        0        0      851 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/job/__init__.py
+-rw-rw-rw-   0        0        0     4428 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/job/_job.py
+-rw-rw-rw-   0        0        0     4681 2022-11-27 09:48:32.000000 cbpi4-4.1.7rc1/cbpi/job/_scheduler.py
+-rw-rw-rw-   0        0        0     1252 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/job/aiohttp.py
+-rw-rw-rw-   0        0        0     2948 2023-01-07 16:16:24.000000 cbpi4-4.1.7rc1/cbpi/satellite.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.694936 cbpi4-4.1.7rc1/cbpi/static/
+-rw-rw-rw-   0        0        0     3329 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/beer_icon.svg
+-rw-rw-rw-   0        0        0     2512 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/calculator_icon.svg
+-rw-rw-rw-   0        0        0     8711 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/cbpi_icon.svg
+-rw-rw-rw-   0        0        0      857 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/control_icon.svg
+-rw-rw-rw-   0        0        0     2755 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/glass_icon.svg
+-rw-rw-rw-   0        0        0     2931 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/grain.svg
+-rw-rw-rw-   0        0        0     4158 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/hops_icon.svg
+-rw-rw-rw-   0        0        0     3654 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/kettle2_icon.svg
+-rw-rw-rw-   0        0        0      509 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/kettle_icon.svg
+-rw-rw-rw-   0        0        0     9743 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/led.svg
+-rw-rw-rw-   0        0        0     2499 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/liquid_icon.svg
+-rw-rw-rw-   0        0        0     5613 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/paddle_icon.svg
+-rw-rw-rw-   0        0        0     3040 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/pipe_icon.svg
+-rw-rw-rw-   0        0        0     1746 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/sensor_icon.svg
+-rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/splash.png
+-rw-rw-rw-   0        0        0     2615 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/svg_icon.svg
+-rw-rw-rw-   0        0        0      713 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/tank_icon.svg
+-rw-rw-rw-   0        0        0     1834 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/target_temp.svg
+-rw-rw-rw-   0        0        0      258 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/test.html
+-rw-rw-rw-   0        0        0     1338 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/thermomenter.svg
+-rw-rw-rw-   0        0        0     2946 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/static/yeast.svg
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.706937 cbpi4-4.1.7rc1/cbpi/utils/
+-rw-rw-rw-   0        0        0       32 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/utils/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-22 15:35:22.000000 cbpi4-4.1.7rc1/cbpi/utils/encoder.py
+-rw-rw-rw-   0        0        0      398 2021-12-30 07:59:04.000000 cbpi4-4.1.7rc1/cbpi/utils/utils.py
+-rw-rw-rw-   0        0        0     3314 2023-01-07 16:16:17.000000 cbpi4-4.1.7rc1/cbpi/websocket.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:16.664484 cbpi4-4.1.7rc1/cbpi4.egg-info/
+-rw-rw-rw-   0        0        0     2773 2023-03-26 14:42:15.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8957 2023-03-26 14:42:16.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       33 2023-03-26 14:42:15.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-03-26 14:42:15.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      439 2023-03-26 14:42:15.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-03-26 14:42:15.000000 cbpi4-4.1.7rc1/cbpi4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-26 14:42:18.835940 cbpi4-4.1.7rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2404 2023-03-24 17:09:07.000000 cbpi4-4.1.7rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-26 14:42:18.829937 cbpi4-4.1.7rc1/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-08 11:20:02.000000 cbpi4-4.1.7rc1/tests/__init__.py
+-rw-rw-rw-   0        0        0      900 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/tests/cbpi_config_fixture.py
+-rw-rw-rw-   0        0        0     2713 2023-01-15 14:28:19.000000 cbpi4-4.1.7rc1/tests/test_actor.py
+-rw-rw-rw-   0        0        0      462 2022-11-17 18:47:01.000000 cbpi4-4.1.7rc1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     1047 2023-01-15 14:33:37.000000 cbpi4-4.1.7rc1/tests/test_config.py
+-rw-rw-rw-   0        0        0      819 2023-01-15 14:33:47.000000 cbpi4-4.1.7rc1/tests/test_dashboard.py
+-rw-rw-rw-   0        0        0      918 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/tests/test_gpio.py
+-rw-rw-rw-   0        0        0     1034 2023-01-15 14:34:07.000000 cbpi4-4.1.7rc1/tests/test_index.py
+-rw-rw-rw-   0        0        0     1402 2023-01-15 14:33:11.000000 cbpi4-4.1.7rc1/tests/test_kettle.py
+-rw-rw-rw-   0        0        0      980 2023-01-15 14:34:18.000000 cbpi4-4.1.7rc1/tests/test_logger.py
+-rw-rw-rw-   0        0        0      245 2023-01-15 14:34:26.000000 cbpi4-4.1.7rc1/tests/test_notification_controller.py
+-rw-rw-rw-   0        0        0     1026 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/tests/test_sensor.py
+-rw-rw-rw-   0        0        0     1427 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/tests/test_step.py
+-rw-rw-rw-   0        0        0      447 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/tests/test_system.py
+-rw-rw-rw-   0        0        0     1814 2022-05-09 15:06:48.000000 cbpi4-4.1.7rc1/tests/test_ws.py
```

### Comparing `cbpi4-4.1.7/LICENSE` & `cbpi4-4.1.7rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/PKG-INFO` & `cbpi4-4.1.7rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4
-Version: 4.1.7
+Version: 4.1.7rc1
 Summary: CraftBeerPi4 Brewing Software
 Home-page: http://web.craftbeerpi.com
 Author: Manuel Fritsch / Alexander Vollkopf
 Author-email: manuel@craftbeerpi.com
 License: GPLv3
 Project-URL: Documentation, https://openbrewing.gitbook.io/craftbeerpi4_support/
 Platform: UNKNOWN
```

### Comparing `cbpi4-4.1.7/README.md` & `cbpi4-4.1.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/__init__.py` & `cbpi4-4.1.7rc1/cbpi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/actor.py` & `cbpi4-4.1.7rc1/cbpi/api/actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/base.py` & `cbpi4-4.1.7rc1/cbpi/api/base.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/dataclasses.py` & `cbpi4-4.1.7rc1/cbpi/api/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/decorator.py` & `cbpi4-4.1.7rc1/cbpi/api/decorator.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/extension.py` & `cbpi4-4.1.7rc1/cbpi/api/extension.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/fermenter_logic.py` & `cbpi4-4.1.7rc1/cbpi/api/fermenter_logic.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/kettle_logic.py` & `cbpi4-4.1.7rc1/cbpi/api/kettle_logic.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/property.py` & `cbpi4-4.1.7rc1/cbpi/api/property.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/sensor.py` & `cbpi4-4.1.7rc1/cbpi/api/sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/step.py` & `cbpi4-4.1.7rc1/cbpi/api/step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/api/timer.py` & `cbpi4-4.1.7rc1/cbpi/api/timer.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/cli.py` & `cbpi4-4.1.7rc1/cbpi/cli.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/config/config.json` & `cbpi4-4.1.7rc1/cbpi/config/config.json`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/config/craftbeerpiboot` & `cbpi4-4.1.7rc1/cbpi/config/craftbeerpiboot`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/config/create_database.sql` & `cbpi4-4.1.7rc1/cbpi/config/create_database.sql`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/config/splash.png` & `cbpi4-4.1.7rc1/cbpi/config/splash.png`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/configFolder.py` & `cbpi4-4.1.7rc1/cbpi/configFolder.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/actor_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/actor_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/basic_controller2.py` & `cbpi4-4.1.7rc1/cbpi/controller/basic_controller2.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/config_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/config_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/dashboard_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/dashboard_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/fermentation_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/fermentation_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/fermenter_recipe_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/fermenter_recipe_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/job_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/job_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/kettle_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/kettle_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/log_file_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/log_file_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/notification_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/notification_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/plugin_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/recipe_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/recipe_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/satellite_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/satellite_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/sensor_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/sensor_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/step_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/step_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/system_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/system_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/controller/upload_controller.py` & `cbpi4-4.1.7rc1/cbpi/controller/upload_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/craftbeerpi.py` & `cbpi4-4.1.7rc1/cbpi/craftbeerpi.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/eventbus.py` & `cbpi4-4.1.7rc1/cbpi/eventbus.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermentationStep/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummyactor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummysensor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/gpioactor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/httpsensor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 cache = {}
 
 @parameters([Property.Text(label="Key", configurable=True, description="Http Key"),
              Property.Number(label="Timeout", configurable="True",unit="sec",description="Timeout in seconds to send notification (default:60 | deactivated: 0)"),
              Property.Kettle(label="Kettle", description="Reduced logging if Kettle is inactive (only Kettle or Fermenter to be selected)"),
              Property.Fermenter(label="Fermenter", description="Reduced logging in seconds if Fermenter is inactive (only Kettle or Fermenter to be selected)"),
-             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default: 60 sec | disabled: 0)")])
+             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default is 60 sec)")])
 
 class HTTPSensor(CBPiSensor):
     def __init__(self, cbpi, id, props):
         super(HTTPSensor, self).__init__(cbpi, id, props)
         self.running = True
         self.value = 0
         self.timeout=int(self.props.get("Timeout", 60))
@@ -26,16 +26,14 @@
         self.notificationsend = False
         self.nextchecktime=self.starttime+self.timeout
         self.sensor=self.get_sensor(self.id)
         self.lastdata=time.time()
 
         self.lastlog=0
         self.reducedfrequency=int(self.props.get("ReducedLogging", 60))
-        if self.reducedfrequency < 0:
-            self.reducedfrequency = 0
         
         self.kettleid=self.props.get("Kettle", None)
         self.fermenterid=self.props.get("Fermenter", None)
         self.reducedlogging = True if self.kettleid or self.fermenterid else False
 
         if self.kettleid is not None and self.fermenterid is not None:
             self.reducedlogging=False
@@ -94,38 +92,36 @@
                 kettlestatus=False
             if kettlestatus:
                 self.log_data(self.value)
                 logging.info("Kettle Active")
                 self.lastlog = time.time()
             else:
                 logging.info("Kettle Inactive")
-                if self.reducedfrequency != 0:
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass   
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass   
 
         if self.fermenter is not None:
             try:
                 fermenterstatus=self.fermenter.instance.state
             except:
                 fermenterstatus=False
             if fermenterstatus:
                 self.log_data(self.value)
                 logging.info("Fermenter Active")
                 self.lastlog = time.time()
             else:
                 logging.info("Fermenter Inactive")
-                if self.reducedfrequency != 0:                    
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass            
 
     def get_state(self):
         # return the current state of the sensor
         return dict(value=self.value)
 
 class HTTPSensorEndpoint(CBPiExtension):
```

### Comparing `cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 27 18:06:03 2023 UTC, .py size: 7783 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0bdb 2164 671e 0000  a.........!dg...
+00000000: 610d 0d0a 0000 0000 35fd 1e64 7b1d 0000  a.......5..d{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 5400 6400 6401 6c04  ..d.d.l.T.d.d.l.
 00000050: 5a04 6400 6404 6c05 6d05 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 6900  d.l.m.Z.m.Z...i.
@@ -194,193 +194,190 @@
 00000c10: 3600 0000 7236 0000 0072 3700 0000 da03  6...r6...r7.....
 00000c20: 7275 6e34 0000 0073 3200 0000 0005 0c01  run4...s2.......
 00000c30: 1c01 1c01 0a01 0801 1401 0e01 0601 0201  ................
 00000c40: 1401 0a01 0a01 0c02 0601 1002 0c01 0a02  ................
 00000c50: 0c01 0c01 0601 0e01 1001 0a01 1601 7a0e  ..............z.
 00000c60: 4854 5450 5365 6e73 6f72 2e72 756e 6301  HTTPSensor.runc.
 00000c70: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00000c80: 0000 00c3 0000 0073 3c01 0000 7c00 6a00  .......s<...|.j.
-00000c90: 6401 6b03 9001 722e 7401 a001 a100 7d01  d.k...r.t.....}.
-00000ca0: 7c00 6a02 6400 7501 729e 7a0e 7c00 6a02  |.j.d.u.r.z.|.j.
-00000cb0: 6a03 6a04 7d02 5700 6e10 0100 0100 0100  j.j.}.W.n.......
-00000cc0: 6402 7d02 5900 6e02 3000 7c02 7264 7c00  d.}.Y.n.0.|.rd|.
-00000cd0: a005 7c00 6a06 a101 0100 7407 a008 6403  ..|.j.....t...d.
-00000ce0: a101 0100 7401 a001 a100 7c00 5f09 6e3a  ....t.....|._.n:
-00000cf0: 7407 a008 6404 a101 0100 7c01 7c00 6a09  t...d.....|.|.j.
-00000d00: 7c00 6a00 1700 6b05 729e 7c00 a005 7c00  |.j...k.r.|...|.
-00000d10: 6a06 a101 0100 7401 a001 a100 7c00 5f09  j.....t.....|._.
-00000d20: 7407 a008 6405 a101 0100 7c00 6a0a 6400  t...d.....|.j.d.
-00000d30: 7501 9001 7238 7a0e 7c00 6a0a 6a03 6a04  u...r8z.|.j.j.j.
-00000d40: 7d03 5700 6e10 0100 0100 0100 6402 7d03  }.W.n.......d.}.
-00000d50: 5900 6e02 3000 7c03 72f0 7c00 a005 7c00  Y.n.0.|.r.|...|.
-00000d60: 6a06 a101 0100 7407 a008 6406 a101 0100  j.....t...d.....
-00000d70: 7401 a001 a100 7c00 5f09 6e3c 7407 a008  t.....|._.n<t...
-00000d80: 6407 a101 0100 7c01 7c00 6a09 7c00 6a00  d.....|.|.j.|.j.
-00000d90: 1700 6b05 9001 7238 7c00 a005 7c00 6a06  ..k...r8|...|.j.
-00000da0: a101 0100 7401 a001 a100 7c00 5f09 7407  ....t.....|._.t.
-00000db0: a008 6405 a101 0100 6e0a 7407 a00b 6408  ..d.....n.t...d.
-00000dc0: a101 0100 6400 5300 2909 4e72 0100 0000  ....d.S.).Nr....
-00000dd0: 467a 0d4b 6574 746c 6520 4163 7469 7665  Fz.Kettle Active
-00000de0: 7a0f 4b65 7474 6c65 2049 6e61 6374 6976  z.Kettle Inactiv
-00000df0: 657a 1c4c 6f67 6765 6420 7769 7468 2072  ez.Logged with r
-00000e00: 6564 7563 6564 2066 7265 7165 6e63 797a  educed freqencyz
-00000e10: 1046 6572 6d65 6e74 6572 2041 6374 6976  .Fermenter Activ
-00000e20: 657a 1246 6572 6d65 6e74 6572 2049 6e61  ez.Fermenter Ina
-00000e30: 6374 6976 657a 0a4e 6f20 6c6f 6767 696e  ctivez.No loggin
-00000e40: 6729 0c72 2900 0000 7220 0000 0072 3e00  g).r)...r ...r>.
-00000e50: 0000 da08 696e 7374 616e 6365 da05 7374  ....instance..st
-00000e60: 6174 6572 4600 0000 721b 0000 0072 4800  aterF...r....rH.
-00000e70: 0000 da04 696e 666f 7228 0000 0072 4000  ....infor(...r@.
-00000e80: 0000 da07 7761 726e 696e 6729 0472 3300  ....warning).r3.
-00000e90: 0000 da03 6e6f 775a 0c6b 6574 746c 6573  ....nowZ.kettles
-00000ea0: 7461 7475 735a 0f66 6572 6d65 6e74 6572  tatusZ.fermenter
-00000eb0: 7374 6174 7573 7236 0000 0072 3600 0000  statusr6...r6...
-00000ec0: 7237 0000 0072 4500 0000 5600 0000 7342  r7...rE...V...sB
-00000ed0: 0000 0000 010c 0108 010a 0102 010e 0106  ................
-00000ee0: 010a 0104 010c 010a 010c 020a 0110 010c  ................
-00000ef0: 010a 010a 030c 0102 010e 0106 010a 0104  ................
-00000f00: 010c 010a 010c 020a 0112 010c 010a 010a  ................
-00000f10: 0102 020a 017a 1348 5454 5053 656e 736f  .....z.HTTPSenso
-00000f20: 722e 6c6f 6776 616c 7565 6301 0000 0000  r.logvaluec.....
-00000f30: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000f40: 0000 0073 0c00 0000 7400 7c00 6a01 6401  ...s....t.|.j.d.
-00000f50: 8d01 5300 2902 4e29 0172 1b00 0000 2902  ..S.).N).r....).
-00000f60: da04 6469 6374 721b 0000 0029 0172 3300  ..dictr....).r3.
-00000f70: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00000f80: 00da 0967 6574 5f73 7461 7465 7e00 0000  ...get_state~...
-00000f90: 7302 0000 0000 027a 1448 5454 5053 656e  s......z.HTTPSen
-00000fa0: 736f 722e 6765 745f 7374 6174 6529 0ada  sor.get_state)..
-00000fb0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000fc0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000fd0: 655f 5f72 1900 0000 7232 0000 0072 3b00  e__r....r2...r;.
-00000fe0: 0000 724d 0000 0072 4500 0000 7254 0000  ..rM...rE...rT..
-00000ff0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00001000: 7236 0000 0072 3600 0000 7234 0000 0072  r6...r6...r4...r
-00001010: 3700 0000 7212 0000 000d 0000 0073 0c00  7...r........s..
-00001020: 0000 0807 0c16 0805 0805 0822 0828 7212  ...........".(r.
-00001030: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001040: 0000 0000 0400 0000 4000 0000 7328 0000  ........@...s(..
-00001050: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-00001060: 0365 0464 0364 0464 058d 0264 0664 0784  .e.d.d.d...d.d..
-00001070: 0083 015a 0564 0853 0029 09da 1248 5454  ...Z.d.S.)...HTT
-00001080: 5053 656e 736f 7245 6e64 706f 696e 7463  PSensorEndpointc
-00001090: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000010a0: 0400 0000 4300 0000 7324 0000 0074 00a0  ....C...s$...t..
-000010b0: 0164 01a1 017c 005f 027c 017c 005f 037c  .d...|._.|.|._.|
-000010c0: 006a 03a0 047c 0064 02a1 0201 0064 0353  .j...|.d.....d.S
-000010d0: 0029 047a 330a 2020 2020 2020 2020 496e  .).z3.        In
-000010e0: 6974 6961 6c69 7a65 720a 0a20 2020 2020  itializer..     
-000010f0: 2020 203a 7061 7261 6d20 6362 7069 3a0a     :param cbpi:.
-00001100: 2020 2020 2020 2020 7a15 5e5b 612d 7a41          z.^[a-zA
-00001110: 2d5a 302d 392c 2e5d 7b30 2c31 307d 247a  -Z0-9,.]{0,10}$z
-00001120: 0b2f 6874 7470 7365 6e73 6f72 4e29 05da  ./httpsensorN)..
-00001130: 0272 65da 0763 6f6d 7069 6c65 da0d 7061  .re..compile..pa
-00001140: 7474 6572 6e5f 6368 6563 6b72 2d00 0000  ttern_checkr-...
-00001150: da08 7265 6769 7374 6572 2902 7233 0000  ..register).r3..
-00001160: 0072 2d00 0000 7236 0000 0072 3600 0000  .r-...r6...r6...
-00001170: 7237 0000 0072 1900 0000 8400 0000 7306  r7...r........s.
-00001180: 0000 0000 060c 0206 037a 1b48 5454 5053  .........z.HTTPS
-00001190: 656e 736f 7245 6e64 706f 696e 742e 5f5f  ensorEndpoint.__
-000011a0: 696e 6974 5f5f 7a0e 2f7b 6b65 797d 2f7b  init__z./{key}/{
-000011b0: 7661 6c75 657d 4629 02da 0470 6174 68da  value}F)...path.
-000011c0: 0d61 7574 685f 7265 7175 6972 6564 6302  .auth_requiredc.
-000011d0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000011e0: 0000 00c3 0000 0073 6c00 0000 7c01 6a00  .......sl...|.j.
-000011f0: 6401 1900 7d02 7c01 6a00 6402 1900 7d03  d...}.|.j.d...}.
-00001200: 7c00 6a01 a002 7c02 a101 6403 7500 7236  |.j...|...d.u.r6
-00001210: 7403 6a04 6404 6405 6406 6901 6407 8d02  t.j.d.d.d.i.d...
-00001220: 5300 7c00 6a01 a002 7c03 a101 6403 7500  S.|.j...|...d.u.
-00001230: 7258 7403 6a04 6404 6405 6408 6901 6407  rXt.j.d.d.d.i.d.
-00001240: 8d02 5300 7c03 7405 7c02 3c00 7403 6a06  ..S.|.t.|.<.t.j.
-00001250: 6409 640a 8d01 5300 290b 61e4 0100 000a  d.d...S.).a.....
-00001260: 2020 2020 2020 2020 2d2d 2d0a 2020 2020          ---.    
-00001270: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00001280: 204b 6574 746c 6520 4865 6174 6572 206f   Kettle Heater o
-00001290: 6e0a 2020 2020 2020 2020 7461 6773 3a0a  n.        tags:.
-000012a0: 2020 2020 2020 2020 2d20 4874 7470 5365          - HttpSe
-000012b0: 6e73 6f72 0a20 2020 2020 2020 2070 6172  nsor.        par
-000012c0: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-000012d0: 202d 206e 616d 653a 2022 6b65 7922 0a20   - name: "key". 
-000012e0: 2020 2020 2020 2020 2069 6e3a 2022 7061           in: "pa
-000012f0: 7468 220a 2020 2020 2020 2020 2020 6465  th".          de
-00001300: 7363 7269 7074 696f 6e3a 2022 5365 6e73  scription: "Sens
-00001310: 6f72 204b 6579 220a 2020 2020 2020 2020  or Key".        
-00001320: 2020 7265 7175 6972 6564 3a20 7472 7565    required: true
-00001330: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-00001340: 2022 7374 7269 6e67 220a 2020 2020 2020   "string".      
-00001350: 2020 2d20 6e61 6d65 3a20 2276 616c 7565    - name: "value
-00001360: 220a 2020 2020 2020 2020 2020 696e 3a20  ".          in: 
-00001370: 2270 6174 6822 0a20 2020 2020 2020 2020  "path".         
-00001380: 2064 6573 6372 6970 7469 6f6e 3a20 2256   description: "V
-00001390: 616c 7565 220a 2020 2020 2020 2020 2020  alue".          
-000013a0: 7265 7175 6972 6564 3a20 7472 7565 0a20  required: true. 
-000013b0: 2020 2020 2020 2020 2074 7970 653a 2022           type: "
-000013c0: 696e 7465 6765 7222 0a20 2020 2020 2020  integer".       
-000013d0: 2020 2066 6f72 6d61 743a 2022 696e 7436     format: "int6
-000013e0: 3422 0a20 2020 2020 2020 2072 6573 706f  4".        respo
-000013f0: 6e73 6573 3a0a 2020 2020 2020 2020 2020  nses:.          
-00001400: 2020 2232 3034 223a 0a20 2020 2020 2020    "204":.       
-00001410: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00001420: 7469 6f6e 3a20 7375 6363 6573 7366 756c  tion: successful
-00001430: 206f 7065 7261 7469 6f6e 0a20 2020 2020   operation.     
-00001440: 2020 20da 036b 6579 721b 0000 004e 69a6     ..keyr....Ni.
-00001450: 0100 0072 4900 0000 7a2e 4b65 7920 6e6f  ...rI...z.Key no
-00001460: 7420 6d61 7463 6869 6e67 2070 6174 7465  t matching patte
-00001470: 726e 205e 5b61 2d7a 412d 5a30 2d39 2c2e  rn ^[a-zA-Z0-9,.
-00001480: 5d7b 302c 3130 7d24 2902 da06 7374 6174  ]{0,10}$)...stat
-00001490: 7573 da04 6461 7461 7a2f 4461 7461 206e  us..dataz/Data n
-000014a0: 6f74 206d 6174 6368 696e 6720 7061 7474  ot matching patt
-000014b0: 6572 6e20 5e5b 612d 7a41 2d5a 302d 392c  ern ^[a-zA-Z0-9,
-000014c0: 2e5d 7b30 2c31 307d 24e9 cc00 0000 2901  .]{0,10}$.....).
-000014d0: 7261 0000 0029 07da 0a6d 6174 6368 5f69  ra...)...match_i
-000014e0: 6e66 6f72 5c00 0000 da05 6d61 7463 6872  nfor\.....matchr
-000014f0: 0200 0000 da0d 6a73 6f6e 5f72 6573 706f  ......json_respo
-00001500: 6e73 6572 4100 0000 da08 5265 7370 6f6e  nserA.....Respon
-00001510: 7365 2904 7233 0000 00da 0772 6571 7565  se).r3.....reque
-00001520: 7374 7260 0000 0072 1b00 0000 7236 0000  str`...r....r6..
-00001530: 0072 3600 0000 7237 0000 00da 0f68 7474  .r6...r7.....htt
-00001540: 705f 6e65 775f 7661 6c75 6532 9200 0000  p_new_value2....
-00001550: 7310 0000 0000 190a 010a 0110 0112 0210  s...............
-00001560: 0112 0308 027a 2248 5454 5053 656e 736f  .....z"HTTPSenso
-00001570: 7245 6e64 706f 696e 742e 6874 7470 5f6e  rEndpoint.http_n
-00001580: 6577 5f76 616c 7565 324e 2906 7255 0000  ew_value2N).rU..
-00001590: 0072 5600 0000 7257 0000 0072 1900 0000  .rV...rW...r....
-000015a0: da0f 7265 7175 6573 745f 6d61 7070 696e  ..request_mappin
-000015b0: 6772 6900 0000 7236 0000 0072 3600 0000  gri...r6...r6...
-000015c0: 7236 0000 0072 3700 0000 7259 0000 0082  r6...r7...rY....
-000015d0: 0000 0073 0600 0000 0802 080e 0a01 7259  ...s..........rY
-000015e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000015f0: 0100 0000 0400 0000 4300 0000 7320 0000  ........C...s ..
-00001600: 007c 006a 00a0 0164 0174 02a1 0201 007c  .|.j...d.t.....|
-00001610: 006a 00a0 0164 0274 03a1 0201 0064 0353  .j...d.t.....d.S
-00001620: 0029 047a a90a 2020 2020 5468 6973 206d  .).z..    This m
-00001630: 6574 686f 6420 6973 2063 616c 6c65 6420  ethod is called 
-00001640: 6279 2074 6865 2073 6572 7665 7220 6475  by the server du
-00001650: 7269 6e67 2073 7461 7274 7570 200a 2020  ring startup .  
-00001660: 2020 4865 7265 2079 6f75 206e 6565 6420    Here you need 
-00001670: 746f 2072 6567 6973 7465 7220 796f 7572  to register your
-00001680: 2070 6c75 6769 6e73 2061 7420 7468 6520   plugins at the 
-00001690: 7365 7276 6572 0a20 2020 200a 2020 2020  server.    .    
-000016a0: 3a70 6172 616d 2063 6270 693a 2074 6865  :param cbpi: the
-000016b0: 2063 6270 6920 636f 7265 200a 2020 2020   cbpi core .    
-000016c0: 3a72 6574 7572 6e3a 200a 2020 2020 7212  :return: .    r.
-000016d0: 0000 0072 5900 0000 4e29 04da 0670 6c75  ...rY...N)...plu
-000016e0: 6769 6e72 5d00 0000 7212 0000 0072 5900  ginr]...r....rY.
-000016f0: 0000 2901 722d 0000 0072 3600 0000 7236  ..).r-...r6...r6
-00001700: 0000 0072 3700 0000 da05 7365 7475 70b9  ...r7.....setup.
-00001710: 0000 0073 0400 0000 0009 0e01 726c 0000  ...s........rl..
-00001720: 0029 1772 4a00 0000 da07 6169 6f68 7474  .).rJ.....aiohtt
-00001730: 7072 0200 0000 5a08 6362 7069 2e61 7069  pr....Z.cbpi.api
-00001740: 7220 0000 0072 0400 0000 725a 0000 0072  r ...r....rZ...r
-00001750: 4800 0000 da14 6362 7069 2e61 7069 2e64  H.....cbpi.api.d
-00001760: 6174 6163 6c61 7373 6573 7205 0000 0072  ataclassesr....r
-00001770: 0600 0000 7241 0000 00da 0a70 6172 616d  ....rA.....param
-00001780: 6574 6572 73da 0850 726f 7065 7274 79da  eters..Property.
-00001790: 0454 6578 74da 064e 756d 6265 7272 0f00  .Text..Numberr..
-000017a0: 0000 7210 0000 00da 0a43 4250 6953 656e  ..r......CBPiSen
-000017b0: 736f 7272 1200 0000 da0d 4342 5069 4578  sorr......CBPiEx
-000017c0: 7465 6e73 696f 6e72 5900 0000 726c 0000  tensionrY...rl..
-000017d0: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-000017e0: 7237 0000 00da 083c 6d6f 6475 6c65 3e02  r7.....<module>.
-000017f0: 0000 0073 2200 0000 0801 0c01 0801 0801  ...s"...........
-00001800: 0c01 0801 0801 1002 0402 1001 1001 0c01  ................
-00001810: 0c01 0efc 0406 126f 1037                 .......o.7
+00000c80: 0000 00c3 0000 0073 2401 0000 7400 a000  .......s$...t...
+00000c90: a100 7d01 7c00 6a01 6400 7501 7292 7a0e  ..}.|.j.d.u.r.z.
+00000ca0: 7c00 6a01 6a02 6a03 7d02 5700 6e10 0100  |.j.j.j.}.W.n...
+00000cb0: 0100 0100 6401 7d02 5900 6e02 3000 7c02  ....d.}.Y.n.0.|.
+00000cc0: 7258 7c00 a004 7c00 6a05 a101 0100 7406  rX|...|.j.....t.
+00000cd0: a007 6402 a101 0100 7400 a000 a100 7c00  ..d.....t.....|.
+00000ce0: 5f08 6e3a 7406 a007 6403 a101 0100 7c01  _.n:t...d.....|.
+00000cf0: 7c00 6a08 7c00 6a09 1700 6b05 7292 7c00  |.j.|.j...k.r.|.
+00000d00: a004 7c00 6a05 a101 0100 7400 a000 a100  ..|.j.....t.....
+00000d10: 7c00 5f08 7406 a007 6404 a101 0100 7c00  |._.t...d.....|.
+00000d20: 6a0a 6400 7501 9001 7220 7a0e 7c00 6a0a  j.d.u...r z.|.j.
+00000d30: 6a02 6a03 7d03 5700 6e10 0100 0100 0100  j.j.}.W.n.......
+00000d40: 6401 7d03 5900 6e02 3000 7c03 72e4 7c00  d.}.Y.n.0.|.r.|.
+00000d50: a004 7c00 6a05 a101 0100 7406 a007 6405  ..|.j.....t...d.
+00000d60: a101 0100 7400 a000 a100 7c00 5f08 6e3c  ....t.....|._.n<
+00000d70: 7406 a007 6406 a101 0100 7c01 7c00 6a08  t...d.....|.|.j.
+00000d80: 7c00 6a09 1700 6b05 9001 7220 7c00 a004  |.j...k...r |...
+00000d90: 7c00 6a05 a101 0100 7400 a000 a100 7c00  |.j.....t.....|.
+00000da0: 5f08 7406 a007 6404 a101 0100 6400 5300  _.t...d.....d.S.
+00000db0: 2907 4e46 7a0d 4b65 7474 6c65 2041 6374  ).NFz.Kettle Act
+00000dc0: 6976 657a 0f4b 6574 746c 6520 496e 6163  ivez.Kettle Inac
+00000dd0: 7469 7665 7a1c 4c6f 6767 6564 2077 6974  tivez.Logged wit
+00000de0: 6820 7265 6475 6365 6420 6672 6571 656e  h reduced freqen
+00000df0: 6379 7a10 4665 726d 656e 7465 7220 4163  cyz.Fermenter Ac
+00000e00: 7469 7665 7a12 4665 726d 656e 7465 7220  tivez.Fermenter 
+00000e10: 496e 6163 7469 7665 290b 7220 0000 0072  Inactive).r ...r
+00000e20: 3e00 0000 da08 696e 7374 616e 6365 da05  >.....instance..
+00000e30: 7374 6174 6572 4600 0000 721b 0000 0072  staterF...r....r
+00000e40: 4800 0000 da04 696e 666f 7228 0000 0072  H.....infor(...r
+00000e50: 2900 0000 7240 0000 0029 0472 3300 0000  )...r@...).r3...
+00000e60: da03 6e6f 775a 0c6b 6574 746c 6573 7461  ..nowZ.kettlesta
+00000e70: 7475 735a 0f66 6572 6d65 6e74 6572 7374  tusZ.fermenterst
+00000e80: 6174 7573 7236 0000 0072 3600 0000 7237  atusr6...r6...r7
+00000e90: 0000 0072 4500 0000 5600 0000 733c 0000  ...rE...V...s<..
+00000ea0: 0000 0108 010a 0102 010e 0106 010a 0104  ................
+00000eb0: 010c 010a 010c 020a 0110 010c 010a 010a  ................
+00000ec0: 030c 0102 010e 0106 010a 0104 010c 010a  ................
+00000ed0: 010c 020a 0112 010c 010a 010a 017a 1348  .............z.H
+00000ee0: 5454 5053 656e 736f 722e 6c6f 6776 616c  TTPSensor.logval
+00000ef0: 7565 6301 0000 0000 0000 0000 0000 0001  uec.............
+00000f00: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
+00000f10: 7400 7c00 6a01 6401 8d01 5300 2902 4e29  t.|.j.d...S.).N)
+00000f20: 0172 1b00 0000 2902 da04 6469 6374 721b  .r....)...dictr.
+00000f30: 0000 0029 0172 3300 0000 7236 0000 0072  ...).r3...r6...r
+00000f40: 3600 0000 7237 0000 00da 0967 6574 5f73  6...r7.....get_s
+00000f50: 7461 7465 7a00 0000 7302 0000 0000 027a  tatez...s......z
+00000f60: 1448 5454 5053 656e 736f 722e 6765 745f  .HTTPSensor.get_
+00000f70: 7374 6174 6529 0ada 085f 5f6e 616d 655f  state)...__name_
+00000f80: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000f90: 5f71 7561 6c6e 616d 655f 5f72 1900 0000  _qualname__r....
+00000fa0: 7232 0000 0072 3b00 0000 724d 0000 0072  r2...r;...rM...r
+00000fb0: 4500 0000 7253 0000 00da 0d5f 5f63 6c61  E...rS.....__cla
+00000fc0: 7373 6365 6c6c 5f5f 7236 0000 0072 3600  sscell__r6...r6.
+00000fd0: 0000 7234 0000 0072 3700 0000 7212 0000  ..r4...r7...r...
+00000fe0: 000d 0000 0073 0c00 0000 0807 0c16 0805  .....s..........
+00000ff0: 0805 0822 0824 7212 0000 0063 0000 0000  ...".$r....c....
+00001000: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00001010: 4000 0000 7328 0000 0065 005a 0164 005a  @...s(...e.Z.d.Z
+00001020: 0264 0164 0284 005a 0365 0464 0364 0464  .d.d...Z.e.d.d.d
+00001030: 058d 0264 0664 0784 0083 015a 0564 0853  ...d.d.....Z.d.S
+00001040: 0029 09da 1248 5454 5053 656e 736f 7245  .)...HTTPSensorE
+00001050: 6e64 706f 696e 7463 0200 0000 0000 0000  ndpointc........
+00001060: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00001070: 7324 0000 0074 00a0 0164 01a1 017c 005f  s$...t...d...|._
+00001080: 027c 017c 005f 037c 006a 03a0 047c 0064  .|.|._.|.j...|.d
+00001090: 02a1 0201 0064 0353 0029 047a 330a 2020  .....d.S.).z3.  
+000010a0: 2020 2020 2020 496e 6974 6961 6c69 7a65        Initialize
+000010b0: 720a 0a20 2020 2020 2020 203a 7061 7261  r..        :para
+000010c0: 6d20 6362 7069 3a0a 2020 2020 2020 2020  m cbpi:.        
+000010d0: 7a15 5e5b 612d 7a41 2d5a 302d 392c 2e5d  z.^[a-zA-Z0-9,.]
+000010e0: 7b30 2c31 307d 247a 0b2f 6874 7470 7365  {0,10}$z./httpse
+000010f0: 6e73 6f72 4e29 05da 0272 65da 0763 6f6d  nsorN)...re..com
+00001100: 7069 6c65 da0d 7061 7474 6572 6e5f 6368  pile..pattern_ch
+00001110: 6563 6b72 2d00 0000 da08 7265 6769 7374  eckr-.....regist
+00001120: 6572 2902 7233 0000 0072 2d00 0000 7236  er).r3...r-...r6
+00001130: 0000 0072 3600 0000 7237 0000 0072 1900  ...r6...r7...r..
+00001140: 0000 8000 0000 7306 0000 0000 060c 0206  ......s.........
+00001150: 037a 1b48 5454 5053 656e 736f 7245 6e64  .z.HTTPSensorEnd
+00001160: 706f 696e 742e 5f5f 696e 6974 5f5f 7a0e  point.__init__z.
+00001170: 2f7b 6b65 797d 2f7b 7661 6c75 657d 4629  /{key}/{value}F)
+00001180: 02da 0470 6174 68da 0d61 7574 685f 7265  ...path..auth_re
+00001190: 7175 6972 6564 6302 0000 0000 0000 0000  quiredc.........
+000011a0: 0000 0004 0000 0004 0000 00c3 0000 0073  ...............s
+000011b0: 6c00 0000 7c01 6a00 6401 1900 7d02 7c01  l...|.j.d...}.|.
+000011c0: 6a00 6402 1900 7d03 7c00 6a01 a002 7c02  j.d...}.|.j...|.
+000011d0: a101 6403 7500 7236 7403 6a04 6404 6405  ..d.u.r6t.j.d.d.
+000011e0: 6406 6901 6407 8d02 5300 7c00 6a01 a002  d.i.d...S.|.j...
+000011f0: 7c03 a101 6403 7500 7258 7403 6a04 6404  |...d.u.rXt.j.d.
+00001200: 6405 6408 6901 6407 8d02 5300 7c03 7405  d.d.i.d...S.|.t.
+00001210: 7c02 3c00 7403 6a06 6409 640a 8d01 5300  |.<.t.j.d.d...S.
+00001220: 290b 61e4 0100 000a 2020 2020 2020 2020  ).a.....        
+00001230: 2d2d 2d0a 2020 2020 2020 2020 6465 7363  ---.        desc
+00001240: 7269 7074 696f 6e3a 204b 6574 746c 6520  ription: Kettle 
+00001250: 4865 6174 6572 206f 6e0a 2020 2020 2020  Heater on.      
+00001260: 2020 7461 6773 3a0a 2020 2020 2020 2020    tags:.        
+00001270: 2d20 4874 7470 5365 6e73 6f72 0a20 2020  - HttpSensor.   
+00001280: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
+00001290: 0a20 2020 2020 2020 202d 206e 616d 653a  .        - name:
+000012a0: 2022 6b65 7922 0a20 2020 2020 2020 2020   "key".         
+000012b0: 2069 6e3a 2022 7061 7468 220a 2020 2020   in: "path".    
+000012c0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+000012d0: 6e3a 2022 5365 6e73 6f72 204b 6579 220a  n: "Sensor Key".
+000012e0: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+000012f0: 6564 3a20 7472 7565 0a20 2020 2020 2020  ed: true.       
+00001300: 2020 2074 7970 653a 2022 7374 7269 6e67     type: "string
+00001310: 220a 2020 2020 2020 2020 2d20 6e61 6d65  ".        - name
+00001320: 3a20 2276 616c 7565 220a 2020 2020 2020  : "value".      
+00001330: 2020 2020 696e 3a20 2270 6174 6822 0a20      in: "path". 
+00001340: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00001350: 7469 6f6e 3a20 2256 616c 7565 220a 2020  tion: "Value".  
+00001360: 2020 2020 2020 2020 7265 7175 6972 6564          required
+00001370: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
+00001380: 2074 7970 653a 2022 696e 7465 6765 7222   type: "integer"
+00001390: 0a20 2020 2020 2020 2020 2066 6f72 6d61  .          forma
+000013a0: 743a 2022 696e 7436 3422 0a20 2020 2020  t: "int64".     
+000013b0: 2020 2072 6573 706f 6e73 6573 3a0a 2020     responses:.  
+000013c0: 2020 2020 2020 2020 2020 2232 3034 223a            "204":
+000013d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013e0: 2064 6573 6372 6970 7469 6f6e 3a20 7375   description: su
+000013f0: 6363 6573 7366 756c 206f 7065 7261 7469  ccessful operati
+00001400: 6f6e 0a20 2020 2020 2020 20da 036b 6579  on.        ..key
+00001410: 721b 0000 004e 69a6 0100 0072 4900 0000  r....Ni....rI...
+00001420: 7a2e 4b65 7920 6e6f 7420 6d61 7463 6869  z.Key not matchi
+00001430: 6e67 2070 6174 7465 726e 205e 5b61 2d7a  ng pattern ^[a-z
+00001440: 412d 5a30 2d39 2c2e 5d7b 302c 3130 7d24  A-Z0-9,.]{0,10}$
+00001450: 2902 da06 7374 6174 7573 da04 6461 7461  )...status..data
+00001460: 7a2f 4461 7461 206e 6f74 206d 6174 6368  z/Data not match
+00001470: 696e 6720 7061 7474 6572 6e20 5e5b 612d  ing pattern ^[a-
+00001480: 7a41 2d5a 302d 392c 2e5d 7b30 2c31 307d  zA-Z0-9,.]{0,10}
+00001490: 24e9 cc00 0000 2901 7260 0000 0029 07da  $.....).r`...)..
+000014a0: 0a6d 6174 6368 5f69 6e66 6f72 5b00 0000  .match_infor[...
+000014b0: da05 6d61 7463 6872 0200 0000 da0d 6a73  ..matchr......js
+000014c0: 6f6e 5f72 6573 706f 6e73 6572 4100 0000  on_responserA...
+000014d0: da08 5265 7370 6f6e 7365 2904 7233 0000  ..Response).r3..
+000014e0: 00da 0772 6571 7565 7374 725f 0000 0072  ...requestr_...r
+000014f0: 1b00 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00001500: 0000 00da 0f68 7474 705f 6e65 775f 7661  .....http_new_va
+00001510: 6c75 6532 8e00 0000 7310 0000 0000 190a  lue2....s.......
+00001520: 010a 0110 0112 0210 0112 0308 027a 2248  .............z"H
+00001530: 5454 5053 656e 736f 7245 6e64 706f 696e  TTPSensorEndpoin
+00001540: 742e 6874 7470 5f6e 6577 5f76 616c 7565  t.http_new_value
+00001550: 324e 2906 7254 0000 0072 5500 0000 7256  2N).rT...rU...rV
+00001560: 0000 0072 1900 0000 da0f 7265 7175 6573  ...r......reques
+00001570: 745f 6d61 7070 696e 6772 6800 0000 7236  t_mappingrh...r6
+00001580: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00001590: 0000 7258 0000 007e 0000 0073 0600 0000  ..rX...~...s....
+000015a0: 0802 080e 0a01 7258 0000 0063 0100 0000  ......rX...c....
+000015b0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000015c0: 4300 0000 7320 0000 007c 006a 00a0 0164  C...s ...|.j...d
+000015d0: 0174 02a1 0201 007c 006a 00a0 0164 0274  .t.....|.j...d.t
+000015e0: 03a1 0201 0064 0353 0029 047a a90a 2020  .....d.S.).z..  
+000015f0: 2020 5468 6973 206d 6574 686f 6420 6973    This method is
+00001600: 2063 616c 6c65 6420 6279 2074 6865 2073   called by the s
+00001610: 6572 7665 7220 6475 7269 6e67 2073 7461  erver during sta
+00001620: 7274 7570 200a 2020 2020 4865 7265 2079  rtup .    Here y
+00001630: 6f75 206e 6565 6420 746f 2072 6567 6973  ou need to regis
+00001640: 7465 7220 796f 7572 2070 6c75 6769 6e73  ter your plugins
+00001650: 2061 7420 7468 6520 7365 7276 6572 0a20   at the server. 
+00001660: 2020 200a 2020 2020 3a70 6172 616d 2063     .    :param c
+00001670: 6270 693a 2074 6865 2063 6270 6920 636f  bpi: the cbpi co
+00001680: 7265 200a 2020 2020 3a72 6574 7572 6e3a  re .    :return:
+00001690: 200a 2020 2020 7212 0000 0072 5800 0000   .    r....rX...
+000016a0: 4e29 04da 0670 6c75 6769 6e72 5c00 0000  N)...pluginr\...
+000016b0: 7212 0000 0072 5800 0000 2901 722d 0000  r....rX...).r-..
+000016c0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+000016d0: da05 7365 7475 70b5 0000 0073 0400 0000  ..setup....s....
+000016e0: 0009 0e01 726b 0000 0029 1772 4a00 0000  ....rk...).rJ...
+000016f0: da07 6169 6f68 7474 7072 0200 0000 5a08  ..aiohttpr....Z.
+00001700: 6362 7069 2e61 7069 7220 0000 0072 0400  cbpi.apir ...r..
+00001710: 0000 7259 0000 0072 4800 0000 da14 6362  ..rY...rH.....cb
+00001720: 7069 2e61 7069 2e64 6174 6163 6c61 7373  pi.api.dataclass
+00001730: 6573 7205 0000 0072 0600 0000 7241 0000  esr....r....rA..
+00001740: 00da 0a70 6172 616d 6574 6572 73da 0850  ...parameters..P
+00001750: 726f 7065 7274 79da 0454 6578 74da 064e  roperty..Text..N
+00001760: 756d 6265 7272 0f00 0000 7210 0000 00da  umberr....r.....
+00001770: 0a43 4250 6953 656e 736f 7272 1200 0000  .CBPiSensorr....
+00001780: da0d 4342 5069 4578 7465 6e73 696f 6e72  ..CBPiExtensionr
+00001790: 5800 0000 726b 0000 0072 3600 0000 7236  X...rk...r6...r6
+000017a0: 0000 0072 3600 0000 7237 0000 00da 083c  ...r6...r7.....<
+000017b0: 6d6f 6475 6c65 3e02 0000 0073 2200 0000  module>....s"...
+000017c0: 0801 0c01 0801 0801 0c01 0801 0801 1002  ................
+000017d0: 0402 1001 1001 0c01 0c01 0efc 0406 126b  ...............k
+000017e0: 1037                                     .7
```

### Comparing `cbpi4-4.1.7/cbpi/extension/hysteresis/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mashstep/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/mashstep/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/generic_mqtt_actor.py` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/generic_mqtt_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_actor/mqtt_actor.py` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_actor/mqtt_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datetime import datetime
 
 @parameters([Property.Text(label="Topic", configurable=True, description="MQTT Topic"),
              Property.Text(label="PayloadDictionary", configurable=True, default_value="",
                            description="Where to find msg in payload, leave blank for raw payload"),
              Property.Kettle(label="Kettle", description="Reduced logging if Kettle is inactive (only Kettle or Fermenter to be selected)"),
              Property.Fermenter(label="Fermenter", description="Reduced logging in seconds if Fermenter is inactive (only Kettle or Fermenter to be selected)"),
-             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default:60 sec | 0 disabled)"),
+             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default is 60 sec)"),
              Property.Number(label="Timeout", configurable=True, unit="sec",
                             description="Timeout in seconds to send notification (default:60 | deactivated: 0)")])
 class MQTTSensor(CBPiSensor):
 
     def __init__(self, cbpi, id, props):
         super(MQTTSensor, self).__init__(cbpi, id, props)
         self.Topic = self.props.get("Topic", None)
@@ -30,16 +30,14 @@
         self.starttime = time.time()
         self.notificationsend = False
         self.nextchecktime=self.starttime+self.timeout
         self.lastdata=time.time()
         self.lastlog=0
         self.sensor=self.get_sensor(self.id)
         self.reducedfrequency=int(self.props.get("ReducedLogging", 60))
-        if self.reducedfrequency < 0:
-            self.reducedfrequency = 0
         self.kettleid=self.props.get("Kettle", None)
         self.fermenterid=self.props.get("Fermenter", None)
         self.reducedlogging = True if self.kettleid or self.fermenterid else False
 
         if self.kettleid is not None and self.fermenterid is not None:
             self.reducedlogging=False
             self.cbpi.notify("MQTTSensor", "Sensor '" + str(self.sensor.name) + "' cant't have Fermenter and Kettle defined for reduced logging.", NotificationType.WARNING, action=[NotificationAction("OK", self.Confirm)])
@@ -89,52 +87,49 @@
                 kettlestatus=False
             if kettlestatus:
                 self.log_data(self.value)
                 logging.info("MQTTSensor {} Kettle Active".format(self.sensor.name))
                 self.lastlog = time.time()
             else:
                 logging.info("MQTTSensor {} Kettle Inactive".format(self.sensor.name))
-                if self.reducedfrequency != 0:
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass   
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass   
 
         if self.fermenter is not None:
             try:
                 fermenterstatus=self.fermenter.instance.state
             except:
                 fermenterstatus=False
             if fermenterstatus:
                 self.log_data(self.value)
                 logging.info("MQTTSensor {} Fermenter Active".format(self.sensor.name))
                 self.lastlog = time.time()
             else:
                 logging.info("MQTTSensor {} Fermenter Inactive".format(self.sensor.name))
-                if self.reducedfrequency != 0:
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass            
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass            
 
     async def run(self):
         while self.running:
             if self.timeout !=0:         
                 if time.time() > self.nextchecktime and self.notificationsend == False:   
                     await self.message()
                     self.notificationsend=True
             await asyncio.sleep(1)
 
     def get_state(self):
         return dict(value=self.value)
 
     async def on_stop(self):
-        was_cancelled=False
         if not self.mqtt_task.done():
             logging.info("Task not done -> cancelling")
             was_cancelled = self.mqtt_task.cancel()
         try:            
             logging.info("Trying to call cancelled task")
             await self.mqtt_task
         except asyncio.CancelledError:
```

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 27 17:54:59 2023 UTC, .py size: 7123 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 73d8 2164 d31b 0000  a.......s.!d....
+00000000: 610d 0d0a 0000 0000 143a 1f64 991b 0000  a........:.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c04  m.Z.m.Z...d.d.l.
 00000060: 5400 6400 6401 6c08 5a08 6400 6401 6c09  T.d.d.l.Z.d.d.l.
 00000070: 5a09 6400 6401 6c0a 5a0a 6400 6405 6c0b  Z.d.d.l.Z.d.d.l.
@@ -201,153 +201,152 @@
 00000c80: 7240 0000 0072 4000 0000 7241 0000 0072  r@...r@...rA...r
 00000c90: 2600 0000 3700 0000 7326 0000 0000 010a  &...7...s&......
 00000ca0: 0102 010a 010a 010e 0210 010a 010c 010a  ................
 00000cb0: 0110 0214 010c 010a 020a 0110 0106 010e  ................
 00000cc0: 010e 017a 154d 5154 5453 656e 736f 722e  ...z.MQTTSensor.
 00000cd0: 6f6e 5f6d 6573 7361 6765 6301 0000 0000  on_messagec.....
 00000ce0: 0000 0000 0000 0004 0000 0006 0000 00c3  ................
-00000cf0: 0000 0073 9001 0000 7c00 6a00 6401 6b02  ...s....|.j.d.k.
-00000d00: 720a 7c00 6a01 6400 7501 7220 7c00 a002  r.|.j.d.u.r |...
-00000d10: 7c00 6a01 a101 6e02 6400 7c00 5f03 7c00  |.j...n.d.|._.|.
-00000d20: 6a04 6400 7501 723c 7c00 a005 7c00 6a04  j.d.u.r<|...|.j.
-00000d30: a101 6e02 6400 7c00 5f06 7407 a007 a100  ..n.d.|._.t.....
-00000d40: 7d01 7c00 6a03 6400 7501 72e8 7a0e 7c00  }.|.j.d.u.r.z.|.
-00000d50: 6a03 6a08 6a09 7d02 5700 6e10 0100 0100  j.j.j.}.W.n.....
-00000d60: 0100 6402 7d02 5900 6e02 3000 7c02 72a4  ..d.}.Y.n.0.|.r.
-00000d70: 7c00 a00a 7c00 6a0b a101 0100 740c a00d  |...|.j.....t...
-00000d80: 6403 a00e 7c00 6a0f 6a10 a101 a101 0100  d...|.j.j.......
-00000d90: 7407 a007 a100 7c00 5f11 6e44 740c a00d  t.....|._.nDt...
-00000da0: 6404 a00e 7c00 6a0f 6a10 a101 a101 0100  d...|.j.j.......
-00000db0: 7c01 7c00 6a11 7c00 6a00 1700 6b05 72e8  |.|.j.|.j...k.r.
-00000dc0: 7c00 a00a 7c00 6a0b a101 0100 7407 a007  |...|.j.....t...
-00000dd0: a100 7c00 5f11 740c a00d 6405 a101 0100  ..|._.t...d.....
-00000de0: 7c00 6a06 6400 7501 9001 728c 7a0e 7c00  |.j.d.u...r.z.|.
-00000df0: 6a06 6a08 6a09 7d03 5700 6e10 0100 0100  j.j.j.}.W.n.....
-00000e00: 0100 6402 7d03 5900 6e02 3000 7c03 9001  ..d.}.Y.n.0.|...
-00000e10: 7246 7c00 a00a 7c00 6a0b a101 0100 740c  rF|...|.j.....t.
-00000e20: a00d 6406 a00e 7c00 6a0f 6a10 a101 a101  ..d...|.j.j.....
-00000e30: 0100 7407 a007 a100 7c00 5f11 6e46 740c  ..t.....|._.nFt.
-00000e40: a00d 6407 a00e 7c00 6a0f 6a10 a101 a101  ..d...|.j.j.....
-00000e50: 0100 7c01 7c00 6a11 7c00 6a00 1700 6b05  ..|.|.j.|.j...k.
-00000e60: 9001 728c 7c00 a00a 7c00 6a0b a101 0100  ..r.|...|.j.....
-00000e70: 7407 a007 a100 7c00 5f11 740c a00d 6405  t.....|._.t...d.
-00000e80: a101 0100 6400 5300 2908 4e72 0100 0000  ....d.S.).Nr....
-00000e90: 467a 1b4d 5154 5453 656e 736f 7220 7b7d  Fz.MQTTSensor {}
-00000ea0: 204b 6574 746c 6520 4163 7469 7665 7a1d   Kettle Activez.
-00000eb0: 4d51 5454 5365 6e73 6f72 207b 7d20 4b65  MQTTSensor {} Ke
-00000ec0: 7474 6c65 2049 6e61 6374 6976 657a 1c4c  ttle Inactivez.L
-00000ed0: 6f67 6765 6420 7769 7468 2072 6564 7563  ogged with reduc
-00000ee0: 6564 2066 7265 7165 6e63 797a 1e4d 5154  ed freqencyz.MQT
-00000ef0: 5453 656e 736f 7220 7b7d 2046 6572 6d65  TSensor {} Ferme
-00000f00: 6e74 6572 2041 6374 6976 657a 204d 5154  nter Activez MQT
-00000f10: 5453 656e 736f 7220 7b7d 2046 6572 6d65  TSensor {} Ferme
-00000f20: 6e74 6572 2049 6e61 6374 6976 6529 1272  nter Inactive).r
-00000f30: 3400 0000 7235 0000 00da 0a67 6574 5f6b  4...r5.....get_k
-00000f40: 6574 746c 65da 066b 6574 746c 6572 3600  ettle..kettler6.
-00000f50: 0000 da0d 6765 745f 6665 726d 656e 7465  ....get_fermente
-00000f60: 72da 0966 6572 6d65 6e74 6572 722b 0000  r..fermenterr+..
-00000f70: 00da 0869 6e73 7461 6e63 65da 0573 7461  ...instance..sta
-00000f80: 7465 7250 0000 0072 2800 0000 724d 0000  terP...r(...rM..
-00000f90: 0072 4e00 0000 724f 0000 0072 3300 0000  .rN...rO...r3...
-00000fa0: 723a 0000 0072 3000 0000 2904 723d 0000  r:...r0...).r=..
-00000fb0: 00da 036e 6f77 da0c 6b65 7474 6c65 7374  ...now..kettlest
-00000fc0: 6174 7573 da0f 6665 726d 656e 7465 7273  atus..fermenters
-00000fd0: 7461 7475 7372 4000 0000 7240 0000 0072  tatusr@...r@...r
-00000fe0: 4100 0000 724c 0000 004f 0000 0073 4200  A...rL...O...sB.
-00000ff0: 0000 0001 0a02 1c01 1c01 0801 0a01 0201  ................
-00001000: 0e01 0601 0a01 0401 0c01 1401 0c02 1401  ................
-00001010: 1001 0c01 0a01 0a03 0c01 0201 0e01 0601  ................
-00001020: 0a01 0601 0c01 1401 0c02 1401 1201 0c01  ................
-00001030: 0a01 0a01 7a13 4d51 5454 5365 6e73 6f72  ....z.MQTTSensor
-00001040: 2e6c 6f67 7661 6c75 6563 0100 0000 0000  .logvaluec......
-00001050: 0000 0000 0000 0100 0000 0300 0000 c300  ................
-00001060: 0000 7352 0000 007c 006a 0072 4e7c 006a  ..sR...|.j.rN|.j
-00001070: 0164 016b 0372 3c74 02a0 02a1 007c 006a  .d.k.r<t.....|.j
-00001080: 036b 0472 3c7c 006a 0464 026b 0272 3c7c  .k.r<|.j.d.k.r<|
-00001090: 00a0 05a1 0049 0064 0048 0001 0064 037c  .....I.d.H...d.|
-000010a0: 005f 0474 06a0 0764 04a1 0149 0064 0048  ._.t...d...I.d.H
-000010b0: 0001 0071 0064 0053 0029 054e 7201 0000  ...q.d.S.).Nr...
-000010c0: 0046 54e9 0100 0000 2908 da07 7275 6e6e  .FT.....)...runn
-000010d0: 696e 6772 2a00 0000 722b 0000 0072 2e00  ingr*...r+...r..
-000010e0: 0000 722d 0000 0072 4600 0000 da07 6173  ..r-...rF.....as
-000010f0: 796e 6369 6fda 0573 6c65 6570 a901 723d  yncio..sleep..r=
-00001100: 0000 0072 4000 0000 7240 0000 0072 4100  ...r@...r@...rA.
-00001110: 0000 da03 7275 6e77 0000 0073 0c00 0000  ....runw...s....
-00001120: 0001 0601 0a01 1801 0e01 0601 7a0e 4d51  ............z.MQ
-00001130: 5454 5365 6e73 6f72 2e72 756e 6301 0000  TTSensor.runc...
-00001140: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001150: 0043 0000 0073 0c00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00001160: 6401 8d01 5300 2902 4e29 0172 2800 0000  d...S.).N).r(...
-00001170: 2902 da04 6469 6374 7228 0000 0072 6300  )...dictr(...rc.
-00001180: 0000 7240 0000 0072 4000 0000 7241 0000  ..r@...r@...rA..
-00001190: 00da 0967 6574 5f73 7461 7465 7f00 0000  ...get_state....
-000011a0: 7302 0000 0000 017a 144d 5154 5453 656e  s......z.MQTTSen
-000011b0: 736f 722e 6765 745f 7374 6174 6563 0100  sor.get_statec..
-000011c0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-000011d0: 0000 c300 0000 736c 0000 007c 006a 00a0  ......sl...|.j..
-000011e0: 01a1 0073 1e74 02a0 0364 01a1 0101 007c  ...s.t...d.....|
-000011f0: 006a 00a0 04a1 007d 017a 1a74 02a0 0364  .j.....}.z.t...d
-00001200: 02a1 0101 007c 006a 0049 0064 0048 0001  .....|.j.I.d.H..
-00001210: 0057 006e 1e04 0074 056a 0679 5601 0001  .W.n...t.j.yV...
-00001220: 0001 0074 02a0 0364 03a1 0101 0059 006e  ...t...d.....Y.n
-00001230: 0230 0074 02a0 0364 04a0 077c 01a1 01a1  .0.t...d...|....
-00001240: 0101 0064 0053 0029 054e 7a1b 5461 736b  ...d.S.).Nz.Task
-00001250: 206e 6f74 2064 6f6e 6520 2d3e 2063 616e   not done -> can
-00001260: 6365 6c6c 696e 677a 1d54 7279 696e 6720  cellingz.Trying 
-00001270: 746f 2063 616c 6c20 6361 6e63 656c 6c65  to call cancelle
-00001280: 6420 7461 736b 7a17 5461 736b 2068 6173  d taskz.Task has
-00001290: 2062 6565 6e20 4361 6e63 656c 6c65 647a   been Cancelledz
-000012a0: 1254 6173 6b20 6361 6e63 656c 6c65 643a  .Task cancelled:
-000012b0: 207b 7d29 0872 2700 0000 da04 646f 6e65   {}).r'.....done
-000012c0: 724d 0000 0072 4e00 0000 da06 6361 6e63  rM...rN.....canc
-000012d0: 656c 7261 0000 00da 0e43 616e 6365 6c6c  elra.....Cancell
-000012e0: 6564 4572 726f 7272 4f00 0000 2902 723d  edErrorrO...).r=
-000012f0: 0000 005a 0d77 6173 5f63 616e 6365 6c6c  ...Z.was_cancell
-00001300: 6564 7240 0000 0072 4000 0000 7241 0000  edr@...r@...rA..
-00001310: 00da 076f 6e5f 7374 6f70 8200 0000 7314  ...on_stop....s.
-00001320: 0000 0000 010a 010a 010a 0102 010a 0110  ................
-00001330: 010e 010a 0106 017a 124d 5154 5453 656e  .......z.MQTTSen
-00001340: 736f 722e 6f6e 5f73 746f 7029 0cda 085f  sor.on_stop)..._
-00001350: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00001360: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00001370: 5f72 1e00 0000 723c 0000 0072 4600 0000  _r....r<...rF...
-00001380: 7226 0000 0072 4c00 0000 7264 0000 0072  r&...rL...rd...r
-00001390: 6600 0000 726a 0000 00da 0d5f 5f63 6c61  f...rj.....__cla
-000013a0: 7373 6365 6c6c 5f5f 7240 0000 0072 4000  sscell__r@...r@.
-000013b0: 0000 723e 0000 0072 4100 0000 7216 0000  ..r>...rA...r...
-000013c0: 000b 0000 0073 1000 0000 080a 0c18 0805  .....s..........
-000013d0: 0805 0818 0828 0808 0803 7216 0000 0063  .....(....r....c
-000013e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000013f0: 0500 0000 4300 0000 732c 0000 0074 007c  ....C...s,...t.|
-00001400: 006a 01a0 0264 0164 02a1 0283 01a0 03a1  .j...d.d........
-00001410: 0064 036b 0272 287c 006a 04a0 0564 0474  .d.k.r(|.j...d.t
-00001420: 06a1 0201 0064 0553 0029 067a a20a 2020  .....d.S.).z..  
-00001430: 2020 5468 6973 206d 6574 686f 6420 6973    This method is
-00001440: 2063 616c 6c65 6420 6279 2074 6865 2073   called by the s
-00001450: 6572 7665 7220 6475 7269 6e67 2073 7461  erver during sta
-00001460: 7274 7570 0a20 2020 2048 6572 6520 796f  rtup.    Here yo
-00001470: 7520 6e65 6564 2074 6f20 7265 6769 7374  u need to regist
-00001480: 6572 2079 6f75 7220 706c 7567 696e 7320  er your plugins 
-00001490: 6174 2074 6865 2073 6572 7665 720a 0a20  at the server.. 
-000014a0: 2020 203a 7061 7261 6d20 6362 7069 3a20     :param cbpi: 
-000014b0: 7468 6520 6362 7069 2063 6f72 650a 2020  the cbpi core.  
-000014c0: 2020 3a72 6574 7572 6e3a 0a20 2020 20da    :return:.    .
-000014d0: 046d 7174 7446 da04 7472 7565 7216 0000  .mqttF..truer...
-000014e0: 004e 2907 7239 0000 00da 0d73 7461 7469  .N).r9.....stati
-000014f0: 635f 636f 6e66 6967 7220 0000 00da 056c  c_configr .....l
-00001500: 6f77 6572 da06 706c 7567 696e da08 7265  ower..plugin..re
-00001510: 6769 7374 6572 7216 0000 0029 0172 2300  gisterr....).r#.
-00001520: 0000 7240 0000 0072 4000 0000 7241 0000  ..r@...r@...rA..
-00001530: 00da 0573 6574 7570 8e00 0000 7304 0000  ...setup....s...
-00001540: 0000 081a 0172 7500 0000 2912 7261 0000  .....ru...).ra..
-00001550: 00da 1463 6270 692e 6170 692e 6461 7461  ...cbpi.api.data
-00001560: 636c 6173 7365 7372 0200 0000 7203 0000  classesr....r...
-00001570: 005a 0863 6270 692e 6170 6972 0400 0000  .Z.cbpi.apir....
-00001580: 7205 0000 0072 0600 0000 724d 0000 0072  r....r....rM...r
-00001590: 4700 0000 722b 0000 0072 0800 0000 da04  G...r+...r......
-000015a0: 5465 7874 7210 0000 0072 1100 0000 da06  Textr....r......
-000015b0: 4e75 6d62 6572 7216 0000 0072 7500 0000  Numberr....ru...
-000015c0: 7240 0000 0072 4000 0000 7240 0000 0072  r@...r@...r@...r
-000015d0: 4100 0000 da08 3c6d 6f64 756c 653e 0200  A.....<module>..
-000015e0: 0000 7328 0000 0008 0110 0114 0108 0108  ..s(............
-000015f0: 0108 0108 010c 0210 010a 0102 ff04 020c  ................
-00001600: 010c 010e 010a 0102 ff04 fa04 0812 7b    ..............{
+00000cf0: 0000 0073 8601 0000 7c00 6a00 6400 7501  ...s....|.j.d.u.
+00000d00: 7216 7c00 a001 7c00 6a00 a101 6e02 6400  r.|...|.j...n.d.
+00000d10: 7c00 5f02 7c00 6a03 6400 7501 7232 7c00  |._.|.j.d.u.r2|.
+00000d20: a004 7c00 6a03 a101 6e02 6400 7c00 5f05  ..|.j...n.d.|._.
+00000d30: 7406 a006 a100 7d01 7c00 6a02 6400 7501  t.....}.|.j.d.u.
+00000d40: 72de 7a0e 7c00 6a02 6a07 6a08 7d02 5700  r.z.|.j.j.j.}.W.
+00000d50: 6e10 0100 0100 0100 6401 7d02 5900 6e02  n.......d.}.Y.n.
+00000d60: 3000 7c02 729a 7c00 a009 7c00 6a0a a101  0.|.r.|...|.j...
+00000d70: 0100 740b a00c 6402 a00d 7c00 6a0e 6a0f  ..t...d...|.j.j.
+00000d80: a101 a101 0100 7406 a006 a100 7c00 5f10  ......t.....|._.
+00000d90: 6e44 740b a00c 6403 a00d 7c00 6a0e 6a0f  nDt...d...|.j.j.
+00000da0: a101 a101 0100 7c01 7c00 6a10 7c00 6a11  ......|.|.j.|.j.
+00000db0: 1700 6b05 72de 7c00 a009 7c00 6a0a a101  ..k.r.|...|.j...
+00000dc0: 0100 7406 a006 a100 7c00 5f10 740b a00c  ..t.....|._.t...
+00000dd0: 6404 a101 0100 7c00 6a05 6400 7501 9001  d.....|.j.d.u...
+00000de0: 7282 7a0e 7c00 6a05 6a07 6a08 7d03 5700  r.z.|.j.j.j.}.W.
+00000df0: 6e10 0100 0100 0100 6401 7d03 5900 6e02  n.......d.}.Y.n.
+00000e00: 3000 7c03 9001 723c 7c00 a009 7c00 6a0a  0.|...r<|...|.j.
+00000e10: a101 0100 740b a00c 6405 a00d 7c00 6a0e  ....t...d...|.j.
+00000e20: 6a0f a101 a101 0100 7406 a006 a100 7c00  j.......t.....|.
+00000e30: 5f10 6e46 740b a00c 6406 a00d 7c00 6a0e  _.nFt...d...|.j.
+00000e40: 6a0f a101 a101 0100 7c01 7c00 6a10 7c00  j.......|.|.j.|.
+00000e50: 6a11 1700 6b05 9001 7282 7c00 a009 7c00  j...k...r.|...|.
+00000e60: 6a0a a101 0100 7406 a006 a100 7c00 5f10  j.....t.....|._.
+00000e70: 740b a00c 6404 a101 0100 6400 5300 2907  t...d.....d.S.).
+00000e80: 4e46 7a1b 4d51 5454 5365 6e73 6f72 207b  NFz.MQTTSensor {
+00000e90: 7d20 4b65 7474 6c65 2041 6374 6976 657a  } Kettle Activez
+00000ea0: 1d4d 5154 5453 656e 736f 7220 7b7d 204b  .MQTTSensor {} K
+00000eb0: 6574 746c 6520 496e 6163 7469 7665 7a1c  ettle Inactivez.
+00000ec0: 4c6f 6767 6564 2077 6974 6820 7265 6475  Logged with redu
+00000ed0: 6365 6420 6672 6571 656e 6379 7a1e 4d51  ced freqencyz.MQ
+00000ee0: 5454 5365 6e73 6f72 207b 7d20 4665 726d  TTSensor {} Ferm
+00000ef0: 656e 7465 7220 4163 7469 7665 7a20 4d51  enter Activez MQ
+00000f00: 5454 5365 6e73 6f72 207b 7d20 4665 726d  TTSensor {} Ferm
+00000f10: 656e 7465 7220 496e 6163 7469 7665 2912  enter Inactive).
+00000f20: 7235 0000 00da 0a67 6574 5f6b 6574 746c  r5.....get_kettl
+00000f30: 65da 066b 6574 746c 6572 3600 0000 da0d  e..kettler6.....
+00000f40: 6765 745f 6665 726d 656e 7465 72da 0966  get_fermenter..f
+00000f50: 6572 6d65 6e74 6572 722b 0000 00da 0869  ermenterr+.....i
+00000f60: 6e73 7461 6e63 65da 0573 7461 7465 7250  nstance..staterP
+00000f70: 0000 0072 2800 0000 724d 0000 0072 4e00  ...r(...rM...rN.
+00000f80: 0000 724f 0000 0072 3300 0000 723a 0000  ..rO...r3...r:..
+00000f90: 0072 3000 0000 7234 0000 0029 0472 3d00  .r0...r4...).r=.
+00000fa0: 0000 da03 6e6f 77da 0c6b 6574 746c 6573  ....now..kettles
+00000fb0: 7461 7475 73da 0f66 6572 6d65 6e74 6572  tatus..fermenter
+00000fc0: 7374 6174 7573 7240 0000 0072 4000 0000  statusr@...r@...
+00000fd0: 7241 0000 0072 4c00 0000 4f00 0000 7340  rA...rL...O...s@
+00000fe0: 0000 0000 011c 011c 0108 010a 0102 010e  ................
+00000ff0: 0106 010a 0104 010c 0114 010c 0214 0110  ................
+00001000: 010c 010a 010a 030c 0102 010e 0106 010a  ................
+00001010: 0106 010c 0114 010c 0214 0112 010c 010a  ................
+00001020: 010a 017a 134d 5154 5453 656e 736f 722e  ...z.MQTTSensor.
+00001030: 6c6f 6776 616c 7565 6301 0000 0000 0000  logvaluec.......
+00001040: 0000 0000 0001 0000 0003 0000 00c3 0000  ................
+00001050: 0073 5200 0000 7c00 6a00 724e 7c00 6a01  .sR...|.j.rN|.j.
+00001060: 6401 6b03 723c 7402 a002 a100 7c00 6a03  d.k.r<t.....|.j.
+00001070: 6b04 723c 7c00 6a04 6402 6b02 723c 7c00  k.r<|.j.d.k.r<|.
+00001080: a005 a100 4900 6400 4800 0100 6403 7c00  ....I.d.H...d.|.
+00001090: 5f04 7406 a007 6404 a101 4900 6400 4800  _.t...d...I.d.H.
+000010a0: 0100 7100 6400 5300 2905 4e72 0100 0000  ..q.d.S.).Nr....
+000010b0: 4654 e901 0000 0029 08da 0772 756e 6e69  FT.....)...runni
+000010c0: 6e67 722a 0000 0072 2b00 0000 722e 0000  ngr*...r+...r...
+000010d0: 0072 2d00 0000 7246 0000 00da 0761 7379  .r-...rF.....asy
+000010e0: 6e63 696f da05 736c 6565 70a9 0172 3d00  ncio..sleep..r=.
+000010f0: 0000 7240 0000 0072 4000 0000 7241 0000  ..r@...r@...rA..
+00001100: 00da 0372 756e 7500 0000 730c 0000 0000  ...runu...s.....
+00001110: 0106 010a 0118 010e 0106 017a 0e4d 5154  ...........z.MQT
+00001120: 5453 656e 736f 722e 7275 6e63 0100 0000  TSensor.runc....
+00001130: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001140: 4300 0000 730c 0000 0074 007c 006a 0164  C...s....t.|.j.d
+00001150: 018d 0153 0029 024e 2901 7228 0000 0029  ...S.).N).r(...)
+00001160: 02da 0464 6963 7472 2800 0000 7263 0000  ...dictr(...rc..
+00001170: 0072 4000 0000 7240 0000 0072 4100 0000  .r@...r@...rA...
+00001180: da09 6765 745f 7374 6174 657d 0000 0073  ..get_state}...s
+00001190: 0200 0000 0001 7a14 4d51 5454 5365 6e73  ......z.MQTTSens
+000011a0: 6f72 2e67 6574 5f73 7461 7465 6301 0000  or.get_statec...
+000011b0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+000011c0: 00c3 0000 0073 6c00 0000 7c00 6a00 a001  .....sl...|.j...
+000011d0: a100 731e 7402 a003 6401 a101 0100 7c00  ..s.t...d.....|.
+000011e0: 6a00 a004 a100 7d01 7a1a 7402 a003 6402  j.....}.z.t...d.
+000011f0: a101 0100 7c00 6a00 4900 6400 4800 0100  ....|.j.I.d.H...
+00001200: 5700 6e1e 0400 7405 6a06 7956 0100 0100  W.n...t.j.yV....
+00001210: 0100 7402 a003 6403 a101 0100 5900 6e02  ..t...d.....Y.n.
+00001220: 3000 7402 a003 6404 a007 7c01 a101 a101  0.t...d...|.....
+00001230: 0100 6400 5300 2905 4e7a 1b54 6173 6b20  ..d.S.).Nz.Task 
+00001240: 6e6f 7420 646f 6e65 202d 3e20 6361 6e63  not done -> canc
+00001250: 656c 6c69 6e67 7a1d 5472 7969 6e67 2074  ellingz.Trying t
+00001260: 6f20 6361 6c6c 2063 616e 6365 6c6c 6564  o call cancelled
+00001270: 2074 6173 6b7a 1754 6173 6b20 6861 7320   taskz.Task has 
+00001280: 6265 656e 2043 616e 6365 6c6c 6564 7a12  been Cancelledz.
+00001290: 5461 736b 2063 616e 6365 6c6c 6564 3a20  Task cancelled: 
+000012a0: 7b7d 2908 7227 0000 00da 0464 6f6e 6572  {}).r'.....doner
+000012b0: 4d00 0000 724e 0000 00da 0663 616e 6365  M...rN.....cance
+000012c0: 6c72 6100 0000 da0e 4361 6e63 656c 6c65  lra.....Cancelle
+000012d0: 6445 7272 6f72 724f 0000 0029 0272 3d00  dErrorrO...).r=.
+000012e0: 0000 5a0d 7761 735f 6361 6e63 656c 6c65  ..Z.was_cancelle
+000012f0: 6472 4000 0000 7240 0000 0072 4100 0000  dr@...r@...rA...
+00001300: da07 6f6e 5f73 746f 7080 0000 0073 1400  ..on_stop....s..
+00001310: 0000 0001 0a01 0a01 0a01 0201 0a01 1001  ................
+00001320: 0e01 0a01 0601 7a12 4d51 5454 5365 6e73  ......z.MQTTSens
+00001330: 6f72 2e6f 6e5f 7374 6f70 290c da08 5f5f  or.on_stop)...__
+00001340: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00001350: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00001360: 721e 0000 0072 3c00 0000 7246 0000 0072  r....r<...rF...r
+00001370: 2600 0000 724c 0000 0072 6400 0000 7266  &...rL...rd...rf
+00001380: 0000 0072 6a00 0000 da0d 5f5f 636c 6173  ...rj.....__clas
+00001390: 7363 656c 6c5f 5f72 4000 0000 7240 0000  scell__r@...r@..
+000013a0: 0072 3e00 0000 7241 0000 0072 1600 0000  .r>...rA...r....
+000013b0: 0b00 0000 7310 0000 0008 0a0c 1808 0508  ....s...........
+000013c0: 0508 1808 2608 0808 0372 1600 0000 6301  ....&....r....c.
+000013d0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+000013e0: 0000 0043 0000 0073 2c00 0000 7400 7c00  ...C...s,...t.|.
+000013f0: 6a01 a002 6401 6402 a102 8301 a003 a100  j...d.d.........
+00001400: 6403 6b02 7228 7c00 6a04 a005 6404 7406  d.k.r(|.j...d.t.
+00001410: a102 0100 6405 5300 2906 7aa2 0a20 2020  ....d.S.).z..   
+00001420: 2054 6869 7320 6d65 7468 6f64 2069 7320   This method is 
+00001430: 6361 6c6c 6564 2062 7920 7468 6520 7365  called by the se
+00001440: 7276 6572 2064 7572 696e 6720 7374 6172  rver during star
+00001450: 7475 700a 2020 2020 4865 7265 2079 6f75  tup.    Here you
+00001460: 206e 6565 6420 746f 2072 6567 6973 7465   need to registe
+00001470: 7220 796f 7572 2070 6c75 6769 6e73 2061  r your plugins a
+00001480: 7420 7468 6520 7365 7276 6572 0a0a 2020  t the server..  
+00001490: 2020 3a70 6172 616d 2063 6270 693a 2074    :param cbpi: t
+000014a0: 6865 2063 6270 6920 636f 7265 0a20 2020  he cbpi core.   
+000014b0: 203a 7265 7475 726e 3a0a 2020 2020 da04   :return:.    ..
+000014c0: 6d71 7474 46da 0474 7275 6572 1600 0000  mqttF..truer....
+000014d0: 4e29 0772 3900 0000 da0d 7374 6174 6963  N).r9.....static
+000014e0: 5f63 6f6e 6669 6772 2000 0000 da05 6c6f  _configr .....lo
+000014f0: 7765 72da 0670 6c75 6769 6eda 0872 6567  wer..plugin..reg
+00001500: 6973 7465 7272 1600 0000 2901 7223 0000  isterr....).r#..
+00001510: 0072 4000 0000 7240 0000 0072 4100 0000  .r@...r@...rA...
+00001520: da05 7365 7475 708c 0000 0073 0400 0000  ..setup....s....
+00001530: 0008 1a01 7275 0000 0029 1272 6100 0000  ....ru...).ra...
+00001540: da14 6362 7069 2e61 7069 2e64 6174 6163  ..cbpi.api.datac
+00001550: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
+00001560: 5a08 6362 7069 2e61 7069 7204 0000 0072  Z.cbpi.apir....r
+00001570: 0500 0000 7206 0000 0072 4d00 0000 7247  ....r....rM...rG
+00001580: 0000 0072 2b00 0000 7208 0000 00da 0454  ...r+...r......T
+00001590: 6578 7472 1000 0000 7211 0000 00da 064e  extr....r......N
+000015a0: 756d 6265 7272 1600 0000 7275 0000 0072  umberr....ru...r
+000015b0: 4000 0000 7240 0000 0072 4000 0000 7241  @...r@...r@...rA
+000015c0: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
+000015d0: 0073 2800 0000 0801 1001 1401 0801 0801  .s(.............
+000015e0: 0801 0801 0c02 1001 0a01 02ff 0402 0c01  ................
+000015f0: 0c01 0e01 0a01 02ff 04fa 0408 1279       .............y
```

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_util/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/onewire/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/onewire/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,41 +50,39 @@
             time.sleep(1)
 
 @parameters([Property.Select(label="Sensor", options=getSensors()), 
              Property.Number(label="offset",configurable = True, default_value = 0, description="Sensor Offset (Default is 0)"),
              Property.Select(label="Interval", options=[1,5,10,30,60], description="Interval in Seconds"),
              Property.Kettle(label="Kettle", description="Reduced logging if Kettle is inactive (only Kettle or Fermenter to be selected)"),
              Property.Fermenter(label="Fermenter", description="Reduced logging in seconds if Fermenter is inactive (only Kettle or Fermenter to be selected)"),
-             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default: 60 sec | disabled: 0)")
+             Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default is 60 sec)")
              ])
 class OneWire(CBPiSensor):
     
     def __init__(self, cbpi, id, props):
         super(OneWire, self).__init__(cbpi, id, props)
         self.value = 200
 
     async def start(self):
         await super().start()
         self.name = self.props.get("Sensor")
         self.interval = int(self.props.get("Interval", 60))
         self.offset = float(self.props.get("offset",0))
 
         self.reducedfrequency=float(self.props.get("ReducedLogging", 60))
-        if self.reducedfrequency < 0:
-            self.reducedfrequency = 0
         self.lastlog=0
         self.sensor=self.get_sensor(self.id)       
         self.kettleid=self.props.get("Kettle", None)
         self.fermenterid=self.props.get("Fermenter", None)
         self.reducedlogging=True if self.kettleid or self.fermenterid else False
 
         if self.kettleid is not None and self.fermenterid is not None:
             self.reducedlogging=False
             self.cbpi.notify("OneWire Sensor", "Sensor '" + str(self.sensor.name) + "' cant't have Fermenter and Kettle defined for reduced logging.", NotificationType.WARNING, action=[NotificationAction("OK", self.Confirm)])
-        if (self.reducedfrequency != 0) and (self.interval >= self.reducedfrequency):
+        if self.interval >= self.reducedfrequency:
             self.reducedlogging=False
             self.cbpi.notify("OneWire Sensor", "Sensor '" + str(self.sensor.name) + "' has shorter or equal 'reduced logging' compared to regular interval.", NotificationType.WARNING, action=[NotificationAction("OK", self.Confirm)])
 
         self.t = ReadThread(self.name)
         self.t.daemon = True
         def shutdown():
             shutdown.cb.shutdown()
@@ -132,38 +130,36 @@
                 kettlestatus=False
             if kettlestatus:
                 self.log_data(self.value)
                 logging.info("OneWire {} Kettle Active".format(self.sensor.name))
                 self.lastlog = time.time()
             else:
                 logging.info("OneWire {} Kettle Inactive".format(self.sensor.name))
-                if self.reducedfrequency != 0:
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass   
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass   
 
         if self.fermenter is not None:
             try:
                 fermenterstatus=self.fermenter.instance.state
             except:
                 fermenterstatus=False
             if fermenterstatus:
                 self.log_data(self.value)
                 logging.info("OneWire {} Fermenter Active".format(self.sensor.name))
                 self.lastlog = time.time()
             else:
                 logging.info("OneWire {} Fermenter Inactive".format(self.sensor.name))
-                if self.reducedfrequency != 0:                    
-                    if now >= self.lastlog + self.reducedfrequency:
-                        self.log_data(self.value)
-                        self.lastlog = time.time()
-                        logging.info("Logged with reduced freqency")
-                        pass            
+                if now >= self.lastlog + self.reducedfrequency:
+                    self.log_data(self.value)
+                    self.lastlog = time.time()
+                    logging.info("Logged with reduced freqency")
+                    pass            
 
     
     def get_state(self):
         return dict(value=self.value)
 
 
 def setup(cbpi):
```

### Comparing `cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 27 17:54:22 2023 UTC, .py size: 7069 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4ed8 2164 9d1b 0000  a.......N.!d....
+00000000: 610d 0d0a 0000 0000 bef5 1e64 631b 0000  a..........dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 5400 6400 6401 6c05 5a05 6400 6401 6c06  T.d.d.l.Z.d.d.l.
 00000060: 5a06 6400 6401 6c07 5a07 6400 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
@@ -276,104 +276,103 @@
 00001130: da07 6173 796e 6369 6f72 2b00 0000 7251  ..asyncior+...rQ
 00001140: 0000 0072 1b00 0000 720f 0000 0072 0f00  ...r....r....r..
 00001150: 0000 7210 0000 0072 2e00 0000 6700 0000  ..r....r....g...
 00001160: 731c 0000 0000 021c 011c 020a 010e 010a  s...............
 00001170: 0118 021e 010c 0106 0110 0214 010c 010a  ................
 00001180: 017a 0b4f 6e65 5769 7265 2e72 756e 6301  .z.OneWire.runc.
 00001190: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-000011a0: 0000 00c3 0000 0073 6c01 0000 7c00 6a00  .......sl...|.j.
-000011b0: 6401 6b02 720a 7401 a001 a100 7d01 7402  d.k.r.t.....}.t.
-000011c0: a003 6402 a004 7c00 6a05 6a06 a101 a101  ..d...|.j.j.....
-000011d0: 0100 7c00 6a07 6400 7501 72c4 7a0e 7c00  ..|.j.d.u.r.z.|.
-000011e0: 6a07 6a08 6a09 7d02 5700 6e10 0100 0100  j.j.j.}.W.n.....
-000011f0: 0100 6403 7d02 5900 6e02 3000 7c02 7280  ..d.}.Y.n.0.|.r.
-00001200: 7c00 a00a 7c00 6a0b a101 0100 7402 a003  |...|.j.....t...
-00001210: 6404 a004 7c00 6a05 6a06 a101 a101 0100  d...|.j.j.......
-00001220: 7401 a001 a100 7c00 5f0c 6e44 7402 a003  t.....|._.nDt...
-00001230: 6405 a004 7c00 6a05 6a06 a101 a101 0100  d...|.j.j.......
-00001240: 7c01 7c00 6a0c 7c00 6a00 1700 6b05 72c4  |.|.j.|.j...k.r.
-00001250: 7c00 a00a 7c00 6a0b a101 0100 7401 a001  |...|.j.....t...
-00001260: a100 7c00 5f0c 7402 a003 6406 a101 0100  ..|._.t...d.....
-00001270: 7c00 6a0d 6400 7501 9001 7268 7a0e 7c00  |.j.d.u...rhz.|.
-00001280: 6a0d 6a08 6a09 7d03 5700 6e10 0100 0100  j.j.j.}.W.n.....
-00001290: 0100 6403 7d03 5900 6e02 3000 7c03 9001  ..d.}.Y.n.0.|...
-000012a0: 7222 7c00 a00a 7c00 6a0b a101 0100 7402  r"|...|.j.....t.
-000012b0: a003 6407 a004 7c00 6a05 6a06 a101 a101  ..d...|.j.j.....
-000012c0: 0100 7401 a001 a100 7c00 5f0c 6e46 7402  ..t.....|._.nFt.
-000012d0: a003 6408 a004 7c00 6a05 6a06 a101 a101  ..d...|.j.j.....
-000012e0: 0100 7c01 7c00 6a0c 7c00 6a00 1700 6b05  ..|.|.j.|.j...k.
-000012f0: 9001 7268 7c00 a00a 7c00 6a0b a101 0100  ..rh|...|.j.....
-00001300: 7401 a001 a100 7c00 5f0c 7402 a003 6406  t.....|._.t...d.
-00001310: a101 0100 6400 5300 2909 4e72 0100 0000  ....d.S.).Nr....
-00001320: 7a1d 4f6e 6557 6972 6520 7b7d 206c 6f67  z.OneWire {} log
-00001330: 6769 6e67 2073 7562 726f 7574 696e 6546  ging subroutineF
-00001340: 7a18 4f6e 6557 6972 6520 7b7d 204b 6574  z.OneWire {} Ket
-00001350: 746c 6520 4163 7469 7665 7a1a 4f6e 6557  tle Activez.OneW
-00001360: 6972 6520 7b7d 204b 6574 746c 6520 496e  ire {} Kettle In
-00001370: 6163 7469 7665 7a1c 4c6f 6767 6564 2077  activez.Logged w
-00001380: 6974 6820 7265 6475 6365 6420 6672 6571  ith reduced freq
-00001390: 656e 6379 7a1b 4f6e 6557 6972 6520 7b7d  encyz.OneWire {}
-000013a0: 2046 6572 6d65 6e74 6572 2041 6374 6976   Fermenter Activ
-000013b0: 657a 1d4f 6e65 5769 7265 207b 7d20 4665  ez.OneWire {} Fe
-000013c0: 726d 656e 7465 7220 496e 6163 7469 7665  rmenter Inactive
-000013d0: 290e 7252 0000 0072 2a00 0000 726d 0000  ).rR...r*...rm..
-000013e0: 0072 6e00 0000 726f 0000 0072 5500 0000  .rn...ro...rU...
-000013f0: 724f 0000 0072 6600 0000 da08 696e 7374  rO...rf.....inst
-00001400: 616e 6365 da05 7374 6174 6572 7000 0000  ance..staterp...
-00001410: 7216 0000 0072 5300 0000 7268 0000 0029  r....rS...rh...)
-00001420: 0472 1900 0000 da03 6e6f 77da 0c6b 6574  .r......now..ket
-00001430: 746c 6573 7461 7475 73da 0f66 6572 6d65  tlestatus..ferme
-00001440: 6e74 6572 7374 6174 7573 720f 0000 0072  nterstatusr....r
-00001450: 0f00 0000 7210 0000 0072 6c00 0000 7b00  ....r....rl...{.
-00001460: 0000 7340 0000 0000 010a 0208 0114 010a  ..s@............
-00001470: 0102 010e 0106 010a 0104 010c 0114 010c  ................
-00001480: 0214 0110 010c 010a 010a 030c 0102 010e  ................
-00001490: 0106 010a 0106 010c 0114 010c 0214 0112  ................
-000014a0: 010c 010a 010a 017a 104f 6e65 5769 7265  .......z.OneWire
-000014b0: 2e6c 6f67 7661 6c75 6563 0100 0000 0000  .logvaluec......
-000014c0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000014d0: 0000 730c 0000 0074 007c 006a 0164 018d  ..s....t.|.j.d..
-000014e0: 0153 0029 024e 2901 7216 0000 0029 02da  .S.).N).r....)..
-000014f0: 0464 6963 7472 1600 0000 721b 0000 0072  .dictr....r....r
-00001500: 0f00 0000 720f 0000 0072 1000 0000 da09  ....r....r......
-00001510: 6765 745f 7374 6174 65a3 0000 0073 0200  get_state....s..
-00001520: 0000 0001 7a11 4f6e 6557 6972 652e 6765  ....z.OneWire.ge
-00001530: 745f 7374 6174 6529 0b72 2f00 0000 7230  t_state).r/...r0
-00001540: 0000 0072 3100 0000 7215 0000 0072 4d00  ...r1...r....rM.
-00001550: 0000 725c 0000 0072 1e00 0000 722e 0000  ..r\...r....r...
-00001560: 0072 6c00 0000 7278 0000 00da 0d5f 5f63  .rl...rx.....__c
-00001570: 6c61 7373 6365 6c6c 5f5f 720f 0000 0072  lasscell__r....r
-00001580: 0f00 0000 7247 0000 0072 1000 0000 7241  ....rG...r....rA
-00001590: 0000 0034 0000 0073 0e00 0000 0809 0c04  ...4...s........
-000015a0: 0c1c 0803 0807 0814 0828 7241 0000 0063  .........(rA...c
-000015b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000015c0: 0a00 0000 4300 0000 7354 0000 007c 006a  ....C...sT...|.j
-000015d0: 00a0 0164 0174 02a1 0201 007a 1c74 0364  ...d.t.....z.t.d
-000015e0: 0264 0367 0283 0101 0074 0364 0264 0467  .d.g.....t.d.d.g
-000015f0: 0283 0101 0057 006e 2404 0074 0479 4e01  .....W.n$..t.yN.
-00001600: 007d 0101 007a 0c57 0059 0064 007d 017e  .}...z.W.Y.d.}.~
-00001610: 016e 0a64 007d 017e 0130 0030 0064 0053  .n.d.}.~.0.0.d.S
-00001620: 0029 054e 7241 0000 00da 086d 6f64 7072  .).NrA.....modpr
-00001630: 6f62 657a 0777 312d 6770 696f 7a08 7731  obez.w1-gpioz.w1
-00001640: 2d74 6865 726d 2905 da06 706c 7567 696e  -therm)...plugin
-00001650: da08 7265 6769 7374 6572 7241 0000 0072  ..registerrA...r
-00001660: 0400 0000 da09 4578 6365 7074 696f 6e29  ......Exception)
-00001670: 0272 4400 0000 da01 6572 0f00 0000 720f  .rD.....er....r.
-00001680: 0000 0072 1000 0000 da05 7365 7475 70a7  ...r......setup.
-00001690: 0000 0073 0c00 0000 0001 0e01 0202 0c01  ...s............
-000016a0: 1001 0e01 727f 0000 0029 1972 7100 0000  ....r....).rq...
-000016b0: 726d 0000 00da 0761 696f 6874 7470 7202  rm.....aiohttpr.
-000016c0: 0000 005a 0863 6270 692e 6170 6972 0900  ...Z.cbpi.apir..
-000016d0: 0000 7213 0000 0072 2a00 0000 da0a 7375  ..r....r*.....su
-000016e0: 6270 726f 6365 7373 7204 0000 00da 1463  bprocessr......c
-000016f0: 6270 692e 6170 692e 6461 7461 636c 6173  bpi.api.dataclas
-00001700: 7365 7372 0500 0000 7206 0000 0072 1100  sesr....r....r..
-00001710: 0000 7214 0000 0072 1200 0000 da0a 7061  ..r....r......pa
-00001720: 7261 6d65 7465 7273 da08 5072 6f70 6572  rameters..Proper
-00001730: 7479 da06 5365 6c65 6374 da06 4e75 6d62  ty..Select..Numb
-00001740: 6572 723e 0000 0072 3f00 0000 da0a 4342  err>...r?.....CB
-00001750: 5069 5365 6e73 6f72 7241 0000 0072 7f00  PiSensorrA...r..
-00001760: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00001770: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001780: 0200 0000 7322 0000 0008 0108 010c 0108  ....s"..........
-00001790: 0118 010c 0110 0208 0b12 1f10 0110 0112  ................
-000017a0: 010c 010c 010e fb04 0712 6c              ..........l
+000011a0: 0000 00c3 0000 0073 6201 0000 7400 a000  .......sb...t...
+000011b0: a100 7d01 7401 a002 6401 a003 7c00 6a04  ..}.t...d...|.j.
+000011c0: 6a05 a101 a101 0100 7c00 6a06 6400 7501  j.......|.j.d.u.
+000011d0: 72ba 7a0e 7c00 6a06 6a07 6a08 7d02 5700  r.z.|.j.j.j.}.W.
+000011e0: 6e10 0100 0100 0100 6402 7d02 5900 6e02  n.......d.}.Y.n.
+000011f0: 3000 7c02 7276 7c00 a009 7c00 6a0a a101  0.|.rv|...|.j...
+00001200: 0100 7401 a002 6403 a003 7c00 6a04 6a05  ..t...d...|.j.j.
+00001210: a101 a101 0100 7400 a000 a100 7c00 5f0b  ......t.....|._.
+00001220: 6e44 7401 a002 6404 a003 7c00 6a04 6a05  nDt...d...|.j.j.
+00001230: a101 a101 0100 7c01 7c00 6a0b 7c00 6a0c  ......|.|.j.|.j.
+00001240: 1700 6b05 72ba 7c00 a009 7c00 6a0a a101  ..k.r.|...|.j...
+00001250: 0100 7400 a000 a100 7c00 5f0b 7401 a002  ..t.....|._.t...
+00001260: 6405 a101 0100 7c00 6a0d 6400 7501 9001  d.....|.j.d.u...
+00001270: 725e 7a0e 7c00 6a0d 6a07 6a08 7d03 5700  r^z.|.j.j.j.}.W.
+00001280: 6e10 0100 0100 0100 6402 7d03 5900 6e02  n.......d.}.Y.n.
+00001290: 3000 7c03 9001 7218 7c00 a009 7c00 6a0a  0.|...r.|...|.j.
+000012a0: a101 0100 7401 a002 6406 a003 7c00 6a04  ....t...d...|.j.
+000012b0: 6a05 a101 a101 0100 7400 a000 a100 7c00  j.......t.....|.
+000012c0: 5f0b 6e46 7401 a002 6407 a003 7c00 6a04  _.nFt...d...|.j.
+000012d0: 6a05 a101 a101 0100 7c01 7c00 6a0b 7c00  j.......|.|.j.|.
+000012e0: 6a0c 1700 6b05 9001 725e 7c00 a009 7c00  j...k...r^|...|.
+000012f0: 6a0a a101 0100 7400 a000 a100 7c00 5f0b  j.....t.....|._.
+00001300: 7401 a002 6405 a101 0100 6400 5300 2908  t...d.....d.S.).
+00001310: 4e7a 1d4f 6e65 5769 7265 207b 7d20 6c6f  Nz.OneWire {} lo
+00001320: 6767 696e 6720 7375 6272 6f75 7469 6e65  gging subroutine
+00001330: 467a 184f 6e65 5769 7265 207b 7d20 4b65  Fz.OneWire {} Ke
+00001340: 7474 6c65 2041 6374 6976 657a 1a4f 6e65  ttle Activez.One
+00001350: 5769 7265 207b 7d20 4b65 7474 6c65 2049  Wire {} Kettle I
+00001360: 6e61 6374 6976 657a 1c4c 6f67 6765 6420  nactivez.Logged 
+00001370: 7769 7468 2072 6564 7563 6564 2066 7265  with reduced fre
+00001380: 7165 6e63 797a 1b4f 6e65 5769 7265 207b  qencyz.OneWire {
+00001390: 7d20 4665 726d 656e 7465 7220 4163 7469  } Fermenter Acti
+000013a0: 7665 7a1d 4f6e 6557 6972 6520 7b7d 2046  vez.OneWire {} F
+000013b0: 6572 6d65 6e74 6572 2049 6e61 6374 6976  ermenter Inactiv
+000013c0: 6529 0e72 2a00 0000 726d 0000 0072 6e00  e).r*...rm...rn.
+000013d0: 0000 726f 0000 0072 5500 0000 724f 0000  ..ro...rU...rO..
+000013e0: 0072 6600 0000 da08 696e 7374 616e 6365  .rf.....instance
+000013f0: da05 7374 6174 6572 7000 0000 7216 0000  ..staterp...r...
+00001400: 0072 5300 0000 7252 0000 0072 6800 0000  .rS...rR...rh...
+00001410: 2904 7219 0000 00da 036e 6f77 da0c 6b65  ).r......now..ke
+00001420: 7474 6c65 7374 6174 7573 da0f 6665 726d  ttlestatus..ferm
+00001430: 656e 7465 7273 7461 7475 7372 0f00 0000  enterstatusr....
+00001440: 720f 0000 0072 1000 0000 726c 0000 007b  r....r....rl...{
+00001450: 0000 0073 3e00 0000 0001 0801 1401 0a01  ...s>...........
+00001460: 0201 0e01 0601 0a01 0401 0c01 1401 0c02  ................
+00001470: 1401 1001 0c01 0a01 0a03 0c01 0201 0e01  ................
+00001480: 0601 0a01 0601 0c01 1401 0c02 1401 1201  ................
+00001490: 0c01 0a01 0a01 7a10 4f6e 6557 6972 652e  ......z.OneWire.
+000014a0: 6c6f 6776 616c 7565 6301 0000 0000 0000  logvaluec.......
+000014b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000014c0: 0073 0c00 0000 7400 7c00 6a01 6401 8d01  .s....t.|.j.d...
+000014d0: 5300 2902 4e29 0172 1600 0000 2902 da04  S.).N).r....)...
+000014e0: 6469 6374 7216 0000 0072 1b00 0000 720f  dictr....r....r.
+000014f0: 0000 0072 0f00 0000 7210 0000 00da 0967  ...r....r......g
+00001500: 6574 5f73 7461 7465 a100 0000 7302 0000  et_state....s...
+00001510: 0000 017a 114f 6e65 5769 7265 2e67 6574  ...z.OneWire.get
+00001520: 5f73 7461 7465 290b 722f 0000 0072 3000  _state).r/...r0.
+00001530: 0000 7231 0000 0072 1500 0000 724d 0000  ..r1...r....rM..
+00001540: 0072 5c00 0000 721e 0000 0072 2e00 0000  .r\...r....r....
+00001550: 726c 0000 0072 7800 0000 da0d 5f5f 636c  rl...rx.....__cl
+00001560: 6173 7363 656c 6c5f 5f72 0f00 0000 720f  asscell__r....r.
+00001570: 0000 0072 4700 0000 7210 0000 0072 4100  ...rG...r....rA.
+00001580: 0000 3400 0000 730e 0000 0008 090c 040c  ..4...s.........
+00001590: 1c08 0308 0708 1408 2672 4100 0000 6301  ........&rA...c.
+000015a0: 0000 0000 0000 0000 0000 0002 0000 000a  ................
+000015b0: 0000 0043 0000 0073 5400 0000 7c00 6a00  ...C...sT...|.j.
+000015c0: a001 6401 7402 a102 0100 7a1c 7403 6402  ..d.t.....z.t.d.
+000015d0: 6403 6702 8301 0100 7403 6402 6404 6702  d.g.....t.d.d.g.
+000015e0: 8301 0100 5700 6e24 0400 7404 794e 0100  ....W.n$..t.yN..
+000015f0: 7d01 0100 7a0c 5700 5900 6400 7d01 7e01  }...z.W.Y.d.}.~.
+00001600: 6e0a 6400 7d01 7e01 3000 3000 6400 5300  n.d.}.~.0.0.d.S.
+00001610: 2905 4e72 4100 0000 da08 6d6f 6470 726f  ).NrA.....modpro
+00001620: 6265 7a07 7731 2d67 7069 6f7a 0877 312d  bez.w1-gpioz.w1-
+00001630: 7468 6572 6d29 05da 0670 6c75 6769 6eda  therm)...plugin.
+00001640: 0872 6567 6973 7465 7272 4100 0000 7204  .registerrA...r.
+00001650: 0000 00da 0945 7863 6570 7469 6f6e 2902  .....Exception).
+00001660: 7244 0000 00da 0165 720f 0000 0072 0f00  rD.....er....r..
+00001670: 0000 7210 0000 00da 0573 6574 7570 a500  ..r......setup..
+00001680: 0000 730c 0000 0000 010e 0102 020c 0110  ..s.............
+00001690: 010e 0172 7f00 0000 2919 7271 0000 0072  ...r....).rq...r
+000016a0: 6d00 0000 da07 6169 6f68 7474 7072 0200  m.....aiohttpr..
+000016b0: 0000 5a08 6362 7069 2e61 7069 7209 0000  ..Z.cbpi.apir...
+000016c0: 0072 1300 0000 722a 0000 00da 0a73 7562  .r....r*.....sub
+000016d0: 7072 6f63 6573 7372 0400 0000 da14 6362  processr......cb
+000016e0: 7069 2e61 7069 2e64 6174 6163 6c61 7373  pi.api.dataclass
+000016f0: 6573 7205 0000 0072 0600 0000 7211 0000  esr....r....r...
+00001700: 0072 1400 0000 7212 0000 00da 0a70 6172  .r....r......par
+00001710: 616d 6574 6572 73da 0850 726f 7065 7274  ameters..Propert
+00001720: 79da 0653 656c 6563 74da 064e 756d 6265  y..Select..Numbe
+00001730: 7272 3e00 0000 723f 0000 00da 0a43 4250  rr>...r?.....CBP
+00001740: 6953 656e 736f 7272 4100 0000 727f 0000  iSensorrA...r...
+00001750: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00001760: 7210 0000 00da 083c 6d6f 6475 6c65 3e02  r......<module>.
+00001770: 0000 0073 2200 0000 0801 0801 0c01 0801  ...s"...........
+00001780: 1801 0c01 1002 080b 121f 1001 1001 1201  ................
+00001790: 0c01 0c01 0efb 0407 126a                 .........j
```

### Comparing `cbpi4-4.1.7/cbpi/extension/timer/__init__.py` & `cbpi4-4.1.7rc1/cbpi/extension/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.1.7rc1/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_actor.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_config.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_config.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_dashboard.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_dashboard.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_fermentation.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_fermentation.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_fermenterrecipe.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_fermenterrecipe.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_kettle.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_kettle.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_log.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_log.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_login.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_login.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_notification.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_notification.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_plugin.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_plugin.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_recipe.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_recipe.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_sensor.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_step.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_system.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_system.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/http_endpoints/http_upload.py` & `cbpi4-4.1.7rc1/cbpi/http_endpoints/http_upload.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/job/__init__.py` & `cbpi4-4.1.7rc1/cbpi/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/job/_job.py` & `cbpi4-4.1.7rc1/cbpi/job/_job.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/job/_scheduler.py` & `cbpi4-4.1.7rc1/cbpi/job/_scheduler.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/job/aiohttp.py` & `cbpi4-4.1.7rc1/cbpi/job/aiohttp.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/satellite.py` & `cbpi4-4.1.7rc1/cbpi/satellite.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/beer_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/beer_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/calculator_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/calculator_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/cbpi_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/cbpi_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/control_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/control_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/glass_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/glass_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/grain.svg` & `cbpi4-4.1.7rc1/cbpi/static/grain.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/hops_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/hops_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/kettle2_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/kettle2_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/led.svg` & `cbpi4-4.1.7rc1/cbpi/static/led.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/liquid_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/liquid_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/paddle_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/paddle_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/pipe_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/pipe_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/sensor_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/sensor_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/splash.png` & `cbpi4-4.1.7rc1/cbpi/static/splash.png`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/svg_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/svg_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/tank_icon.svg` & `cbpi4-4.1.7rc1/cbpi/static/tank_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/target_temp.svg` & `cbpi4-4.1.7rc1/cbpi/static/target_temp.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/thermomenter.svg` & `cbpi4-4.1.7rc1/cbpi/static/thermomenter.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/static/yeast.svg` & `cbpi4-4.1.7rc1/cbpi/static/yeast.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/utils/encoder.py` & `cbpi4-4.1.7rc1/cbpi/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi/websocket.py` & `cbpi4-4.1.7rc1/cbpi/websocket.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/cbpi4.egg-info/PKG-INFO` & `cbpi4-4.1.7rc1/cbpi4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4
-Version: 4.1.7
+Version: 4.1.7rc1
 Summary: CraftBeerPi4 Brewing Software
 Home-page: http://web.craftbeerpi.com
 Author: Manuel Fritsch / Alexander Vollkopf
 Author-email: manuel@craftbeerpi.com
 License: GPLv3
 Project-URL: Documentation, https://openbrewing.gitbook.io/craftbeerpi4_support/
 Platform: UNKNOWN
```

### Comparing `cbpi4-4.1.7/cbpi4.egg-info/SOURCES.txt` & `cbpi4-4.1.7rc1/cbpi4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/setup.py` & `cbpi4-4.1.7rc1/setup.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/cbpi_config_fixture.py` & `cbpi4-4.1.7rc1/tests/cbpi_config_fixture.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_actor.py` & `cbpi4-4.1.7rc1/tests/test_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_config.py` & `cbpi4-4.1.7rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_dashboard.py` & `cbpi4-4.1.7rc1/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_gpio.py` & `cbpi4-4.1.7rc1/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_index.py` & `cbpi4-4.1.7rc1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_kettle.py` & `cbpi4-4.1.7rc1/tests/test_kettle.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_logger.py` & `cbpi4-4.1.7rc1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_sensor.py` & `cbpi4-4.1.7rc1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_step.py` & `cbpi4-4.1.7rc1/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.1.7/tests/test_ws.py` & `cbpi4-4.1.7rc1/tests/test_ws.py`

 * *Files identical despite different names*

