# Comparing `tmp/torchqtm-0.0.3.tar.gz` & `tmp/torchqtm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchqtm-0.0.3.tar", last modified: Tue Jun  6 06:25:12 2023, max compression
+gzip compressed data, was "torchqtm-0.1.0.tar", last modified: Sat Jun 10 15:56:28 2023, max compression
```

## Comparing `torchqtm-0.0.3.tar` & `torchqtm-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,94 @@
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.032804 torchqtm-0.0.3/
--rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-05-21 08:16:14.000000 torchqtm-0.0.3/LICENSE
--rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:25:12.032622 torchqtm-0.0.3/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     1291 2023-06-03 06:24:39.000000 torchqtm-0.0.3/README.md
--rw-r--r--   0 nymath     (501) staff       (20)       38 2023-06-06 06:25:12.032863 torchqtm-0.0.3/setup.cfg
--rw-r--r--   0 nymath     (501) staff       (20)      952 2023-06-06 06:24:57.000000 torchqtm-0.0.3/setup.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.022024 torchqtm-0.0.3/test/
--rw-r--r--   0 nymath     (501) staff       (20)        2 2023-05-20 16:39:21.000000 torchqtm-0.0.3/test/test_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testfunc_.py
--rw-r--r--   0 nymath     (501) staff       (20)     1994 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testgplearn.py
--rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testop.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.023114 torchqtm-0.0.3/torchqtm/
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025032 torchqtm-0.0.3/torchqtm/_C/
--rw-r--r--   0 nymath     (501) staff       (20)   108922 2023-06-06 01:03:03.000000 torchqtm-0.0.3/torchqtm/_C/__init__.c
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/_C/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)   289042 2023-06-06 01:03:03.000000 torchqtm-0.0.3/torchqtm/_C/_functional.c
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 06:09:18.000000 torchqtm-0.0.3/torchqtm/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025508 torchqtm-0.0.3/torchqtm/autoalpha/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:33:58.000000 torchqtm-0.0.3/torchqtm/autoalpha/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025618 torchqtm-0.0.3/torchqtm/autoalpha/boost/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-21 03:29:04.000000 torchqtm-0.0.3/torchqtm/autoalpha/boost/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025730 torchqtm-0.0.3/torchqtm/autoalpha/cnn/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:35:23.000000 torchqtm-0.0.3/torchqtm/autoalpha/cnn/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.027849 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/
--rw-r--r--   0 nymath     (501) staff       (20)      218 2023-02-04 05:13:39.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/_program.py
--rw-r--r--   0 nymath     (501) staff       (20)     6595 2023-05-20 06:10:27.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/fitness.py
--rw-r--r--   0 nymath     (501) staff       (20)     7239 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/functions.py
--rw-r--r--   0 nymath     (501) staff       (20)    66949 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/genetic.py
--rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-02-04 05:13:39.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/utils.py
--rw-r--r--   0 nymath     (501) staff       (20)      119 2023-05-21 02:33:17.000000 torchqtm-0.0.3/torchqtm/config.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.028080 torchqtm-0.0.3/torchqtm/edbt/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-21 09:03:13.000000 torchqtm-0.0.3/torchqtm/edbt/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.029070 torchqtm-0.0.3/torchqtm/op/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-17 06:33:06.000000 torchqtm-0.0.3/torchqtm/op/CrossSectionalOperators.py
--rw-r--r--   0 nymath     (501) staff       (20)       20 2023-05-25 13:48:11.000000 torchqtm-0.0.3/torchqtm/op/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)       68 2023-05-26 11:03:24.000000 torchqtm-0.0.3/torchqtm/op/algos.py
--rw-r--r--   0 nymath     (501) staff       (20)     2136 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/op/base.py
--rw-r--r--   0 nymath     (501) staff       (20)     9803 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/op/functional.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.030247 torchqtm-0.0.3/torchqtm/option/
--rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/Option.py
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1640 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/functional.py
--rw-r--r--   0 nymath     (501) staff       (20)      586 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/option/main.py
--rw-r--r--   0 nymath     (501) staff       (20)      629 2023-06-06 03:21:03.000000 torchqtm-0.0.3/torchqtm/utils.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.031851 torchqtm-0.0.3/torchqtm/vbt/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:36:01.000000 torchqtm-0.0.3/torchqtm/vbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     7983 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/vbt/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/vbt/benchmark.py
--rw-r--r--   0 nymath     (501) staff       (20)      278 2023-05-25 11:20:21.000000 torchqtm-0.0.3/torchqtm/vbt/dataset.py
--rw-r--r--   0 nymath     (501) staff       (20)     2142 2023-05-25 14:46:07.000000 torchqtm-0.0.3/torchqtm/vbt/rebalance.py
--rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/vbt/stats.py
--rw-r--r--   0 nymath     (501) staff       (20)     1452 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/vbt/universe.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.032236 torchqtm-0.0.3/torchqtm/visualization/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:36:40.000000 torchqtm-0.0.3/torchqtm/visualization/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1803 2023-05-18 06:40:49.000000 torchqtm-0.0.3/torchqtm/visualization/visualization.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.023776 torchqtm-0.0.3/torchqtm.egg-info/
--rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     1205 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/SOURCES.txt
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/dependency_links.txt
--rw-r--r--   0 nymath     (501) staff       (20)        9 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/top_level.txt
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.422512 torchqtm-0.1.0/
+-rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-05-21 08:16:14.000000 torchqtm-0.1.0/LICENSE
+-rw-r--r--   0 nymath     (501) staff       (20)     2886 2023-06-10 15:56:28.422322 torchqtm-0.1.0/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     2431 2023-06-10 15:47:20.000000 torchqtm-0.1.0/README.md
+-rw-r--r--   0 nymath     (501) staff       (20)       38 2023-06-10 15:56:28.422610 torchqtm-0.1.0/setup.cfg
+-rw-r--r--   0 nymath     (501) staff       (20)     1312 2023-06-10 15:55:41.000000 torchqtm-0.1.0/setup.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.405187 torchqtm-0.1.0/test/
+-rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-10 15:47:20.000000 torchqtm-0.1.0/test/testFunctional.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-10 15:47:20.000000 torchqtm-0.1.0/test/testRolling.py
+-rw-r--r--   0 nymath     (501) staff       (20)        2 2023-05-20 16:39:21.000000 torchqtm-0.1.0/test/test_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testfunc_.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1994 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testgplearn.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testop.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.405685 torchqtm-0.1.0/torchqtm/
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.407438 torchqtm-0.1.0/torchqtm/_C/
+-rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/_C/__init__.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_C/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   289927 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/_C/_functional.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)  1199949 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm/_C/_rolling.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.408267 torchqtm-0.1.0/torchqtm/_libs/
+-rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.410413 torchqtm-0.1.0/torchqtm/_libs/tslibs/
+-rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/tslibs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.410678 torchqtm-0.1.0/torchqtm/_libs/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/window/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.411714 torchqtm-0.1.0/torchqtm/alphas/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    21667 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/alpha101.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/alphas.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/chatgpt.py
+-rw-r--r--   0 nymath     (501) staff       (20)      699 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/ml.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.411924 torchqtm-0.1.0/torchqtm/autoalpha/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.412028 torchqtm-0.1.0/torchqtm/autoalpha/boost/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/boost/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.412128 torchqtm-0.1.0/torchqtm/autoalpha/cnn/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/cnn/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.413639 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/
+-rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/_program.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6595 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/fitness.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7239 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/functions.py
+-rw-r--r--   0 nymath     (501) staff       (20)    66949 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/genetic.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6459 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/base.py
+-rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/config.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.413833 torchqtm-0.1.0/torchqtm/core/
+-rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-08 10:01:51.000000 torchqtm-0.1.0/torchqtm/core/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.414272 torchqtm-0.1.0/torchqtm/core/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 10:01:51.000000 torchqtm-0.1.0/torchqtm/core/window/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6829 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/core/window/rolling.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.415626 torchqtm-0.1.0/torchqtm/edbt/
+-rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2231 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/datahandler.py
+-rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/setup.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3706 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/test.py
+-rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/testsearch.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.416529 torchqtm-0.1.0/torchqtm/op/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/op/CrossSectionalOperators.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/_numba.py
+-rw-r--r--   0 nymath     (501) staff       (20)       68 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/op/algos.py
+-rw-r--r--   0 nymath     (501) staff       (20)    20222 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/functional.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.417792 torchqtm-0.1.0/torchqtm/option/
+-rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/Option.py
+-rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.418593 torchqtm-0.1.0/torchqtm/option/data/
+-rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/data/load_data.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/functional.py
+-rw-r--r--   0 nymath     (501) staff       (20)      586 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/main.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.419167 torchqtm-0.1.0/torchqtm/uniquant/
+-rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/uniquant/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.421404 torchqtm-0.1.0/torchqtm/utils/
+-rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/benchmark.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/rebalance.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/stats.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1452 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/universe.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/visualization.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/warnings.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.422007 torchqtm-0.1.0/torchqtm/vbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/vbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     5615 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/vbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/vbt/dataset.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.406458 torchqtm-0.1.0/torchqtm.egg-info/
+-rw-r--r--   0 nymath     (501) staff       (20)     2886 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     1895 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/SOURCES.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/dependency_links.txt
+-rw-r--r--   0 nymath     (501) staff       (20)       44 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/requires.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        9 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/top_level.txt
```

### Comparing `torchqtm-0.0.3/LICENSE` & `torchqtm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/PKG-INFO` & `torchqtm-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.0.3
+Version: 0.1.0
 Summary: None
 Home-page: https://github.com/nymath/torchquantum/tree/main
+Download-URL: https://github.com/nymath/torchquantum/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -22,51 +23,87 @@
 
 ## Contents
 
 - [Installation](#installation)
 - [Features](#features)
 - [Contribution](#contribution)
 
-
 ## Installation
+
 for Unix:
+
 ```shell
 cd /path/to/your/directory
 git clone git@github.com:nymath/torchquantum.git
 cd ./torchquantum
 ```
+
 Before running examples, you should compile the cython code.
+
 ```shell
 python setup.py build_ext --inplace
 ```
+
 Now you can run examples
+
 ```shell
 python ./examples/main.py
 ```
 
 If you are not downloading the dataset, then you should
+
 ```shell
 cd ./examples
 mkdir largedata
 cd ./largedata
 wget https://github.com/nymath/torchquantum/releases/download/V0.1/Stocks.pkl.zip
 unzip Stocks.pkl.zip
 rm Stocks.pkl.zip
 cd ../
 cd ../
 ```
 
+## Example
+
+You can easily create an alpha through torchquantum!
+
+```python
+import torchqtm.op as op
+import torchqtm.op.functional as F
+class NeutralizePE(op.Fundamental):
+    def __init__(self, env):
+        super().__init__(env)
+        self.lag = op.Parameter(5, required_optim=False, feasible_region=None)
+
+    def forward(self):
+        self.data = F.divide(1, self.env.PE)
+        self.data = F.winsorize(self.data, 'std', 4)
+        self.data = F.normalize(self.data)
+        self.data = F.group_neutralize(self.data, self.env.Sector)
+        self.data = F.regression_neut(self.data, self.env.MktVal)
+        self.data = F.ts_mean(self.data, self.lag)
+        return self.data
+```
+- `F` is library that contains the operators defined by WorldQuant.
+- `op.Fundamental` implies the NeutralizePE belongs to fundamental alpha.
+- `self.lag` is the parameter of rolling mean, which can be optimized through grid search.
+
+
 
 
 ## Features
 
-- High-speed backtesting framework.
+- High-speed backtesting framework (most of the operators are implemented through cython)
 - A revised gplearn library that is compatible with Alpha mining.
 - CNN and other state of the art models for mining alphas.
-- Event Driven backtesting framework will be available.
+- Event Driven backtesting framework is available.
 
 ## Contribution
 
 For more information, we refer to [Documentation](https://nymath.github.io/torchquantum/navigate).
 
 
+## Join us
+
+If you are interested in quantitative finance and are committed to devoting 
+your life to alpha mining, you can contact me through WeChat at Ny_math.
```

### Comparing `torchqtm-0.0.3/setup.py` & `torchqtm-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,49 @@
 from setuptools import find_packages
 from Cython.Build import cythonize
 import numpy
 import glob
 
 extensions = glob.glob("torchqtm/_C/*.pyx")
 
-setup(
-    ext_modules=cythonize(extensions),
-    include_dirs=[numpy.get_include()],
-    name="torchqtm",
-    version="0.0.3",
-    author="ny",
-    author_email="nymath@163.com",
-    description="None",
-    long_description=open('README.md', 'r').read(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/nymath/torchquantum/tree/main",
-    packages=find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: Unix",
-    ],
-    python_requires='>=3.6',
-)
+install_requires = [
+    'numpy',
+    'pandas',
+    'pandas_market_calendars',
+    'cython',
+]
 
 
+def main():
+    setup(
+        ext_modules=cythonize(extensions, language='c++'),
+        include_dirs=[numpy.get_include()],
+        name="torchqtm",
+        version="0.1.0",
+        author="ny",
+        author_email="nymath@163.com",
+        install_requires=install_requires,
+        description="None",
+        long_description=open('README.md', 'r').read(),
+        long_description_content_type="text/markdown",
+        url="https://github.com/nymath/torchquantum/tree/main",
+        download_url="https://github.com/nymath/torchquantum/releases/tag/",
+        packages=find_packages(),
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: Unix",
+        ],
+        python_requires='>=3.6',
+    )
+
+
+if __name__ == "__main__":
+    main()
+
 ## setup cython
 # python setup.py build_ext --inplace
 ## setup package
 # pip install twine
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 # twine upload --skip-existing dist/*
```

### Comparing `torchqtm-0.0.3/test/testgplearn.py` & `torchqtm-0.1.0/test/testgplearn.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/test/testop.py` & `torchqtm-0.1.0/test/testop.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/_C/__init__.c` & `torchqtm-0.1.0/torchqtm/_C/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
+        "language": "c++",
         "name": "torchqtm._C.__init__",
         "sources": [
             "torchqtm/_C/__init__.pyx"
         ]
     },
     "module_name": "torchqtm._C.__init__"
 }
@@ -359,27 +360,41 @@
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
 
+#ifndef __cplusplus
+  #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
+#endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
-  #elif defined(__GNUC__)
-    #define CYTHON_INLINE __inline__
-  #elif defined(_MSC_VER)
-    #define CYTHON_INLINE __inline
-  #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
-    #define CYTHON_INLINE inline
   #else
-    #define CYTHON_INLINE
+    #define CYTHON_INLINE inline
   #endif
 #endif
+template<typename T>
+void __Pyx_call_destructor(T& x) {
+    x.~T();
+}
+template<typename T>
+class __Pyx_FakeReference {
+  public:
+    __Pyx_FakeReference() : ptr(NULL) { }
+    __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
+    T *operator->() { return ptr; }
+    T *operator&() { return ptr; }
+    operator T&() { return *ptr; }
+    template<typename U> bool operator ==(U other) { return *ptr == other; }
+    template<typename U> bool operator !=(U other) { return *ptr != other; }
+  private:
+    T *ptr;
+};
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
```

### Comparing `torchqtm-0.0.3/torchqtm/_C/_functional.c` & `torchqtm-0.1.0/torchqtm/_C/_functional.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
+        "language": "c++",
         "name": "torchqtm._C._functional",
         "sources": [
             "torchqtm/_C/_functional.pyx"
         ]
     },
     "module_name": "torchqtm._C._functional"
 }
@@ -360,27 +361,41 @@
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
 
+#ifndef __cplusplus
+  #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
+#endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
-  #elif defined(__GNUC__)
-    #define CYTHON_INLINE __inline__
-  #elif defined(_MSC_VER)
-    #define CYTHON_INLINE __inline
-  #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
-    #define CYTHON_INLINE inline
   #else
-    #define CYTHON_INLINE
+    #define CYTHON_INLINE inline
   #endif
 #endif
+template<typename T>
+void __Pyx_call_destructor(T& x) {
+    x.~T();
+}
+template<typename T>
+class __Pyx_FakeReference {
+  public:
+    __Pyx_FakeReference() : ptr(NULL) { }
+    __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
+    T *operator->() { return ptr; }
+    T *operator&() { return ptr; }
+    operator T&() { return *ptr; }
+    template<typename U> bool operator ==(U other) { return *ptr == other; }
+    template<typename U> bool operator !=(U other) { return *ptr != other; }
+  private:
+    T *ptr;
+};
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
@@ -3024,15 +3039,15 @@
     }
 
     /* "torchqtm/_C/_functional.pyx":56
  *             return _regression_neuts(Y, others)
  *         else:
  *             pass             # <<<<<<<<<<<<<<
  * 
- * 
+ * # roll_apply.pyx
  */
     /*else*/ {
     }
   }
 
   /* "torchqtm/_C/_functional.pyx":48
  * @cython.wraparound(False)
@@ -4696,14 +4711,26 @@
  *     if not isinstance(others, list):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_11_functional_5regression_neut, NULL, __pyx_n_s_torchqtm__C__functional); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_regression_neut_2, __pyx_t_1) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+  /* "torchqtm/_C/_functional.pyx":60
+ * # roll_apply.pyx
+ * cimport cython
+ * import numpy as np             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
   /* "torchqtm/_C/_functional.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # https://cython.readthedocs.io/en/stable/src/userguide/numpy_tutorial.html
  * cimport numpy
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
```

### Comparing `torchqtm-0.0.3/torchqtm/autoalpha/gplearn/_program.py` & `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/_program.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/autoalpha/gplearn/fitness.py` & `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/fitness.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/autoalpha/gplearn/functions.py` & `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/functions.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/autoalpha/gplearn/genetic.py` & `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/genetic.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/autoalpha/gplearn/utils.py` & `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/option/main.py` & `torchqtm-0.1.0/torchqtm/option/main.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/utils.py` & `torchqtm-0.1.0/torchqtm/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,8 @@
         self.start = None
 
     def __enter__(self):
         self.start = time.time()
         return self
 
     def __exit__(self, exc_type, exc_value, trace):
-        print("{}: {:.4f}ms".format(self.program, 1000*(time.time() - self.start)))
-
-
+        print("{}: {:.4f}ms".format(self.program, 1000*(time.time() - self.start)))
```

### Comparing `torchqtm-0.0.3/torchqtm/vbt/benchmark.py` & `torchqtm-0.1.0/torchqtm/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/vbt/rebalance.py` & `torchqtm-0.1.0/torchqtm/utils/rebalance.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,30 @@
     def create_weekly_groups(self):
         rlt = defaultdict(list)
         for key, value in zip(self.trade_dates, [(x.year, x.week) for x in self.trade_dates]):
             rlt[value].append(key)
         return rlt
 
 
+class Daily(object):
+    def __init__(self, start_date, end_date):
+        self.start_date = start_date
+        self.end_date = end_date
+        self.rebalance_dates = None
+        self._create_trade_dates()
+
+    def _create_trade_dates(self):
+        calendar = Calendar(self.start_date, self.end_date)
+        self.rebalance_dates = calendar.trade_dates
+
+    @property
+    def data(self):
+        return self.rebalance_dates
+
+
 class Weekly(object):
     def __init__(self, start_date, end_date, days: Iterable[int]):
         self.start_date = start_date
         self.end_date = end_date
         self.days = days
         self.rebalance_dates = None
         self._create_trade_dates()
```

### Comparing `torchqtm-0.0.3/torchqtm/vbt/stats.py` & `torchqtm-0.1.0/torchqtm/utils/stats.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/vbt/universe.py` & `torchqtm-0.1.0/torchqtm/utils/universe.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.3/torchqtm/visualization/visualization.py` & `torchqtm-0.1.0/torchqtm/utils/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,22 @@
         ax.set_yticks([])
         plt.show()
 
 
 class ColorGenerator:
     def __init__(self, n_groups):
         self.n_groups = n_groups
-
-    def __call__(self):
         cmap = plt.get_cmap('coolwarm')
         colors = [cmap(i) for i in np.linspace(0, 1, self.n_groups)]
-        return [mcolors.rgb2hex(color) for color in colors]
+        self.data = [mcolors.rgb2hex(color) for color in colors]
+
+    def __call__(self):
+        return self.data
 
 
-colors = ['#ADD8E6', '#90EE90', '#FFFF00', '#FFA500', '#8B0000']
+# colors = ['#ADD8E6', '#90EE90', '#FFFF00', '#FFA500', '#8B0000']
 
 
 # if __name__ == "__main__":
 #     # gradient_color = GradientColor("tab:green", "tab:red", 5)
 #     # gradient_color.print_hex_colors()
 #     # gradient_color.plot_colors()
```

### Comparing `torchqtm-0.0.3/torchqtm.egg-info/PKG-INFO` & `torchqtm-0.1.0/torchqtm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.0.3
+Version: 0.1.0
 Summary: None
 Home-page: https://github.com/nymath/torchquantum/tree/main
+Download-URL: https://github.com/nymath/torchquantum/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -22,51 +23,87 @@
 
 ## Contents
 
 - [Installation](#installation)
 - [Features](#features)
 - [Contribution](#contribution)
 
-
 ## Installation
+
 for Unix:
+
 ```shell
 cd /path/to/your/directory
 git clone git@github.com:nymath/torchquantum.git
 cd ./torchquantum
 ```
+
 Before running examples, you should compile the cython code.
+
 ```shell
 python setup.py build_ext --inplace
 ```
+
 Now you can run examples
+
 ```shell
 python ./examples/main.py
 ```
 
 If you are not downloading the dataset, then you should
+
 ```shell
 cd ./examples
 mkdir largedata
 cd ./largedata
 wget https://github.com/nymath/torchquantum/releases/download/V0.1/Stocks.pkl.zip
 unzip Stocks.pkl.zip
 rm Stocks.pkl.zip
 cd ../
 cd ../
 ```
 
+## Example
+
+You can easily create an alpha through torchquantum!
+
+```python
+import torchqtm.op as op
+import torchqtm.op.functional as F
+class NeutralizePE(op.Fundamental):
+    def __init__(self, env):
+        super().__init__(env)
+        self.lag = op.Parameter(5, required_optim=False, feasible_region=None)
+
+    def forward(self):
+        self.data = F.divide(1, self.env.PE)
+        self.data = F.winsorize(self.data, 'std', 4)
+        self.data = F.normalize(self.data)
+        self.data = F.group_neutralize(self.data, self.env.Sector)
+        self.data = F.regression_neut(self.data, self.env.MktVal)
+        self.data = F.ts_mean(self.data, self.lag)
+        return self.data
+```
+- `F` is library that contains the operators defined by WorldQuant.
+- `op.Fundamental` implies the NeutralizePE belongs to fundamental alpha.
+- `self.lag` is the parameter of rolling mean, which can be optimized through grid search.
+
+
 
 
 ## Features
 
-- High-speed backtesting framework.
+- High-speed backtesting framework (most of the operators are implemented through cython)
 - A revised gplearn library that is compatible with Alpha mining.
 - CNN and other state of the art models for mining alphas.
-- Event Driven backtesting framework will be available.
+- Event Driven backtesting framework is available.
 
 ## Contribution
 
 For more information, we refer to [Documentation](https://nymath.github.io/torchquantum/navigate).
 
 
+## Join us
+
+If you are interested in quantitative finance and are committed to devoting 
+your life to alpha mining, you can contact me through WeChat at Ny_math.
```

