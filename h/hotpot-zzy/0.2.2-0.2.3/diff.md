# Comparing `tmp/hotpot-zzy-0.2.2.tar.gz` & `tmp/hotpot-zzy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-53s7j1d6/hotpot-zzy-0.2.2.tar", last modified: Thu Jun  8 01:49:14 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-nj6lpy9t/hotpot-zzy-0.2.3.tar", last modified: Sat Jun 10 07:50:00 2023, max compression
```

## Comparing `hotpot-zzy-0.2.2.tar` & `hotpot-zzy-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,121 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/PKG-INFO
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.2/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.2/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    14652 2023-06-06 11:58:39.000000 hotpot-zzy-0.2.2/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    88345 2023-06-08 01:37:04.000000 hotpot-zzy-0.2.2/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-06-06 06:50:07.000000 hotpot-zzy-0.2.2/hotpot/data/periodic_table.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tanks/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      365 2023-06-05 01:59:39.000000 hotpot-zzy-0.2.2/hotpot/tanks/cc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.2/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.2/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.2/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      813 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       26 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      263 2023-06-08 01:48:17.000000 hotpot-zzy-0.2.2/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/test/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/test/test_amorphous_maker.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.2/test/test_bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-06-08 01:38:26.000000 hotpot-zzy-0.2.2/test/test_chemif.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.595230 hotpot-zzy-0.2.3/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-10 07:50:00.595230 hotpot-zzy-0.2.3/PKG-INFO
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.563230 hotpot-zzy-0.2.3/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.3/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.3/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    14652 2023-06-06 11:58:39.000000 hotpot-zzy-0.2.3/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    93006 2023-06-10 07:41:56.000000 hotpot-zzy-0.2.3/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.563230 hotpot-zzy-0.2.3/hotpot/data/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.563230 hotpot-zzy-0.2.3/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.571230 hotpot-zzy-0.2.3/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.3/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.571230 hotpot-zzy-0.2.3/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-06-06 06:50:07.000000 hotpot-zzy-0.2.3/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.579230 hotpot-zzy-0.2.3/hotpot/data/solvents/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      973 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1068 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      783 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      780 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2586 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1447 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      970 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      780 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1731 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1558 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1,4-dioxane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1626 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1912 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1-pentanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1342 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2017 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1626 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1727 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1443 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2-methoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1636 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1760 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1920 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      670 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/DCM.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1335 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/DMF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1146 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/DMSO.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1638 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1756 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1455 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/THF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      963 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/acetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1149 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/acetone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      774 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/acetonitrile.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1364 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/benzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2104 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/butylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      687 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1370 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/chlorobenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      677 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/chloroform.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2218 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/cumene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/cyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1629 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/diethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2298 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/diisopropylamine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1054 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/ethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1250 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/ethyl_formate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1534 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/ethylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1156 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/ethyleneglycol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      771 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/formamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      678 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/formic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2384 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/heptane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2098 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/hexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2108 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/isobutyl_acetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2671 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/isooctane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1343 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/isopropanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1823 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/isopropylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2201 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/isopropylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/meta-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      770 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1751 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methoxybenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1250 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2014 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylbutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2229 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylcyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1444 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylethylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2017 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylisobutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1733 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/methylisopropylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1652 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/morpholine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      869 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/nitromethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1939 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/ortho-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/para-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1814 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/pentane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1820 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/propylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1270 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/pyridine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1651 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/sulfolane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1920 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/t-butylmethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2340 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/tetralin.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1649 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/toluene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      972 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      972 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      482 2022-11-18 20:33:01.000000 hotpot-zzy-0.2.3/hotpot/data/solvents/water.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.579230 hotpot-zzy-0.2.3/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      365 2023-06-05 01:59:39.000000 hotpot-zzy-0.2.3/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.3/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.579230 hotpot-zzy-0.2.3/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/hotpot/tanks/lmp/materials.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.3/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.3/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.579230 hotpot-zzy-0.2.3/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1723 2023-06-10 01:35:08.000000 hotpot-zzy-0.2.3/hotpot/utils/load_chem_lib.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.3/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.579230 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-10 07:50:00.000000 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3809 2023-06-10 07:50:00.000000 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-10 07:50:00.000000 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       26 2023-06-10 07:50:00.000000 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-10 07:50:00.000000 hotpot-zzy-0.2.3/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      263 2023-06-10 07:49:19.000000 hotpot-zzy-0.2.3/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-10 07:50:00.595230 hotpot-zzy-0.2.3/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-10 07:50:00.595230 hotpot-zzy-0.2.3/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/test/test_amorphous_maker.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.3/test/test_bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2291 2023-06-10 07:41:13.000000 hotpot-zzy-0.2.3/test/test_chemif.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.3/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.2.2/hotpot/_io.py` & `hotpot-zzy-0.2.3/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/bundle.py` & `hotpot-zzy-0.2.3/hotpot/bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/cheminfo.py` & `hotpot-zzy-0.2.3/hotpot/cheminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 import re
 from abc import ABC, abstractmethod
 from io import IOBase
 from os import PathLike
 from os.path import join as ptj
 from pathlib import Path
 from typing import *
+from itertools import product
 
 import numpy as np
 from openbabel import openbabel as ob, pybel as pb
 
 from hotpot import data_root
 from hotpot.tanks import lmp
 from hotpot.tanks.quantum import Gaussian
+from hotpot.utils.load_chem_lib import library as _lib  # The chemical library
 
 # Define Exceptions
 class OperateOBMolFail(BaseException):
     """ Raise for any fail that trys to operate the OBMol """
 class AddAtomFail(OperateOBMolFail):
     """ Raise when add an atom into Molecule fail """
 
@@ -103,17 +105,17 @@
         ('all_atom_charges', 'all_atom_spin_densities'),
         (),
         ('all_coordinates', 'all_forces')
     )
 
     def __init__(self, ob_mol: ob.OBMol = None, _data: dict = None, **kwargs):
         if _data:
-            self._data = _data
+            self._data: dict = _data
         else:
-            self._data = {
+            self._data: dict = {
                 'ob_mol': ob_mol if ob_mol else ob.OBMol()
             }
         self._set_attrs(**kwargs)
         self._load_atoms()
         self._load_bonds()
 
     def __repr__(self):
@@ -639,18 +641,18 @@
         # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
         success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
 
         if success:
             new_ob_bond_idx = [obb for obb in (ob.OBMolBondIter(self.ob_mol))][-1].GetIdx()
             bond = self._load_bonds()[new_ob_bond_idx]  # the new atoms should place in the terminal of the bond list
 
-        elif atoms[0] not in self.atom_indices:
+        elif atoms[0].ob_id not in self.atom_indices:
             raise KeyError("the start atom1 doesn't exist in molecule")
 
-        elif atoms[1] not in self.atom_indices:
+        elif atoms[1].ob_id not in self.atom_indices:
             raise KeyError("the end atom2 doesn't exist in molecule")
 
         else:
             raise RuntimeError('add bond not successful!')
 
         # Return the bond have add into the molecule
         return bond
@@ -690,64 +692,14 @@
     def all_energy(self):
         return self._data.get('all_energy')
 
     @property
     def angles(self):
         return [Angle(self, a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
 
-    def generate_metal_ligand_pair(
-            self, metal_symbol: str, acceptor_atoms: Sequence = ('O',), opti_force_field: str = 'UFF'
-    ) -> Generator['Molecule', None, None]:
-        """
-        This method could work if the molecule is an organic ligand, or raise AttributeError.
-        Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
-
-        Args:
-            metal_symbol: which metal element link to the ligand
-            acceptor_atoms: which elements to be acceptor atom to link to metal
-            opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
-
-        Return:
-            A generator for M-L pair
-
-        Raise:
-            AttributeError: if the molecule is not an organic ligand
-        """
-        if not self.is_organic:
-            raise AttributeError('the accepting molecule should be organic compound')
-
-        ligand = self.copy()
-        ligand.localed_optimize(opti_force_field)  # locally optimize the ligand
-        ligand.normalize_labels()
-
-        for atom in ligand.atoms:
-            if atom.symbol in acceptor_atoms:
-                acceptor_ligand = ligand.copy()
-
-                # assign the initial coordinates
-                # the sum of vector of relative position relate to the accepting atom
-                sum_relative_coordinates = sum([c for _, c in atom.neighbours_position])
-                metal_init_coordinates = atom.coordinates - sum_relative_coordinates
-
-                # add metal atom into the acceptor_ligand
-                added_metal = acceptor_ligand.add_atom(metal_symbol, coordinates=metal_init_coordinates)
-
-                # add the coordinating bond between metal atom and acceptor atoms
-                acceptor_ligand.add_bond(added_metal, atom.label, 1)
-
-                # remove redundant hydrogen
-                accepting_atom = acceptor_ligand.atom(atom.label)
-                while accepting_atom.valence > accepting_atom.valence_max and accepting_atom.neigh_hydrogens:
-                    acceptor_ligand.remove_atoms(accepting_atom.neigh_hydrogens[0])
-
-                # localize optimization of M-L pair by classical force field
-                acceptor_ligand.localed_optimize(opti_force_field)
-
-                yield acceptor_ligand
-
     def assign_bond_types(self):
         self.ob_mol.PerceiveBondOrders()
 
     def atom(self, id_label: Union[int, str]) -> 'Atom':
         """ get atom by label or idx """
         if not self.is_labels_unique:
             print(AttributeError('the molecule atoms labels are not unique!'))
@@ -855,15 +807,15 @@
     def bonds(self):
         bonds = self._load_bonds()
         return list(bonds.values())
 
     def build_bonds(self):
         self.ob_mol.ConnectTheDots()
 
-    def build_conformer(self, force_field: str = 'mmff94', steps: int = 50):
+    def build_conformer(self, force_field: str = 'UFF', steps: int = 50):
         """ build 3D coordinates for the molecule """
         pymol = pb.Molecule(self.ob_mol)
         pymol.make3D(force_field, steps)
 
     @property
     def center_of_masses(self):
         return (self.masses * self.coordinates.T).T.sum(axis=0) / self.masses.sum()
@@ -896,16 +848,41 @@
 
         if pop:
             return all_coordinates
 
     @property
     def components(self):
         """ get all fragments don't link each by any bonds """
+        if not self.has_3d:
+            self.build_conformer()
+
+        # split to fragment
         separated_obmol = self.ob_mol.Separate()
-        return [Molecule(obmol) for obmol in separated_obmol]
+        components = [Molecule(ob_mol) for ob_mol in separated_obmol]
+
+        # match parents_atoms to children atoms
+        atoms = self.atoms
+        parent_atoms_coordinates = [a.coordinates for a in atoms]
+        match_atoms: Dict[Atom, Atom] = \
+            {atoms[parent_atoms_coordinates.index(a.coordinates)]: a for c in components for a in c.atoms}
+
+        # transfer the parent atoms attribute to the children
+        for pa, ca in match_atoms.items():
+            ca_data = ca.copy_data()
+            pa_data = pa.copy_data()
+
+            # Remove the ob_atom and molecule information
+            pa_data.pop('ob_atom')
+            pa_data.pop('_mol')
+
+            ca_data.update(pa_data)
+
+            ca.replace_attr_data(ca_data)
+
+        return components
 
     @property
     def configure_number(self):
         all_coordinates = self._data.get('all_coordinates')
         if isinstance(all_coordinates, np.ndarray):
             return all_coordinates.shape[0]
         else:
@@ -1121,14 +1098,39 @@
          """
         if not feature_names:
             feature_names = ('atomic_orbital',)
 
         # Matrix with shape (atom_numbers, feature_length)
         return np.stack([atom.element_features(*feature_names) for atom in self.atoms])
 
+    def fingerprint(self, fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2'):
+        """
+        Calculate the molecular fingerprint for this molecule, the supporting fingerprint include:
+
+        1. "FP2": The FP2 fingerprint is a path-based fingerprint that encodes the presence of linear
+        fragments up to 7 atoms long. It is a 1024-bit fingerprint and is commonly used for substructure
+        searches and similarity calculations.
+
+        2. "FP3": The FP3 fingerprint is designed for searching 3D conformations, such as those found
+        in protein-ligand complexes. It encodes the presence of particular pharmacophoric features,
+        such as hydrogen bond donors, acceptors, and hydrophobic regions.
+
+        3. "FP4": The FP4 fingerprint is a circular fingerprint based on the Morgan algorithm. It
+        captures information about the local environment of each atom in the molecule, up to a certain
+        radius. It is useful for similarity calculations and machine learning tasks.
+
+        4. "MACCS": The MACCS fingerprint is a 166-bit structural key-based fingerprint. It represents
+        the presence of specific substructures or functional groups defined by the MACCS keys. It is
+        commonly used for similarity calculations and substructure searches.
+
+        Return:
+            the Fingerprint object in pybel module
+        """
+        return pb.Molecule(self.ob_mol).calcfp(fptype)
+
     @property
     def forces(self):
         """ return the all force vectors for all atoms in the molecule """
         return np.vstack((atom.force_vector for atom in self.atoms))
 
     @property
     def all_forces(self):
@@ -1193,14 +1195,59 @@
         if path_err_file:
             with open(path_err_file, 'w') as writer:
                 writer.write(stderr)
 
         # return results and error info
         return stdout, stderr
 
+    def generate_metal_ligand_pair(
+            self, metal_symbol: str, acceptor_atoms: Sequence = ('O',), opti_force_field: str = 'UFF'
+    ) -> Generator['Molecule', None, None]:
+        """
+        This method could work if the molecule is an organic ligand, or raise AttributeError.
+        Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
+
+        Args:
+            metal_symbol: which metal element link to the ligand
+            acceptor_atoms: which elements to be acceptor atom to link to metal
+            opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
+
+        Return:
+            A generator for M-L pair
+        """
+
+        ligand = self.copy()
+        ligand.localed_optimize(opti_force_field)  # locally optimize the ligand
+        ligand.normalize_labels()
+
+        for atom in ligand.atoms:
+            if atom.symbol in acceptor_atoms:
+                acceptor_ligand = ligand.copy()
+
+                # assign the initial coordinates
+                # the sum of vector of relative position relate to the accepting atom
+                sum_relative_coordinates = sum([c for _, c in atom.neighbours_position])
+                metal_init_coordinates = atom.coordinates_array - sum_relative_coordinates
+
+                # add metal atom into the acceptor_ligand
+                added_metal = acceptor_ligand.add_atom(metal_symbol, coordinates=metal_init_coordinates)
+
+                # add the coordinating bond between metal atom and acceptor atoms
+                acceptor_ligand.add_bond(added_metal, atom.label, 1)
+
+                # remove redundant hydrogen
+                accepting_atom = acceptor_ligand.atom(atom.label)
+                while accepting_atom.valence > accepting_atom.valence_max and accepting_atom.neighbours_hydrogen:
+                    acceptor_ligand.remove_atoms(accepting_atom.neighbours_hydrogen[0])
+
+                # localize optimization of M-L pair by classical force field
+                acceptor_ligand.localed_optimize(opti_force_field)
+
+                yield acceptor_ligand
+
     def graph_representation(self, *feature_names):
         return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
 
     @property
     def has_3d(self):
         """ Whether atoms in the molecule have 3d coordinates """
         return self.ob_mol.Has3D()
@@ -1221,16 +1268,15 @@
     @property
     def inchi(self):
         return self.dump('inchi').strip()
 
     @property
     def is_labels_unique(self):
         """ Determine whether all atom labels are unique """
-        labels = set(self.labels)
-        return len(labels) == self.atom_num
+        return len(set(self.labels)) == self.atom_num
 
     @property
     def is_organic(self):
         """ To judge whether the molecule is organic, an organic compound is with carbon atoms and without metal """
         if any(a.is_metal for a in self.atoms):
             return False
         elif any(a.symbol == 'C' for a in self.atoms):
@@ -1239,15 +1285,15 @@
         return False
 
     @property
     def ob_mol(self):
         return self._data['ob_mol']
 
     def ob_mol_pop(self):
-        data = self._data
+        data: dict = self._data
 
         atoms: Dict[int, Atom] = data.get('atoms')
         if atoms:
             for ob_id, atom in atoms.items():
                 atom.ob_atom_pop()
 
         bonds: Dict[int, Bond] = data.get('bonds')
@@ -1257,16 +1303,16 @@
 
         return self._data.pop('ob_mol')
 
     def ob_mol_rewrap(self, ob_mol: ob.OBMol):
         if not isinstance(ob_mol, ob.OBMol):
             raise TypeError('the ob_mol should be OBMol object')
 
-        atoms: Dict[int, Atom] = self._data.get('atoms')
-        bonds: Dict[int, Bond] = self._data.get('bonds')
+        atoms = self._data.get('atoms')
+        bonds = self._data.get('bonds')
 
         if any(oba.GetId() not in atoms for oba in ob.OBMolAtomIter(ob_mol)):
             raise ValueError('the atom number between the wrapper and the core OBMol is not match')
         if any(obb.GetIdx() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
             raise ValueError('the bond number between the wrapper and the core OBMol is not match')
 
         self._data['ob_mol'] = ob_mol
@@ -1294,15 +1340,15 @@
     def lmp_setup(self, *args, **kwargs):
         self._data['lmp'] = lmp.HpLammps(self, **kwargs)
 
     @property
     def link_matrix(self):
         return np.array([[b.ob_atom1_id, b.ob_atom2_id] for b in self.bonds]).T
 
-    def localed_optimize(self, force_field: str = 'mmff94', steps: int = 500):
+    def localed_optimize(self, force_field: str = 'UFF', steps: int = 500):
         """ Locally optimize the coordinates. seeing openbabel.pybel package """
         pymol = pb.Molecule(self.ob_mol)
         pymol.localopt(force_field, steps)
 
     def make_crystal(self, a: float, b: float, c: float, alpha: float, beta: float, gamma: float) -> 'Crystal':
         """ Put this molecule into the specified crystal """
         ob_unit_cell = ob.OBUnitCell()
@@ -1358,14 +1404,18 @@
             a=a, b=b, c=c, alpha=alpha, beta=beta, gamma=gamma, time_step=time_step,
             origin_temp=origin_temp, melt_temp=melt_temp, highest_temp=highest_temp,
             ff_args=ff_args, path_writefile=path_writefile, path_dump_to=path_dump_to,
             dump_every=dump_every, mol=self
         )
 
     @property
+    def metals(self) -> List['Atom']:
+        return [a for a in self.atoms if a.is_metal]
+
+    @property
     def mol_orbital_energies(self):
         energies = self._data.get('mol_orbital_energies')
         if energies:
             return energies
         else:
             return None
 
@@ -1494,15 +1544,15 @@
             else:
                 raise ValueError(f'the arguments should be specified for {type(source)} source')
 
         mol = Parser(fmt, source, *args, **kwargs)()  # initialize parser object and call self
 
         # Specify the mol identifier if it's None
         if not mol.identifier:
-            mol.identifier = source
+            mol.identifier = str(source)
 
         return mol
 
     def register_critical_params(self, name: str, temperature: float, pressure: float, acentric: float):
         """ Register new critical parameters into the critical parameters sheet """
         data = json.load(open(ptj(data_root, 'thermo', 'critical.json')))
         data[self.smiles] = {'name': name, 'temperature': temperature, 'pressure': pressure, 'acentric': acentric}
@@ -1530,38 +1580,86 @@
                 if not (atom.molecule is self):
                     raise AttributeError('the given atom not in the molecule')
             else:
                 raise TypeError('the given atom should be int, str or Atom')
 
             # remove connecting hydrogens
             if remove_hydrogens:
-                for nh in atom.neigh_hydrogens:
+                for nh in atom.neighbours_hydrogen:
                     self.ob_mol.DeleteAtom(nh.ob_atom)
 
             # Removing the atom
             self.ob_mol.DeleteAtom(atom.ob_atom)
             atom._data['_mol'] = None
 
             # Reload atoms
             self._load_atoms()
 
     def remove_hydrogens(self):
         self.ob_mol.DeleteHydrogens()
 
+    def remove_metals(self):
+        """ remove all of metal atoms in the molecule """
+        self.remove_atoms(*self.metals)
+
+    def remove_solvents(self):
+        """ remove all solvents in the molecule """
+        self.normalize_labels()
+        for ligand in self.retrieve_ligands():
+            if _lib.get('Solvents').is_solvent(ligand):  # To judge if the ligand is solvents
+                self.remove_atoms(*ligand.atom_labels, remove_hydrogens=False)
+
+    def retrieve_ligands(self) -> List['Molecule']:
+        """ Retrieve all ligand molecule from this """
+        clone = self.copy()
+        clone.remove_metals()
+
+        return clone.components
+
+    def retrieve_metal_ligand_pairs(self) -> List['Molecule']:
+        """ Retrieve all clone of metal-ligand pairs in the molecule """
+        if not self.is_labels_unique:
+            self.normalize_labels()
+
+        ml_pairs = []
+        for metal, ligand in product(self.metals, self.retrieve_ligands()):
+            if set(metal.neighbours_label) & set(ligand.atom_labels):
+                pair = self.copy()
+
+                # Remove all the atoms is not the metal and not on the ligand
+                other_atoms = [a for a in pair.atoms if a.label != metal.label and a.label not in ligand.atom_labels]
+                pair.remove_atoms(*other_atoms, remove_hydrogens=False)
+
+                ml_pairs.append(pair)
+
+        return ml_pairs
+
     @property
     def rotatable_bonds_number(self):
         return self.ob_mol.NumRotors()
 
     def set(self, **kwargs):
         """ Set the attributes directly """
         self._set_attrs(**kwargs)
 
     def set_label(self, ob_id: int, label: str):
         self.atoms_dict[ob_id].label = label
 
+    def similarity(self, other: 'Molecule', fptype: Literal['FP2', 'FP3', 'FP4', 'MACCS'] = 'FP2') -> int:
+        """
+        Compare the similarity with other molecule, based on specified fingerprint
+        Args:
+            other(Molecule): the other Molecule
+            fptype(str): the fingerprint type to perform comparison of similarity
+
+        Return:
+            the similarity(int)
+        """
+        return self.fingerprint(fptype) | other.fingerprint(fptype)
+
     @property
     def smiles(self):
         return self.dump('smi').split()[0]
 
     @property
     def spin(self):
         return self.ob_mol.GetTotalSpinMultiplicity()
@@ -1753,15 +1851,16 @@
             # '_mol': _mol,
         }
 
         self._set_attrs(**kwargs)
 
     def __eq__(self, other):
         if isinstance(other, Atom):
-            return self.symbol == other.symbol
+            # return self.symbol == other.symbol
+            return self.ob_atom == other.ob_atom
 
     def __hash__(self):
         return hash(f'Atom({self.atomic_number})')
 
     @property
     def ob_atom(self):
         return self._data['ob_atom']
@@ -1847,21 +1946,26 @@
         return self.ob_atom.GetType()
 
     @property
     def atomic_number(self):
         return self.ob_atom.GetAtomicNum()
 
     @property
-    def coordinates(self) -> np.ndarray:
-        return np.array([self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()])
+    def coordinates(self) -> (float, float, float):
+        return self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()
 
     @coordinates.setter
     def coordinates(self, value):
         self._set_coordinate(value)
 
+    @property
+    def coordinates_array(self) -> np.ndarray:
+        """ the array of coordinates """
+        return np.array(self.coordinates)
+
     def copy(self):
         """ Make a copy of self """
         # Extract old data
         data = self.copy_data()
         data.pop('ob_atom')  # Remove the old OBAtom
         # Remove molecule if the parent atom in a molecule
         if self.mol:
@@ -2019,31 +2123,37 @@
         return _max_total_bond_order[self.symbol]
 
     @property
     def molecule(self) -> Molecule:
         return self.mol
 
     @property
-    def neigh_hydrogens(self):
+    def neighbours_hydrogen(self) -> List['Atom']:
+        """ return all neigh hydrogen atoms """
         return [a for a in self.neighbours if a.is_hydrogen]
 
     @property
     def neighbours(self) -> List['Atom']:
         """ Get all atoms bond with this atom in same molecule """
         if self.mol:
             _ = self.mol.atoms  # update the atoms dict
             return [self.mol.data.get('atoms')[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
         else:
             return []
 
     @property
+    def neighbours_label(self) -> List[str]:
+        """ return all neighbours labels """
+        return [a.label for a in self.neighbours]
+
+    @property
     def neighbours_position(self) -> Generator[Tuple[Union['Atom', np.ndarray]], None, None]:
         """ Retrieve the relative position of neigh atoms, assign this atom as the origin """
         for neigh_atom in self.neighbours:
-            yield neigh_atom, neigh_atom.coordinates - self.coordinates
+            yield neigh_atom, neigh_atom.coordinates_array - self.coordinates_array
 
     @property
     def partial_charge(self):
         return self.ob_atom.GetPartialCharge()
 
     @partial_charge.setter
     def partial_charge(self, value: float):
```

### Comparing `hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.2.3/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.2.3/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/data/periodic_table.json` & `hotpot-zzy-0.2.3/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.2.3/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.2.3/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.2.3/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tanks/quantum.py` & `hotpot-zzy-0.2.3/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tmo.py` & `hotpot-zzy-0.2.3/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/tools.py` & `hotpot-zzy-0.2.3/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/hotpot/utils/units_convert.py` & `hotpot-zzy-0.2.3/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/test/test_amorphous_maker.py` & `hotpot-zzy-0.2.3/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/test/test_bundle.py` & `hotpot-zzy-0.2.3/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.2/test/test_chemif.py` & `hotpot-zzy-0.2.3/test/test_chemif.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     mol = ci.Molecule.read_from(path_cif, 'cif')
     gen = mol.perturb_mol_lattice(mol_distance=0.05, max_generate_num=2)
 
     for i, gen_mol in enumerate(gen):
         gen_mol.writefile('cif', f'output/gen_cif/aCarbon_{i}.cif')
 
 
-if __name__ == '__main__':
+def gen_pairs():
     from openbabel import openbabel as ob
     mol = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
     mol2 = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
     mol.build_conformer('UFF')
     mol2.build_conformer()
     mol.normalize_labels()
     mol2.normalize_labels()
@@ -60,7 +60,19 @@
 
     # for a1, a2 in zip(mol.atoms, mol2.atoms):
     #     print(f'{a1.label}: {a1.partial_charge}---{a2.label}: {a2.partial_charge}')
 
     ps = [p for i, p in enumerate(g)]
     ps[1].remove_atoms('C1', 'C2')
     ps[1].writefile('mol2', f'/home/zz1/g01.mol2')
+
+
+if __name__ == '__main__':
+    mol = ci.Molecule.read_from('/home/zz1/ZONTOO.cif')
+    # mol.build_conformer()
+    # mol.remove_solvents()
+    # mol.writefile('mol2', '/home/zz1/self.mol2')
+    ligands = mol.retrieve_ligands()
+    for ligand in ligands:
+        ligand.add_hydrogens()
+        ligand.localed_optimize()
+    pairs = [p for l in ligands for p in l.generate_metal_ligand_pair('Sr')]
```

### Comparing `hotpot-zzy-0.2.2/test/test_lmp.py` & `hotpot-zzy-0.2.3/test/test_lmp.py`

 * *Files identical despite different names*

