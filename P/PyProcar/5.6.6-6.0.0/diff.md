# Comparing `tmp/PyProcar-5.6.6.tar.gz` & `tmp/PyProcar-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProcar-5.6.6.tar", last modified: Sun Mar  6 20:10:55 2022, max compression
+gzip compressed data, was "dist\PyProcar-6.0.0.tar", last modified: Sat Jun 10 16:58:20 2023, max compression
```

## Comparing `PyProcar-5.6.6.tar` & `PyProcar-6.0.0.tar`

### file list

```diff
@@ -1,117 +1,110 @@
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.242202 PyProcar-5.6.6/
--rwxr--r--   0 uthpala    (501) staff       (20)    42868 2018-03-28 17:26:35.000000 PyProcar-5.6.6/LICENSE.txt
--rwxr--r--   0 uthpala    (501) staff       (20)       61 2020-11-25 10:07:39.000000 PyProcar-5.6.6/MANIFEST.in
--rw-r--r--   0 uthpala    (501) staff       (20)      639 2022-03-06 20:10:55.242504 PyProcar-5.6.6/PKG-INFO
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.158014 PyProcar-5.6.6/PyProcar.egg-info/
--rwxr--r--   0 uthpala    (501) staff       (20)      639 2022-03-06 20:10:54.000000 PyProcar-5.6.6/PyProcar.egg-info/PKG-INFO
--rwxr--r--   0 uthpala    (501) staff       (20)     2667 2022-03-06 20:10:54.000000 PyProcar-5.6.6/PyProcar.egg-info/SOURCES.txt
--rwxr--r--   0 uthpala    (501) staff       (20)        1 2022-03-06 20:10:54.000000 PyProcar-5.6.6/PyProcar.egg-info/dependency_links.txt
--rwxr--r--   0 uthpala    (501) staff       (20)       68 2022-03-06 20:10:54.000000 PyProcar-5.6.6/PyProcar.egg-info/requires.txt
--rwxr--r--   0 uthpala    (501) staff       (20)        9 2022-03-06 20:10:54.000000 PyProcar-5.6.6/PyProcar.egg-info/top_level.txt
--rwxr--r--   0 uthpala    (501) staff       (20)     8581 2021-06-11 03:30:58.000000 PyProcar-5.6.6/README.md
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.175800 PyProcar-5.6.6/pyprocar/
--rwxr--r--   0 uthpala    (501) staff       (20)     2836 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/__init__.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.176801 PyProcar-5.6.6/pyprocar/abinitparser/
--rwxr--r--   0 uthpala    (501) staff       (20)       40 2020-03-08 07:14:15.000000 PyProcar-5.6.6/pyprocar/abinitparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     1329 2021-04-22 15:38:51.000000 PyProcar-5.6.6/pyprocar/abinitparser/abinitparser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.178328 PyProcar-5.6.6/pyprocar/bxsfparser/
--rwxr--r--   0 uthpala    (501) staff       (20)       36 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/bxsfparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     4599 2021-04-27 01:25:51.000000 PyProcar-5.6.6/pyprocar/bxsfparser/bxsf_parser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.186270 PyProcar-5.6.6/pyprocar/core/
--rwxr-xr-x   0 uthpala    (501) staff       (20)      285 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/core/__init__.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     5770 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/core/dos.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)    24136 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/core/ebs.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     4578 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/core/elements.py
--rwxr--r--   0 uthpala    (501) staff       (20)    14489 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/core/isosurface.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     5936 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/core/kpath.py
--rwxr--r--   0 uthpala    (501) staff       (20)     9583 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/core/structure.py
--rwxr--r--   0 uthpala    (501) staff       (20)    10001 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/core/surface.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.187785 PyProcar-5.6.6/pyprocar/doscarplot/
--rwxr--r--   0 uthpala    (501) staff       (20)       30 2020-05-21 18:08:35.000000 PyProcar-5.6.6/pyprocar/doscarplot/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    23275 2021-01-12 03:07:51.000000 PyProcar-5.6.6/pyprocar/doscarplot/dosplot.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.189749 PyProcar-5.6.6/pyprocar/elkparser/
--rwxr--r--   0 uthpala    (501) staff       (20)       33 2020-03-03 19:50:15.000000 PyProcar-5.6.6/pyprocar/elkparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    11090 2021-04-22 16:22:49.000000 PyProcar-5.6.6/pyprocar/elkparser/elkparser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.192898 PyProcar-5.6.6/pyprocar/fermisurface/
--rwxr--r--   0 uthpala    (501) staff       (20)       39 2018-09-17 23:14:34.000000 PyProcar-5.6.6/pyprocar/fermisurface/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     7318 2020-11-12 18:45:59.000000 PyProcar-5.6.6/pyprocar/fermisurface/fermisurface.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.199125 PyProcar-5.6.6/pyprocar/fermisurface3d/
--rwxr--r--   0 uthpala    (501) staff       (20)      105 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/fermisurface3d/__init__.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     4281 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/fermisurface3d/brillouin_zone.py
--rwxr--r--   0 uthpala    (501) staff       (20)    39605 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/fermisurface3d/fermisurface3D.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.201282 PyProcar-5.6.6/pyprocar/frmsfparser/
--rwxr--r--   0 uthpala    (501) staff       (20)       37 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/frmsfparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     6057 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/frmsfparser/frmsfParser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.204142 PyProcar-5.6.6/pyprocar/io/
--rwxr-xr-x   0 uthpala    (501) staff       (20)       20 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/io/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    11629 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/io/abinit.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)    67757 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/io/vasp.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.207842 PyProcar-5.6.6/pyprocar/lobsterparser/
--rwxr--r--   0 uthpala    (501) staff       (20)      143 2021-01-12 03:07:51.000000 PyProcar-5.6.6/pyprocar/lobsterparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    20487 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/lobsterparser/lobster_doscar_parser.py
--rwxr--r--   0 uthpala    (501) staff       (20)    15248 2021-04-22 16:22:49.000000 PyProcar-5.6.6/pyprocar/lobsterparser/lobsterfermiparser.py
--rwxr--r--   0 uthpala    (501) staff       (20)    15489 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/lobsterparser/lobsterparser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.208994 PyProcar-5.6.6/pyprocar/plotter/
--rwxr--r--   0 uthpala    (501) staff       (20)       53 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/plotter/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    14848 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/plotter/ebs_plot.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.210352 PyProcar-5.6.6/pyprocar/procarfilefilter/
--rwxr--r--   0 uthpala    (501) staff       (20)       85 2020-03-05 02:06:04.000000 PyProcar-5.6.6/pyprocar/procarfilefilter/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    17863 2020-04-14 14:02:58.000000 PyProcar-5.6.6/pyprocar/procarfilefilter/procarfilefilter.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.212654 PyProcar-5.6.6/pyprocar/procarparser/
--rwxr--r--   0 uthpala    (501) staff       (20)       77 2020-03-05 02:06:04.000000 PyProcar-5.6.6/pyprocar/procarparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    30595 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/procarparser/procarparser.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.215783 PyProcar-5.6.6/pyprocar/procarplot/
--rwxr--r--   0 uthpala    (501) staff       (20)       35 2020-03-05 02:06:05.000000 PyProcar-5.6.6/pyprocar/procarplot/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    13609 2020-11-25 01:38:43.000000 PyProcar-5.6.6/pyprocar/procarplot/procarplot.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.217581 PyProcar-5.6.6/pyprocar/procarselect/
--rwxr--r--   0 uthpala    (501) staff       (20)       77 2020-03-05 02:06:05.000000 PyProcar-5.6.6/pyprocar/procarselect/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     8335 2020-07-28 06:22:59.000000 PyProcar-5.6.6/pyprocar/procarselect/procarselect.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.219198 PyProcar-5.6.6/pyprocar/procarsymmetry/
--rwxr--r--   0 uthpala    (501) staff       (20)       43 2018-09-17 23:14:36.000000 PyProcar-5.6.6/pyprocar/procarsymmetry/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)     8491 2020-03-05 02:06:05.000000 PyProcar-5.6.6/pyprocar/procarsymmetry/procarsymmetry.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.223576 PyProcar-5.6.6/pyprocar/procarunfold/
--rwxr--r--   0 uthpala    (501) staff       (20)       44 2019-03-19 23:18:32.000000 PyProcar-5.6.6/pyprocar/procarunfold/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    23921 2020-03-05 02:06:06.000000 PyProcar-5.6.6/pyprocar/procarunfold/_bak.procarparser.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     5229 2021-01-21 20:54:07.000000 PyProcar-5.6.6/pyprocar/procarunfold/fatband.py
--rwxr--r--   0 uthpala    (501) staff       (20)     4409 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/procarunfold/procar_unfolder.py
--rwxr--r--   0 uthpala    (501) staff       (20)     5013 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/procarunfold/unfolder.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.226898 PyProcar-5.6.6/pyprocar/qeparser/
--rwxr--r--   0 uthpala    (501) staff       (20)      110 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/qeparser/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    23349 2021-04-22 16:22:49.000000 PyProcar-5.6.6/pyprocar/qeparser/qe_dos_parser.py
--rwxr--r--   0 uthpala    (501) staff       (20)    22250 2021-01-12 03:07:51.000000 PyProcar-5.6.6/pyprocar/qeparser/qefermiparser.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)    25595 2021-04-22 19:48:36.000000 PyProcar-5.6.6/pyprocar/qeparser/qeparser.py
--rwxr--r--   0 uthpala    (501) staff       (20)     3217 2020-11-30 16:16:33.000000 PyProcar-5.6.6/pyprocar/scriptBandGap.py
--rwxr--r--   0 uthpala    (501) staff       (20)    20862 2021-04-27 01:25:51.000000 PyProcar-5.6.6/pyprocar/scriptBandsDosplot.py
--rwxr--r--   0 uthpala    (501) staff       (20)    15480 2022-02-10 15:34:29.000000 PyProcar-5.6.6/pyprocar/scriptBandsplot.py
--rwxr--r--   0 uthpala    (501) staff       (20)     9061 2021-03-07 23:43:16.000000 PyProcar-5.6.6/pyprocar/scriptCat.py
--rwxr--r--   0 uthpala    (501) staff       (20)    22120 2022-03-05 20:53:14.000000 PyProcar-5.6.6/pyprocar/scriptDosplot.py
--rwxr--r--   0 uthpala    (501) staff       (20)     6699 2022-02-10 16:51:10.000000 PyProcar-5.6.6/pyprocar/scriptFermi2D.py
--rwxr--r--   0 uthpala    (501) staff       (20)    35109 2021-08-25 02:41:40.000000 PyProcar-5.6.6/pyprocar/scriptFermi3D.py
--rwxr--r--   0 uthpala    (501) staff       (20)     2374 2020-03-05 02:06:06.000000 PyProcar-5.6.6/pyprocar/scriptFilter.py
--rwxr--r--   0 uthpala    (501) staff       (20)      618 2020-03-05 02:06:06.000000 PyProcar-5.6.6/pyprocar/scriptKmesh2D.py
--rwxr--r--   0 uthpala    (501) staff       (20)     3526 2020-10-23 16:33:15.000000 PyProcar-5.6.6/pyprocar/scriptKpath.py
--rwxr--r--   0 uthpala    (501) staff       (20)      375 2020-03-05 02:06:06.000000 PyProcar-5.6.6/pyprocar/scriptRepair.py
--rwxr--r--   0 uthpala    (501) staff       (20)     7690 2020-08-28 16:18:31.000000 PyProcar-5.6.6/pyprocar/scriptSpin_asymmetry.py
--rwxr--r--   0 uthpala    (501) staff       (20)     3595 2020-11-30 16:24:21.000000 PyProcar-5.6.6/pyprocar/scriptUnfold.py
--rwxr--r--   0 uthpala    (501) staff       (20)     3277 2020-11-30 16:26:02.000000 PyProcar-5.6.6/pyprocar/scriptVector.py
--rwxr--r--   0 uthpala    (501) staff       (20)      943 2021-01-12 03:12:00.000000 PyProcar-5.6.6/pyprocar/splash.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.233026 PyProcar-5.6.6/pyprocar/utils/
--rwxr-xr-x   0 uthpala    (501) staff       (20)       81 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/utils/__init__.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     2268 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/utils/info.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     1956 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/utils/mathematics.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)     5983 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/utils/unfolder.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.236624 PyProcar-5.6.6/pyprocar/utilsprocar/
--rwxr--r--   0 uthpala    (501) staff       (20)       37 2019-11-04 02:21:35.000000 PyProcar-5.6.6/pyprocar/utilsprocar/__init__.py
--rwxr--r--   0 uthpala    (501) staff       (20)    27676 2020-06-17 17:57:53.000000 PyProcar-5.6.6/pyprocar/utilsprocar/scriptFermi3D.py
--rwxr--r--   0 uthpala    (501) staff       (20)    10630 2020-05-11 04:18:18.000000 PyProcar-5.6.6/pyprocar/utilsprocar/utilsprocar.py
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.238842 PyProcar-5.6.6/pyprocar/vaspxml/
--rwxr--r--   0 uthpala    (501) staff       (20)       53 2020-08-28 16:18:31.000000 PyProcar-5.6.6/pyprocar/vaspxml/__init__.py
--rwxr-xr-x   0 uthpala    (501) staff       (20)    24555 2021-08-25 02:42:27.000000 PyProcar-5.6.6/pyprocar/vaspxml/vaspxml.py
--rwxr--r--   0 uthpala    (501) staff       (20)      603 2022-03-06 20:10:54.000000 PyProcar-5.6.6/pyprocar/version.py
--rwxr--r--   0 uthpala    (501) staff       (20)       68 2020-07-01 19:39:57.000000 PyProcar-5.6.6/requirements.txt
-drwxr-xr-x   0 uthpala    (501) staff       (20)        0 2022-03-06 20:10:55.239750 PyProcar-5.6.6/scripts/
--rwxr--r--   0 uthpala    (501) staff       (20)    32646 2020-07-27 03:07:47.000000 PyProcar-5.6.6/scripts/procar.py
--rwxr--r--   0 uthpala    (501) staff       (20)       79 2022-03-06 20:10:55.243524 PyProcar-5.6.6/setup.cfg
--rwxr--r--   0 uthpala    (501) staff       (20)      674 2022-03-06 20:09:50.000000 PyProcar-5.6.6/setup.json
--rwxr--r--   0 uthpala    (501) staff       (20)     2127 2020-11-25 10:33:48.000000 PyProcar-5.6.6/setup.py
--rwxr--r--   0 uthpala    (501) staff       (20)       72 2021-04-22 16:22:49.000000 PyProcar-5.6.6/todo.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.860260 PyProcar-6.0.0/
+-rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.0.0/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      674 2023-06-10 16:58:20.861262 PyProcar-6.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.733145 PyProcar-6.0.0/PyProcar.egg-info/
+-rw-rw-rw-   0        0        0      674 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8913 2023-06-10 16:55:55.000000 PyProcar-6.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.736147 PyProcar-6.0.0/pyprocar/
+-rw-rw-rw-   0        0        0     2507 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.755166 PyProcar-6.0.0/pyprocar/core/
+-rw-rw-rw-   0        0        0      456 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/__init__.py
+-rw-rw-rw-   0        0        0     4408 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/brillouin_zone.py
+-rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.0.0/pyprocar/core/dos.py
+-rw-rw-rw-   0        0        0    38748 2023-05-25 15:22:33.000000 PyProcar-6.0.0/pyprocar/core/ebs.py
+-rw-rw-rw-   0        0        0    18179 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/fermisurface.py
+-rw-rw-rw-   0        0        0    37312 2023-05-23 18:08:09.000000 PyProcar-6.0.0/pyprocar/core/fermisurface3D.py
+-rw-rw-rw-   0        0        0    14082 2023-05-23 14:16:14.000000 PyProcar-6.0.0/pyprocar/core/isosurface.py
+-rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/kpath.py
+-rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarselect.py
+-rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarsymmetry.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.762171 PyProcar-6.0.0/pyprocar/core/procarunfold/
+-rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/__init__.py
+-rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/_bak.procarparser.py
+-rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/fatband.py
+-rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/procar_unfolder.py
+-rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/unfolder.py
+-rw-rw-rw-   0        0        0    15028 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/structure.py
+-rw-rw-rw-   0        0        0    11039 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/surface.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.778186 PyProcar-6.0.0/pyprocar/io/
+-rw-rw-rw-   0        0        0      885 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/__init__.py
+-rw-rw-rw-   0        0        0    15461 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinit.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.781189 PyProcar-6.0.0/pyprocar/io/abinitparser/
+-rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinitparser/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinitparser/abinitparser.py
+-rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/bxsf.py
+-rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elk.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.785192 PyProcar-6.0.0/pyprocar/io/elkparser/
+-rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elkparser/__init__.py
+-rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elkparser/elkparser.py
+-rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/frmsf.py
+-rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobster.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.791198 PyProcar-6.0.0/pyprocar/io/lobsterparser/
+-rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/__init__.py
+-rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py
+-rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterfermiparser.py
+-rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterparser.py
+-rw-rw-rw-   0        0        0     6099 2023-05-23 13:49:31.000000 PyProcar-6.0.0/pyprocar/io/parser.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.794200 PyProcar-6.0.0/pyprocar/io/procarparser/
+-rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/procarparser/__init__.py
+-rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/procarparser/procarparser.py
+-rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.0.0/pyprocar/io/qe.py
+-rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/siesta.py
+-rw-rw-rw-   0        0        0    79901 2023-05-25 16:59:57.000000 PyProcar-6.0.0/pyprocar/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.797203 PyProcar-6.0.0/pyprocar/io/vaspxml/
+-rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/vaspxml/__init__.py
+-rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/vaspxml/vaspxml.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.803208 PyProcar-6.0.0/pyprocar/plotter/
+-rw-rw-rw-   0        0        0      123 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/__init__.py
+-rw-rw-rw-   0        0        0    51559 2023-05-25 18:16:18.000000 PyProcar-6.0.0/pyprocar/plotter/dos_plot.py
+-rw-rw-rw-   0        0        0    21401 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/ebs_plot.py
+-rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/procarplot.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.838240 PyProcar-6.0.0/pyprocar/scripts/
+-rw-rw-rw-   0        0        0      744 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/depreciated_scriptVector.py
+-rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandGap.py
+-rw-rw-rw-   0        0        0     9000 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsDosplot.py
+-rw-rw-rw-   0        0        0     8223 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot_2d.py
+-rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptCat.py
+-rw-rw-rw-   0        0        0    17304 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptDosplot.py
+-rw-rw-rw-   0        0        0    11769 2023-05-25 19:52:39.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermi2D.py
+-rw-rw-rw-   0        0        0    33276 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermi3D.py
+-rw-rw-rw-   0        0        0    90799 2023-05-25 16:53:05.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermiHandler.py
+-rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFilter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptKmesh2D.py
+-rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptKpath.py
+-rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptRepair.py
+-rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptSpin_asymmetry.py
+-rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold.py
+-rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_new.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_old.py
+-rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_v2.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptVector.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.857258 PyProcar-6.0.0/pyprocar/utils/
+-rw-rw-rw-   0        0        0      273 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/default_settings.ini
+-rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/defaults.py
+-rw-rw-rw-   0        0        0     5433 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/download_examples.py
+-rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/elements.py
+-rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/info.py
+-rw-rw-rw-   0        0        0     2038 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/mathematics.py
+-rw-rw-rw-   0        0        0    18332 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/procarfilefilter.py
+-rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/scriptFermi3D.py
+-rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/sorting.py
+-rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/splash.py
+-rw-rw-rw-   0        0        0     6062 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/unfolder.py
+-rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/utilsprocar.py
+-rw-rw-rw-   0        0        0      688 2023-06-10 16:58:19.000000 PyProcar-6.0.0/pyprocar/version.py
+-rw-rw-rw-   0        0        0       81 2023-05-08 12:33:47.000000 PyProcar-6.0.0/requirements.txt
+-rw-rw-rw-   0        0        0     1740 2023-05-08 12:33:47.000000 PyProcar-6.0.0/requirements_docs.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.859259 PyProcar-6.0.0/scripts/
+-rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.0.0/scripts/procar.py
+-rw-rw-rw-   0        0        0       86 2023-06-10 16:58:20.866266 PyProcar-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-05-23 14:24:52.000000 PyProcar-6.0.0/setup.json
+-rw-rw-rw-   0        0        0     1590 2023-05-23 14:48:41.000000 PyProcar-6.0.0/setup.py
```

### Comparing `PyProcar-5.6.6/LICENSE.txt` & `PyProcar-6.0.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,843 +1,843 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
---------------------------------------------------------------------------------
-
-		   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
-
+                  GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies
+of this license document, but changing it is not allowed.
+
+                          Preamble
+
+The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+                      TERMS AND CONDITIONS
+
+0. Definitions.
+
+"This License" refers to version 3 of the GNU General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+The Corresponding Source for a work in source code form is that
+same work.
+
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+  a) The work must carry prominent notices stating that you modified
+  it, and giving a relevant date.
+
+  b) The work must carry prominent notices stating that it is
+  released under this License and any conditions added under section
+  7.  This requirement modifies the requirement in section 4 to
+  "keep intact all notices".
+
+  c) You must license the entire work, as a whole, under this
+  License to anyone who comes into possession of a copy.  This
+  License will therefore apply, along with any applicable section 7
+  additional terms, to the whole of the work, and all its parts,
+  regardless of how they are packaged.  This License gives no
+  permission to license the work in any other way, but it does not
+  invalidate such permission if you have separately received it.
+
+  d) If the work has interactive user interfaces, each must display
+  Appropriate Legal Notices; however, if the Program has interactive
+  interfaces that do not display Appropriate Legal Notices, your
+  work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+  a) Convey the object code in, or embodied in, a physical product
+  (including a physical distribution medium), accompanied by the
+  Corresponding Source fixed on a durable physical medium
+  customarily used for software interchange.
+
+  b) Convey the object code in, or embodied in, a physical product
+  (including a physical distribution medium), accompanied by a
+  written offer, valid for at least three years and valid for as
+  long as you offer spare parts or customer support for that product
+  model, to give anyone who possesses the object code either (1) a
+  copy of the Corresponding Source for all the software in the
+  product that is covered by this License, on a durable physical
+  medium customarily used for software interchange, for a price no
+  more than your reasonable cost of physically performing this
+  conveying of source, or (2) access to copy the
+  Corresponding Source from a network server at no charge.
+
+  c) Convey individual copies of the object code with a copy of the
+  written offer to provide the Corresponding Source.  This
+  alternative is allowed only occasionally and noncommercially, and
+  only if you received the object code with such an offer, in accord
+  with subsection 6b.
+
+  d) Convey the object code by offering access from a designated
+  place (gratis or for a charge), and offer equivalent access to the
+  Corresponding Source in the same way through the same place at no
+  further charge.  You need not require recipients to copy the
+  Corresponding Source along with the object code.  If the place to
+  copy the object code is a network server, the Corresponding Source
+  may be on a different server (operated by you or a third party)
+  that supports equivalent copying facilities, provided you maintain
+  clear directions next to the object code saying where to find the
+  Corresponding Source.  Regardless of what server hosts the
+  Corresponding Source, you remain obligated to ensure that it is
+  available for as long as needed to satisfy these requirements.
+
+  e) Convey the object code using peer-to-peer transmission, provided
+  you inform other peers where the object code and Corresponding
+  Source of the work are being offered to the general public at no
+  charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+  a) Disclaiming warranty or limiting liability differently from the
+  terms of sections 15 and 16 of this License; or
+
+  b) Requiring preservation of specified reasonable legal notices or
+  author attributions in that material or in the Appropriate Legal
+  Notices displayed by works containing it; or
+
+  c) Prohibiting misrepresentation of the origin of that material, or
+  requiring that modified versions of such material be marked in
+  reasonable ways as different from the original version; or
+
+  d) Limiting the use for publicity purposes of names of licensors or
+  authors of the material; or
+
+  e) Declining to grant rights under trademark law for use of some
+  trade names, trademarks, or service marks; or
+
+  f) Requiring indemnification of licensors and authors of that
+  material by anyone who conveys the material (or modified versions of
+  it) with contractual assumptions of liability to the recipient, for
+  any liability that these contractual assumptions directly impose on
+  those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                    END OF TERMS AND CONDITIONS
+
+          How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+  <one line to give the program's name and a brief idea of what it does.>
+  Copyright (C) <year>  <name of author>
+
+  This program is free software: you can redistribute it and/or modify
+  it under the terms of the GNU General Public License as published by
+  the Free Software Foundation, either version 3 of the License, or
+  (at your option) any later version.
+
+  This program is distributed in the hope that it will be useful,
+  but WITHOUT ANY WARRANTY; without even the implied warranty of
+  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+  GNU General Public License for more details.
+
+  You should have received a copy of the GNU General Public License
+  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+<program>  Copyright (C) <year>  <name of author>
+This program comes with ABSOLUTELY NO WARRANTY; for details type 'show w'.
+This is free software, and you are welcome to redistribute it
+under certain conditions; type 'show c' for details.
+
+The hypothetical commands 'show w' and 'show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+
+--------------------------------------------------------------------------------
+
+      GNU LESSER GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies
+of this license document, but changing it is not allowed.
+
+
+This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+"The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+
+You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+
+If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+  a) under this License, provided that you make a good faith effort to
+  ensure that, in the event an Application does not supply the
+  function or data, the facility still operates, and performs
+  whatever part of its purpose remains meaningful, or
+
+  b) under the GNU GPL, with none of the additional permissions of
+  this License applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+
+The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+  a) Give prominent notice with each copy of the object code that the
+  Library is used in it and that the Library and its use are
+  covered by this License.
+
+  b) Accompany the object code with a copy of the GNU GPL and this license
+  document.
+
+4. Combined Works.
+
+You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+  a) Give prominent notice with each copy of the Combined Work that
+  the Library is used in it and that the Library and its use are
+  covered by this License.
+
+  b) Accompany the Combined Work with a copy of the GNU GPL and this license
+  document.
+
+  c) For a Combined Work that displays copyright notices during
+  execution, include the copyright notice for the Library among
+  these notices, as well as a reference directing the user to the
+  copies of the GNU GPL and this license document.
+
+  d) Do one of the following:
+
+      0) Convey the Minimal Corresponding Source under the terms of this
+      License, and the Corresponding Application Code in a form
+      suitable for, and under terms that permit, the user to
+      recombine or relink the Application with a modified version of
+      the Linked Version to produce a modified Combined Work, in the
+      manner specified by section 6 of the GNU GPL for conveying
+      Corresponding Source.
+
+      1) Use a suitable shared library mechanism for linking with the
+      Library.  A suitable mechanism is one that (a) uses at run time
+      a copy of the Library already present on the user's computer
+      system, and (b) will operate properly with a modified version
+      of the Library that is interface-compatible with the Linked
+      Version.
+
+  e) Provide Installation Information, but only if you would otherwise
+  be required to provide such information under section 6 of the
+  GNU GPL, and only to the extent that such information is
+  necessary to install and execute a modified version of the
+  Combined Work produced by recombining or relinking the
+  Application with a modified version of the Linked Version. (If
+  you use option 4d0, the Installation Information must accompany
+  the Minimal Corresponding Source and Corresponding Application
+  Code. If you use option 4d1, you must provide the Installation
+  Information in the manner specified by section 6 of the GNU GPL
+  for conveying Corresponding Source.)
+
+5. Combined Libraries.
+
+You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+  a) Accompany the combined library with a copy of the same work based
+  on the Library, uncombined with any other library facilities,
+  conveyed under the terms of this License.
+
+  b) Give prominent notice with the combined library that part of it
+  is a work based on the Library, and explaining where to find the
+  accompanying uncombined form of the same work.
+
+6. Revised Versions of the GNU Lesser General Public License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
+
```

### Comparing `PyProcar-5.6.6/PKG-INFO` & `PyProcar-6.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1
-Name: PyProcar
-Version: 5.6.6
-Summary: A Python library for electronic structure pre/post-processing. 
-Home-page: https://github.com/romerogroup/pyprocar
-Author: Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
-Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
-License: LICENSE.txt
-Download-URL: https://github.com/romerogroup/pyprocar/archive/5.6.5.tar.gz
-Platform: UNKNOWN
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: PyProcar
+Version: 6.0.0
+Summary: A Python library for electronic structure pre/post-processing. 
+Home-page: https://github.com/romerogroup/pyprocar
+Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
+Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
+License: LICENSE
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz
+Platform: UNKNOWN
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+UNKNOWN
+
```

### Comparing `PyProcar-5.6.6/PyProcar.egg-info/PKG-INFO` & `PyProcar-6.0.0/PyProcar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1
-Name: PyProcar
-Version: 5.6.6
-Summary: A Python library for electronic structure pre/post-processing. 
-Home-page: https://github.com/romerogroup/pyprocar
-Author: Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
-Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
-License: LICENSE.txt
-Download-URL: https://github.com/romerogroup/pyprocar/archive/5.6.5.tar.gz
-Platform: UNKNOWN
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: PyProcar
+Version: 6.0.0
+Summary: A Python library for electronic structure pre/post-processing. 
+Home-page: https://github.com/romerogroup/pyprocar
+Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
+Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
+License: LICENSE
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz
+Platform: UNKNOWN
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+UNKNOWN
+
```

### Comparing `PyProcar-5.6.6/README.md` & `PyProcar-6.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-[![PyPI version](https://badge.fury.io/py/pyprocar.svg)](https://badge.fury.io/py/pyprocar)
-[![conda-forge version](https://img.shields.io/conda/v/conda-forge/pyprocar.svg?label=conda-forge&colorB=027FD5)](https://anaconda.org/conda-forge/pyprocar)
-[![Build Status](https://travis-ci.org/romerogroup/pyprocar.svg?branch=master)](https://travis-ci.org/romerogroup/pyprocar)
-[![HitCount](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar.svg)](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/pyprocar)
-
-PyProcar
-===========
-
-PyProcar is a robust, open-source Python library used for pre- and post-processing of the electronic structure data coming from DFT calculations. PyProcar provides a set of functions that manage data obtained from the PROCAR format. Basically, the PROCAR format is a projection of the Kohn-Sham states over atomic orbitals. That projection is performed to every k-point in the considered mesh, every energy band and every atom. PyProcar is capable of performing a multitude of tasks including plotting plain and spin/atom/orbital projected band structures and Fermi surfaces- both in 2D and 3D, Fermi velocity plots, unfolding bands of a super  cell, comparing band structures from multiple DFT calculations, plotting partial density of states and generating a k-path for a given crystal structure.
-
-Currently supports:
-
-1. VASP
-2. Elk
-3. Quantum Espresso
-4. Abinit
-5. Lobster
-
-![](welcome.png)
-
-Documentation
--------------
-
-https://romerogroup.github.io/pyprocar/
-
-Developers
-------------
-Francisco Muñoz <br />
-Aldo Romero <br />
-Sobhit Singh <br />
-Uthpala Herath <br />
-Pedram Tavadze <br />
-Eric Bousquet <br />
-Xu He <br />
-Reese Boucher <br />
-Logan Lang <br />
-Freddy Farah <br />
-
-
-How to cite
------------
-If you have used PyProcar in your work, please cite:
-
-[Uthpala Herath, Pedram Tavadze, Xu He, Eric Bousquet, Sobhit Singh, Francisco Muñoz, and Aldo H. Romero. "PyProcar: A Python library for electronic structure pre/post-processing". Computer Physics Communications 251 (2020): 107080.](https://www.sciencedirect.com/science/article/pii/S0010465519303935)
-
-Thank you.
-
-BibTex:
-
-    @article{HERATH2020107080,
-    title = "PyProcar: A Python library for electronic structure pre/post-processing",
-    journal = "Computer Physics Communications",
-    volume = "251",
-    pages = "107080",
-    year = "2020",
-    issn = "0010-4655",
-    doi = "https://doi.org/10.1016/j.cpc.2019.107080",
-    url = "http://www.sciencedirect.com/science/article/pii/S0010465519303935",
-    author = "Uthpala Herath and Pedram Tavadze and Xu He and Eric Bousquet and Sobhit Singh and Francisco Muñoz and Aldo H. Romero",
-    keywords = "DFT, Bandstructure, Electronic properties, Fermi-surface, Spin texture, Python, Condensed matter",
-    }
-
-Mailing list
--------------
-Please post your questions on our forum.
-
-https://groups.google.com/d/forum/pyprocar
-
-Dependencies
-------------
-matplotlib <br />
-numpy <br />
-scipy <br />
-seekpath <br />
-ase <br />
-scikit-image <br />
-pychemia <br />
-pyvista <br />
-
-Installation
-------------
-
-with pip:
-
-	pip install pyprocar
-
-with conda:
-
-    conda install -c conda-forge pyprocar
-
-Usage
------
-Typical use is as follows
-
-    import pyprocar
-    pyprocar.bandsplot('PROCAR',outcar='OUTCAR',mode='plain',code='vasp')
-
-Refer to the documentation for further details.
-
-Stand-alone mode:
-
-    procar.py -h
-
-will bring a help menu.
-
-Changelog
---------------
-
-v5.6.4 May 6th, 2021 -- Updates to Fermi surface plotter. <br />
-v5.6.3 Mar 5th, 2021 -- QE and elk bug fixes. <br />
-v5.6.2 Jan 11th, 2021 -- Updates and bugfixes to fermi surface and dos plotter. <br />
-v5.6.1 Dec 7th, 2020 -- Fixed bug in PyProcar.cat() for merging parallel Abinit files for spin polarized calculations. Converted units Ha to eV. <br />
-v5.6.0 Nov 30th, 2020 -- Repairs PROCAR file by default. Set flag repair=False to disable. <br />
-v5.5.8 Nov 24th, 2020 -- Updates to parametric band structure plotting. Ability to change linewidths with ``linewidth`` flag. <br />
-v5.4.4 Oct 23rd, 2020 -- Updates to DOS plotting, Fermi3D and bxsf parser and other bugfixes. <br />
-v5.5.2 July 27th, 2020 -- Updated spin colinear calculations for Quantum Espresso and Lobster codes. <br />
-v5.4.3 July 25th, 2020 -- Bug fixes in stand-alone version and updates to bandgap calculation. <br />
-v5.4.0 Jun 17th, 2020 -- Improved 3D Fermi Surface plotter, added support for Quantum Espresso, conda support.  <br />
-v5.3.3 May 22nd, 2020 -- Added DOS plotting feature. <br />
-v5.2.1 May 11th, 2020 -- Bugfixes in pyprocar.cat and improving comparison method. <br />
-v5.2.0 Apr 21st, 2020 -- Added spin colinear plotting feature for Elk calculations and a method to plot spin up and spin down plots separately without the need to filter the PROCAR file. <br />
-v5.1.9 Apr 14th, 2020 -- Added feature to filter colinear spins in pyprocar.filter(). <br />
-v5.1.8 Mar 27th, 2020 -- Fix iband reading error due to vasp incorrectly writting iband>999. <br />
-v5.1.5 Mar 8th, 2020 -- Fixed summation issues in ElkParser. <br />
-v5.1.4 Mar 7th, 2020 -- Added new class for parsing Abinit data.<br />
-v5.1.3 Mar 5th, 2020 -- Fixed Abinit PROCAR formatting issues in PyProcar cat function.<br />
-v5.1.1 Mar 5th, 2020 -- Removed bandscompare() due to redundancy with exportplt.<br />
-v5.1.0 Mar 4th, 2020 -- Elk implementation.<br />
-v5.0.1 Mar 2nd, 2020 -- Added orbital header array for newer version of VASP.<br />
-v5.0.0 Mar 1st, 2020 -- Added discontinuous band-plotting feature and other improvements. <br />
-v4.1.4 Feb 28th, 2020 -- Added option to convert k-points between reduced and cartesian when OUTCAR is supplied. <br />
-v4.1.3 Feb 27th, 2020 -- Renormalize alpha values in band unfolder for values > 1. <br />
-v4.1.2 Feb 24th, 2020 -- Bug fixes in band unfolder. <br />
-v4.1.1 Feb 12th, 2020 -- Added feature to compare two parametric plots with colormaps in bandscompare.<br />
-v4.1.0 Jan 10th, 2020 -- Added feature to export plots as matplotlib.pyplot objects for further processing through matplotlib options. <br />
-v4.0.4 Dec 6th, 2019 -- Added command-line compatibility to standalone version and better Latex rendering.<br />
-v4.0.1 Nov 17th, 2019 -- Added feature to filter k-points. <br />
-v4.0.0 Nov 6th, 2019 -- Various bug fixes. Release of standalone version. Updated documentation.<br />
-v3.9.2 Oct 4, 2019 -- Fixed bug in 2D Kmesh generator. <br />
-v3.9.1 Sep 15, 2019 -- Fixed unfold spin polarized eigenvalue bug and spin up/down band energy error in unfolding.<br />
-v3.9.0 Sep 12, 2019 -- Fixed spin polarized band unfolding.  <br />
-v3.8.9 Sep 9, 2019 -- Added bbox_inches='tight' for savefig.<br />
-v3.8.8 Jul 24, 2019 -- Fixed ambiguity in spin flag. <br />
-v3.8.7 Jul 21, 2019 -- Fixed bug in K-mesh generator. <br />
-v3.8.6 Jun 26, 2019 -- Bug fixes in band unfolding Fermi shift energy and band structure labels for Fermi shifts. <br />
-v3.8.5 Jun 13, 2019 -- Bug fixes in Fermi surface plotting. <br />
-v3.8.4 Jun 11, 2019 -- Fixed parsing old PROCAR format. <br />
-v3.8.3 Jun 05, 2019 -- Updated parsing for PROCAR with phase. <br />
-v3.8.2 Jun 05, 2019 -- Updated docs. <br />
-v3.8.1 Jun 05, 2019 -- Updated reading from gzip for binary data. Increased parsing speed when phase factors are present. <br />
-v3.71 Jun 05, 2019 -- More bug fixes. <br />
-v3.7 Jun 04, 2019 -- Bug fixes for Fermi surface.<br />
-v3.6 Jun 04, 2019 -- Added 3D Fermi surface utility.<br />
-v3.5 May 22, 2019 -- added automatic high symmetry point labeling from KPOINTS file.<br />
-v3.4 May 21, 2019 -- Bug fixes for plotting and added capability to plot meta-GGA. <br />
-v3.3 Mar 19, 2019 -- Added band unfolder. <br />
-v3.2 Nov 26, 2018 -- Moved project to romerogroup.<br />
-v3.1 Sep 19, 2018 -- Minor bug fixes. <br />
-v3.0 Sep 17, 2018 -- Added method to compare two PROCARs. Moved to Python3. <br />
-v2.9 Jul 29,2018 -- Created PyProcar Mailing list.<br />
-v2.8 May 23,2018 -- Fixed procar.cat()<br />
-v2.7 May 18,2018 -- Fixed out-of-bounds error in k path generator.<br />
-v2.6 May 18,2018 -- Fixed more issues with fermi2D<br />
-v2.5 May 18.2018 -- Fixed issue with Vector<br />
-v2.4 May 18,2018 -- Fixed minor issues with fermi2D and procarsymmetry<br />
-v2.3 May 17,2018 -- Added k path generator.<br />
-v2.2 May 14,2018 -- Updated documentation.<br />
-v2.1 Apr 03,2018 -- Fixed issue with input arguments when using OUTCAR as an input <br />
-v2.0 Mar 21,2018 -- Created PyProcar package version with added support to Abinit. <br />
-v0.1.0, June 10, 2013 -- Initial release.<br />
+[![PyPI version](https://badge.fury.io/py/pyprocar.svg)](https://badge.fury.io/py/pyprocar)
+[![conda-forge version](https://img.shields.io/conda/v/conda-forge/pyprocar.svg?label=conda-forge&colorB=027FD5)](https://anaconda.org/conda-forge/pyprocar)
+[![Build Status](https://travis-ci.org/romerogroup/pyprocar.svg?branch=master)](https://travis-ci.org/romerogroup/pyprocar)
+[![HitCount](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar.svg)](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyprocar)
+
+PyProcar
+===========
+
+PyProcar is a robust, open-source Python library used for pre- and post-processing of the electronic structure data coming from DFT calculations. PyProcar provides a set of functions that manage data obtained from the PROCAR format. Basically, the PROCAR format is a projection of the Kohn-Sham states over atomic orbitals. That projection is performed to every k-point in the considered mesh, every energy band and every atom. PyProcar is capable of performing a multitude of tasks including plotting plain and spin/atom/orbital projected band structures and Fermi surfaces- both in 2D and 3D, Fermi velocity plots, unfolding bands of a super  cell, comparing band structures from multiple DFT calculations, plotting partial density of states and generating a k-path for a given crystal structure.
+
+Currently supports:
+
+1. VASP
+2. Elk (Stll in development)
+3. Quantum Espresso
+4. Abinit (DOS Stll in development)
+5. Lobster (Stll in development)
+
+![](welcome.png)
+
+Documentation
+-------------
+
+https://romerogroup.github.io/pyprocar/
+
+Developers
+------------
+Francisco Muñoz <br />
+Aldo Romero <br />
+Sobhit Singh <br />
+Uthpala Herath <br />
+Pedram Tavadze <br />
+Eric Bousquet <br />
+Xu He <br />
+Reese Boucher <br />
+Logan Lang <br />
+Freddy Farah <br />
+
+
+How to cite
+-----------
+If you have used PyProcar in your work, please cite:
+
+[Uthpala Herath, Pedram Tavadze, Xu He, Eric Bousquet, Sobhit Singh, Francisco Muñoz, and Aldo H. Romero. "PyProcar: A Python library for electronic structure pre/post-processing". Computer Physics Communications 251 (2020): 107080.](https://www.sciencedirect.com/science/article/pii/S0010465519303935)
+
+Thank you.
+
+BibTex:
+
+    @article{HERATH2020107080,
+    title = "PyProcar: A Python library for electronic structure pre/post-processing",
+    journal = "Computer Physics Communications",
+    volume = "251",
+    pages = "107080",
+    year = "2020",
+    issn = "0010-4655",
+    doi = "https://doi.org/10.1016/j.cpc.2019.107080",
+    url = "http://www.sciencedirect.com/science/article/pii/S0010465519303935",
+    author = "Uthpala Herath and Pedram Tavadze and Xu He and Eric Bousquet and Sobhit Singh and Francisco Muñoz and Aldo H. Romero",
+    keywords = "DFT, Bandstructure, Electronic properties, Fermi-surface, Spin texture, Python, Condensed matter",
+    }
+
+Mailing list
+-------------
+Please post your questions on our forum.
+
+https://groups.google.com/d/forum/pyprocar
+
+Dependencies
+------------
+matplotlib <br />
+numpy <br />
+scipy <br />
+seekpath <br />
+ase <br />
+scikit-image <br />
+pychemia <br />
+pyvista <br />
+
+Installation
+------------
+
+with pip:
+
+	pip install pyprocar
+
+with conda:
+
+    conda install -c conda-forge pyprocar
+
+Usage
+-----
+Typical use is as follows
+
+    import pyprocar
+    pyprocar.bandsplot('PROCAR',outcar='OUTCAR',mode='plain',code='vasp')
+
+Refer to the documentation for further details.
+
+Stand-alone mode:
+
+    procar.py -h
+
+will bring a help menu.
+
+Changelog
+--------------
+v6.0.0 May 6th, 2021 -- Directory changes. This version is not backwards compatible. <br />
+v5.6.4 May 6th, 2021 -- Updates to Fermi surface plotter. <br />
+v5.6.3 Mar 5th, 2021 -- QE and elk bug fixes. <br />
+v5.6.2 Jan 11th, 2021 -- Updates and bugfixes to fermi surface and dos plotter. <br />
+v5.6.1 Dec 7th, 2020 -- Fixed bug in PyProcar.cat() for merging parallel Abinit files for spin polarized calculations. Converted units Ha to eV. <br />
+v5.6.0 Nov 30th, 2020 -- Repairs PROCAR file by default. Set flag repair=False to disable. <br />
+v5.5.8 Nov 24th, 2020 -- Updates to parametric band structure plotting. Ability to change linewidths with ``linewidth`` flag. <br />
+v5.4.4 Oct 23rd, 2020 -- Updates to DOS plotting, Fermi3D and bxsf parser and other bugfixes. <br />
+v5.5.2 July 27th, 2020 -- Updated spin colinear calculations for Quantum Espresso and Lobster codes. <br />
+v5.4.3 July 25th, 2020 -- Bug fixes in stand-alone version and updates to bandgap calculation. <br />
+v5.4.0 Jun 17th, 2020 -- Improved 3D Fermi Surface plotter, added support for Quantum Espresso, conda support.  <br />
+v5.3.3 May 22nd, 2020 -- Added DOS plotting feature. <br />
+v5.2.1 May 11th, 2020 -- Bugfixes in pyprocar.cat and improving comparison method. <br />
+v5.2.0 Apr 21st, 2020 -- Added spin colinear plotting feature for Elk calculations and a method to plot spin up and spin down plots separately without the need to filter the PROCAR file. <br />
+v5.1.9 Apr 14th, 2020 -- Added feature to filter colinear spins in pyprocar.filter(). <br />
+v5.1.8 Mar 27th, 2020 -- Fix iband reading error due to vasp incorrectly writting iband>999. <br />
+v5.1.5 Mar 8th, 2020 -- Fixed summation issues in ElkParser. <br />
+v5.1.4 Mar 7th, 2020 -- Added new class for parsing Abinit data.<br />
+v5.1.3 Mar 5th, 2020 -- Fixed Abinit PROCAR formatting issues in PyProcar cat function.<br />
+v5.1.1 Mar 5th, 2020 -- Removed bandscompare() due to redundancy with exportplt.<br />
+v5.1.0 Mar 4th, 2020 -- Elk implementation.<br />
+v5.0.1 Mar 2nd, 2020 -- Added orbital header array for newer version of VASP.<br />
+v5.0.0 Mar 1st, 2020 -- Added discontinuous band-plotting feature and other improvements. <br />
+v4.1.4 Feb 28th, 2020 -- Added option to convert k-points between reduced and cartesian when OUTCAR is supplied. <br />
+v4.1.3 Feb 27th, 2020 -- Renormalize alpha values in band unfolder for values > 1. <br />
+v4.1.2 Feb 24th, 2020 -- Bug fixes in band unfolder. <br />
+v4.1.1 Feb 12th, 2020 -- Added feature to compare two parametric plots with colormaps in bandscompare.<br />
+v4.1.0 Jan 10th, 2020 -- Added feature to export plots as matplotlib.pyplot objects for further processing through matplotlib options. <br />
+v4.0.4 Dec 6th, 2019 -- Added command-line compatibility to standalone version and better Latex rendering.<br />
+v4.0.1 Nov 17th, 2019 -- Added feature to filter k-points. <br />
+v4.0.0 Nov 6th, 2019 -- Various bug fixes. Release of standalone version. Updated documentation.<br />
+v3.9.2 Oct 4, 2019 -- Fixed bug in 2D Kmesh generator. <br />
+v3.9.1 Sep 15, 2019 -- Fixed unfold spin polarized eigenvalue bug and spin up/down band energy error in unfolding.<br />
+v3.9.0 Sep 12, 2019 -- Fixed spin polarized band unfolding.  <br />
+v3.8.9 Sep 9, 2019 -- Added bbox_inches='tight' for savefig.<br />
+v3.8.8 Jul 24, 2019 -- Fixed ambiguity in spin flag. <br />
+v3.8.7 Jul 21, 2019 -- Fixed bug in K-mesh generator. <br />
+v3.8.6 Jun 26, 2019 -- Bug fixes in band unfolding Fermi shift energy and band structure labels for Fermi shifts. <br />
+v3.8.5 Jun 13, 2019 -- Bug fixes in Fermi surface plotting. <br />
+v3.8.4 Jun 11, 2019 -- Fixed parsing old PROCAR format. <br />
+v3.8.3 Jun 05, 2019 -- Updated parsing for PROCAR with phase. <br />
+v3.8.2 Jun 05, 2019 -- Updated docs. <br />
+v3.8.1 Jun 05, 2019 -- Updated reading from gzip for binary data. Increased parsing speed when phase factors are present. <br />
+v3.71 Jun 05, 2019 -- More bug fixes. <br />
+v3.7 Jun 04, 2019 -- Bug fixes for Fermi surface.<br />
+v3.6 Jun 04, 2019 -- Added 3D Fermi surface utility.<br />
+v3.5 May 22, 2019 -- added automatic high symmetry point labeling from KPOINTS file.<br />
+v3.4 May 21, 2019 -- Bug fixes for plotting and added capability to plot meta-GGA. <br />
+v3.3 Mar 19, 2019 -- Added band unfolder. <br />
+v3.2 Nov 26, 2018 -- Moved project to romerogroup.<br />
+v3.1 Sep 19, 2018 -- Minor bug fixes. <br />
+v3.0 Sep 17, 2018 -- Added method to compare two PROCARs. Moved to Python3. <br />
+v2.9 Jul 29,2018 -- Created PyProcar Mailing list.<br />
+v2.8 May 23,2018 -- Fixed procar.cat()<br />
+v2.7 May 18,2018 -- Fixed out-of-bounds error in k path generator.<br />
+v2.6 May 18,2018 -- Fixed more issues with fermi2D<br />
+v2.5 May 18.2018 -- Fixed issue with Vector<br />
+v2.4 May 18,2018 -- Fixed minor issues with fermi2D and procarsymmetry<br />
+v2.3 May 17,2018 -- Added k path generator.<br />
+v2.2 May 14,2018 -- Updated documentation.<br />
+v2.1 Apr 03,2018 -- Fixed issue with input arguments when using OUTCAR as an input <br />
+v2.0 Mar 21,2018 -- Created PyProcar package version with added support to Abinit. <br />
+v0.1.0, June 10, 2013 -- Initial release.<br />
```

### Comparing `PyProcar-5.6.6/pyprocar/core/isosurface.py` & `PyProcar-6.0.0/pyprocar/core/isosurface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,482 +1,447 @@
-from .surface import Surface
-import numpy as np
-from scipy import interpolate
-from skimage import measure
-
-__author__ = "Pedram Tavadze"
-__maintainer__ = "Pedram Tavadze"
-__email__ = "petavazohi@mail.wvu.edu"
-__date__ = "March 31, 2020"
-
-
-class Isosurface(Surface):
-    def __init__(
-            self,
-            XYZ=None,
-            V=None,
-            isovalue=None,
-            V_matrix=None,
-            algorithm='lewiner',
-            interpolation_factor=1,
-            padding=None,
-            transform_matrix=None,
-            boundaries=None,
-    ):
-        """
-        This class contains a surface that finds all the poins correcponding
-        to the following equation
-        V(X,Y,Z) = f
-
-        Parameters
-        ----------
-        XYZ : TYPE, list of lists of floats, (n,3)
-            DESCRIPTION. a list of coordinates [[x1,y1,z1],[x2,y2,z2],...]
-            corresponding V
-        V : TYPE, list of floats, (n,)
-            DESCRIPTION. a list of values [V1,V2,...] corresponding to XYZ
-            XYZ[0] >>> V[0]
-            XYZ[1] >>> V[1]
-        isovalue : TYPE, float
-            DESCRIPTION. The constant value of the surface (f)
-        V_matrix : TYPE, float (nx,ny,nz)
-            DESCRIPTION. one can present V_matrix instead of XYZ and V.
-            V_matrix is a matrix representation of XYZ and V together. This
-            matrix is generated if XYZ and V are provided.
-        algorithm : TYPE, string
-            DESCRIPTION. The default is 'lewiner'. The algorithm used to find the isosurface, This
-            function used scikit-image to find the isosurface. possibilities
-            ['classic','lewiner']
-        interpolation_factor : TYPE, int
-            DESCRIPTION. The default is 1. This module uses Fourier Transform
-            interpolation. interpolation factor will increase the grid points
-            in each direction by a this factor, the dafault is set to 1
-        padding : TYPE, list of float (3,)
-            DESCRIPTION. padding is used for periodic datasets such as bands in
-            a solid state calculation. e.g. The 1st BZ is not covered fully so
-            one might want to pad the matrix with wrap(look at padding in
-            numpy for wrap), afterwards one has to clip the surface to the
-            first BZ. easily doable using pyvista of trimesh
-            padding goes as follows np.pad(self.eigen_matrix,
-                              ((padding[0]/2, padding[0]/2),
-                              (padding[1]/2, padding[1]/2)
-                              (padding[2]/2, padding[2])),
-                              "wrap")
-            In other words it creates a super cell withpadding
-        transform_matrix : TYPE, (3,3) float
-            DESCRIPTION. applies an transformation to the vertices VERTS_prime=T*VERTS
-        boundaries : TYPE, pyprocar surface
-            DESCRIPTION. The default is None. The boundaries in which the isosurface will be clipped with
-            for example the first brillouin zone
-
-        """
-
-        self.XYZ = np.array(XYZ)
-        self.V = V
-        self.isovalue = isovalue
-        self.V_matrix = V_matrix
-        self.algorithm = algorithm
-        self.padding = padding
-        self.interpolation_factor = interpolation_factor
-        self.transform_matrix = transform_matrix
-        self.boundaries = boundaries
-        
-        if self.algorithm not in ['classic', 'lewiner']:
-
-            print(
-                "The algorithm chose has to be from ['classic','lewiner'], automtically choosing 'lewiner'"
-            )
-            self.algorithm = "lewiner"
-
-        if self.V_matrix is None:
-            self.V_matrix = map2matrix(self.XYZ, self.V)
-
-        if self.padding is None:
-            
-            self.padding = [self.nX*2 // 2, self.nY*2 // 2, self.nZ*2 // 2]
-
-        else:
-            
-            self.padding = [
-                self.nX // 2 * padding[0],
-                self.nY // 2 * padding[1],
-                self.nZ // 2 * padding[2],
-            ]
-
-        verts, faces, normals, values = self._get_isosurface(interpolation_factor)
-
-        if verts is not None and faces is not None:
-            if transform_matrix is not None:
-                verts = np.dot(verts,  transform_matrix)
-            """
-            Python, unlike statically typed languages such as Java, allows complete
-            freedom when calling methods during object initialization. However, 
-            standard object-oriented principles apply to Python classes using deep 
-            inheritance hierarchies. Therefore the developer has responsibility for 
-            ensuring that objects are properly initialized when there are multiple 
-            __init__ methods that need to be called.
-            For this reason I will make one temporary surface and from there I will
-            using the other surface provided.
-            """
-
-            if boundaries is not None:
-                suprecell_surface = Surface(
-                    verts=verts, faces=faces, face_normals=normals
-                )
-                if not np.isnan(suprecell_surface.pyvista_obj.points[0, 0]):
-                    verts, faces = self.clip(suprecell_surface, boundaries)
-                # verts, faces = self.clip(suprecell_surface, boundaries)
-
-        
-   
-        Surface.__init__(self, verts=verts, faces=faces, face_normals=normals)
-
-    def clip(self, S1, S2):
-        """
-        This function clips S1 using the boundaries of S2 and returns
-
-        Parameters
-        ----------
-        S1 : TYPE pyprocar surface
-            DESCRIPTION.
-        S2 : TYPE pyprocar surface
-            DESCRIPTION.
-
-        Returns
-        -------
-        verts,faces
-
-        """
-
-        for iface in range(len(S2.faces)):
-            normal = S2.face_normals[iface]
-
-            center = np.average(S2.verts[S2.faces[iface]], axis=0)
-
-            S1.pyvista_obj.clip(origin=center, normal=normal, inplace=True)
-
-        faces = []
-        courser = 0
-        for i in range(S1.pyvista_obj.n_faces):
-            npoints = S1.pyvista_obj.faces[courser]
-            face = []
-            courser += 1
-            for ipoint in range(npoints):
-                face.append(S1.pyvista_obj.faces[courser])
-                courser += 1
-            faces.append(face)
-
-        return S1.pyvista_obj.points, faces
-
-    @property
-    def X(self):
-        """
-
-
-        Returns
-        -------
-        TYPE numpy array
-            DESCRIPTION. list of grids in X direction
-
-        """
-        return np.unique(self.XYZ[:, 0])
-
-    @property
-    def Y(self):
-        """
-
-
-        Returns
-        -------
-        TYPE numpy array
-            DESCRIPTION. list of grids in Y direction
-        """
-        return np.unique(self.XYZ[:, 1])
-
-    @property
-    def Z(self):
-        """
-
-
-        Returns
-        -------
-        TYPE numpy array
-            DESCRIPTION. list of grids in Z direction
-
-        """
-        return np.unique(self.XYZ[:, 2])
-
-    @property
-    def dxyz(self):
-        """
-
-
-        Returns
-        -------
-        list
-            DESCRIPTION. length between points in each direction
-
-        """
-        dx = np.abs(self.X[-1] - self.X[-2])
-        dy = np.abs(self.Y[-1] - self.Y[-2])
-        dz = np.abs(self.Z[-1] - self.Z[-2])
-        return [dx, dy, dz]
-
-    @property
-    def nX(self):
-        """
-
-
-        Returns
-        -------
-        TYPE int
-            DESCRIPTION. number of points in the grid in X direction
-
-        """
-        return len(self.X)
-
-    @property
-    def nY(self):
-        """
-
-
-        Returns
-        -------
-        TYPE int
-            DESCRIPTION. number of points in the grid in Y direction
-
-        """
-        return len(self.Y)
-
-    @property
-    def nZ(self):
-        """
-
-
-        Returns
-        -------
-        TYPE int
-            DESCRIPTION. number of points in the grid in Z direction
-
-        """
-        return len(self.Z)
-
-    @property
-    def surface_boundaries(self):
-        """
-        This function tries to find the isosurface using no interpolation to find the
-        correct positions of the surface to be able to shift to the interpolated one
-        to the correct position
-
-        Returns
-        -------
-        list of tuples
-            DESCRIPTION. [(mins[0],maxs[0]),(mins[1],maxs[1]),(mins[2],maxs[2])]
-
-        """
-
-        padding_x = self.padding[0]
-        padding_y = self.padding[1]
-        padding_z = self.padding[2]
-
-        eigen_matrix = np.pad(
-            self.V_matrix,
-            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
-            "wrap",
-        )
-        try:
-            verts, faces, normals, values = measure.marching_cubes_lewiner(
-                eigen_matrix, self.isovalue
-            )
-            for ix in range(3):
-                verts[:, ix] -= verts[:, ix].min()
-                verts[:, ix] -= (
-                    verts[:, ix].max() - verts[:, ix].min()
-                ) / 2  # +self.origin[ix]
-                verts[:, ix] *= self.dxyz[ix]
-            mins = verts.min(axis=0)
-            maxs = verts.max(axis=0)
-
-            return [(mins[0], maxs[0]), (mins[1], maxs[1]), (mins[2], maxs[2])]
-        except:
-            return None
-
-    def _get_isosurface(self, interp_factor=1):
-        """
-
-
-        Parameters
-        ----------
-        interp_factor : TYPE, optional
-            DESCRIPTION. The default is 1.
-
-        Returns
-        -------
-        TYPE
-            DESCRIPTION. verts
-        TYPE
-            DESCRIPTION. faces
-        TYPE
-            DESCRIPTION. normals
-        TYPE
-            DESCRIPTION. vlues
-
-        """
-
-        # Amount of kpoints needed to add on to fully sample 1st BZ
-
-        padding_x = self.padding[0]
-        padding_y = self.padding[1]
-        padding_z = self.padding[2]
-
-        eigen_matrix = np.pad(
-            self.V_matrix,
-            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
-            "wrap",
-        )
-
-        bnd = self.surface_boundaries
-
-        if interp_factor != 1:
-            # Fourier interpolate the mapped function E(x,y,z)
-
-            eigen_matrix = fft_interpolate(eigen_matrix, interp_factor)
-
-            # after the FFT we loose the center of the BZ, using numpy roll we
-            # bring back the center of the BZ
-            # eigen_matrix = np.roll(eigen_matrix, 4  ,
-            #     axis=[0, 1, 2])
-
-        try:
-
-            verts, faces, normals, values = measure.marching_cubes_lewiner(
-                eigen_matrix, self.isovalue
-            )
-
-        except BaseException:
-            print("No isosurface for this band")
-            return None, None, None, None
-        # recenter
-
-        for ix in range(3):
-            
-            if np.any(self.XYZ >= 0.5):
-                verts[:, ix] *= self.dxyz[ix] / interp_factor
-                verts[:, ix] -= 1*self.supercell[ix]
-                # verts[:, ix] -= 1*self.padding[ix]
- 
-                   
-            else:
-                verts[:, ix] -= verts[:, ix].min()
-                verts[:, ix] -= (verts[:, ix].max() -
-                                  verts[:, ix].min()) / 2
-                
-                verts[:, ix] *= self.dxyz[ix] / interp_factor
-
-                if bnd is not None and interp_factor != 1:
-                    verts[:, ix] -= (verts[:, ix].min() - bnd[ix][0])
-                    
-                    
-                    
-                    
-                    
-
-            # verts[:, ix] *= self.dxyz[ix] / interp_factor
-
-            # print(self.dxyz)
-
-            # if self.file == "bxsf":
-            #     verts[:, ix] -= 0.5
-            # if bnd is not None and interp_factor != 1:
-            #     print((verts[:, ix].min() - bnd[ix][0]))
-            #     verts[:, ix] -= (verts[:, ix].min() - bnd[ix][0])
-            #     if self.file == "bxsf":
-            #         verts[:, ix] -= 0.50
-
-            #     x_shift = verts[:,0].min() - bnd[0]
-            # y_shift = verts[:,1].min() - bnd[1]
-            # z_shift = verts[:,2].min() - bnd[2]
-
-        # transfare from fraction to cartesian
-        # verts = np.dot(verts, self.reciprocal_)
-        # new_faces = np.zeros(shape=(len(faces), 4))
-        # new_faces[:, 0] = 3
-        # new_faces[:, 1:] = faces
-        # faces = new_faces
-        return verts, faces, normals, values
-
-
-def map2matrix(XYZ, V):
-    """
-    mapps an Irregular grid to a regular grid
-
-    Parameters
-    ----------
-    XYZ : TYPE
-        DESCRIPTION.
-    V : TYPE
-        DESCRIPTION.
-
-    Returns
-    -------
-    mapped_func : TYPE
-        DESCRIPTION.
-
-    """
-    XYZ = XYZ
-    V = V
-
-    X = np.unique(XYZ[:, 0])
-    Y = np.unique(XYZ[:, 1])
-    Z = np.unique(XYZ[:, 2])
-
-    mapped_func = np.zeros(shape=(len(X), len(Y), len(Z)))
-    # kpoint_matrix = np.zeros(shape=(len(kx), len(ky), len(kz), 3)) This was added to check if the mesh grid is working
-
-    count = 0
-    for ix in range(len(X)):
-        condition1 = XYZ[:, 0] == X[ix]
-        count += 1
-
-        for iy in range(len(Y)):
-            condition2 = XYZ[:, 1] == Y[iy]
-
-            # print(count)
-            for iz in range(len(Z)):
-
-                condition3 = XYZ[:, 2] == Z[iz]
-                tot_cond = np.all([condition1, condition2, condition3], axis=0)
-                if len(V[tot_cond]) != 0:
-
-                    mapped_func[ix, iy, iz] = V[tot_cond][0]
-                    # kpoint_matrix[ikx, iky, ikz] = [
-                    #     kx[ikx], ky[iky], kz[ikz]]
-                else:
-                    mapped_func[ix, iy, iz] = np.nan
-                    # kpoint_matrix[ikx, iky, ikz] = [np.nan, np.nan, np.nan]
-    return mapped_func
-
-
-def fft_interpolate(function, interpolation_factor=2):
-    """
-    if I = interpolation_factor
-    This function withh recieve f(x,y,z) with dimensions of (nx,ny,nz)
-    and returns f(x,y,z) with dimensions of (nx*I,ny*I,nz*I)
-    """
-
-    eigen_fft = np.fft.fftn(function)
-    shifted_fft = np.fft.fftshift(eigen_fft)
-    nx, ny, nz = np.array(shifted_fft.shape)
-    pad_x = nx * (interpolation_factor - 1) // 2
-    pad_y = ny * (interpolation_factor - 1) // 2
-    pad_z = nz * (interpolation_factor - 1) // 2
-    new_matrix = np.pad(
-        shifted_fft,
-        ((pad_x, pad_x), (pad_y, pad_y), (pad_z, pad_z)),
-        "constant",
-        constant_values=0,
-    )
-
-    new_matrix = np.fft.ifftshift(new_matrix)
-    interpolated = np.real(np.fft.ifftn(new_matrix)) * (interpolation_factor ** 3)
-
-    return interpolated
+__author__ = "Pedram Tavadze and Logan Lang"
+__maintainer__ = "Pedram Tavadze and Logan Lang"
+__email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
+__date__ = "March 31, 2020"
+
+from typing import List
+import numpy as np
+from scipy import interpolate
+from skimage import measure
+import pyvista as pv
+
+from .surface import Surface
+
+class Isosurface(Surface):
+    """
+    This class contains a surface that finds all the points corresponding
+    to the following equation. 
+    V(X,Y,Z) = f
+
+    Parameters
+    ----------
+    XYZ : List of lists of floats, (n,3)
+        XYZ must be between (0.5,0.5]. a list of coordinates [[x1,y1,z1],[x2,y2,z2],...]
+        corresponding V
+    V : TYPE, list of floats, (n,)
+        DESCRIPTION. a list of values [V1,V2,...] corresponding to XYZ
+        XYZ[0] >>> V[0]
+        XYZ[1] >>> V[1]
+    isovalue : float
+        The constant value of the surface (f)
+    V_matrix : float (nx,ny,nz)
+        One can present V_matrix instead of XYZ and V.
+        V_matrix is a matrix representation of XYZ and V together. 
+        This matrix is generated if XYZ and V are provided.
+    algorithm : str
+        The default is 'lewiner'. The algorithm used to find the isosurface, This
+        function used scikit-image to find the isosurface. possibilities
+        ['classic','lewiner']
+    interpolation_factor : int
+        The default is 1. This module uses Fourier Transform
+        interpolation. interpolation factor will increase the grid points
+        in each direction by a this factor, the dafault is set to 1
+    padding : list of float (3,)
+        Padding is used for periodic datasets such as bands in
+        a solid state calculation. e.g. The 1st BZ is not covered fully so
+        one might want to pad the matrix with wrap(look at padding in
+        numpy for wrap), afterwards one has to clip the surface to the
+        first BZ. easily doable using pyvista of trimesh
+        padding goes as follows 
+        
+        .. code-block::
+            :linenos: 
+            
+            np.pad(self.eigen_matrix,
+                    ((padding[0]/2, padding[0]/2),
+                    (padding[1]/2, padding[1]/2)
+                    (padding[2]/2, padding[2])),
+                    "wrap")
+
+        In other words it creates a super cell withpadding
+    transform_matrix : np.ndarray (3,3) float
+        Applies an transformation to the vertices VERTS_prime=T*VERTS
+    boundaries : pyprocar.core.surface
+        The default is None. The boundaries in which the isosurface will be clipped with
+        for example the first brillouin zone
+
+    """
+
+    def __init__(
+            self,
+            XYZ:np.ndarray,
+            V:np.ndarray,
+            isovalue:float,
+            V_matrix=None,
+            algorithm:str='lewiner',
+            interpolation_factor:int=1,
+            padding:List[int]=None,
+            transform_matrix:np.ndarray=None,
+            boundaries=None,
+        ):
+        
+
+        self.XYZ = np.array(XYZ)
+        self.V = V
+        self.isovalue = isovalue
+        self.V_matrix = V_matrix
+        self.algorithm = algorithm
+        self.padding = padding
+        self.supercell = padding 
+        self.interpolation_factor = interpolation_factor
+        self.transform_matrix = transform_matrix
+        self.boundaries = boundaries
+        
+        if self.algorithm not in ['classic', 'lewiner']:
+
+            print(
+                "The algorithm chose has to be from ['classic','lewiner'], automtically choosing 'lewiner'"
+            )
+            self.algorithm = "lewiner"
+
+        if self.V_matrix is None:
+            self.V_matrix = map2matrix(self.XYZ, self.V)
+
+        if self.padding is None:
+            
+            self.padding = [self.nX*2 // 2, self.nY*2 // 2, self.nZ*2 // 2]
+
+        else:
+            
+            self.padding = [
+                self.nX // 2 * padding[0],
+                self.nY // 2 * padding[1],
+                self.nZ // 2 * padding[2],
+            ]
+        
+        verts, faces, normals, values = self._get_isosurface(interpolation_factor)
+        
+
+        
+        if verts is not None and faces is not None:
+            if transform_matrix is not None:
+                verts = np.dot(verts,  transform_matrix)
+                column_of_verts_of_triangles = [3 for _ in range(len(faces[:,0])) ]
+                faces = np.insert(arr = faces,obj=0, values = column_of_verts_of_triangles, axis = 1)
+            """
+            Python, unlike statically typed languages such as Java, allows complete
+            freedom when calling methods during object initialization. However, 
+            standard object-oriented principles apply to Python classes using deep 
+            inheritance hierarchies. Therefore the developer has responsibility for 
+            ensuring that objects are properly initialized when there are multiple 
+            __init__ methods that need to be called.
+            For this reason I will make one temporary surface and from there I will
+            using the other surface provided.
+            """
+
+            if boundaries is not None:
+                supercell_surface = pv.PolyData(var_inp=verts, faces=faces)
+                for normal,center in zip(boundaries.face_normals, boundaries.centers):
+                    supercell_surface.clip(origin=center, normal=normal, inplace=True)
+
+                if len(supercell_surface.points) == 0:
+                    raise Exception("Clippping destroyed mesh.")
+    
+                verts = supercell_surface.points
+                faces = supercell_surface.faces
+
+ 
+        super().__init__(verts=verts, faces=faces)
+
+        return None
+        
+     
+
+    @property
+    def X(self):
+        """
+        Returns the unique x values of the grid
+
+        Returns
+        -------
+        np.ndarray
+            list of grids in X direction
+
+        """
+        return np.unique(self.XYZ[:, 0])
+
+    @property
+    def Y(self):
+        """
+        Returns the unique y values of the grid
+
+        Returns
+        -------
+        np.ndarray
+            List of grids in Y direction
+        """
+        return np.unique(self.XYZ[:, 1])
+
+    @property
+    def Z(self):
+        """
+        Returns the unique z values of the grid
+
+        Returns
+        -------
+        np.ndarray
+            List of grids in Z direction
+
+        """
+        return np.unique(self.XYZ[:, 2])
+
+    @property
+    def dxyz(self):
+        """
+        Returns the spacings of the grid in the x,y,z directions.
+
+        Returns
+        -------
+        List[float]
+            Length between points in each direction
+
+        """
+        dx = np.abs(self.X[-1] - self.X[-2])
+        dy = np.abs(self.Y[-1] - self.Y[-2])
+        dz = np.abs(self.Z[-1] - self.Z[-2])
+        return [dx, dy, dz]
+
+    @property
+    def nX(self):
+        """
+        Returns the number of points in the grid in X direction
+
+        Returns
+        -------
+        int
+            The number of points in the grid in X direction
+
+        """
+        return len(self.X)
+
+    @property
+    def nY(self):
+        """
+        Returns the number of points in the grid in Y direction
+
+        Returns
+        -------
+        int
+            The number of points in the grid in Y direction
+
+        """
+        return len(self.Y)
+
+    @property
+    def nZ(self):
+        """
+        Returns the number of points in the grid in Z direction
+
+        Returns
+        -------
+        int
+            The number of points in the grid in Z direction
+
+        """
+        return len(self.Z)
+
+    @property
+    def surface_boundaries(self):
+        """
+        This function tries to find the isosurface using no interpolation to find the
+        correct positions of the surface to be able to shift to the interpolated one
+        to the correct position
+
+        Returns
+        -------
+        list of tuples
+            DESCRIPTION. [(mins[0],maxs[0]),(mins[1],maxs[1]),(mins[2],maxs[2])]
+
+        """
+
+        padding_x = self.padding[0]
+        padding_y = self.padding[1]
+        padding_z = self.padding[2]
+
+        eigen_matrix = np.pad(
+            self.V_matrix,
+            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
+            "wrap",
+        )
+        try:
+            verts, faces, normals, values = measure.marching_cubes(
+                eigen_matrix, self.isovalue
+            )
+            for ix in range(3):
+                verts[:, ix] -= verts[:, ix].min()
+                verts[:, ix] -= (
+                    verts[:, ix].max() - verts[:, ix].min()
+                ) / 2  # +self.origin[ix]
+                verts[:, ix] *= self.dxyz[ix]
+            mins = verts.min(axis=0)
+            maxs = verts.max(axis=0)
+
+            return [(mins[0], maxs[0]), (mins[1], maxs[1]), (mins[2], maxs[2])]
+        except Exception as e:
+            # print(e)
+            print("No isosurface for this band")
+            return None
+
+    def _get_isosurface(self, interp_factor:float=1):
+        """
+        The helper method will try to find the iso surface by using the marching cubes algorithm
+
+        Parameters
+        ----------
+        interp_factor : float, optional
+            Interpolation factor. The default is 1.
+
+        Returns
+        -------
+        np.ndarray
+            The vertices of the isosurface. verts
+        np.ndarray
+            The faces of the isosurface. faces
+        np.ndarray
+            The normals to the faces of the isosurface. normals
+        np.ndarray
+            The values of the isosurface. values
+
+        """
+
+        # Amount of kpoints needed to add on to fully sample 1st BZ
+
+        padding_x = self.padding[0]
+        padding_y = self.padding[1]
+        padding_z = self.padding[2]
+
+        eigen_matrix = np.pad(
+            self.V_matrix,
+            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
+            "wrap",
+        )
+
+        bnd = self.surface_boundaries
+
+        if interp_factor != 1:
+            # Fourier interpolate the mapped function E(x,y,z)
+
+            eigen_matrix = fft_interpolate(eigen_matrix, interp_factor)
+
+            # after the FFT we loose the center of the BZ, using numpy roll we
+            # bring back the center of the BZ
+            # eigen_matrix = np.roll(eigen_matrix, 4  ,
+            #     axis=[0, 1, 2])
+
+        try:
+            verts, faces, normals, values = measure.marching_cubes(
+                eigen_matrix, self.isovalue
+            )
+
+        except Exception as e:
+            # print(e)
+            print("No isosurface for this band")
+            return None, None, None, None
+            
+        # recenter
+        for ix in range(3):
+            verts[:, ix] -= verts[:, ix].min()
+            verts[:, ix] -= (verts[:, ix].max() -
+                                verts[:, ix].min()) / 2
+            
+            verts[:, ix] *= self.dxyz[ix] / interp_factor
+
+            if bnd is not None and interp_factor != 1:
+                verts[:, ix] -= (verts[:, ix].min() - bnd[ix][0])
+                    
+        return verts, faces, normals, values
+
+
+    
+def map2matrix(XYZ, V):
+    """
+    Maps an Irregular grid to a regular grid
+
+    Parameters
+    ----------
+    XYZ : np.ndarray
+        The points of the irregular grid.
+    V : np.ndarray
+        The values of the irregular grid.
+
+    Returns
+    -------
+    mapped_func : np.ndarray
+        The points of the regular grid.
+
+    """
+    XYZ = XYZ
+    V = V
+
+    X = np.unique(XYZ[:, 0])
+    Y = np.unique(XYZ[:, 1])
+    Z = np.unique(XYZ[:, 2])
+
+    mapped_func = np.zeros(shape=(len(X), len(Y), len(Z)))
+    # kpoint_matrix = np.zeros(shape=(len(kx), len(ky), len(kz), 3)) This was added to check if the mesh grid is working
+
+    count = 0
+    for ix in range(len(X)):
+        condition1 = XYZ[:, 0] == X[ix]
+        count += 1
+
+        for iy in range(len(Y)):
+            condition2 = XYZ[:, 1] == Y[iy]
+
+            # print(count)
+            for iz in range(len(Z)):
+
+                condition3 = XYZ[:, 2] == Z[iz]
+                tot_cond = np.all([condition1, condition2, condition3], axis=0)
+                if len(V[tot_cond]) != 0:
+
+                    mapped_func[ix, iy, iz] = V[tot_cond][0]
+                    # kpoint_matrix[ikx, iky, ikz] = [
+                    #     kx[ikx], ky[iky], kz[ikz]]
+                else:
+                    mapped_func[ix, iy, iz] = np.nan
+                    # kpoint_matrix[ikx, iky, ikz] = [np.nan, np.nan, np.nan]
+    return mapped_func
+
+def fft_interpolate(function, interpolation_factor=2):
+    """
+    This method will interpolate using a Fast-Fourier Transform
+    
+    if I = interpolation_factor
+    This function withh recieve f(x,y,z) with dimensions of (nx,ny,nz)
+    and returns f(x,y,z) with dimensions of (nx*I,ny*I,nz*I)
+
+    Parameters
+    ----------
+    function : np.ndarray
+        The values array to do the interpolation on.
+    interpolation_factor : int, optional
+        Interpolation Factor, by default 2
+
+    Returns
+    -------
+    np.ndarray
+        The interpolated points
+    """
+
+    eigen_fft = np.fft.fftn(function)
+    shifted_fft = np.fft.fftshift(eigen_fft)
+    nx, ny, nz = np.array(shifted_fft.shape)
+    pad_x = nx * (interpolation_factor - 1) // 2
+    pad_y = ny * (interpolation_factor - 1) // 2
+    pad_z = nz * (interpolation_factor - 1) // 2
+    new_matrix = np.pad(
+        shifted_fft,
+        ((pad_x, pad_x), (pad_y, pad_y), (pad_z, pad_z)),
+        "constant",
+        constant_values=0,
+    )
+
+    new_matrix = np.fft.ifftshift(new_matrix)
+    interpolated = np.real(np.fft.ifftn(new_matrix)) * (interpolation_factor ** 3)
+
+    return interpolated
```

### Comparing `PyProcar-5.6.6/pyprocar/elkparser/elkparser.py` & `PyProcar-6.0.0/pyprocar/io/elkparser/elkparser.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-"""
-Created on Fri March 2 2020
-@author: Pedram Tavadze
-
-"""
-
-from re import findall
-
-import numpy as np
-
-
-class ElkParser:
-    def __init__(self, elkin="elk.in", kdirect=True):
-
-        # elk specific inp
-        self.fin = elkin
-        self.file_names = []
-        self.elkin = None
-        self.nbands = None
-
-        self.nspin = None
-        self.kticks = None
-
-        self.kdirect = kdirect
-
-        self.kpoints = None
-        self.bands = None
-
-        self.spd = None
-        self.cspd = None
-
-        # spin polarized parameters
-        self.spinpol = None
-
-        self.orbitalName = [
-            "Y00",
-            "Y1-1",
-            "Y10",
-            "Y11",
-            "Y2-2",
-            "Y2-1",
-            "Y20",
-            "Y21",
-            "Y22",
-            "Y3-3",
-            "Y3-2",
-            "Y3-1",
-            "Y30",
-            "Y3-1",
-            "Y3-2",
-            "Y3-3",
-        ]
-        self.orbital_name_short = ["s", "p", "d", "f"]
-        self.norbital = None  # number of orbitals
-
-        # number of spin components (blocks of data), 1: non-magnetic non
-        # polarized, 2: spin polarized collinear, 4: non-collinear
-        # spin.
-        # NOTE: before calling to `self._readOrbital` the case '4'
-        # is marked as '1'
-
-        self._read_elkin()
-        self._read_bands()
-
-        return
-
-    #    @property
-    #    def nspin(self):
-    #        """
-    #        number of spin, default is 1.
-    #        """
-    #        nspindict = {1: 1, 2: 2, 4: 2, None: 1}
-    #        return nspindict[self.ispin]
-
-    @property
-    def spd_orb(self):
-        # indices: ikpt, iband, ispin, iion, iorb
-        # remove indices and total from iorb.
-        return self.spd[:, :, :, 1:-1]
-
-    @property
-    def nhigh_sym(self):
-        """
-        Returns nu,ber of high symmetry points
-        """
-        return int(findall("plot1d\n\s*([0-9]*)\s*[0-9]*", self.elkin)[0])
-
-    @property
-    def nkpoints(self):
-        """
-        Returns total number of kpoints
-        """
-        return int(findall("plot1d\n\s*[0-9]*\s*([0-9]*)", self.elkin)[0])
-
-    @property
-    def tasks(self):
-        """
-        Returns the tasks calculated by elk
-        """
-        return [int(x) for x in findall("tasks\s*([0-9\s\n]*)", self.elkin)[0].split()]
-
-    @property
-    def high_symmetry_points(self):
-        """
-        Returns the corrdinates of high symmtery points provided in elk.in
-        """
-        if 20 in self.tasks or 21 in self.tasks or 22 in self.tasks:
-            raw_hsp = findall(
-                "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * "([0-9\s\.-]*).*\n",
-                self.elkin,
-            )[0]
-            high_symmetry_points = np.zeros(shape=(self.nhigh_sym, 3))
-            for ihs in range(self.nhigh_sym):
-                high_symmetry_points[ihs, :] = [
-                    float(x) for x in raw_hsp[ihs].split()[0:3]
-                ]
-            return high_symmetry_points
-
-    @property
-    def nspecies(self):
-        """
-        Returns number of species
-        """
-
-        return int(findall("atoms\n\s*([0-9]*)", self.elkin)[0])
-
-    @property
-    def natom(self):
-        """
-        Returns number of atoms in the structure
-        """
-        natom = 0
-        for ispc in findall("'([A-Za-z]*).in'.*\n\s*([0-9]*)", self.elkin):
-            natom += int(ispc[1])
-        return natom
-
-    @property
-    def composition(self):
-        """
-        Returns the composition of the structure
-        """
-        composition = {}
-        for ispc in findall("'([A-Za-z]*).in'.*\n\s*([0-9]*)", self.elkin):
-            composition[ispc[0]] = int(ispc[1])
-        return composition
-
-    @property
-    def knames(self):
-        """
-        Returns the names of the high symmetry points(x ticks) provided in elk.in
-
-        """
-        raw_ticks = findall(
-            "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * ".*:(.*)\n", self.elkin
-        )[0]
-        if len(raw_ticks) != self.nhigh_sym:
-            knames = [str(x) for x in range(self.nhigh_sym)]
-        else:
-            knames = [
-                "$%s$" % (x.replace(",", "").replace("vlvp1d", "").replace(" ", ""))
-                for x in findall(
-                    "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * ".*:(.*)\n",
-                    self.elkin,
-                )[0]
-            ]
-        return knames
-
-    def _read_elkin(self):
-        """
-        Reads and parses elk.in
-        """
-        rf = open(self.fin, "r")
-        self.elkin = rf.read()
-        rf.close()
-
-        if 20 in self.tasks:
-            self.file_names.append("BANDS.OUT")
-        if 21 in self.tasks or 22 in self.tasks:
-            ispc = 1
-            for spc in self.composition:
-                for iatom in range(self.composition[spc]):
-                    self.file_names.append(
-                        "BAND_S{:02d}_A{:04d}.OUT".format(ispc, iatom + 1)
-                    )
-                ispc += 1
-
-        # Checking if spinpol = .true. in elk.in
-        try:
-            self.spinpol = findall(r"spinpol\s*([.a-zA-Z]*)", self.elkin)[0]
-        except IndexError:
-            self.spinpol = None
-
-        if self.spinpol:
-            if self.spinpol == ".true.":
-                print("\nElk colinear spin calculation detected.\n")
-                self.spinpol = True
-                self.nspin = 2
-            else:
-                print("\nElk non spin calculation detected.\n")
-                self.nspin = 1
-        else:
-            print(
-                "\nNo spinpol keyword found in elk.in. Assuming non spin calculation.\n"
-            )
-            self.nspin = 1
-
-    def _read_bands(self):
-        """
-        if the task is any of 20,21,22 it parses the BANDS*.OUT files
-        and prepares the spd, bands and kpoints for bandsplot
-        """
-        if np.any([x in self.tasks for x in [20, 21, 22]]):
-
-            rf = open(self.file_names[0], "r")
-            lines = rf.readlines()
-            rf.close()
-
-            self.nbands = int(len(lines) / (self.nkpoints + 1))
-            self.bands = np.zeros(shape=(self.nkpoints, self.nbands))
-
-            rf = open("BANDLINES.OUT", "r")
-            bandLines = rf.readlines()
-            rf.close()
-
-            tick_pos = []
-            # using strings for a better comparision and avoiding rounding by python
-            for iline in range(0, len(bandLines), 3):
-                tick_pos.append(bandLines[iline].split()[0])
-            x_points = []
-            for iline in range(self.nkpoints):
-                x_points.append(lines[iline].split()[0])
-
-            self.kpoints = np.zeros(shape=(self.nkpoints, 3))
-            x_points = np.array(x_points)
-            tick_pos = np.array(tick_pos)
-
-            self.kticks = []
-            for ihs in range(1, self.nhigh_sym):
-                start = np.where(x_points == tick_pos[ihs - 1])[0][0]
-                end = np.where(x_points == tick_pos[ihs])[0][0] + 1
-                self.kpoints[start:end][:] = np.linspace(
-                    self.high_symmetry_points[ihs - 1],
-                    self.high_symmetry_points[ihs],
-                    end - start,
-                )
-
-                self.kticks.append(start)
-            self.kticks.append(self.nkpoints - 1)
-            if not self.kdirect:
-                self.kpoints = np.dot(self.kpoints, self.reclat)
-
-            rf = open(self.file_names[0], "r")
-            lines = rf.readlines()
-            rf.close()
-
-            iline = 0
-            for iband in range(self.nbands):
-                for ikpoint in range(self.nkpoints):
-                    self.bands[ikpoint, iband] = float(lines[iline].split()[1])
-                    iline += 1
-                if ikpoint == self.nkpoints - 1:
-                    iline += 1
-            self.bands *= 27.21138386
-
-            self.norbital = 16
-            self.spd = np.zeros(
-                shape=(
-                    self.nkpoints,
-                    self.nbands,
-                    self.nspin,
-                    self.natom + 1,
-                    self.norbital + 2,
-                )
-            )
-            idx_bands_out = None
-            for ifile in range(len(self.file_names)):
-                if self.file_names[ifile] == "BANDS.OUT":
-                    idx_bands_out = ifile
-            if idx_bands_out != None:
-                del self.file_names[idx_bands_out]
-
-            for ifile in range(self.natom):
-                rf = open(self.file_names[ifile], "r")
-                lines = rf.readlines()
-                rf.close()
-                iline = 0
-
-                for iband in range(self.nbands):
-                    for ikpoint in range(self.nkpoints):
-                        temp = np.array([float(x) for x in lines[iline].split()])
-                        self.spd[ikpoint, iband, 0, ifile, 0] = ifile + 1
-                        self.spd[ikpoint, iband, 0, ifile, 1:-1] = temp[2:]
-                        iline += 1
-                    if ikpoint == self.nkpoints - 1:
-                        iline += 1
-            # self.spd[:,:,:,-1,:] = self.spd.sum(axis=3)
-            self.spd[:, :, :, :, -1] = np.sum(self.spd[:, :, :, :, 1:-1], axis=4)
-            self.spd[:, :, :, -1, :] = self.spd.sum(axis=3)
-            self.spd[:, :, 0, -1, 0] = 0
-
-            if self.nspin == 2:
-                # spin up block for spin = 1
-                self.spd[:, : self.nbands // 2, 1, :, :] = self.spd[
-                    :, : self.nbands // 2, 0, :, :
-                ]
-                # spin down block for spin = 1
-                self.spd[:, self.nbands // 2 :, 1, :, :] = (
-                    -1 * self.spd[:, self.nbands // 2 :, 0, :, :]
-                )
-
-                # manipulating spd array for spin polarized calculations.
-                # The shape is (nkpoints,2*nbands,2,natoms,norbitals)
-                # The third dimension is for spin.
-                # When this is zero, the bands*2 (all spin up and down bands) have positive projections.
-                # When this is one, the the first half of bands (spin up) will have positive projections
-                # and the second half (spin down) will have negative projections. This is to adhere to
-                # the convention used in PyProcar to obtain spin density and spin magnetization.
-
-                # spin up and spin down block for spin = 0
-                # spd2[:, :, 0, :, :] = self.spd[:, :, 0, :, :]
-
-    @property
-    def fermi(self):
-        """
-        Returns the fermi energy read from FERMI.OUT
-        """
-        rf = open("EFERMI.OUT", "r")
-        fermi = float(rf.readline().split()[0])
-        rf.close()
-        return fermi
-
-    @property
-    def reclat(self):
-        """
-        Returns the reciprocal lattice read from LATTICE.OUT
-        """
-        rf = open("LATTICE.OUT", "r")
-        data = rf.read()
-        rf.close()
-        lattice_block = findall(r"matrix\s*:([-+\s0-9.]*)Inverse", data)
-        lattice_array = np.array(lattice_block[1].split(), dtype=float)
-        reclat = lattice_array.reshape((3, 3))
-        return reclat
+"""
+Created on Fri March 2 2020
+@author: Pedram Tavadze
+
+"""
+
+from re import findall
+
+import numpy as np
+
+
+class ElkParser:
+    def __init__(self, elkin="elk.in", kdirect=True):
+
+        # elk specific inp
+        self.fin = elkin
+        self.file_names = []
+        self.elkin = None
+        self.nbands = None
+
+        self.nspin = None
+        self.kticks = None
+
+        self.kdirect = kdirect
+
+        self.kpoints = None
+        self.bands = None
+
+        self.spd = None
+        self.cspd = None
+
+        # spin polarized parameters
+        self.spinpol = None
+
+        self.orbitalName = [
+            "Y00",
+            "Y1-1",
+            "Y10",
+            "Y11",
+            "Y2-2",
+            "Y2-1",
+            "Y20",
+            "Y21",
+            "Y22",
+            "Y3-3",
+            "Y3-2",
+            "Y3-1",
+            "Y30",
+            "Y3-1",
+            "Y3-2",
+            "Y3-3",
+        ]
+        self.orbital_name_short = ["s", "p", "d", "f"]
+        self.norbital = None  # number of orbitals
+
+        # number of spin components (blocks of data), 1: non-magnetic non
+        # polarized, 2: spin polarized collinear, 4: non-collinear
+        # spin.
+        # NOTE: before calling to `self._readOrbital` the case '4'
+        # is marked as '1'
+
+        self._read_elkin()
+        self._read_bands()
+
+        return
+
+    #    @property
+    #    def nspin(self):
+    #        """
+    #        number of spin, default is 1.
+    #        """
+    #        nspindict = {1: 1, 2: 2, 4: 2, None: 1}
+    #        return nspindict[self.ispin]
+
+    @property
+    def spd_orb(self):
+        # indices: ikpt, iband, ispin, iion, iorb
+        # remove indices and total from iorb.
+        return self.spd[:, :, :, 1:-1]
+
+    @property
+    def nhigh_sym(self):
+        """
+        Returns nu,ber of high symmetry points
+        """
+        return int(findall("plot1d\n\s*([0-9]*)\s*[0-9]*", self.elkin)[0])
+
+    @property
+    def nkpoints(self):
+        """
+        Returns total number of kpoints
+        """
+        return int(findall("plot1d\n\s*[0-9]*\s*([0-9]*)", self.elkin)[0])
+
+    @property
+    def tasks(self):
+        """
+        Returns the tasks calculated by elk
+        """
+        return [int(x) for x in findall("tasks\s*([0-9\s\n]*)", self.elkin)[0].split()]
+
+    @property
+    def high_symmetry_points(self):
+        """
+        Returns the corrdinates of high symmtery points provided in elk.in
+        """
+        if 20 in self.tasks or 21 in self.tasks or 22 in self.tasks:
+            raw_hsp = findall(
+                "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * "([0-9\s\.-]*).*\n",
+                self.elkin,
+            )[0]
+            high_symmetry_points = np.zeros(shape=(self.nhigh_sym, 3))
+            for ihs in range(self.nhigh_sym):
+                high_symmetry_points[ihs, :] = [
+                    float(x) for x in raw_hsp[ihs].split()[0:3]
+                ]
+            return high_symmetry_points
+
+    @property
+    def nspecies(self):
+        """
+        Returns number of species
+        """
+
+        return int(findall("atoms\n\s*([0-9]*)", self.elkin)[0])
+
+    @property
+    def natom(self):
+        """
+        Returns number of atoms in the structure
+        """
+        natom = 0
+        for ispc in findall("'([A-Za-z]*).in'.*\n\s*([0-9]*)", self.elkin):
+            natom += int(ispc[1])
+        return natom
+
+    @property
+    def composition(self):
+        """
+        Returns the composition of the structure
+        """
+        composition = {}
+        for ispc in findall("'([A-Za-z]*).in'.*\n\s*([0-9]*)", self.elkin):
+            composition[ispc[0]] = int(ispc[1])
+        return composition
+
+    @property
+    def knames(self):
+        """
+        Returns the names of the high symmetry points(x ticks) provided in elk.in
+
+        """
+        raw_ticks = findall(
+            "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * ".*:(.*)\n", self.elkin
+        )[0]
+        if len(raw_ticks) != self.nhigh_sym:
+            knames = [str(x) for x in range(self.nhigh_sym)]
+        else:
+            knames = [
+                "$%s$" % (x.replace(",", "").replace("vlvp1d", "").replace(" ", ""))
+                for x in findall(
+                    "plot1d\n\s*[0-9]*\s*[0-9]*.*\n" + self.nhigh_sym * ".*:(.*)\n",
+                    self.elkin,
+                )[0]
+            ]
+        return knames
+
+    def _read_elkin(self):
+        """
+        Reads and parses elk.in
+        """
+        rf = open(self.fin, "r")
+        self.elkin = rf.read()
+        rf.close()
+
+        if 20 in self.tasks:
+            self.file_names.append("BANDS.OUT")
+        if 21 in self.tasks or 22 in self.tasks:
+            ispc = 1
+            for spc in self.composition:
+                for iatom in range(self.composition[spc]):
+                    self.file_names.append(
+                        "BAND_S{:02d}_A{:04d}.OUT".format(ispc, iatom + 1)
+                    )
+                ispc += 1
+
+        # Checking if spinpol = .true. in elk.in
+        try:
+            self.spinpol = findall(r"spinpol\s*([.a-zA-Z]*)", self.elkin)[0]
+        except IndexError:
+            self.spinpol = None
+
+        if self.spinpol:
+            if self.spinpol == ".true.":
+                print("\nElk colinear spin calculation detected.\n")
+                self.spinpol = True
+                self.nspin = 2
+            else:
+                print("\nElk non spin calculation detected.\n")
+                self.nspin = 1
+        else:
+            print(
+                "\nNo spinpol keyword found in elk.in. Assuming non spin calculation.\n"
+            )
+            self.nspin = 1
+
+    def _read_bands(self):
+        """
+        if the task is any of 20,21,22 it parses the BANDS*.OUT files
+        and prepares the spd, bands and kpoints for bandsplot
+        """
+        if np.any([x in self.tasks for x in [20, 21, 22]]):
+
+            rf = open(self.file_names[0], "r")
+            lines = rf.readlines()
+            rf.close()
+
+            self.nbands = int(len(lines) / (self.nkpoints + 1))
+            self.bands = np.zeros(shape=(self.nkpoints, self.nbands))
+
+            rf = open("BANDLINES.OUT", "r")
+            bandLines = rf.readlines()
+            rf.close()
+
+            tick_pos = []
+            # using strings for a better comparision and avoiding rounding by python
+            for iline in range(0, len(bandLines), 3):
+                tick_pos.append(bandLines[iline].split()[0])
+            x_points = []
+            for iline in range(self.nkpoints):
+                x_points.append(lines[iline].split()[0])
+
+            self.kpoints = np.zeros(shape=(self.nkpoints, 3))
+            x_points = np.array(x_points)
+            tick_pos = np.array(tick_pos)
+
+            self.kticks = []
+            for ihs in range(1, self.nhigh_sym):
+                start = np.where(x_points == tick_pos[ihs - 1])[0][0]
+                end = np.where(x_points == tick_pos[ihs])[0][0] + 1
+                self.kpoints[start:end][:] = np.linspace(
+                    self.high_symmetry_points[ihs - 1],
+                    self.high_symmetry_points[ihs],
+                    end - start,
+                )
+
+                self.kticks.append(start)
+            self.kticks.append(self.nkpoints - 1)
+            if not self.kdirect:
+                self.kpoints = np.dot(self.kpoints, self.reclat)
+
+            rf = open(self.file_names[0], "r")
+            lines = rf.readlines()
+            rf.close()
+
+            iline = 0
+            for iband in range(self.nbands):
+                for ikpoint in range(self.nkpoints):
+                    self.bands[ikpoint, iband] = float(lines[iline].split()[1])
+                    iline += 1
+                if ikpoint == self.nkpoints - 1:
+                    iline += 1
+            self.bands *= 27.21138386
+
+            self.norbital = 16
+            self.spd = np.zeros(
+                shape=(
+                    self.nkpoints,
+                    self.nbands,
+                    self.nspin,
+                    self.natom + 1,
+                    self.norbital + 2,
+                )
+            )
+            idx_bands_out = None
+            for ifile in range(len(self.file_names)):
+                if self.file_names[ifile] == "BANDS.OUT":
+                    idx_bands_out = ifile
+            if idx_bands_out != None:
+                del self.file_names[idx_bands_out]
+
+            for ifile in range(self.natom):
+                rf = open(self.file_names[ifile], "r")
+                lines = rf.readlines()
+                rf.close()
+                iline = 0
+
+                for iband in range(self.nbands):
+                    for ikpoint in range(self.nkpoints):
+                        temp = np.array([float(x) for x in lines[iline].split()])
+                        self.spd[ikpoint, iband, 0, ifile, 0] = ifile + 1
+                        self.spd[ikpoint, iband, 0, ifile, 1:-1] = temp[2:]
+                        iline += 1
+                    if ikpoint == self.nkpoints - 1:
+                        iline += 1
+            # self.spd[:,:,:,-1,:] = self.spd.sum(axis=3)
+            self.spd[:, :, :, :, -1] = np.sum(self.spd[:, :, :, :, 1:-1], axis=4)
+            self.spd[:, :, :, -1, :] = self.spd.sum(axis=3)
+            self.spd[:, :, 0, -1, 0] = 0
+
+            if self.nspin == 2:
+                # spin up block for spin = 1
+                self.spd[:, : self.nbands // 2, 1, :, :] = self.spd[
+                    :, : self.nbands // 2, 0, :, :
+                ]
+                # spin down block for spin = 1
+                self.spd[:, self.nbands // 2 :, 1, :, :] = (
+                    -1 * self.spd[:, self.nbands // 2 :, 0, :, :]
+                )
+
+                # manipulating spd array for spin polarized calculations.
+                # The shape is (nkpoints,2*nbands,2,natoms,norbitals)
+                # The third dimension is for spin.
+                # When this is zero, the bands*2 (all spin up and down bands) have positive projections.
+                # When this is one, the the first half of bands (spin up) will have positive projections
+                # and the second half (spin down) will have negative projections. This is to adhere to
+                # the convention used in PyProcar to obtain spin density and spin magnetization.
+
+                # spin up and spin down block for spin = 0
+                # spd2[:, :, 0, :, :] = self.spd[:, :, 0, :, :]
+
+    @property
+    def fermi(self):
+        """
+        Returns the fermi energy read from FERMI.OUT
+        """
+        rf = open("EFERMI.OUT", "r")
+        fermi = float(rf.readline().split()[0])
+        rf.close()
+        return fermi
+
+    @property
+    def reclat(self):
+        """
+        Returns the reciprocal lattice read from LATTICE.OUT
+        """
+        rf = open("LATTICE.OUT", "r")
+        data = rf.read()
+        rf.close()
+        lattice_block = findall(r"matrix\s*:([-+\s0-9.]*)Inverse", data)
+        lattice_array = np.array(lattice_block[1].split(), dtype=float)
+        reclat = lattice_array.reshape((3, 3))
+        return reclat
```

### Comparing `PyProcar-5.6.6/pyprocar/lobsterparser/lobster_doscar_parser.py` & `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,565 +1,565 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Jun 15 15:50:22 2020
-
-@author: lllan
-"""
-
-import os
-import numpy as np
-
-from ..core import DensityOfStates, Structure
-from re import findall, search, match, DOTALL, MULTILINE, finditer, compile, sub
-
-
-class LobsterDOSParser:
-    def __init__(self, filename='DOSCAR.lobster', dos_interpolation_factor = None ):
-
-        if not os.path.isfile(filename):
-            raise ValueError('ERROR: DOSCAR file not found')
-
-        self.filename = filename
-        self.data = self.read()
-        
-        self.dos_interpolation_factor = dos_interpolation_factor
-        self.test = None
-        self.test2 = None
-        
-        self.ionsList = None
-        if 'projected' in self.data:
-            self.has_projected = True
-            self.nions = len(self.data['projected'])
-        else:
-            self.has_projected = False
-            self.nions = None
-
-        self.ndos, self.total_ncols = self.data['total'].shape
-
-        if self.total_ncols == 5:
-            self.is_spin_polarized = True
-            self.spins = ['dos_up','dos_down']
-        else:
-            self.is_spin_polarized = False
-
-        # self.total_dos = self.dos_to_dict['total']
-
-        # if self.has_projected:
-        #     self.projected_dos = self.dos_to_dict['projected']
-            
-        rf = open('lobsterout', "r")
-        self.lobsterout = rf.read()
-        rf.close()
-
-    ###########################################################################
-    # This section parse for the total density of states and puts it in a 
-    #Pychemia Density of States Object
-    ###########################################################################
-    def read(self):
-        """
-        Read and parse vasprun.xml.
-        Returns
-        -------
-        TYPE
-            DESCRIPTION.
-        """
-        return self.parse_doscar(self.filename)
-
-
-    def _get_dos_total(self):
-        
-        energies = self.data['total'][:, 0]
-        dos_total = {'energies': energies}
-        
-        if self.is_spin_polarized:
-            dos_total['Spin-up'] = self.data['total'][:, 1]
-            dos_total['Spin-down'] = self.data['total'][:, 2]
-            #dos_total['integrated_dos_up'] = self.data['total'][:, 3]
-            #dos_total['integrated_dos_down'] = self.data['total'][:, 4]
-        else:
-            dos_total['Spin-up'] = self.data['total'][:, 1]
-            #dos_total['integrated_dos'] = self.data['total'][:, 2]
-
-        return dos_total,list(dos_total.keys())
-
-
-    def _get_dos_projected(self, atoms=[]):
-
-        if len(atoms) == 0:
-            atoms = np.arange(self.initial_structure.natoms)
-
-        if 'projected' in list(self.data.keys()):
-            dos_projected = {}
-            ion_list = ["ion %s" % str(x + 1) for x in atoms
-                        ]  # using this name as vasrun.xml uses ion #
-            for i in range(len(ion_list)):
-                iatom = ion_list[i]
-                name = self.initial_structure.atoms[atoms[i]]
-
-                energies = self.data['projected'][i][:,0,0]
-                
-                dos_projected[name] = {'energies': energies}
-                if self.is_spin_polarized:
-                    dos_projected[name]['Spin-up'] = self.data['projected'][i][:, 1:,0]
-                    dos_projected[name]['Spin-down'] = self.data['projected'][i][:, 1:,1]
-                else:
-                    dos_projected[name]['Spin-up'] = self.data['projected'][i][:, 1:,0]
-            
-            return dos_projected, self.data['projected_labels_info']
-        else:
-            print(
-                "This calculation does not include partial density of states")
-            return None, None
-    
-    @property
-    def dos(self):
-        energies = self.dos_total['energies']
-        total = []
-        for ispin in self.dos_total:
-            if ispin == 'energies':
-                continue
-            total.append(self.dos_total[ispin])
-        # total = np.array(total).T
-        return DensityOfStates(
-            energies=energies,
-            total=total,
-            projected=self.dos_projected,
-            interpolation_factor=self.dos_interpolation_factor)
-  
-    @property
-    def dos_to_dict(self):
-        """
-        Returns the complete density (total,projected) of states as a python dictionary
-        """
-        return {
-            'total': self._get_dos_total(),
-            'projected': self._get_dos_projected()
-        }
-    
-    @property
-    def dos_total(self):
-        """
-        Returns the total density of states as a pychemia.visual.DensityOfSates object
-        """
-        dos_total, labels = self._get_dos_total()
-        #dos_total['energies'] -= self.fermi
-
-        return dos_total
-
-    @property
-    def dos_projected(self):
-        """
-        Returns the projected DOS as a multi-dimentional array, to be used in the
-        pyprocar.core.dos object
-        """
-        ret = []
-        dos_projected, info = self._get_dos_projected()
-        if dos_projected is None:
-            return None
-        norbitals = len(info) - 1
-        info[0] = info[0].capitalize()
-        labels = []
-        labels.append(info[0])
-        ret = []
-        for iatom in dos_projected:
-            temp_atom = []
-            for iorbital in range(norbitals):
-                temp_spin = []
-                for key in dos_projected[iatom]:
-                    if key == 'energies':
-                        continue
-                    temp_spin.append(dos_projected[iatom][key][:, iorbital])
-                temp_atom.append(temp_spin)
-            ret.append([temp_atom])
-        return ret   
-    
-    
-#     ###########################################################################
-#     # This section parses for the projected density of states and puts it in a 
-#     # Pychemia Density of States Object
-#     ###########################################################################
-
-    @property
-    def species(self):
-        """
-        Returns the species in POSCAR
-        """
-        return self.initial_structure.species
-
-    @property
-    def structures(self):
-        """
-        Returns a list of pychemia.core.Structure representing all the ionic step structures
-        """
-        symbols = [x.strip() for x in self.data['ions']]
-        structures = []
-
-        st = Structure(atoms=symbols)
-                      
-        structures.append(st)
-        return structures
-
-    @property
-    def structure(self):
-        """
-        crystal structure of the last step
-        """
-        return self.structures[-1]
-    
-    @property
-    def initial_structure(self):
-        """
-        Returns the initial Structure as a pychemia structure
-        """
-        return self.structures[0]
-    
-    @property
-    def final_structure(self):
-        """
-        Returns the final Structure as a pychemia structure
-        """
-
-        return self.structures[-1]
-
-
-#     ###########################################################################
-#     ###########################################################################
-#     ###########################################################################
-    
-    def dos_parametric(self,atoms=None,orbitals=None,spin=None,title=None):
-        """
-        This function sums over the list of atoms and orbitals given 
-        for example dos_paramateric(atoms=[0,1,2],orbitals=[1,2,3],spin=[0,1])
-        will sum all the projections of atoms 0,1,2 and all the orbitals of 1,2,3 (px,py,pz)
-        and return separatly for the 2 spins as a DensityOfStates object from pychemia.visual.DensityofStates
-        
-        :param atoms: list of atom index needed to be sumed over. count from zero with the same 
-                      order as POSCAR
-        
-        :param orbitals: list of orbitals needed to be sumed over 
-        |  s  ||  py ||  pz ||  px || dxy || dyz || dz2 || dxz ||x2-y2||
-        |  0  ||  1  ||  2  ||  3  ||  4  ||  5  ||  6  ||  7  ||  8  ||
-        
-        :param spin: which spins to be included. count from 0
-                      There are no sum over spins
-        
-        """
-        projected = self.dos_projected
-        dos_projected,labelsInfo = self._get_dos_projected()
-        self.availiableOrbitals = list(labelsInfo.keys())
-        self.availiableOrbitals.pop(0)
-        if atoms == None :
-            atoms = np.arange(self.nions,dtype=int)
-        if spin == None :
-            spin = [0,1]
-        if orbitals == None :
-            orbitals = np.arange((len(projected[0].labels)-1)//2,dtype=int)
-        if title == None:
-            title = 'Sum'
-        orbitals = np.array(orbitals)
-        
-        
-        if len(spin) == 2:
-            labels = ['Energy','Spin-Up','Spin-Down']
-            new_orbitals = []
-            for ispin in spin :
-                new_orbitals.append(list(orbitals+ispin*(len(projected[0].labels)-1)//2))
-                
-            orbitals = new_orbitals
-            
-        else : 
-            
-            for x in orbitals:
-                
-                if (x+1 > (len(projected[0].labels)-1)//2 ):
-                    print('listed wrong amount of orbitals')
-                    print('Only use one or more of the following ' + str(np.arange((len(projected[0].labels)-1)//2,dtype=int)))
-                    print('Only use one or more of the following ' + str(np.arange((len(projected[0].labels)-1)//2,dtype=int)))
-                    print('They correspond to the following orbitals : ' + str(self.availiableOrbitals) )
-                    print('Again do not trust the plot that was just produced' )
-            if spin[0] == 0:
-                labels = ['Energy','Spin-Up']
-            elif spin[0] == 1:
-                labels = ['Energy','Spin-Down']
-            
-        
-        
-        ret = np.zeros(shape=(len(projected[0].energies),len(spin)+1))
-        ret[:,0] = projected[0].energies
-        
-        for iatom in atoms :
-            if len(spin) == 2 :
-                ret[:,1:]+=self.dos_projected[iatom].values[:,orbitals].sum(axis=2)
-            elif len(spin) == 1 :
-                ret[:,1]+=self.dos_projected[iatom].values[:,orbitals].sum(axis=1)
-                
-        return DensityOfStates(table=ret,title=title,labels=labels)
-    
-    
-    ###########################################################################
-    # This section parses for the projected density of states and puts it in a 
-    # Pychemia Density of States Object
-    ###########################################################################
-
-
-    @staticmethod
-    def parse_doscar(filename):
-
-        rf = open(filename)
-        data = rf.readlines()
-        rf.close()
-
-        rf = open("lobsterout", "r")
-        lobsterout = rf.read()
-        rf.close()
-        
-
-        if len(data) < 5:
-            raise ValueError('DOSCAR seems truncated')
-
-        ionsList = findall("calculating FatBand for Element: (.*) Orbital.*", lobsterout)
-      
-        proj_ions = findall("calculating FatBand for Element: (.*) Orbital\(s\):\s*.*", lobsterout)
-  
-        # Skipping the first lines of header
-        iline = 5
-
-        header = [float(x) for x in data[iline].strip().split()]
-        ndos = int(header[2])
-        iline += 1
-
-        total_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
-        total_dos = np.array(total_dos)
-
-        iline += ndos
-        ndos, total_ncols = total_dos.shape
-        is_spin_polarized = False
-        if total_ncols == 5:
-            is_spin_polarized = True
-            spins = ['dos_up','dos_down']
-        # In case there are more lines of data, they are the projected DOS
-        if len(data) > iline:
-
-            projected_dos = []
-            proj_orbitals = []
-            ion_index =0
-            
-            while iline < len(data):
-       
-                header = [float(x) for x in data[iline].split(";")[0].split()]
-                
-                #print(header)
-  
-                proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
-                #print(proj_orbitals)
-                ion_index += 1    
-                
-                
-                ndos = int(header[2])
-                iline += 1
-                tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
-                tmp_dos = np.array(tmp_dos)
-                
-                projected_dos.append(tmp_dos)
-               
-                iline += ndos
-                
-            final_projected = []
-            
-            for i_ion in range(len(projected_dos)):
-                tmp_dos = np.zeros(shape = [len(projected_dos[i_ion][:,0]),10,2])
-                for ilabel, label in enumerate(proj_orbitals[i_ion][1].split(),1): 
-                    if is_spin_polarized == False :
-                        tmp_dos[:,0,0] = projected_dos[i_ion][:,0]
-                        if (label.find('s') == True):
-                            tmp_dos[:,1,0] += projected_dos[i_ion][:,ilabel] 
-                        elif(label.find('p_y') == True):
-                            tmp_dos[:,2,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('p_z') == True):
-                            tmp_dos[:,3,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('p_x') == True):
-                            tmp_dos[:,4,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('d_xy') == True):
-                            tmp_dos[:,5,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('d_yz') == True):
-                            tmp_dos[:,6,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('d_z^2') == True):
-                            tmp_dos[:,7,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('d_xz') == True):
-                            tmp_dos[:,8,0] += projected_dos[i_ion][:,ilabel]
-                        elif(label.find('d_x^2-y^2') == True):
-                            tmp_dos[:,9,0] += projected_dos[i_ion][:,ilabel]
-                    else:
-                        tmp_dos[:,0,0] = projected_dos[i_ion][:,0]
-                        tmp_dos[:,0,1] = projected_dos[i_ion][:,0]
-                        if (label.find('s') == True):
-                            tmp_dos[:,1,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,1,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('p_y') == True):
-                            tmp_dos[:,2,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,2,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('p_z') == True):
-                            tmp_dos[:,3,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,3,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('p_x') == True):
-                            tmp_dos[:,4,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,4,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('d_xy') == True):
-                            tmp_dos[:,5,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,5,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('d_yz') == True):
-                            tmp_dos[:,6,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,6,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('d_z^2') == True):
-                            tmp_dos[:,7,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,7,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('d_xz') == True):
-                            tmp_dos[:,8,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,8,1] += projected_dos[i_ion][:,2*ilabel]
-                        elif(label.find('d_x^2-y^2') == True):
-                            tmp_dos[:,9,0] += projected_dos[i_ion][:,2*ilabel-1]
-                            tmp_dos[:,9,1] += projected_dos[i_ion][:,2*ilabel]
-                final_projected.append(tmp_dos)
-                final_labels_index = {'energies':None,'s':0,'p_y':1,'p_z':2, 'p_x':3 , 'd_xy': 4,  'd_yz': 5, 'd_z^2': 6, 'd_xz':7,'d_x^2-y^2':8}
-                final_labels = list(final_labels_index.keys())        
-                        
-            
-           
-            return {'total': total_dos, 'projected': final_projected, 'projected_labels_info':final_labels , 'ions':ionsList}
-
-        else:
-            
-            return {'total': total_dos}
-
-    # @staticmethod
-    # def parse_doscar(filename):
-
-    #     if not os.path.isfile(filename):
-    #         raise ValueError('ERROR: DOSCAR file not found')
-
-    #     rf = open(filename)
-    #     data = rf.readlines()
-    #     rf.close()
-
-    #     rf = open("lobsterout", "r")
-    #     lobsterout = rf.read()
-    #     rf.close()
-        
-
-    #     if len(data) < 5:
-    #         raise ValueError('DOSCAR seems truncated')
-
-    #     ionsList = findall("calculating FatBand for Element: (.*) Orbital.*", lobsterout)
-
-      
-    #     proj_ions = findall("calculating FatBand for Element: (.*) Orbital\(s\):\s*.*", lobsterout)
-  
-
-
-    #     # Skipping the first lines of header
-    #     iline = 5
-
-    #     header = [float(x) for x in data[iline].strip().split()]
-    #     ndos = int(header[2])
-    #     iline += 1
-
-    #     total_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
-    #     total_dos = np.array(total_dos)
-
-    #     iline += ndos
-
-    #     # In case there are more lines of data, they are the projected DOS
-        
-    #     if len(data) > iline:
-    #         projected_dos = []
-    #         proj_orbitals = []
-    #         ion_index =0
-            
-    #         while iline < len(data):
-       
-    #             header = [float(x) for x in data[iline].split(";")[0].split()]
-                
-    #             #print(header)
-  
-    #             proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
-    #             #print(proj_orbitals)
-    #             ion_index += 1    
-                
-                
-    #             ndos = int(header[2])
-    #             iline += 1
-    #             tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
-    #             tmp_dos = np.array(tmp_dos)
-                
-    #             projected_dos.append(tmp_dos)
-               
-    #             iline += ndos
-    #         #[int(s) for s in str.split() if s.isdigit()]
-    #         final_projected = []
-    #         principal_list = []
-    #         for ion in proj_orbitals:
-    #             principalNum = [int(s) for s in ion[1] if s.isdigit()]
-    #             for n in principalNum:
-    #                 if n not in principal_list:
-    #                     principal_list.append(n)
-    #         print(principal_list)
-    #         return {'total': total_dos, 'projected': projected_dos, 'proj_labels_info':proj_orbitals, 'ions':ionsList,'principal_num':principal_list }
-     
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-
-        #if len(data) > iline:
-
-        #     projected_dos = []
-        #     proj_orbitals = []
-        #     ion_index =0
-        #     while iline < len(data):
-       
-        #         header = [float(x) for x in data[iline].split(";")[0].split()]
-                
-        #         #print(header)
-  
-        #         proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
-        #         #print(proj_orbitals)
-        #         ion_index += 1    
-                
-                
-        #         ndos = int(header[2])
-        #         iline += 1
-        #         tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
-        #         tmp_dos = np.array(tmp_dos)
-                
-        #         projected_dos.append(tmp_dos)
-               
-        #         iline += ndos
-            #self.test = proj_orbitals
-            
-            
-           
-        #     return {'total': total_dos, 'projected': projected_dos, 'proj_labels_info':proj_orbitals, 'ions':ionsList}
-
-        # else:
-
-        #     return {'total': total_dos}
-        
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Jun 15 15:50:22 2020
+
+@author: lllan
+"""
+
+import os
+import numpy as np
+
+from ...core import DensityOfStates, Structure
+from re import findall, search, match, DOTALL, MULTILINE, finditer, compile, sub
+
+
+class LobsterDOSParser:
+    def __init__(self, filename='DOSCAR.lobster', dos_interpolation_factor = None ):
+
+        if not os.path.isfile(filename):
+            raise ValueError('ERROR: DOSCAR file not found')
+
+        self.filename = filename
+        self.data = self.read()
+        
+        self.dos_interpolation_factor = dos_interpolation_factor
+        self.test = None
+        self.test2 = None
+        
+        self.ionsList = None
+        if 'projected' in self.data:
+            self.has_projected = True
+            self.nions = len(self.data['projected'])
+        else:
+            self.has_projected = False
+            self.nions = None
+
+        self.ndos, self.total_ncols = self.data['total'].shape
+
+        if self.total_ncols == 5:
+            self.is_spin_polarized = True
+            self.spins = ['dos_up','dos_down']
+        else:
+            self.is_spin_polarized = False
+
+        # self.total_dos = self.dos_to_dict['total']
+
+        # if self.has_projected:
+        #     self.projected_dos = self.dos_to_dict['projected']
+            
+        rf = open('lobsterout', "r")
+        self.lobsterout = rf.read()
+        rf.close()
+
+    ###########################################################################
+    # This section parse for the total density of states and puts it in a 
+    #Pychemia Density of States Object
+    ###########################################################################
+    def read(self):
+        """
+        Read and parse vasprun.xml.
+        Returns
+        -------
+        TYPE
+            DESCRIPTION.
+        """
+        return self.parse_doscar(self.filename)
+
+
+    def _get_dos_total(self):
+        
+        energies = self.data['total'][:, 0]
+        dos_total = {'energies': energies}
+        
+        if self.is_spin_polarized:
+            dos_total['Spin-up'] = self.data['total'][:, 1]
+            dos_total['Spin-down'] = self.data['total'][:, 2]
+            #dos_total['integrated_dos_up'] = self.data['total'][:, 3]
+            #dos_total['integrated_dos_down'] = self.data['total'][:, 4]
+        else:
+            dos_total['Spin-up'] = self.data['total'][:, 1]
+            #dos_total['integrated_dos'] = self.data['total'][:, 2]
+
+        return dos_total,list(dos_total.keys())
+
+
+    def _get_dos_projected(self, atoms=[]):
+
+        if len(atoms) == 0:
+            atoms = np.arange(self.initial_structure.natoms)
+
+        if 'projected' in list(self.data.keys()):
+            dos_projected = {}
+            ion_list = ["ion %s" % str(x + 1) for x in atoms
+                        ]  # using this name as vasrun.xml uses ion #
+            for i in range(len(ion_list)):
+                iatom = ion_list[i]
+                name = self.initial_structure.atoms[atoms[i]]
+
+                energies = self.data['projected'][i][:,0,0]
+                
+                dos_projected[name] = {'energies': energies}
+                if self.is_spin_polarized:
+                    dos_projected[name]['Spin-up'] = self.data['projected'][i][:, 1:,0]
+                    dos_projected[name]['Spin-down'] = self.data['projected'][i][:, 1:,1]
+                else:
+                    dos_projected[name]['Spin-up'] = self.data['projected'][i][:, 1:,0]
+            
+            return dos_projected, self.data['projected_labels_info']
+        else:
+            print(
+                "This calculation does not include partial density of states")
+            return None, None
+    
+    @property
+    def dos(self):
+        energies = self.dos_total['energies']
+        total = []
+        for ispin in self.dos_total:
+            if ispin == 'energies':
+                continue
+            total.append(self.dos_total[ispin])
+        # total = np.array(total).T
+        return DensityOfStates(
+            energies=energies,
+            total=total,
+            projected=self.dos_projected,
+            interpolation_factor=self.dos_interpolation_factor)
+  
+    @property
+    def dos_to_dict(self):
+        """
+        Returns the complete density (total,projected) of states as a python dictionary
+        """
+        return {
+            'total': self._get_dos_total(),
+            'projected': self._get_dos_projected()
+        }
+    
+    @property
+    def dos_total(self):
+        """
+        Returns the total density of states as a pychemia.visual.DensityOfSates object
+        """
+        dos_total, labels = self._get_dos_total()
+        #dos_total['energies'] -= self.fermi
+
+        return dos_total
+
+    @property
+    def dos_projected(self):
+        """
+        Returns the projected DOS as a multi-dimentional array, to be used in the
+        pyprocar.core.dos object
+        """
+        ret = []
+        dos_projected, info = self._get_dos_projected()
+        if dos_projected is None:
+            return None
+        norbitals = len(info) - 1
+        info[0] = info[0].capitalize()
+        labels = []
+        labels.append(info[0])
+        ret = []
+        for iatom in dos_projected:
+            temp_atom = []
+            for iorbital in range(norbitals):
+                temp_spin = []
+                for key in dos_projected[iatom]:
+                    if key == 'energies':
+                        continue
+                    temp_spin.append(dos_projected[iatom][key][:, iorbital])
+                temp_atom.append(temp_spin)
+            ret.append([temp_atom])
+        return ret   
+    
+    
+#     ###########################################################################
+#     # This section parses for the projected density of states and puts it in a 
+#     # Pychemia Density of States Object
+#     ###########################################################################
+
+    @property
+    def species(self):
+        """
+        Returns the species in POSCAR
+        """
+        return self.initial_structure.species
+
+    @property
+    def structures(self):
+        """
+        Returns a list of pychemia.core.Structure representing all the ionic step structures
+        """
+        symbols = [x.strip() for x in self.data['ions']]
+        structures = []
+
+        st = Structure(atoms=symbols)
+                      
+        structures.append(st)
+        return structures
+
+    @property
+    def structure(self):
+        """
+        crystal structure of the last step
+        """
+        return self.structures[-1]
+    
+    @property
+    def initial_structure(self):
+        """
+        Returns the initial Structure as a pychemia structure
+        """
+        return self.structures[0]
+    
+    @property
+    def final_structure(self):
+        """
+        Returns the final Structure as a pychemia structure
+        """
+
+        return self.structures[-1]
+
+
+#     ###########################################################################
+#     ###########################################################################
+#     ###########################################################################
+    
+    def dos_parametric(self,atoms=None,orbitals=None,spin=None,title=None):
+        """
+        This function sums over the list of atoms and orbitals given 
+        for example dos_paramateric(atoms=[0,1,2],orbitals=[1,2,3],spin=[0,1])
+        will sum all the projections of atoms 0,1,2 and all the orbitals of 1,2,3 (px,py,pz)
+        and return separatly for the 2 spins as a DensityOfStates object from pychemia.visual.DensityofStates
+        
+        :param atoms: list of atom index needed to be sumed over. count from zero with the same 
+                      order as POSCAR
+        
+        :param orbitals: list of orbitals needed to be sumed over 
+        |  s  ||  py ||  pz ||  px || dxy || dyz || dz2 || dxz ||x2-y2||
+        |  0  ||  1  ||  2  ||  3  ||  4  ||  5  ||  6  ||  7  ||  8  ||
+        
+        :param spin: which spins to be included. count from 0
+                      There are no sum over spins
+        
+        """
+        projected = self.dos_projected
+        dos_projected,labelsInfo = self._get_dos_projected()
+        self.availiableOrbitals = list(labelsInfo.keys())
+        self.availiableOrbitals.pop(0)
+        if atoms == None :
+            atoms = np.arange(self.nions,dtype=int)
+        if spin == None :
+            spin = [0,1]
+        if orbitals == None :
+            orbitals = np.arange((len(projected[0].labels)-1)//2,dtype=int)
+        if title == None:
+            title = 'Sum'
+        orbitals = np.array(orbitals)
+        
+        
+        if len(spin) == 2:
+            labels = ['Energy','Spin-Up','Spin-Down']
+            new_orbitals = []
+            for ispin in spin :
+                new_orbitals.append(list(orbitals+ispin*(len(projected[0].labels)-1)//2))
+                
+            orbitals = new_orbitals
+            
+        else : 
+            
+            for x in orbitals:
+                
+                if (x+1 > (len(projected[0].labels)-1)//2 ):
+                    print('listed wrong amount of orbitals')
+                    print('Only use one or more of the following ' + str(np.arange((len(projected[0].labels)-1)//2,dtype=int)))
+                    print('Only use one or more of the following ' + str(np.arange((len(projected[0].labels)-1)//2,dtype=int)))
+                    print('They correspond to the following orbitals : ' + str(self.availiableOrbitals) )
+                    print('Again do not trust the plot that was just produced' )
+            if spin[0] == 0:
+                labels = ['Energy','Spin-Up']
+            elif spin[0] == 1:
+                labels = ['Energy','Spin-Down']
+            
+        
+        
+        ret = np.zeros(shape=(len(projected[0].energies),len(spin)+1))
+        ret[:,0] = projected[0].energies
+        
+        for iatom in atoms :
+            if len(spin) == 2 :
+                ret[:,1:]+=self.dos_projected[iatom].values[:,orbitals].sum(axis=2)
+            elif len(spin) == 1 :
+                ret[:,1]+=self.dos_projected[iatom].values[:,orbitals].sum(axis=1)
+                
+        return DensityOfStates(table=ret,title=title,labels=labels)
+    
+    
+    ###########################################################################
+    # This section parses for the projected density of states and puts it in a 
+    # Pychemia Density of States Object
+    ###########################################################################
+
+
+    @staticmethod
+    def parse_doscar(filename):
+
+        rf = open(filename)
+        data = rf.readlines()
+        rf.close()
+
+        rf = open("lobsterout", "r")
+        lobsterout = rf.read()
+        rf.close()
+        
+
+        if len(data) < 5:
+            raise ValueError('DOSCAR seems truncated')
+
+        ionsList = findall("calculating FatBand for Element: (.*) Orbital.*", lobsterout)
+      
+        proj_ions = findall("calculating FatBand for Element: (.*) Orbital\(s\):\s*.*", lobsterout)
+  
+        # Skipping the first lines of header
+        iline = 5
+
+        header = [float(x) for x in data[iline].strip().split()]
+        ndos = int(header[2])
+        iline += 1
+
+        total_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
+        total_dos = np.array(total_dos)
+
+        iline += ndos
+        ndos, total_ncols = total_dos.shape
+        is_spin_polarized = False
+        if total_ncols == 5:
+            is_spin_polarized = True
+            spins = ['dos_up','dos_down']
+        # In case there are more lines of data, they are the projected DOS
+        if len(data) > iline:
+
+            projected_dos = []
+            proj_orbitals = []
+            ion_index =0
+            
+            while iline < len(data):
+       
+                header = [float(x) for x in data[iline].split(";")[0].split()]
+                
+                #print(header)
+  
+                proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
+                #print(proj_orbitals)
+                ion_index += 1    
+                
+                
+                ndos = int(header[2])
+                iline += 1
+                tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
+                tmp_dos = np.array(tmp_dos)
+                
+                projected_dos.append(tmp_dos)
+               
+                iline += ndos
+                
+            final_projected = []
+            
+            for i_ion in range(len(projected_dos)):
+                tmp_dos = np.zeros(shape = [len(projected_dos[i_ion][:,0]),10,2])
+                for ilabel, label in enumerate(proj_orbitals[i_ion][1].split(),1): 
+                    if is_spin_polarized == False :
+                        tmp_dos[:,0,0] = projected_dos[i_ion][:,0]
+                        if (label.find('s') == True):
+                            tmp_dos[:,1,0] += projected_dos[i_ion][:,ilabel] 
+                        elif(label.find('p_y') == True):
+                            tmp_dos[:,2,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('p_z') == True):
+                            tmp_dos[:,3,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('p_x') == True):
+                            tmp_dos[:,4,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('d_xy') == True):
+                            tmp_dos[:,5,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('d_yz') == True):
+                            tmp_dos[:,6,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('d_z^2') == True):
+                            tmp_dos[:,7,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('d_xz') == True):
+                            tmp_dos[:,8,0] += projected_dos[i_ion][:,ilabel]
+                        elif(label.find('d_x^2-y^2') == True):
+                            tmp_dos[:,9,0] += projected_dos[i_ion][:,ilabel]
+                    else:
+                        tmp_dos[:,0,0] = projected_dos[i_ion][:,0]
+                        tmp_dos[:,0,1] = projected_dos[i_ion][:,0]
+                        if (label.find('s') == True):
+                            tmp_dos[:,1,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,1,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('p_y') == True):
+                            tmp_dos[:,2,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,2,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('p_z') == True):
+                            tmp_dos[:,3,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,3,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('p_x') == True):
+                            tmp_dos[:,4,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,4,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('d_xy') == True):
+                            tmp_dos[:,5,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,5,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('d_yz') == True):
+                            tmp_dos[:,6,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,6,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('d_z^2') == True):
+                            tmp_dos[:,7,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,7,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('d_xz') == True):
+                            tmp_dos[:,8,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,8,1] += projected_dos[i_ion][:,2*ilabel]
+                        elif(label.find('d_x^2-y^2') == True):
+                            tmp_dos[:,9,0] += projected_dos[i_ion][:,2*ilabel-1]
+                            tmp_dos[:,9,1] += projected_dos[i_ion][:,2*ilabel]
+                final_projected.append(tmp_dos)
+                final_labels_index = {'energies':None,'s':0,'p_y':1,'p_z':2, 'p_x':3 , 'd_xy': 4,  'd_yz': 5, 'd_z^2': 6, 'd_xz':7,'d_x^2-y^2':8}
+                final_labels = list(final_labels_index.keys())        
+                        
+            
+           
+            return {'total': total_dos, 'projected': final_projected, 'projected_labels_info':final_labels , 'ions':ionsList}
+
+        else:
+            
+            return {'total': total_dos}
+
+    # @staticmethod
+    # def parse_doscar(filename):
+
+    #     if not os.path.isfile(filename):
+    #         raise ValueError('ERROR: DOSCAR file not found')
+
+    #     rf = open(filename)
+    #     data = rf.readlines()
+    #     rf.close()
+
+    #     rf = open("lobsterout", "r")
+    #     lobsterout = rf.read()
+    #     rf.close()
+        
+
+    #     if len(data) < 5:
+    #         raise ValueError('DOSCAR seems truncated')
+
+    #     ionsList = findall("calculating FatBand for Element: (.*) Orbital.*", lobsterout)
+
+      
+    #     proj_ions = findall("calculating FatBand for Element: (.*) Orbital\(s\):\s*.*", lobsterout)
+  
+
+
+    #     # Skipping the first lines of header
+    #     iline = 5
+
+    #     header = [float(x) for x in data[iline].strip().split()]
+    #     ndos = int(header[2])
+    #     iline += 1
+
+    #     total_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
+    #     total_dos = np.array(total_dos)
+
+    #     iline += ndos
+
+    #     # In case there are more lines of data, they are the projected DOS
+        
+    #     if len(data) > iline:
+    #         projected_dos = []
+    #         proj_orbitals = []
+    #         ion_index =0
+            
+    #         while iline < len(data):
+       
+    #             header = [float(x) for x in data[iline].split(";")[0].split()]
+                
+    #             #print(header)
+  
+    #             proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
+    #             #print(proj_orbitals)
+    #             ion_index += 1    
+                
+                
+    #             ndos = int(header[2])
+    #             iline += 1
+    #             tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
+    #             tmp_dos = np.array(tmp_dos)
+                
+    #             projected_dos.append(tmp_dos)
+               
+    #             iline += ndos
+    #         #[int(s) for s in str.split() if s.isdigit()]
+    #         final_projected = []
+    #         principal_list = []
+    #         for ion in proj_orbitals:
+    #             principalNum = [int(s) for s in ion[1] if s.isdigit()]
+    #             for n in principalNum:
+    #                 if n not in principal_list:
+    #                     principal_list.append(n)
+    #         print(principal_list)
+    #         return {'total': total_dos, 'projected': projected_dos, 'proj_labels_info':proj_orbitals, 'ions':ionsList,'principal_num':principal_list }
+     
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+
+        #if len(data) > iline:
+
+        #     projected_dos = []
+        #     proj_orbitals = []
+        #     ion_index =0
+        #     while iline < len(data):
+       
+        #         header = [float(x) for x in data[iline].split(";")[0].split()]
+                
+        #         #print(header)
+  
+        #         proj_orbitals.append((proj_ions[ion_index],data[iline].split(";")[2]))
+        #         #print(proj_orbitals)
+        #         ion_index += 1    
+                
+                
+        #         ndos = int(header[2])
+        #         iline += 1
+        #         tmp_dos = [[float(x) for x in y.split()] for y in data[iline:iline + ndos]]
+        #         tmp_dos = np.array(tmp_dos)
+                
+        #         projected_dos.append(tmp_dos)
+               
+        #         iline += ndos
+            #self.test = proj_orbitals
+            
+            
+           
+        #     return {'total': total_dos, 'projected': projected_dos, 'proj_labels_info':proj_orbitals, 'ions':ionsList}
+
+        # else:
+
+        #     return {'total': total_dos}
+
```

### Comparing `PyProcar-5.6.6/pyprocar/lobsterparser/lobsterfermiparser.py` & `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterparser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,427 +1,421 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jun 25 03:12:50 2020
-@author: Logan Lang
-"""
-
-
-from re import findall, search, match, DOTALL, MULTILINE, finditer, compile, sub
-
-from numpy import array, dot, linspace, sum, where, zeros, pi, concatenate
-import logging
-
-
-class LobsterFermiParser:
-    def __init__(
-        self,
-        lobsterin="lobsterin",
-        lobsterout="lobsterout",
-        scfin="scf.in",
-        outfile="scf.out",
-        kdirect=True,
-        lobstercode="qe",
-    ):
-
-        self.lobsterin = lobsterin
-        self.scfin = scfin
-        self.outfile = outfile
-        self.lobsterout = lobsterout
-        self.dosin = "DOSCAR.lobster"
-
-        self.file_names = []
-
-        self.discontinuities = []
-        self.kdirect = kdirect
-        ############################
-        self.high_symmetry_points = None
-        self.nhigh_sym = None
-        self.nspecies = None
-
-        self.composition = {}
-
-        self.kticks = None
-        self.knames = None
-
-        self.speciesList = None
-
-        self.kpoints = None
-        self.kpointsCount = None
-        self.bands = None
-        self.bandsCount = None
-        self.ionsList = None
-        self.ionsCount = None
-        self.spinCount = None
-
-        # Used to store atomic states at the top of the kpdos.out file
-        self.states = None
-
-        
-
-        self.spd = None
-        """ for l=1:
-              1 pz     (m=0)
-              2 px     (real combination of m=+/-1 with cosine)
-              3 py     (real combination of m=+/-1 with sine)
-            for l=2:
-              1 dz2    (m=0)
-              2 dzx    (real combination of m=+/-1 with cosine)
-              3 dzy    (real combination of m=+/-1 with sine)
-              4 dx2-y2 (real combination of m=+/-2 with cosine)
-              5 dxy    (real combination of m=+/-2 with sine)"""
-        # Oribital order. This is the way it goes into the spd Array. index 0 is resered for totals
-        self.orbitals = [
-            "s",
-            "p_y",
-            "p_z",
-            "p_x",
-            "d_xy",
-            "d_yz",
-            "d_z^2",
-            "d_x^2-y^2",
-            "d_xz",
-        ]
-
-        # These are not used
-        self.orbitalName_short = ["s", "p", "d", "tot"]
-        self.orbitalCount = None
-
-        # Opens the needed files
-        rf = open(self.lobsterin, "r")
-        self.lobsterin = rf.read()
-        rf.close()
-
-        rf = open(self.lobsterout, "r")
-        self.lobsterout = rf.read()
-        rf.close()
-
-        rf = open(self.scfin, "r")
-        self.scfin = rf.read()
-        rf.close()
-        self.dos = None
-
-        self._readFileNames()
-        self._readProjFiles()
-        # self._readHighKpoint()
-
-        return
-
-    ##########################################################################################
-    # Finding high symmetry points
-    ##########################################################################################
-
-    # def _readHighKpoint(self):
-    #     numK = int(findall("K_POINTS.*\n([0-9]*)", self.scfin)[0])
-
-    #     raw_khigh_sym = findall(
-    #         "K_POINTS.*\n\s*[0-9]*.*\n" + numK * "(.*)\n", self.scfin,
-    #     )[0]
-
-    #     tickCountIndex = 0
-    #     raw_high_symmetry = []
-    #     self.knames = []
-    #     self.kticks = []
-
-    #     for x in raw_khigh_sym:
-    #         if len(x.split()) == 5:
-
-    #             raw_high_symmetry.append(
-    #                 (float(x.split()[0]), float(x.split()[1]), float(x.split()[2]))
-    #             )
-    #             self.knames.append("$%s$" % x.split()[4].replace("!", ""))
-    #             self.kticks.append(tickCountIndex)
-    #         if float(x.split()[3]) == 0:
-    #             tickCountIndex += 1
-    #     self.high_symmetry_points = array(raw_high_symmetry)
-    #     self.nhigh_sym = len(self.knames)
-
-
-
-    #     # finds discontinuities 
-    #     for i in range(len(self.kticks)):
-    #         if(i < len(self.kticks)-1):
-    #             diff = self.kticks[ i+1 ] - self.kticks[i]
-    #             if diff == 1 :
-                    
-    #                 self.discontinuities.append(self.kticks[i])
-
-                    
-    #                 discon_name = "$" + self.knames[i].replace("$","") +"|"+ self.knames[i+1].replace("$","") + "$"
-    #                 self.knames.pop(i+1)
-    #                 self.knames[i] = discon_name
-    #                 self.kticks.pop(i+1)
-
-
-    ##########################################################################################
-    # Finding file names
-    ##########################################################################################
-
-    def _readFileNames(self):
-
-        self.ionsList = findall(
-            "calculating FatBand for Element: (.*) Orbital.*", self.lobsterout
-        )
-        raw_speciesList = findall(
-            "calculating FatBand for Element: ([a-zA-Z]*)[0-9] Orbital.*",
-            self.lobsterout,
-        )
-        self.speciesList = []
-        for x in raw_speciesList:
-            if x not in self.speciesList:
-                self.speciesList.append(x)
-                self.composition.update({str(x): 0})
-        self.nspecies = len(self.speciesList)
-        for x in raw_speciesList:
-            if x in self.speciesList:
-                self.composition[x] += 1
-
-        self.ionsCount = len(self.ionsList)
-
-        proj_orbitals = findall(
-            "calculating FatBand for Element: (.*) Orbital\(s\):\s*(.*)",
-            self.lobsterout,
-        )
-        for proj in proj_orbitals:
-            orbitals = proj[1].split()
-            for orbital in orbitals:
-                fileName = "FATBAND_" + proj[0] + "_" + orbital + ".lobster"
-                self.file_names.append(fileName)
-
-    ##########################################################################################
-    # Reading projection files
-    ##########################################################################################
-
-    def _readProjFiles(self):
-        rf = open(self.file_names[0], "r")
-        projFile = rf.read()
-        rf.close()
-
-        ##########################################################################################
-        # kpoints
-        ##########################################################################################
-
-        raw_kpoints = findall(
-            "# K-Point \d+ :\s*([-\.\\d]*)\s*([-\.\\d]*)\s*([-\.\\d]*)", projFile
-        )
-
-        self.kpointsCount = len(raw_kpoints)
-        self.kpoints = zeros(shape=(self.kpointsCount, 3))
-        for ik in range(len(raw_kpoints)):
-            for coord in range(3):
-                self.kpoints[ik][coord] = raw_kpoints[ik][coord]
-        # raw_kpoints = findall("(# K-Point \d+ :\s*[-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile)
-        # for kp in self.kpoints:
-        #     for x in range(3):
-        #         if kp[x] >= 0.5:
-        #             kp[x] -= 1
-
-        # If kdirect=False, then the kgrid will be in cartesian coordinates.
-        # Requires the reciprocal lattice vectors to be parsed from the output.
-        if not self.kdirect:
-            self.kpoints = dot(self.kpoints, self.reclat)
-
-        #########################################################################################
-        # bands
-        #########################################################################################
-
-        raw_kpoints = findall(
-            "# K-Point \d+ :\s*([-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile
-        )
-
-        # Checks for spin polarization
-        if len(findall("spillings for spin channel", self.lobsterout)) == 2:
-            self.spinCount = 2
-            bandsCount = int(findall("NBANDS\s*(\d*)", projFile)[0]) * self.spinCount
-            self.bandsCount = bandsCount // 2
-        else:
-            self.spinCount = 1
-            bandsCount = int(findall("NBANDS\s*(\d*)", projFile)[0])
-            self.bandsCount = bandsCount
-
-        band_info = []
-        for ik in range(len(raw_kpoints)):
-            expression = "# K-Point \d+ :\s*" + raw_kpoints[ik] + ".*\n"
-            kpoint_bands = findall(expression + bandsCount * "(.*)\n", projFile)[0]
-            for ikband in kpoint_bands:
-                band_info.append(ikband)
-
-        #        if len(band_info) == self.bandsCount * self.kpointsCount:
-        #            print("Number of bands headers match")
-        raw_bands = zeros(shape=(self.kpointsCount, bandsCount))
-        
-        ik = 0
-        ib = 0
-        for i in range(len(band_info)):
-            raw_bands[ik, ib] = float(band_info[i].split()[1])
-            ib += 1
-            if int(ib == bandsCount):
-                ik += 1
-                ib = 0
-        # Checks for spin polarization
-        if self.spinCount == 2:
-
-            self.bands = zeros(
-                shape=(self.kpointsCount, self.bandsCount, self.spinCount)
-            )
-            self.bands[:, 0 : self.bandsCount, 0] = raw_bands[:, 0 : self.bandsCount]
-            self.bands[:, 0 : self.bandsCount, 1] = raw_bands[
-                :, self.bandsCount : self.bandsCount * 2
-            ]
-        else:
-            
-            self.bands = zeros(
-                shape=(self.kpointsCount, self.bandsCount, self.spinCount)
-            )
-            self.bands[:, 0 : self.bandsCount, 0] = raw_bands[:, 0 : self.bandsCount]
-        #########################################################################################
-        # Forming SPD array
-        #########################################################################################
-
-        # Checks for spin polarization
-        if len(findall("spillings for spin channel", self.lobsterout)) == 2:
-            self.spinCount = 2
-        else:
-            self.spinCount = 1
-        
-        self.orbitalCount = 10
-        self.spd = zeros(
-            shape=(
-                self.kpointsCount,
-                self.bandsCount,
-                self.spinCount,
-                self.ionsCount + 1,
-                len(self.orbitals) + 2,
-            )
-        )
-
-        for file in range(len(self.file_names)):
-            rf = open(self.file_names[file], "r")
-            projFile = rf.read()
-            rf.close()
-
-            raw_kpoints = findall(
-                "# K-Point \d+ :\s*([-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile
-            )
-            ionIndex = 0
-            orbitalIndex = 0
-            current_orbital = findall("(# FATBAND.*)", projFile)[0].split()[4]
-            for i in range(len(self.ionsList)):
-                if self.ionsList[i] == self.file_names[file].split("_")[1]:
-                    ionIndex = i
-                    # print(ionIndex)
-            for i in range(len(self.orbitals)):
-                if self.orbitals[i] == sub("[0-9]", "", current_orbital):
-                    orbitalIndex = i + 1
-                    # print(orbitalIndex)
-                    # print(self.orbitals[orbitalIndex])
-
-            band_info = []
-            for ik in range(len(raw_kpoints)):
-                expression = "# K-Point \d+ :\s*" + raw_kpoints[ik] + ".*\n"
-                bands_wSpin = self.bandsCount * self.spinCount
-                band = findall(expression + bands_wSpin * "(.*)\n", projFile)[0]
-                for iband in range(self.bandsCount):
-                    if self.spinCount == 2:
-                        self.spd[ik, iband, 0, ionIndex, orbitalIndex] += float(
-                            band[iband].split()[2]
-                        )
-                        self.spd[ik, iband, 0, ionIndex, 0] = ionIndex + 1
-                        self.spd[ik, iband, 1, ionIndex, orbitalIndex] += float(
-                            band[iband + self.bandsCount].split()[2]
-                        )
-                        self.spd[ik, iband, 1, ionIndex, 0] = ionIndex + 1
-                    else:
-                        self.spd[ik, iband, 0, ionIndex, orbitalIndex] += float(
-                            band[iband].split()[2]
-                        )
-                        self.spd[ik, iband, 0, ionIndex, 0] = ionIndex + 1
-
-            self.spd[:, :, :, :, -1] = sum(self.spd[:, :, :, :, 1:-1], axis=4)
-            self.spd[:, :, :, -1, :] = sum(self.spd[:, :, :, 0:-1, :], axis=3)
-            self.spd[:, :, :, -1, 0] = 0
-
-        # colinear spin polarized case
-
-        # manipulating spd array for spin polarized calculations.
-        # The shape is (nkpoints,2*nbands,2,natoms,norbitals)
-        # The third dimension is for spin.
-        # When this is zero, the bands*2 (all spin up and down bands) have positive projections.
-        # When this is one, the the first half of bands (spin up) will have positive projections
-        # and the second half (spin down) will have negative projections. This is to adhere to
-        # the convention used in PyProcar to obtain spin density and spin magnetization.
-
-        if self.spinCount == 2:
-            print("\nLobster colinear spin calculation detected.\n")
-            self.spd2 = zeros(
-                shape=(
-                    self.kpointsCount,
-                    self.bandsCount * 2,
-                    self.spinCount,
-                    self.ionsCount + 1,
-                    len(self.orbitals) + 2,
-                )
-            )
-
-            # spin up block for spin=0
-            self.spd2[:, : self.bandsCount, 0, :, :] = self.spd[:, :, 0, :, :]
-
-            # spin down block for spin=0
-            self.spd2[:, self.bandsCount :, 0, :, :] = self.spd[:, :, 1, :, :]
-
-            # spin up block for spin=1
-            self.spd2[:, : self.bandsCount, 1, :, :] = self.spd[:, :, 0, :, :]
-
-            # spin down block for spin=1
-            self.spd2[:, self.bandsCount :, 1, :, :] = -1 * self.spd[:, :, 1, :, :]
-
-            self.spd = self.spd2
-
-            # Reshaping bands array to inlcude all bands (spin up and down)
-            # self.bands = concatenate((self.bands, self.bands), axis=1)
-
-            # Reshaping bands array to inlcude all bands (spin up and down)
-            self.bands = self.bands.reshape(
-                self.kpointsCount, self.bandsCount * 2, order="F"
-            )
-        else:
-            self.bands = self.bands.reshape(
-                self.kpointsCount, self.bandsCount, order="F"
-            )
-    @property
-    def fermi(self):
-        """
-        Returns the fermi energy read from .out
-        """
-
-        fi = open(self.outfile, "r")
-        data = fi.read()
-        fi.close()
-        fermi = float(findall(r"the\s*Fermi\s*energy\s*is\s*([\s\d.]*)ev", data)[0])
-        return fermi
-
-    @property
-    def reclat(self):
-        """
-        Returns the reciprocal lattice read from .out
-        """
-        rf = open(self.outfile, "r")
-        data = rf.read()
-        rf.close()
-
-        alat = float(findall(r"alat\)\s*=\s*([\d.e+-]*)", data)[0])
-
-        b1 = array(
-            findall(r"b\(1\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
-        )
-        b2 = array(
-            findall(r"b\(2\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
-        )
-        b3 = array(
-            findall(r"b\(3\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
-        )
-
-        reclat = array((b1, b2, b3))
-
-        # Transposing to get the correct format
-        # reclat = reclat
-
-        return reclat
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Jun 25 03:12:50 2020
+@author: Logan Lang
+"""
+
+
+from re import findall, search, match, DOTALL, MULTILINE, finditer, compile, sub
+
+from numpy import array, dot, linspace, sum, where, zeros, pi, concatenate
+import logging
+
+
+class LobsterParser:
+    def __init__(
+        self,
+        lobsterin="lobsterin",
+        lobsterout="lobsterout",
+        scfin="scf.in",
+        outfile="scf.out",
+        kdirect=True,
+        lobstercode="qe",
+    ):
+
+        self.lobsterin = lobsterin
+        self.scfin = scfin
+        self.outfile = outfile
+        self.lobsterout = lobsterout
+        self.dosin = "DOSCAR.lobster"
+
+        self.file_names = []
+
+        self.discontinuities = []
+        self.kdirect = kdirect
+        ############################
+        self.high_symmetry_points = None
+        self.nhigh_sym = None
+        self.nspecies = None
+
+        self.composition = {}
+
+        self.kticks = None
+        self.knames = None
+
+        self.speciesList = None
+
+        self.kpoints = None
+        self.kpointsCount = None
+        self.bands = None
+        self.bandsCount = None
+        self.ionsList = None
+        self.ionsCount = None
+        self.spinCount = None
+
+        # Used to store atomic states at the top of the kpdos.out file
+        self.states = None
+
+        
+
+        self.spd = None
+        """ for l=1:
+              1 pz     (m=0)
+              2 px     (real combination of m=+/-1 with cosine)
+              3 py     (real combination of m=+/-1 with sine)
+            for l=2:
+              1 dz2    (m=0)
+              2 dzx    (real combination of m=+/-1 with cosine)
+              3 dzy    (real combination of m=+/-1 with sine)
+              4 dx2-y2 (real combination of m=+/-2 with cosine)
+              5 dxy    (real combination of m=+/-2 with sine)"""
+        # Oribital order. This is the way it goes into the spd Array. index 0 is resered for totals
+        self.orbitals = [
+            "s",
+            "p_y",
+            "p_z",
+            "p_x",
+            "d_xy",
+            "d_yz",
+            "d_z^2",
+            "d_x^2-y^2",
+            "d_xz",
+        ]
+
+        # These are not used
+        self.orbitalName_short = ["s", "p", "d", "tot"]
+        self.orbitalCount = None
+
+        # Opens the needed files
+        rf = open(self.lobsterin, "r")
+        self.lobsterin = rf.read()
+        rf.close()
+
+        rf = open(self.lobsterout, "r")
+        self.lobsterout = rf.read()
+        rf.close()
+
+        rf = open(self.scfin, "r")
+        self.scfin = rf.read()
+        rf.close()
+        self.dos = None
+
+        self._readFileNames()
+        self._readProjFiles()
+        self._readHighKpoint()
+
+        return
+
+    ##########################################################################################
+    # Finding high symmetry points
+    ##########################################################################################
+
+    def _readHighKpoint(self):
+        numK = int(findall("K_POINTS.*\n([0-9]*)", self.scfin)[0])
+
+        raw_khigh_sym = findall(
+            "K_POINTS.*\n\s*[0-9]*.*\n" + numK * "(.*)\n", self.scfin,
+        )[0]
+
+        tickCountIndex = 0
+        raw_high_symmetry = []
+        self.knames = []
+        self.kticks = []
+
+        for x in raw_khigh_sym:
+            if len(x.split()) == 5:
+
+                raw_high_symmetry.append(
+                    (float(x.split()[0]), float(x.split()[1]), float(x.split()[2]))
+                )
+                self.knames.append("$%s$" % x.split()[4].replace("!", ""))
+                self.kticks.append(tickCountIndex)
+            if float(x.split()[3]) == 0:
+                tickCountIndex += 1
+        self.high_symmetry_points = array(raw_high_symmetry)
+        self.nhigh_sym = len(self.knames)
+
+
+
+        # finds discontinuities 
+        for i in range(len(self.kticks)):
+            if(i < len(self.kticks)-1):
+                diff = self.kticks[ i+1 ] - self.kticks[i]
+                if diff == 1 :
+                    
+                    self.discontinuities.append(self.kticks[i])
+
+                    
+                    discon_name = "$" + self.knames[i].replace("$","") +"|"+ self.knames[i+1].replace("$","") + "$"
+                    self.knames.pop(i+1)
+                    self.knames[i] = discon_name
+                    self.kticks.pop(i+1)
+
+
+    ##########################################################################################
+    # Finding file names
+    ##########################################################################################
+
+    def _readFileNames(self):
+
+        self.ionsList = findall(
+            "calculating FatBand for Element: (.*) Orbital.*", self.lobsterout
+        )
+        raw_speciesList = findall(
+            "calculating FatBand for Element: ([a-zA-Z]*)[0-9] Orbital.*",
+            self.lobsterout,
+        )
+        self.speciesList = []
+        for x in raw_speciesList:
+            if x not in self.speciesList:
+                self.speciesList.append(x)
+                self.composition.update({str(x): 0})
+        self.nspecies = len(self.speciesList)
+        for x in raw_speciesList:
+            if x in self.speciesList:
+                self.composition[x] += 1
+
+        self.ionsCount = len(self.ionsList)
+
+        proj_orbitals = findall(
+            "calculating FatBand for Element: (.*) Orbital\(s\):\s*(.*)",
+            self.lobsterout,
+        )
+        for proj in proj_orbitals:
+            orbitals = proj[1].split()
+            for orbital in orbitals:
+                fileName = "FATBAND_" + proj[0] + "_" + orbital + ".lobster"
+                self.file_names.append(fileName)
+
+    ##########################################################################################
+    # Reading projection files
+    ##########################################################################################
+
+    def _readProjFiles(self):
+        rf = open(self.file_names[0], "r")
+        projFile = rf.read()
+        rf.close()
+
+        ##########################################################################################
+        # kpoints
+        ##########################################################################################
+
+        raw_kpoints = findall(
+            "# K-Point \d+ :\s*([-\.\\d]*)\s*([-\.\\d]*)\s*([-\.\\d]*)", projFile
+        )
+
+        self.kpointsCount = len(raw_kpoints)
+        self.kpoints = zeros(shape=(self.kpointsCount, 3))
+        for ik in range(len(raw_kpoints)):
+            for coord in range(3):
+                self.kpoints[ik][coord] = raw_kpoints[ik][coord]
+        # raw_kpoints = findall("(# K-Point \d+ :\s*[-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile)
+
+        # If kdirect=False, then the kgrid will be in cartesian coordinates.
+        # Requires the reciprocal lattice vectors to be parsed from the output.
+        if not self.kdirect:
+            self.kpoints = dot(self.kpoints, self.reclat)
+
+        #########################################################################################
+        # bands
+        #########################################################################################
+
+        raw_kpoints = findall(
+            "# K-Point \d+ :\s*([-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile
+        )
+
+        # Checks for spin polarization
+        if len(findall("spillings for spin channel", self.lobsterout)) == 2:
+            self.spinCount = 2
+            bandsCount = int(findall("NBANDS\s*(\d*)", projFile)[0]) * self.spinCount
+            self.bandsCount = bandsCount // 2
+        else:
+            self.spinCount = 1
+            bandsCount = int(findall("NBANDS\s*(\d*)", projFile)[0])
+            self.bandsCount = bandsCount
+
+        band_info = []
+        for ik in range(len(raw_kpoints)):
+            expression = "# K-Point \d+ :\s*" + raw_kpoints[ik] + ".*\n"
+            kpoint_bands = findall(expression + bandsCount * "(.*)\n", projFile)[0]
+            for ikband in kpoint_bands:
+                band_info.append(ikband)
+
+        #        if len(band_info) == self.bandsCount * self.kpointsCount:
+        #            print("Number of bands headers match")
+        raw_bands = zeros(shape=(self.kpointsCount, bandsCount))
+        
+        ik = 0
+        ib = 0
+        for i in range(len(band_info)):
+            raw_bands[ik, ib] = float(band_info[i].split()[1])
+            ib += 1
+            if int(ib == bandsCount):
+                ik += 1
+                ib = 0
+        # Checks for spin polarization
+        if self.spinCount == 2:
+
+            self.bands = zeros(
+                shape=(self.kpointsCount, self.bandsCount, self.spinCount)
+            )
+            self.bands[:, 0 : self.bandsCount, 0] = raw_bands[:, 0 : self.bandsCount]
+            self.bands[:, 0 : self.bandsCount, 1] = raw_bands[
+                :, self.bandsCount : self.bandsCount * 2
+            ]
+        else:
+            
+            self.bands = zeros(
+                shape=(self.kpointsCount, self.bandsCount, self.spinCount)
+            )
+            self.bands[:, 0 : self.bandsCount, 0] = raw_bands[:, 0 : self.bandsCount]
+        #########################################################################################
+        # Forming SPD array
+        #########################################################################################
+
+        # Checks for spin polarization
+        if len(findall("spillings for spin channel", self.lobsterout)) == 2:
+            self.spinCount = 2
+        else:
+            self.spinCount = 1
+        
+        self.orbitalCount = 10
+        self.spd = zeros(
+            shape=(
+                self.kpointsCount,
+                self.bandsCount,
+                self.spinCount,
+                self.ionsCount + 1,
+                len(self.orbitals) + 2,
+            )
+        )
+
+        for file in range(len(self.file_names)):
+            rf = open(self.file_names[file], "r")
+            projFile = rf.read()
+            rf.close()
+
+            raw_kpoints = findall(
+                "# K-Point \d+ :\s*([-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile
+            )
+            ionIndex = 0
+            orbitalIndex = 0
+            current_orbital = findall("(# FATBAND.*)", projFile)[0].split()[4]
+            for i in range(len(self.ionsList)):
+                if self.ionsList[i] == self.file_names[file].split("_")[1]:
+                    ionIndex = i
+                    # print(ionIndex)
+            for i in range(len(self.orbitals)):
+                if self.orbitals[i] == sub("[0-9]", "", current_orbital):
+                    orbitalIndex = i + 1
+
+            band_info = []
+            for ik in range(len(raw_kpoints)):
+                expression = "# K-Point \d+ :\s*" + raw_kpoints[ik] + ".*\n"
+                bands_wSpin = self.bandsCount * self.spinCount
+                band = findall(expression + bands_wSpin * "(.*)\n", projFile)[0]
+                for iband in range(self.bandsCount):
+                    if self.spinCount == 2:
+                        self.spd[ik, iband, 0, ionIndex, orbitalIndex] += float(
+                            band[iband].split()[2]
+                        )
+                        self.spd[ik, iband, 0, ionIndex, 0] = ionIndex + 1
+                        self.spd[ik, iband, 1, ionIndex, orbitalIndex] += float(
+                            band[iband + self.bandsCount].split()[2]
+                        )
+                        self.spd[ik, iband, 1, ionIndex, 0] = ionIndex + 1
+                    else:
+                        self.spd[ik, iband, 0, ionIndex, orbitalIndex] += float(
+                            band[iband].split()[2]
+                        )
+                        self.spd[ik, iband, 0, ionIndex, 0] = ionIndex + 1
+
+            self.spd[:, :, :, :, -1] = sum(self.spd[:, :, :, :, 1:-1], axis=4)
+            self.spd[:, :, :, -1, :] = sum(self.spd[:, :, :, 0:-1, :], axis=3)
+            self.spd[:, :, :, -1, 0] = 0
+
+        # colinear spin polarized case
+
+        # manipulating spd array for spin polarized calculations.
+        # The shape is (nkpoints,2*nbands,2,natoms,norbitals)
+        # The third dimension is for spin.
+        # When this is zero, the bands*2 (all spin up and down bands) have positive projections.
+        # When this is one, the the first half of bands (spin up) will have positive projections
+        # and the second half (spin down) will have negative projections. This is to adhere to
+        # the convention used in PyProcar to obtain spin density and spin magnetization.
+
+        if self.spinCount == 2:
+            print("\nLobster colinear spin calculation detected.\n")
+            self.spd2 = zeros(
+                shape=(
+                    self.kpointsCount,
+                    self.bandsCount * 2,
+                    self.spinCount,
+                    self.ionsCount + 1,
+                    len(self.orbitals) + 2,
+                )
+            )
+
+            # spin up block for spin=0
+            self.spd2[:, : self.bandsCount, 0, :, :] = self.spd[:, :, 0, :, :]
+
+            # spin down block for spin=0
+            self.spd2[:, self.bandsCount :, 0, :, :] = self.spd[:, :, 1, :, :]
+
+            # spin up block for spin=1
+            self.spd2[:, : self.bandsCount, 1, :, :] = self.spd[:, :, 0, :, :]
+
+            # spin down block for spin=1
+            self.spd2[:, self.bandsCount :, 1, :, :] = -1 * self.spd[:, :, 1, :, :]
+
+            self.spd = self.spd2
+
+            # Reshaping bands array to inlcude all bands (spin up and down)
+            # self.bands = concatenate((self.bands, self.bands), axis=1)
+
+            # Reshaping bands array to inlcude all bands (spin up and down)
+            self.bands = self.bands.reshape(
+                self.kpointsCount, self.bandsCount * 2, order="F"
+            )
+        else:
+            self.bands = self.bands.reshape(
+                self.kpointsCount, self.bandsCount, order="F"
+            )
+    @property
+    def fermi(self):
+        """
+        Returns the fermi energy read from .out
+        """
+
+        fi = open(self.outfile, "r")
+        data = fi.read()
+        fi.close()
+        fermi = float(findall(r"the\s*Fermi\s*energy\s*is\s*([\s\d.]*)ev", data)[0])
+        return fermi
+
+    @property
+    def reclat(self):
+        """
+        Returns the reciprocal lattice read from .out
+        """
+        rf = open(self.outfile, "r")
+        data = rf.read()
+        rf.close()
+
+        alat = float(findall(r"alat\)\s*=\s*([\d.e+-]*)", data)[0])
+
+        b1 = array(
+            findall(r"b\(1\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
+        )
+        b2 = array(
+            findall(r"b\(2\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
+        )
+        b3 = array(
+            findall(r"b\(3\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
+        )
+
+        reclat = (2 * pi / alat) * (array((b1, b2, b3)))
+
+        # Transposing to get the correct format
+        reclat = reclat.T
+
+        return reclat
```

### Comparing `PyProcar-5.6.6/pyprocar/lobsterparser/lobsterparser.py` & `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterfermiparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from re import findall, search, match, DOTALL, MULTILINE, finditer, compile, sub
 
 from numpy import array, dot, linspace, sum, where, zeros, pi, concatenate
 import logging
 
 
-class LobsterParser:
+class LobsterFermiParser:
     def __init__(
         self,
         lobsterin="lobsterin",
         lobsterout="lobsterout",
         scfin="scf.in",
         outfile="scf.out",
         kdirect=True,
@@ -97,62 +97,62 @@
         rf = open(self.scfin, "r")
         self.scfin = rf.read()
         rf.close()
         self.dos = None
 
         self._readFileNames()
         self._readProjFiles()
-        self._readHighKpoint()
+        # self._readHighKpoint()
 
         return
 
     ##########################################################################################
     # Finding high symmetry points
     ##########################################################################################
 
-    def _readHighKpoint(self):
-        numK = int(findall("K_POINTS.*\n([0-9]*)", self.scfin)[0])
+    # def _readHighKpoint(self):
+    #     numK = int(findall("K_POINTS.*\n([0-9]*)", self.scfin)[0])
 
-        raw_khigh_sym = findall(
-            "K_POINTS.*\n\s*[0-9]*.*\n" + numK * "(.*)\n", self.scfin,
-        )[0]
-
-        tickCountIndex = 0
-        raw_high_symmetry = []
-        self.knames = []
-        self.kticks = []
-
-        for x in raw_khigh_sym:
-            if len(x.split()) == 5:
-
-                raw_high_symmetry.append(
-                    (float(x.split()[0]), float(x.split()[1]), float(x.split()[2]))
-                )
-                self.knames.append("$%s$" % x.split()[4].replace("!", ""))
-                self.kticks.append(tickCountIndex)
-            if float(x.split()[3]) == 0:
-                tickCountIndex += 1
-        self.high_symmetry_points = array(raw_high_symmetry)
-        self.nhigh_sym = len(self.knames)
+    #     raw_khigh_sym = findall(
+    #         "K_POINTS.*\n\s*[0-9]*.*\n" + numK * "(.*)\n", self.scfin,
+    #     )[0]
+
+    #     tickCountIndex = 0
+    #     raw_high_symmetry = []
+    #     self.knames = []
+    #     self.kticks = []
+
+    #     for x in raw_khigh_sym:
+    #         if len(x.split()) == 5:
+
+    #             raw_high_symmetry.append(
+    #                 (float(x.split()[0]), float(x.split()[1]), float(x.split()[2]))
+    #             )
+    #             self.knames.append("$%s$" % x.split()[4].replace("!", ""))
+    #             self.kticks.append(tickCountIndex)
+    #         if float(x.split()[3]) == 0:
+    #             tickCountIndex += 1
+    #     self.high_symmetry_points = array(raw_high_symmetry)
+    #     self.nhigh_sym = len(self.knames)
 
 
 
-        # finds discontinuities 
-        for i in range(len(self.kticks)):
-            if(i < len(self.kticks)-1):
-                diff = self.kticks[ i+1 ] - self.kticks[i]
-                if diff == 1 :
+    #     # finds discontinuities 
+    #     for i in range(len(self.kticks)):
+    #         if(i < len(self.kticks)-1):
+    #             diff = self.kticks[ i+1 ] - self.kticks[i]
+    #             if diff == 1 :
                     
-                    self.discontinuities.append(self.kticks[i])
+    #                 self.discontinuities.append(self.kticks[i])
 
                     
-                    discon_name = "$" + self.knames[i].replace("$","") +"|"+ self.knames[i+1].replace("$","") + "$"
-                    self.knames.pop(i+1)
-                    self.knames[i] = discon_name
-                    self.kticks.pop(i+1)
+    #                 discon_name = "$" + self.knames[i].replace("$","") +"|"+ self.knames[i+1].replace("$","") + "$"
+    #                 self.knames.pop(i+1)
+    #                 self.knames[i] = discon_name
+    #                 self.kticks.pop(i+1)
 
 
     ##########################################################################################
     # Finding file names
     ##########################################################################################
 
     def _readFileNames(self):
@@ -205,14 +205,18 @@
 
         self.kpointsCount = len(raw_kpoints)
         self.kpoints = zeros(shape=(self.kpointsCount, 3))
         for ik in range(len(raw_kpoints)):
             for coord in range(3):
                 self.kpoints[ik][coord] = raw_kpoints[ik][coord]
         # raw_kpoints = findall("(# K-Point \d+ :\s*[-\.\\d]*\s*[-\.\\d]*\s*[-\.\\d]*)", projFile)
+        # for kp in self.kpoints:
+        #     for x in range(3):
+        #         if kp[x] >= 0.5:
+        #             kp[x] -= 1
 
         # If kdirect=False, then the kgrid will be in cartesian coordinates.
         # Requires the reciprocal lattice vectors to be parsed from the output.
         if not self.kdirect:
             self.kpoints = dot(self.kpoints, self.reclat)
 
         #########################################################################################
@@ -411,13 +415,13 @@
         b2 = array(
             findall(r"b\(2\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
         )
         b3 = array(
             findall(r"b\(3\)\s*=\s*\(([\d.\s+-e]*)", data)[0].split(), dtype="float64"
         )
 
-        reclat = (2 * pi / alat) * (array((b1, b2, b3)))
+        reclat = array((b1, b2, b3))
 
         # Transposing to get the correct format
-        reclat = reclat.T
+        # reclat = reclat
 
         return reclat
```

### Comparing `PyProcar-5.6.6/pyprocar/procarfilefilter/procarfilefilter.py` & `PyProcar-6.0.0/pyprocar/utils/procarfilefilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,475 +1,475 @@
-import logging
-import re
-import sys
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from ..utilsprocar import UtilsProcar
-
-
-class ProcarFileFilter:
-    """Process a PROCAR file fields line-wise, specially useful for HUGE
-  files. This could be thought as pre-processing, writting a new
-  PROCAR-like file but reduced in some way.
-
-  A PROCAR File is basically an multi-dimmensional arrays of data, the
-  largest being:
-  spd_data[#kpoints][#band][#ispin][#atom][#orbital]
-
-  while the number of Kpoints d'ont seems a target for reduction
-  (omission or averaging), the other fields can be reduced, for
-  instance: grouping the atoms by species or as "surtrate" and
-  "adsorbate", or just keeping the bands close to the Fermi energy, or
-  discarding the d-orbitals in a s-p system. You got the idea, rigth?
-
-  Example:
-
-  -To group the "s", "p" y "d" orbitals from the file PROCAR and write
-   them in PROCAR-spd:
-
-   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
-   >>> a.FilterOrbitals([[0],[1,2,3],[4,5,6,7,8]], ['s','p', 'd'])
-
-       The PROCAR-new will have just 3+1 columns (orbitals are colum-wise
-       , take a look to the file). If you omit the ['s', 'p', 'd'] list,
-       the new orbitals will have a generic meaningless name (o1, o2, o3)
-
-  -To group the atoms 1,2,5,6 and 3,4,7,8 from PROCAR and write them
-   in PROCAR-new (note the 0-based indexes):
-
-   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
-   >>> a.FilterAtoms([[0,1,4,5],[2,3,6,7]])
-
-   -To select just the total density (ie: ignoring the spin-resolved stuff,
-    if any)from PROCAR and write it in PROCAR-new:
-
-   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
-   >>> a.FilterSpin([0])
-
-  """
-
-    def __init__(self, infile=None, outfile=None, loglevel=logging.WARNING):
-        """Initialize the class.
-
-    Params: `infile=None`, input fileName
-    """
-        self.infile = infile
-        self.outfile = outfile
-
-        # We want a logging to tell us what is happening
-        self.log = logging.getLogger("ProcarFileFilter")
-        self.log.setLevel(loglevel)
-        # This is a handler for logging, by now just keep it
-        # untouched. Dont really matters its usage
-        self.ch = logging.StreamHandler()
-        self.ch.setFormatter(
-            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
-        )
-        self.ch.setLevel(logging.DEBUG)
-        self.log.addHandler(self.ch)
-        # At last, one message to the logger.
-        self.log.debug("ProcarFileFilter instanciated")
-        return
-
-    ##########################SCRIPTS#################################
-
-    # def scriptFilter(self,inFile,outFile,atoms=None,orbitals=None,orbital_names=None,bands=None,spin=None,human_atoms=False):
-    #   print "Input file  :", inFile
-    #   print "Output file :", outFile
-
-    #   print "atoms       :", atoms
-    #   if atoms:
-    #     print "human_atoms     :", human_atoms
-    #   print "orbitals  :", orbitals
-    #   if orbitals:
-    #       print "orb. names  :", orbital_names
-    #     print "bands       :", bands
-    #     print "spins       :", spin
-
-    #   #Access init class of ProcarFileFilter and pass two arguments
-    #   FileFilter = ProcarFileFilter(inFile,outFile)
-
-    #   #for atoms
-    #   if atoms:
-    #     print "Manipulating the atoms"
-
-    #     if human_atoms:
-    #       atoms = [[y-1 for y in x] for x in atoms]
-    #       print "new atoms list :", atoms
-
-    #     #Now just left to call the driver member
-    #     FileFilter.FilterAtoms(atoms)
-
-    #   #for orbitals
-    #   elif orbitals:
-    #     print "Manipulating the orbitals"
-    #     #If orbitals orbital_names is None, it needs to be filled
-    #     if orbital_names is None:
-    #       orbital_names = ["o"+str(x) for x in range(len(orbitals))]
-    #       print "New orbitals names (default): ", orbital_names
-    #     #testing if makes sense
-    #     if len(orbitals) != len(orbital_names):
-    #       raise RuntimeError("length of orbitals and orbitals names do not match")
-
-    #     FileFilter.FilterOrbitals(orbitals,orbital_names)
-
-    #   #for bands
-    #   elif bands:
-    #     print "Manipulating the bands"
-
-    #     bmin = bands[0]
-    #     bmax = bands[1]
-    #     if bmax < bmin:
-    #       bmax, bmin = bmin, bmax
-    #       print "New bands limits: ", bmin, " to ", bmax
-
-    #     FileFilter.FilterBands(bmin,bmax)
-
-    #   #for spin
-    #   elif spin:
-    #     print "Manipulating the spin"
-
-    #     FileFilter.FilterSpin(spin)
-
-    #   return
-
-    ##################################################################
-
-    def setInFile(self, infile):
-        """Sets a input file `infile`, it can contains the path to the file"""
-        self.infile = infile
-        self.log.info("Input File: " + infile)
-        return
-
-    def setOutFile(self, outfile):
-        """Sets a output file `outfile`, it can contains the path to the file"""
-        self.outfile = outfile
-        self.log.info("Out File: " + outfile)
-        return
-
-    def FilterOrbitals(self, orbitals, orbitalsNames):
-        """
-    Reads the file already set by SetInFile() and writes a new
-    file already set by SetOutFile(). The new file only has the
-    selected/grouped orbitals.
-
-    Args:
-
-    -orbitals: nested iterable with the orbitals indexes to be
-      considered. For example: [[0],[2]] means select the first
-      orbital ("s") and the second one ("pz").
-      [[0],[1,2,3],[4,5,6,7,8]] is ["s", "p", "d"].
-
-    -orbitalsNames: The name to be put in each new orbital field (of a
-      orbital line). For example ["s","p","d"] is a good
-      `orbitalsName` for the `orbitals`=[[0],[1,2,3],[4,5,6,7,8]].
-      However, ["foo", "bar", "baz"] is equally valid.
-
-    Note:
-      -The atom index is not counted as the first field.
-      -The last column ('tot') is so important that it is always
-       included. Do not needs to be called
-    """
-        # setting iostuff, this method -and class- should not made any
-        # checking about IO, that is the job of the caller
-        self.log.info("In File: " + self.infile)
-        self.log.info("Out File: " + self.outfile)
-        # open the files
-        fout = open(self.outfile, "w")
-        fopener = UtilsProcar()
-        fin = fopener.OpenFile(self.infile)
-        for line in fin:
-            if re.match(r"\s*ion\s*", line):
-                # self.log.debug("orbital line found: " + line)
-                line = " ".join(["ion"] + orbitalsNames + ["tot"]) + "\n"
-
-            elif re.match(r"\s*\d+\s*", line) or re.match(r"\s*tot\s*", line):
-                # self.log.debug("data line found: " + line)
-                line = line.split()
-                # all floats to an array
-                data = np.array(line[1:], dtype=float)
-                # setting a new line, keeping just the first value
-                line = line[:1]
-                for orbset in orbitals:
-                    line.append(data[orbset].sum())
-                # the last value ("tot") always  should be written
-                line.append(data[-1])
-                # converting to str
-                line = [str(x) for x in line]
-                line = " ".join(line) + "\n"
-            fout.write(line)
-
-        return
-
-    def FilterAtoms(self, atomsGroups):
-        """
-    Reads the file already set by SetInFile() and writes a new
-    file already set by SetOutFile(). The new file only has the
-    selected/grouped atoms.
-
-    Args:
-
-    -atomsGroups: nested iterable with the atoms indexes (0-based) to
-      be considered. For example: [[0],[2]] means select the first and
-      the second atoms. While [[1,2,3],[4,5,6,7,8]] means select the
-      contribution of atoms 1+2+3 and 4+5+6+7+8
-
-    Note:
-      -The atom index is c-based (or python) beginning with 0
-      -The output has a dummy atom index, without any intrisic meaning
-
-    """
-        # setting iostuff, this method -and class- should not made any
-        # checking about IO, that is the job of the caller
-        self.log.info("In File: " + self.infile)
-        self.log.info("Out File: " + self.outfile)
-        # open the files
-        fout = open(self.outfile, "w")
-        fopener = UtilsProcar()
-        with fopener.OpenFile(self.infile) as fin:
-            # I need to change the numbers of ions, it will needs the second
-            # line. The first one is not needed
-            fout.write(fin.readline())
-            line = fin.readline()
-            line = line.split()
-            # the very last value needs to be changed
-            line[-1] = str(len(atomsGroups))
-            line = " ".join(line)
-            fout.write(line + "\n")
-
-            # now parsing the rest of the file
-            data = []
-            for line in fin:
-                # if line has data just capture it
-                if re.match(r"\s*\d+\s*", line):
-                    # self.log.debug("atoms line found: " + line)
-                    data.append(line)
-                # if `line` is a end of th block (begins with 'tot'), do the
-                # work. And clean up data then
-                elif re.match(r"\s*tot\s*", line):
-                    # self.log.debug("tot line found: " + line)
-                    # making an array
-                    data = [x.split() for x in data]
-                    data = np.array(data, dtype=float)
-                    # iterating on the atoms groups
-                    for index in range(len(atomsGroups)):
-                        atoms = atomsGroups[index]
-                        # summing colum-wise
-                        atomLine = data[atoms].sum(axis=0)
-                        atomLine = [str(x) for x in atomLine]
-                        # the atom index should not be averaged (anyway now is
-                        # meaningless)
-                        atomLine[0] = str(index + 1)
-                        atomLine = " ".join(atomLine)
-                        fout.write(atomLine + "\n")
-
-                    # clean the buffer
-                    data = []
-                    # and write the `tot` line
-                    fout.write(line)
-                # otherwise just write this line
-                else:
-                    fout.write(line)
-
-        return
-
-    def FilterBands(self, Min, Max):
-        """
-    Reads the file already set by SetInFile() and writes a new
-    file already set by SetOutFile(). The new file only has the
-    selected bands.
-
-    Args:
-
-    -Min, Max:
-      the minimum/maximum band  index to be considered, the indexes
-      are the same used by vasp (ie written in the file).
-
-
-    Note: -Since bands are somewhat disordered in vasp you may like to
-      consider a large region and made some trial and error
-
-    """
-        # setting iostuff, this method -and class- should not made any
-        # checking about IO, that is the job of the caller
-        self.log.info("In File: " + self.infile)
-        self.log.info("Out File: " + self.outfile)
-        # open the files
-        fout = open(self.outfile, "w")
-        fopener = UtilsProcar()
-        fin = fopener.OpenFile(self.infile)
-
-        # I need to change the numbers of kpoints, it will needs the second
-        # line. The first one is not needed
-        fout.write(fin.readline())
-        line = fin.readline()
-        # the third value needs to be changed, however better print it
-        self.log.debug("The line contaning bands number is " + line)
-        line = line.split()
-        self.log.debug("The number of bands is: " + line[7])
-        line[7] = str(Max - Min + 1)
-        line = " ".join(line)
-        fout.write(line + "\n")
-
-        # now parsing the rest of the file
-        write = True
-        for line in fin:
-            if re.match(r"\s*band\s*", line):
-                # self.log.debug("bands line found: " + line)
-                band = int(re.match(r"\s*band\s*(\d+)", line).group(1))
-                if band < Min or band > Max:
-                    write = False
-                else:
-                    write = True
-            if re.match(r"\s*k-point\s*", line):
-                write = True
-            if write:
-                fout.write(line)
-        return
-
-    def FilterSpin(self, components):
-        """Reads the file already set by SetInFile() and writes a new
-    file already set by SetOutFile(). The new file only has the
-    selected part of the density (sigma_i).
-
-    Args:
-
-    -components: For non colinear spin calculations
-      the spin component block, for instante [0] menas just
-      the density, while [1,2] would be the the sigma_x and sigma_y.
-      For colinear spin polarized calculations [0] means spin up
-      component and [1] spin down component.
-
-
-    UPDATE: Colinear spin calculation implemented. It uses regex to
-            check for the type of calculation. Hopefully, this won't
-            be an issue with memory nowadays.
-    """
-        # setting iostuff, this method -and class- should not made any
-        # checking about IO, that is the job of the caller
-        self.log.info("In File: " + self.infile)
-        self.log.info("Out File: " + self.outfile)
-
-        # First let's see if this is a spin colinear calculation.
-        fopener = UtilsProcar()
-        fin_test = fopener.OpenFile(self.infile)
-        data = fin_test.read()
-        colinear_counter = re.findall(r"#\sof\sk-points:", data)
-
-        if len(colinear_counter) == 1:
-            # This is a non colinear spin calculation.
-            # (Or no spin. But why would anyone want to filter spins in that?)
-
-            print("Non colinear spin calculation detected.")
-
-            # open the files
-            fout = open(self.outfile, "w")
-            fopener = UtilsProcar()
-            with fopener.OpenFile(self.infile) as fin:
-                counter = 0
-                for line in fin:
-                    # if any data found
-                    if re.match(r"\s*\d", line):
-                        # check if should be written
-                        if counter in components:
-                            fout.write(line)
-                    elif re.match(r"\s*tot", line):
-                        if counter in components:
-                            fout.write(line)
-                        # the next block will belong to other component
-                        counter += 1
-                    elif re.match(r"\s*ion", line):
-                        fout.write(line)
-                        counter = 0
-                    else:
-                        fout.write(line)
-
-        elif len(colinear_counter) == 2:
-            # This is a colinear spin calculation.
-            # The idea is to seperate spin up [0] and down [1] components
-            # and store them in two different PROCARS.
-            # They can then be used to plot spin up and spin down
-            # bands seperately without plotting spin density or
-            # spin magnetization.
-
-            print("Colinear spin calculation detected.")
-
-            # open the files
-            fout = open(self.outfile, "w")
-            fopener = UtilsProcar()
-            spindown_buffer = []
-            component_counter = 0
-
-            with fopener.OpenFile(self.infile) as fin:
-                for line in fin:
-                    if re.match(r"PROCAR\s*", line):
-                        # First line of the file.
-                        spindown_buffer.append(line)
-
-                    if re.match(r"#\sof\sk-points:", line):
-                        component_counter += 1
-
-                    if component_counter < 2:
-                        if components[0] == 0:
-                            # Write to file for spin up component.
-                            fout.write(line)
-                            # Keep on writing line by line until the start of
-                            # the next component, i.e. "# of k-points:".
-                    else:
-                        # Save spin down component to buffer.
-                        # Save later if asked.
-                        spindown_buffer.append(line)
-
-            if components[0] == 1:
-                for i in spindown_buffer:
-                    fout.write(i)
-
-        return
-
-    def FilterKpoints(self, Min, Max):
-        """
-    Reads the file already set by SetInFile() and writes a new
-    file already set by SetOutFile(). The new file the
-    selected bands.
-
-    Args:
-
-    -Min, Max:
-      the minimum/maximum band  kpoint to be considered, the indexes
-      are the same used by vasp (i.e. written in the file). Not starting from zero
-    """
-        # setting iostuff, this method -and class- should not made any
-        # checking about IO, that is the job of the caller
-        self.log.info("In File: " + self.infile)
-        self.log.info("Out File: " + self.outfile)
-        # open the files
-        fout = open(self.outfile, "w")
-        fopener = UtilsProcar()
-        fin = fopener.OpenFile(self.infile)
-
-        # I need to change the numbers of kpoints, it will needs the second
-        # line. The first one is not needed
-        fout.write(fin.readline())
-        line = fin.readline()
-        # the third value needs to be changed, however better print it
-        self.log.debug("The line contaning kpoints number is " + line)
-        line = line.split()
-        self.log.debug("The number of kpoints is: " + line[3])
-        line[3] = str(Max - Min + 1)
-        line = " ".join(line)
-        fout.write(line + "\n")
-
-        # now parsing the rest of the file
-        write = True
-        for line in fin:
-            if re.match(r"\s*k-point\s*", line):
-                self.log.debug("bands line found: " + line)
-                kpoint = int(re.match(r"\s*k-point\s*(\d+)", line).group(1))
-                if kpoint < Min or kpoint > Max:
-                    write = False
-                else:
-                    write = True
-            if write:
-                fout.write(line)
-        return
+import logging
+import re
+import sys
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from ..utils import UtilsProcar
+
+
+class ProcarFileFilter:
+    """Process a PROCAR file fields line-wise, specially useful for HUGE
+  files. This could be thought as pre-processing, writting a new
+  PROCAR-like file but reduced in some way.
+
+  A PROCAR File is basically an multi-dimmensional arrays of data, the
+  largest being:
+  spd_data[#kpoints][#band][#ispin][#atom][#orbital]
+
+  while the number of Kpoints d'ont seems a target for reduction
+  (omission or averaging), the other fields can be reduced, for
+  instance: grouping the atoms by species or as "surtrate" and
+  "adsorbate", or just keeping the bands close to the Fermi energy, or
+  discarding the d-orbitals in a s-p system. You got the idea, rigth?
+
+  Example:
+
+  -To group the "s", "p" y "d" orbitals from the file PROCAR and write
+   them in PROCAR-spd:
+
+   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
+   >>> a.FilterOrbitals([[0],[1,2,3],[4,5,6,7,8]], ['s','p', 'd'])
+
+       The PROCAR-new will have just 3+1 columns (orbitals are colum-wise
+       , take a look to the file). If you omit the ['s', 'p', 'd'] list,
+       the new orbitals will have a generic meaningless name (o1, o2, o3)
+
+  -To group the atoms 1,2,5,6 and 3,4,7,8 from PROCAR and write them
+   in PROCAR-new (note the 0-based indexes):
+
+   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
+   >>> a.FilterAtoms([[0,1,4,5],[2,3,6,7]])
+
+   -To select just the total density (ie: ignoring the spin-resolved stuff,
+    if any)from PROCAR and write it in PROCAR-new:
+
+   >>> a = procar.ProcarFileFilter("PROCAR", "PROCAR-new")
+   >>> a.FilterSpin([0])
+
+  """
+
+    def __init__(self, infile=None, outfile=None, loglevel=logging.WARNING):
+        """Initialize the class.
+
+    Params: `infile=None`, input fileName
+    """
+        self.infile = infile
+        self.outfile = outfile
+
+        # We want a logging to tell us what is happening
+        self.log = logging.getLogger("ProcarFileFilter")
+        self.log.setLevel(loglevel)
+        # This is a handler for logging, by now just keep it
+        # untouched. Dont really matters its usage
+        self.ch = logging.StreamHandler()
+        self.ch.setFormatter(
+            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
+        )
+        self.ch.setLevel(logging.DEBUG)
+        self.log.addHandler(self.ch)
+        # At last, one message to the logger.
+        self.log.debug("ProcarFileFilter instanciated")
+        return
+
+    ##########################SCRIPTS#################################
+
+    # def scriptFilter(self,inFile,outFile,atoms=None,orbitals=None,orbital_names=None,bands=None,spin=None,human_atoms=False):
+    #   print "Input file  :", inFile
+    #   print "Output file :", outFile
+
+    #   print "atoms       :", atoms
+    #   if atoms:
+    #     print "human_atoms     :", human_atoms
+    #   print "orbitals  :", orbitals
+    #   if orbitals:
+    #       print "orb. names  :", orbital_names
+    #     print "bands       :", bands
+    #     print "spins       :", spin
+
+    #   #Access init class of ProcarFileFilter and pass two arguments
+    #   FileFilter = ProcarFileFilter(inFile,outFile)
+
+    #   #for atoms
+    #   if atoms:
+    #     print "Manipulating the atoms"
+
+    #     if human_atoms:
+    #       atoms = [[y-1 for y in x] for x in atoms]
+    #       print "new atoms list :", atoms
+
+    #     #Now just left to call the driver member
+    #     FileFilter.FilterAtoms(atoms)
+
+    #   #for orbitals
+    #   elif orbitals:
+    #     print "Manipulating the orbitals"
+    #     #If orbitals orbital_names is None, it needs to be filled
+    #     if orbital_names is None:
+    #       orbital_names = ["o"+str(x) for x in range(len(orbitals))]
+    #       print "New orbitals names (default): ", orbital_names
+    #     #testing if makes sense
+    #     if len(orbitals) != len(orbital_names):
+    #       raise RuntimeError("length of orbitals and orbitals names do not match")
+
+    #     FileFilter.FilterOrbitals(orbitals,orbital_names)
+
+    #   #for bands
+    #   elif bands:
+    #     print "Manipulating the bands"
+
+    #     bmin = bands[0]
+    #     bmax = bands[1]
+    #     if bmax < bmin:
+    #       bmax, bmin = bmin, bmax
+    #       print "New bands limits: ", bmin, " to ", bmax
+
+    #     FileFilter.FilterBands(bmin,bmax)
+
+    #   #for spin
+    #   elif spin:
+    #     print "Manipulating the spin"
+
+    #     FileFilter.FilterSpin(spin)
+
+    #   return
+
+    ##################################################################
+
+    def setInFile(self, infile):
+        """Sets a input file `infile`, it can contains the path to the file"""
+        self.infile = infile
+        self.log.info("Input File: " + infile)
+        return
+
+    def setOutFile(self, outfile):
+        """Sets a output file `outfile`, it can contains the path to the file"""
+        self.outfile = outfile
+        self.log.info("Out File: " + outfile)
+        return
+
+    def FilterOrbitals(self, orbitals, orbitalsNames):
+        """
+    Reads the file already set by SetInFile() and writes a new
+    file already set by SetOutFile(). The new file only has the
+    selected/grouped orbitals.
+
+    Args:
+
+    -orbitals: nested iterable with the orbitals indexes to be
+      considered. For example: [[0],[2]] means select the first
+      orbital ("s") and the second one ("pz").
+      [[0],[1,2,3],[4,5,6,7,8]] is ["s", "p", "d"].
+
+    -orbitalsNames: The name to be put in each new orbital field (of a
+      orbital line). For example ["s","p","d"] is a good
+      `orbitalsName` for the `orbitals`=[[0],[1,2,3],[4,5,6,7,8]].
+      However, ["foo", "bar", "baz"] is equally valid.
+
+    Note:
+      -The atom index is not counted as the first field.
+      -The last column ('tot') is so important that it is always
+       included. Do not needs to be called
+    """
+        # setting iostuff, this method -and class- should not made any
+        # checking about IO, that is the job of the caller
+        self.log.info("In File: " + self.infile)
+        self.log.info("Out File: " + self.outfile)
+        # open the files
+        fout = open(self.outfile, "w")
+        fopener = UtilsProcar()
+        fin = fopener.OpenFile(self.infile)
+        for line in fin:
+            if re.match(r"\s*ion\s*", line):
+                # self.log.debug("orbital line found: " + line)
+                line = " ".join(["ion"] + orbitalsNames + ["tot"]) + "\n"
+
+            elif re.match(r"\s*\d+\s*", line) or re.match(r"\s*tot\s*", line):
+                # self.log.debug("data line found: " + line)
+                line = line.split()
+                # all floats to an array
+                data = np.array(line[1:], dtype=float)
+                # setting a new line, keeping just the first value
+                line = line[:1]
+                for orbset in orbitals:
+                    line.append(data[orbset].sum())
+                # the last value ("tot") always  should be written
+                line.append(data[-1])
+                # converting to str
+                line = [str(x) for x in line]
+                line = " ".join(line) + "\n"
+            fout.write(line)
+
+        return
+
+    def FilterAtoms(self, atomsGroups):
+        """
+    Reads the file already set by SetInFile() and writes a new
+    file already set by SetOutFile(). The new file only has the
+    selected/grouped atoms.
+
+    Args:
+
+    -atomsGroups: nested iterable with the atoms indexes (0-based) to
+      be considered. For example: [[0],[2]] means select the first and
+      the second atoms. While [[1,2,3],[4,5,6,7,8]] means select the
+      contribution of atoms 1+2+3 and 4+5+6+7+8
+
+    Note:
+      -The atom index is c-based (or python) beginning with 0
+      -The output has a dummy atom index, without any intrisic meaning
+
+    """
+        # setting iostuff, this method -and class- should not made any
+        # checking about IO, that is the job of the caller
+        self.log.info("In File: " + self.infile)
+        self.log.info("Out File: " + self.outfile)
+        # open the files
+        fout = open(self.outfile, "w")
+        fopener = UtilsProcar()
+        with fopener.OpenFile(self.infile) as fin:
+            # I need to change the numbers of ions, it will needs the second
+            # line. The first one is not needed
+            fout.write(fin.readline())
+            line = fin.readline()
+            line = line.split()
+            # the very last value needs to be changed
+            line[-1] = str(len(atomsGroups))
+            line = " ".join(line)
+            fout.write(line + "\n")
+
+            # now parsing the rest of the file
+            data = []
+            for line in fin:
+                # if line has data just capture it
+                if re.match(r"\s*\d+\s*", line):
+                    # self.log.debug("atoms line found: " + line)
+                    data.append(line)
+                # if `line` is a end of th block (begins with 'tot'), do the
+                # work. And clean up data then
+                elif re.match(r"\s*tot\s*", line):
+                    # self.log.debug("tot line found: " + line)
+                    # making an array
+                    data = [x.split() for x in data]
+                    data = np.array(data, dtype=float)
+                    # iterating on the atoms groups
+                    for index in range(len(atomsGroups)):
+                        atoms = atomsGroups[index]
+                        # summing colum-wise
+                        atomLine = data[atoms].sum(axis=0)
+                        atomLine = [str(x) for x in atomLine]
+                        # the atom index should not be averaged (anyway now is
+                        # meaningless)
+                        atomLine[0] = str(index + 1)
+                        atomLine = " ".join(atomLine)
+                        fout.write(atomLine + "\n")
+
+                    # clean the buffer
+                    data = []
+                    # and write the `tot` line
+                    fout.write(line)
+                # otherwise just write this line
+                else:
+                    fout.write(line)
+
+        return
+
+    def FilterBands(self, Min, Max):
+        """
+    Reads the file already set by SetInFile() and writes a new
+    file already set by SetOutFile(). The new file only has the
+    selected bands.
+
+    Args:
+
+    -Min, Max:
+      the minimum/maximum band  index to be considered, the indexes
+      are the same used by vasp (ie written in the file).
+
+
+    Note: -Since bands are somewhat disordered in vasp you may like to
+      consider a large region and made some trial and error
+
+    """
+        # setting iostuff, this method -and class- should not made any
+        # checking about IO, that is the job of the caller
+        self.log.info("In File: " + self.infile)
+        self.log.info("Out File: " + self.outfile)
+        # open the files
+        fout = open(self.outfile, "w")
+        fopener = UtilsProcar()
+        fin = fopener.OpenFile(self.infile)
+
+        # I need to change the numbers of kpoints, it will needs the second
+        # line. The first one is not needed
+        fout.write(fin.readline())
+        line = fin.readline()
+        # the third value needs to be changed, however better print it
+        self.log.debug("The line contaning bands number is " + line)
+        line = line.split()
+        self.log.debug("The number of bands is: " + line[7])
+        line[7] = str(Max - Min + 1)
+        line = " ".join(line)
+        fout.write(line + "\n")
+
+        # now parsing the rest of the file
+        write = True
+        for line in fin:
+            if re.match(r"\s*band\s*", line):
+                # self.log.debug("bands line found: " + line)
+                band = int(re.match(r"\s*band\s*(\d+)", line).group(1))
+                if band < Min or band > Max:
+                    write = False
+                else:
+                    write = True
+            if re.match(r"\s*k-point\s*", line):
+                write = True
+            if write:
+                fout.write(line)
+        return
+
+    def FilterSpin(self, components):
+        """Reads the file already set by SetInFile() and writes a new
+    file already set by SetOutFile(). The new file only has the
+    selected part of the density (sigma_i).
+
+    Args:
+
+    -components: For non colinear spin calculations
+      the spin component block, for instante [0] menas just
+      the density, while [1,2] would be the the sigma_x and sigma_y.
+      For colinear spin polarized calculations [0] means spin up
+      component and [1] spin down component.
+
+
+    UPDATE: Colinear spin calculation implemented. It uses regex to
+            check for the type of calculation. Hopefully, this won't
+            be an issue with memory nowadays.
+    """
+        # setting iostuff, this method -and class- should not made any
+        # checking about IO, that is the job of the caller
+        self.log.info("In File: " + self.infile)
+        self.log.info("Out File: " + self.outfile)
+
+        # First let's see if this is a spin colinear calculation.
+        fopener = UtilsProcar()
+        fin_test = fopener.OpenFile(self.infile)
+        data = fin_test.read()
+        colinear_counter = re.findall(r"#\sof\sk-points:", data)
+
+        if len(colinear_counter) == 1:
+            # This is a non colinear spin calculation.
+            # (Or no spin. But why would anyone want to filter spins in that?)
+
+            print("Non colinear spin calculation detected.")
+
+            # open the files
+            fout = open(self.outfile, "w")
+            fopener = UtilsProcar()
+            with fopener.OpenFile(self.infile) as fin:
+                counter = 0
+                for line in fin:
+                    # if any data found
+                    if re.match(r"\s*\d", line):
+                        # check if should be written
+                        if counter in components:
+                            fout.write(line)
+                    elif re.match(r"\s*tot", line):
+                        if counter in components:
+                            fout.write(line)
+                        # the next block will belong to other component
+                        counter += 1
+                    elif re.match(r"\s*ion", line):
+                        fout.write(line)
+                        counter = 0
+                    else:
+                        fout.write(line)
+
+        elif len(colinear_counter) == 2:
+            # This is a colinear spin calculation.
+            # The idea is to seperate spin up [0] and down [1] components
+            # and store them in two different PROCARS.
+            # They can then be used to plot spin up and spin down
+            # bands seperately without plotting spin density or
+            # spin magnetization.
+
+            print("Colinear spin calculation detected.")
+
+            # open the files
+            fout = open(self.outfile, "w")
+            fopener = UtilsProcar()
+            spindown_buffer = []
+            component_counter = 0
+
+            with fopener.OpenFile(self.infile) as fin:
+                for line in fin:
+                    if re.match(r"PROCAR\s*", line):
+                        # First line of the file.
+                        spindown_buffer.append(line)
+
+                    if re.match(r"#\sof\sk-points:", line):
+                        component_counter += 1
+
+                    if component_counter < 2:
+                        if components[0] == 0:
+                            # Write to file for spin up component.
+                            fout.write(line)
+                            # Keep on writing line by line until the start of
+                            # the next component, i.e. "# of k-points:".
+                    else:
+                        # Save spin down component to buffer.
+                        # Save later if asked.
+                        spindown_buffer.append(line)
+
+            if components[0] == 1:
+                for i in spindown_buffer:
+                    fout.write(i)
+
+        return
+
+    def FilterKpoints(self, Min, Max):
+        """
+    Reads the file already set by SetInFile() and writes a new
+    file already set by SetOutFile(). The new file the
+    selected bands.
+
+    Args:
+
+    -Min, Max:
+      the minimum/maximum band  kpoint to be considered, the indexes
+      are the same used by vasp (i.e. written in the file). Not starting from zero
+    """
+        # setting iostuff, this method -and class- should not made any
+        # checking about IO, that is the job of the caller
+        self.log.info("In File: " + self.infile)
+        self.log.info("Out File: " + self.outfile)
+        # open the files
+        fout = open(self.outfile, "w")
+        fopener = UtilsProcar()
+        fin = fopener.OpenFile(self.infile)
+
+        # I need to change the numbers of kpoints, it will needs the second
+        # line. The first one is not needed
+        fout.write(fin.readline())
+        line = fin.readline()
+        # the third value needs to be changed, however better print it
+        self.log.debug("The line contaning kpoints number is " + line)
+        line = line.split()
+        self.log.debug("The number of kpoints is: " + line[3])
+        line[3] = str(Max - Min + 1)
+        line = " ".join(line)
+        fout.write(line + "\n")
+
+        # now parsing the rest of the file
+        write = True
+        for line in fin:
+            if re.match(r"\s*k-point\s*", line):
+                self.log.debug("bands line found: " + line)
+                kpoint = int(re.match(r"\s*k-point\s*(\d+)", line).group(1))
+                if kpoint < Min or kpoint > Max:
+                    write = False
+                else:
+                    write = True
+            if write:
+                fout.write(line)
+        return
```

### Comparing `PyProcar-5.6.6/pyprocar/procarparser/procarparser.py` & `PyProcar-6.0.0/pyprocar/core/procarunfold/_bak.procarparser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,751 +1,584 @@
-import numpy as np
-import re
-import logging
-import matplotlib.pyplot as plt
-import sys
-from ..utilsprocar import UtilsProcar
-
-
-class ProcarParser:
-    """Parses a PROCAR file and store it in memory. It only deals with
-    PROCAR files, that means no Fermi energy (UtilsProcar.FermiOutcar
-    can help), and the reciprocal vectors should be supplied (if used,
-    see UtilsProcar class).
-
-    Members:
-
-    __init__(self, loglevel): The setup the variables internally, `loglevel`
-      sets the verbosity level ie: `loglevel=logging.DEBUG` for debugging. Its
-      default is `logging.WARNING`
-
-    readFile(self, procar=None, permissive=False, recLattice=None):
-      The only method of the API it load the file completely.
-
-      Arguments:
-    `procar=None`: name of the PROCAR file, can be a gzipped file (the
-                    extension is no required). The default covers a wide range
-                    of obvious alternatives.
-      `permissive=False`: Set to `True` if the PROCAR file has problems reading
-                        the Kpoints (stupid Fortran), but in that case the
-                          Kpoints mesh will be discarded. Future updates could
-                          allow it to handle other formating/corruption issues.
-      `recLattice`=None: Reciprical Vectors, you want to provide them since not
-                        all the paths on the BZ are the same.
-
-    Don't use the other methods beggining with underscores "_"
-
-    Example:
-    To read a PROCAR or PROCAR.gz file:
-    >>> foo = ProcarParser()
-    >>> foo.readFile()
-
-    To include the reciprocal vectors, and file name MyFirstPROCAR
-    >>> outcarparser = UtilsProcar()
-    >>> recLat = outcarparser.RecLatOutcar(args.outcar)
-    >>> foo = ProcarParser()
-    >>> foo.readFile("MyFirstPROCAR", recLat=recLat)
-
-    """
-
-    def __init__(self, loglevel=logging.WARNING):
-        # array with k-points, they have the following values
-        # -None: if not parsed (yet) or parsed with a `permissive` flag on
-        # -direct coordinates: if a recLattice was not supplied to the parser
-        # -cartesian coords: if a recLattice was supplied to the parser.
-        # In the later cases, self.kpoints.shape=(self.kpointsCount, 3)
-        self.kpoints = None
-        # Number of kpoints, as given by the KPOINTS header (PROCAR file)
-        self.kpointsCount = None
-
-        # bands headers present in PROCAR file.
-        # self.bands.shape=(self.kpointsCount,self.bandsCount)
-        self.bands = None
-        # Number of bands. For a spin polarized calculation the number of
-        # bands is double (spin ip + spin down). On this array there is no
-        # distinction between spin up and down
-        self.bandsCount = None
-
-        # Number of ions+1 the +1 is the 'tot' field, ie: the sum over all atoms
-        self.ionsCount = None
-
-        self.fileStr = None  # the actual file, stored in memory
-        self.spd = None  # the atom/orbital projected data
-        self.cspd = None  # spd data with the phase
-        self.orbitalName = [
-            "s",
-            "py",
-            "pz",
-            "px",
-            "dxy",
-            "dyz",
-            "dz2",
-            "dxz",
-            "x2-y2",
-            "fy3x2",
-            "fxyz",
-            "fyz2",
-            "fz3",
-            "fxz2",
-            "fzx2",
-            "fx3",
-            "tot",
-        ]
-        self.orbitalName_old = [
-            "s",
-            "py",
-            "pz",
-            "px",
-            "dxy",
-            "dyz",
-            "dz2",
-            "dxz",
-            "dx2",
-            "tot",
-        ]
-        self.orbitalName_short = ["s", "p", "d", "f", "tot"]
-        self.orbitalCount = None  # number of orbitals
-
-        # number of spin components (blocks of data), 1: non-magnetic non
-        # polarized, 2: spin polarized collinear, 4: non-collinear
-        # spin.
-        # NOTE: before calling to `self._readOrbital` the case '4'
-        # is marked as '1'
-        self.ispin = None
-        self.recLattice = None  # reciprocal lattice vectors
-        self.utils = UtilsProcar()
-
-        self.log = logging.getLogger("ProcarParser")
-        self.log.setLevel(loglevel)
-        self.ch = logging.StreamHandler()
-        self.ch.setFormatter(
-            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
-        )
-        self.ch.setLevel(logging.DEBUG)
-        self.log.addHandler(self.ch)
-        # At last, one message to the logger.
-        self.log.debug("Procar instanciated")
-        return
-
-    @property
-    def nspin(self):
-        """
-        number of spin, default is 1.
-        """
-        nspindict = {1: 1, 2: 2, 4: 2, None: 1}
-        return nspindict[self.ispin]
-
-    @property
-    def spd_orb(self):
-        # indices: ikpt, iband, ispin, iion, iorb
-        # remove indices and total from iorb.
-        return self.spd[:, :, :, 1:-1]
-
-    def _readKpoints(self, permissive=False):
-        """Reads the k-point headers. A typical k-point line is:
-        k-point    1 :    0.00000000 0.00000000 0.00000000  weight = 0.00003704\n
-        fills self.kpoint[kpointsCount][3]
-        The weights are discarded (are they useful?)
-        """
-        self.log.debug("readKpoints")
-        if not self.fileStr:
-            self.log.warning("You should invoke `procar.readFile()` instead. Returning")
-            return
-
-        # finding all the K-points headers
-        self.kpoints = re.findall(r"k-point\s+\d+\s*:\s+([-.\d\s]+)", self.fileStr)
-        self.log.debug(str(len(self.kpoints)) + " K-point headers found")
-        self.log.debug("The first match found is: " + str(self.kpoints[0]))
-
-        # trying to build an array
-        self.kpoints = [x.split() for x in self.kpoints]
-        try:
-            self.kpoints = np.array(self.kpoints, dtype=float)
-        except ValueError:
-            self.log.error("Ill-formatted data:")
-            print("\n".join([str(x) for x in self.kpoints]))
-            if permissive is True:
-                # Discarding the kpoints list, however I need to set
-                # self.ispin beforehand.
-                if len(self.kpoints) == self.kpointsCount:
-                    self.ispin = 1
-                elif len(self.kpoints) == 2 * self.kpointsCount:
-                    self.ispin = 2
-                else:
-                    raise ValueError("Kpoints do not match with ispin=1 or 2.")
-                self.kpoints = None
-                self.log.warning("K-points list is useless, setting it to `None`")
-                return
-            else:
-                raise ValueError("Badly formated Kpoints headers, try `--permissive`")
-        # if successful, go on
-
-        # trying to identify an non-polarized or non-collinear case, a
-        # polarized case or a defective file
-
-        if len(self.kpoints) != self.kpointsCount:
-            # if they do not match, may means two things a spin polarized
-            # case or a bad file, lets check
-            self.log.debug(
-                "Number of kpoints do not match, looking for a " "spin-polarized case"
-            )
-            # lets start testing if it is spin polarized, if so, there
-            # should be 2 identical blocks of kpoints.
-            up, down = np.vsplit(self.kpoints, 2)
-            if (up == down).all():
-                self.log.info("Spin-polarized calculation found")
-                self.ispin = 2
-                # just keeping one set of kpoints (the other will be
-                # discarded)
-                self.kpoints = up
-            else:
-                self.log.error("Number of K-points do not match! check them.")
-                raise RuntimeError("Bad Kpoints list.")
-        # if ISPIN != 2 setting ISPIN=1 (later for the non-collinear case 1->4)
-        # It is unknown until parsing the projected data
-        else:
-            self.ispin = 1
-
-        # checking again, for compatibility,
-        if len(self.kpoints) != self.kpointsCount:
-            raise RuntimeError(
-                "Kpoints number do not match with metadata (header of PROCAR)"
-            )
-
-        self.log.debug(str(self.kpoints))
-        self.log.info("The kpoints shape is " + str(self.kpoints.shape))
-
-        if self.recLattice is not None:
-            self.log.info("Changing to cartesians coordinates")
-            self.kpoints = np.dot(self.kpoints, self.recLattice)
-            self.log.debug("New kpoints: \n" + str(self.kpoints))
-        return
-
-    def _readBands(self):
-        """Reads the bands header. A typical bands is:
-        band   1 # energy   -7.11986315 # occ.  1.00000000
-
-        fills self.bands[kpointsCount][bandsCount]
-
-        The occupation numbers are discarded (are they useful?)"""
-        self.log.debug("readBands")
-        if not self.fileStr:
-            log.warning("You should invoke `procar.read()` instead. Returning")
-            return
-
-        # finding all bands
-        self.bands = re.findall(
-            r"band\s*(\d+)\s*#\s*energy\s*([-.\d\s]+)", self.fileStr
-        )
-        self.log.debug(
-            str(len(self.bands))
-            + " bands headers found, bands*Kpoints = "
-            + str(self.bandsCount * self.kpointsCount)
-        )
-        self.log.debug("The first match found is: " + str(self.bands[0]))
-
-        # checking if the number of bands match
-
-        if len(self.bands) != self.bandsCount * self.kpointsCount * self.ispin:
-            self.log.error("Number of bands headers do not match")
-            raise RuntimeError("Number of bands don't match")
-
-        # casting to array to manipulate the bands
-        self.bands = np.array(self.bands, dtype=float)
-        self.log.debug(str(self.bands))
-
-        # Now I will deal with the spin polarized case. The goal is join
-        # them like for a non-magnetic case
-        if self.ispin == 2:
-            # up and down are along the first axis
-            up, down = np.vsplit(self.bands, 2)
-            self.log.debug("up   , " + str(up.shape))
-            self.log.debug("down , " + str(down.shape))
-
-            # reshapping (the 2  means both band index and energy)
-            up.shape = (self.kpointsCount, self.bandsCount, 2)
-            down.shape = (self.kpointsCount, self.bandsCount, 2)
-
-            # setting the correct number of bands (up+down)
-            self.bandsCount *= 2
-            self.log.debug("New number of bands : " + str(self.bandsCount))
-
-            # and joining along the second axis (axis=1), ie: bands-like
-            self.bands = np.concatenate((up, down), axis=1)
-
-        # otherwise just reshaping is needed
-        else:
-            self.bands.shape = (self.kpointsCount, self.bandsCount, 2)
-
-        # Making a test if the broadcast is rigth, otherwise just print
-        test = [x.max() - x.min() for x in self.bands[:, :, 0].transpose()]
-        if np.array(test).any():
-            self.log.warning(
-                "The indexes of bands do not match. CHECK IT. "
-                "Likely the data was wrongly broadcasted"
-            )
-            self.log.warning(str(self.bands[:, :, 0]))
-        # Now safely removing the band index
-        self.bands = self.bands[:, :, 1]
-        self.log.info("The bands shape is " + str(self.bands.shape))
-        return
-
-    def _readOrbital(self):
-        """Reads all the spd-projected data. A typical/expected block is:
-    ion      s     py     pz     px    dxy    dyz    dz2    dxz    dx2    tot
-      1  0.079  0.000  0.001  0.000  0.000  0.000  0.000  0.000  0.000  0.079
-      2  0.152  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.152
-      3  0.079  0.000  0.001  0.000  0.000  0.000  0.000  0.000  0.000  0.079
-      4  0.188  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.188
-      5  0.188  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.188
-    tot  0.686  0.000  0.002  0.000  0.000  0.000  0.000  0.000  0.000  0.688
-    (x2 for spin-polarized -akwardkly formatted-, x4 non-collinear -nicely
-    formatted-).
-
-    The data is stored in an array self.spd[kpoint][band][ispin][atom][orbital]
-
-    Undefined behavior in case of phase factors (LORBIT = 12).
-    """
-        self.log.debug("readOrbital")
-        if not self.fileStr:
-            log.warning("You should invoke `procar.readFile()` instead. Returning")
-            return
-
-        # finding all orbital headers
-        self.spd = re.findall(r"ion(.+)", self.fileStr)
-        self.log.info("the first orbital match reads: " + self.spd[0])
-        self.log.debug("And I found " + str(len(self.spd)) + " orbitals headers")
-
-        # testing if the orbital names are known (the standard ones)
-        FoundOrbs = self.spd[0].split()
-        size = len(FoundOrbs)
-        # only the first 'size' orbital
-        StdOrbs = self.orbitalName[: size - 1] + self.orbitalName[-1:]
-        StdOrbs_short = self.orbitalName_short[: size - 1] + self.orbitalName_short[-1:]
-        StdOrbs_old = self.orbitalName_old[: size - 1] + self.orbitalName_old[-1:]
-        if (
-            FoundOrbs != (StdOrbs)
-            and FoundOrbs != (StdOrbs_short)
-            and FoundOrbs != (StdOrbs_old)
-        ):
-            self.log.warning(
-                str(size) + " orbitals. (Some of) They are unknow (if "
-                "you did 'filter' them it is OK)."
-            )
-        self.orbitalCount = size
-        self.orbitalNames = self.spd[0].split()
-        self.log.debug(
-            "Anyway, I will use the following set of orbitals: "
-            + str(self.orbitalNames)
-        )
-
-        # Now reading the bulk of data
-        self.log.debug("Now searching the values")
-        # The case of just one atom is handled differently since the VASP
-        # output is a little different
-        if self.ionsCount == 1:
-            self.spd = re.findall(r"^(\s*1\s+.+)$", self.fileStr, re.MULTILINE)
-        else:
-            # Added by Francisco to speed up filtering on June 4th, 2019
-            # get rid of phase factors
-            self.spd = re.findall(r"ion.+tot\n([-.\d\seto]+)", self.fileStr)
-            self.spd = "".join(self.spd)
-            self.spd = re.findall(r"([-.\d\se]+tot.+)\n", self.spd)
-        # free the memory (could be a lot)
-        self.fileStr = None
-        self.log.debug("the first entry is \n" + self.spd[0])
-
-        # Now the method will try to find the value of self.ispin,
-        # previously it was set to either 1 or 2. If "1", it could be 1 or
-        # 4, but previously it was impossible to find the rigth value. If
-        # "2" it has to macth with the number of entries of spd data.
-
-        self.log.debug("Number of entries found: " + str(len(self.spd)))
-        expected = self.bandsCount * self.kpointsCount
-        self.log.debug(
-            "The number of entries for a non magnetic calc. is: " + str(expected)
-        )
-        if expected == len(self.spd):
-            self.log.info("Both numbers match, ok, going ahead")
-        # catching a non-collinear calc.
-        elif expected * 4 == len(self.spd):
-            self.log.info("non-collinear calculation found")
-            # testing if previous ispin value is ok
-            if self.ispin != 1:
-                self.log.warning(
-                    "Incompatible data: self.ispin= " + str(self.ispin) + ". Now is 4"
-                )
-            self.ispin = 4
-        else:
-            self.log.error("The parser or data is wrong!!!")
-            self.log.info("bandsCount: " + str(self.bandsCount))
-            self.log.info("KpointsCount: " + str(self.kpointsCount))
-            raise RuntimeError("Shit happens")
-
-        # checking for consistency
-        for line in self.spd:
-            if len(line.split()) != (self.ionsCount) * (self.orbitalCount + 1):
-                self.log.error(
-                    "Expected: "
-                    + str(self.ionsCount)
-                    + "*"
-                    + str(self.orbitalCount + 1)
-                    + " = "
-                    + str((self.ionsCount) * (self.orbitalCount + 1))
-                    + " Fields. Present block: "
-                    + str(len(line.split()))
-                )
-                raise RuntimeError("Flats happens")
-
-        # replacing the "tot" string by a number, to allows a conversion
-        # to numpy
-        self.spd = [x.replace("tot", "0") for x in self.spd]
-        self.spd = [x.split() for x in self.spd]
-        self.spd = np.array(self.spd, dtype=float)
-        self.log.debug("The spd (old) array shape is:" + str(self.spd.shape))
-
-        # handling collinear polarized case
-        if self.ispin == 2:
-            self.log.debug("Handling spin-polarized collinear case...")
-            # splitting both spin components, now they are along k-points
-            # axis (1st axis) but, then should be concatenated along the
-            # bands.
-            up, down = np.vsplit(self.spd, 2)
-            # ispin = 1 for a while, we will made the distinction
-            up.shape = (
-                self.kpointsCount,
-                int(self.bandsCount / 2),
-                1,
-                self.ionsCount,
-                self.orbitalCount + 1,
-            )
-            down.shape = (
-                self.kpointsCount,
-                int(self.bandsCount / 2),
-                1,
-                self.ionsCount,
-                self.orbitalCount + 1,
-            )
-            # concatenating bandwise. Density and magntization, their
-            # meaning is obvious, and do uses 2 times more memory than
-            # required, but I *WANT* to keep it as close as possible to the
-            # non-collinear or non-polarized case
-            density = np.concatenate((up, down), axis=1)
-            magnet = np.concatenate((up, -down), axis=1)
-            # concatenated along 'ispin axis'
-            self.spd = np.concatenate((density, magnet), axis=2)
-            self.log.debug("polarized collinear spd.shape= " + str(self.spd.shape))
-
-        # otherwise, just a reshaping suffices
-        else:
-            self.spd.shape = (
-                self.kpointsCount,
-                self.bandsCount,
-                self.ispin,
-                self.ionsCount,
-                self.orbitalCount + 1,
-            )
-
-        self.log.info("spd array ready. Its shape is:" + str(self.spd.shape))
-        return
-
-    def readFile(self, procar=None, phase=False, permissive=False, recLattice=None):
-        """Reads and parses the whole PROCAR file. This method is a sort
-    of metamethod: it opens the file, reads the meta data and call the
-    respective functions for parsing kpoints, bands, and projected
-    data.
-
-    Args:
-
-    -procar: The file name, if `None` or a directory, a suitable set
-     of defaults will be used. Default=None
-
-    -permissive: turn on (or off) some features to deal with badly
-     written PROCAR files (stupid fortran), up to now just ignores the
-     kpoints coordinates, which -as side effect- prevent he rigth
-     space between kpoints. Default=False (off)
-
-
-    -recLattice: a 3x3 array containing the reciprocal vectors, to
-     change the Kpoints from rec. coordinates to cartesians. Rarely
-     given by hand, see `UtilsProcar.RecLatProcar`. If given, the
-     kpoints will be converted from direct coordinates to cartesian
-     ones. Default=None
-
-    """
-        self.log.debug("readFile...")
-
-        self.recLattice = recLattice
-
-        self.log.debug("Opening file: '" + str(procar) + "'")
-        f = self.utils.OpenFile(procar)
-        # Line 1: PROCAR lm decomposed
-        f.readline()  # throwaway
-        # Line 2: # of k-points:  816   # of bands:  52   # of ions:   8
-        metaLine = f.readline()  # metadata
-        self.log.debug("The metadata line is: " + metaLine)
-        re.findall(r"#[^:]+:([^#]+)", metaLine)
-        self.kpointsCount, self.bandsCount, self.ionsCount = map(
-            int, re.findall(r"#[^:]+:([^#]+)", metaLine)
-        )
-        self.log.info("kpointsCount = " + str(self.kpointsCount))
-        self.log.info("bandsCount = " + str(self.bandsCount))
-        self.log.info("ionsCount = " + str(self.ionsCount))
-        if self.ionsCount == 1:
-            self.log.warning(
-                "Special case: only one atom found. The program may not work as expected"
-            )
-        else:
-            self.log.debug("An extra ion representing the  total value will be added")
-            self.ionsCount = self.ionsCount + 1
-
-        # reading all the rest of the file to be parsed below
-        self.fileStr = f.read()
-        self._readKpoints(permissive)
-        self._readBands()
-        self._readOrbital()
-        self.log.debug("readfile...done")
-        return
-
-    # Slower way to parse the phase included PROCAR. He Xu implemented a faster way. See readFile2()
-    # if phase == False:
-    #     self.log.debug("readFile...")
-
-    #     self.recLattice = recLattice
-
-    #     self.log.debug("Opening file: '" + str(procar) + "'")
-    #     f = self.utils.OpenFile(procar)
-    #     # Line 1: PROCAR lm decomposed
-    #     f.readline()  # throwaway
-    #     # Line 2: # of k-points:  816   # of bands:  52   # of ions:   8
-    #     metaLine = f.readline()  # metadata
-    #     self.log.debug("The metadata line is: " + metaLine)
-    #     re.findall(r"#[^:]+:([^#]+)", metaLine)
-    #     self.kpointsCount, self.bandsCount, self.ionsCount = \
-    #         list(map(int, re.findall(r"#[^:]+:([^#]+)", metaLine)))
-    #     self.log.info("kpointsCount = " + str(self.kpointsCount))
-    #     self.log.info("bandsCount = " + str(self.bandsCount))
-    #     self.log.info("ionsCount = " + str(self.ionsCount))
-    #     if self.ionsCount is 1:
-    #         self.log.warning(
-    #             "Special case: only one atom found. The program may not work as expected"
-    #         )
-    #     else:
-    #         self.log.debug(
-    #             "An extra ion representing the  total value will be added")
-    #         self.ionsCount = self.ionsCount + 1
-
-    #     #reading all the rest of the file to be parsed below
-    #     self.fileStr = f.read()
-    #     self._readKpoints(permissive)
-    #     self._readBands()
-    #     self._readOrbital()
-    #     self.log.debug("readfile...done")
-
-    # elif phase == True:  #for LORBIT=12
-    #     self.recLattice = recLattice
-    #     f = self.utils.OpenFile(procar)
-    #     f.readline()  #throw away first line
-    #     metaLine = f.readline()  # header
-
-    #     #parsing header information
-    #     self.kpointsCount, self.bandsCount, self.ionsCount = list(
-    #         map(int, re.findall(r"#[^:]+:([^#]+)", metaLine)))
-
-    #     if self.ionsCount is 1:
-    #         self.log.warning(
-    #             "Special case: only one atom found. The program may not work as expected"
-    #         )
-    #     else:
-    #         self.log.debug(
-    #             "An extra ion representing the  total value will be added")
-    #         self.ionsCount = self.ionsCount + 1
-
-    #     #reading all the rest of the file to be parsed below saved as spd
-    #     self.fileStr = f.read()
-    #     self._readKpoints(permissive)
-    #     self._readBands()
-    #     self._readOrbital()
-    #     self.log.debug("readfile...done")
-
-    #     #reading the complex phase data. will be saved as cspd
-    #     f2 = self.utils.OpenFile(procar)
-    #     f2.readline()  #throw away first line
-    #     f2.readline()  #throw away header line
-    #     data2 = f2.read()
-
-    #     #parsing
-    #     spd0 = re.findall(r"ion(.+)", data2)  #headers of the blocks
-    #     FoundOrbs = spd0[1].split()
-    #     size = len(FoundOrbs)
-    #     corbitalCount = size
-    #     spd_phase = re.findall(
-    #         r"(?<=dx2-y2)([charge0-9.\s-]*)(?=band|k-point|\Z)",
-    #         data2)  #for LORBIT=12
-
-    #     spd_new = []
-    #     for i in range(len(spd_phase)):
-    #         #get last list of original block and replace spd last line and append all to get new spd.
-    #         # for charge line use spd instead of spd_real
-    #         spd_last = spd_phase[i].split()[-(corbitalCount + 2):]
-    #         result = []
-    #         for counter, value in enumerate(spd_last):
-    #             result.append(value)
-    #             result.append('0')
-    #         del result[1]
-    #         del result[-1]
-
-    #         #replace last line of each spd block
-    #         spd_block = spd_phase[i].split()
-    #         spd_block[-(corbitalCount + 2):] = result
-    #         spd_block = [x.replace('charge', '0') for x in spd_block]
-    #         spd_new.append(spd_block)
-
-    #     # conversion to numpy
-    #     spd_phase = np.array(spd_new, dtype=float)
-
-    #     #reshaping
-    #     spd_phase.shape = (self.kpointsCount, self.bandsCount, 1,
-    #                        self.ionsCount, 2 * corbitalCount + 2)
-
-    #     #matrix to hold complex values
-    #     self.cspd = np.zeros([
-    #         self.kpointsCount, self.bandsCount, 1, self.ionsCount,
-    #         corbitalCount + 2
-    #     ],
-    #                          dtype='complex')
-
-    #     for ikpointsCount in range(self.kpointsCount):
-    #         for ibandsCount in range(self.bandsCount):
-    #             for iionsCount in range(self.ionsCount):
-    #                 orbs_real = spd_phase[ikpointsCount][ibandsCount][0][
-    #                     iionsCount][1:-1:2]
-    #                 orbs_imag = spd_phase[ikpointsCount][ibandsCount][0][
-    #                     iionsCount][2::2]
-    #                 orbs_all = orbs_real + (1j * orbs_imag)
-    #                 self.cspd[ikpointsCount, ibandsCount, 0,
-    #                           iionsCount, :] = np.concatenate(
-    #                               [[
-    #                                   spd_phase[ikpointsCount][ibandsCount]
-    #                                   [0][iionsCount][0]
-    #                               ], orbs_all,
-    #                                [
-    #                                    spd_phase[ikpointsCount]
-    #                                    [ibandsCount][0][iionsCount][-1]
-    #                                ]])
-
-    # return
-
-    def readFile2(
-        self,
-        procar=None,
-        phase=False,
-        permissive=False,
-        recciprocal_lattice=None,
-        ispin=None,  # the only spin channle to read
-    ):
-        """
-        Read file in a line by line manner.
-        Only used when the phase factor is in procar. (for vasp, lorbit=12)
-        """
-        # Fall back to readFile function if no phase
-        self.bands = None
-        
-        if ispin is None:
-            nspin = 1
-        else:
-            nspin = 2
-        iispin = 0
-        self.projections = None
-        ikpt = 0
-        iband = 0
-        nkread = 0
-        # with open(self.fname) as myfile:
-        f = self.utils.OpenFile(procar)
-        lines = iter(f.readlines())
-        last_iband = -1
-        for line in lines:
-            if line.startswith("# of k-points"):
-                a = re.findall(":\s*([0-9]*)", line)
-                self.kpointsCount, self.bandsCount, self.ionsCount = map(int, a)
-                self.kpoints = np.zeros([self.kpointsCount, 3])
-                self.kweights = np.zeros(self.kpointsCount)
-                if self.bands is None:
-                    self.bands = np.zeros(
-                        [nspin, self.kpointsCount, self.bandsCount]
-                    )
-            if line.strip().startswith("k-point"):
-                ss = line.strip().split()
-                ikpt = int(ss[1]) - 1
-                k0 = float(ss[3])
-                k1 = float(ss[4])
-                k2 = float(ss[5])
-                w = float(ss[-1])
-                self.kpoints[ikpt, :] = [k0, k1, k2]
-                self.kweights[ikpt] = w
-                nkread += 1
-                if nkread <= self.kpointsCount:
-                    iispin = 0
-                else:
-                    iispin = 1
-            if line.strip().startswith("band"):
-                ss = line.strip().split()
-                try:
-                    iband = int(ss[1]) - 1
-                except ValueError:
-                    iband = last_iband + 1
-                last_iband = iband
-                e = float(ss[4])
-                occ = float(ss[-1])
-                self.bands[iispin, ikpt, iband] = e
-            if line.strip().startswith("ion"):
-                if line.strip().endswith("tot"):
-                    self.orbitalName = line.strip().split()[1:-1]
-                    self.orbitalCount = len(self.orbitalName)
-                if self.projections is None:
-                    self.projections = np.zeros(
-                        [
-                            self.kpointsCount,
-                            self.bandsCount,
-                            self.ionsCount,
-                            self.orbitalCount,
-                        ]
-                    )
-                    self.carray = np.zeros(
-                        [
-                            self.kpointsCount,
-                            self.bandsCount,
-                            nspin,
-                            self.ionsCount,
-                            self.orbitalCount,
-                        ],
-                        dtype="complex",
-                    )
-                for i in range(self.ionsCount):
-                    line = next(lines)
-                    t = line.strip().split()
-                    if len(t) == self.orbitalCount + 2:
-                        self.projections[ikpt, iband, iispin, :] = [
-                            float(x) for x in t[1:-1]
-                        ]
-                    elif len(t) == self.orbitalCount * 2 + 2:
-                        self.carray[ikpt, iband, iispin, i, :] += np.array(
-                            [float(x) for x in t[1:-1:2]]
-                        )
-                        self.carray[ikpt, iband, iispin, i, :] += 1j * np.array(
-                            [float(x) for x in t[2::2]]
-                        )
-
-                    # Added by Francisco to parse older version of PROCAR format on Jun 11, 2019
-                    elif len(t) == self.orbitalCount * 1 + 1:
-                        self.carray[ikpt, iband, iispin, i, :] += np.array(
-                            [float(x) for x in t[1:]]
-                        )
-                        line = next(lines)
-                        t = line.strip().split()
-                        self.carray[ikpt, iband, iispin, i, :] += 1j * np.array(
-                            [float(x) for x in t[1:]]
-                        )
-                    else:
-                        raise Exception(
-                            "Cannot parse line to projection: %s" % line
-                        )
+import numpy as np
+import re
+import logging
+import matplotlib.pyplot as plt
+import sys
+from ...utils import UtilsProcar
+
+
+class ProcarParser:
+    """Parses a PROCAR file and store it in memory. It only deals with
+  PROCAR files, that means no Fermi energy (UtilsProcar.FermiOutcar
+  can help), and the reciprocal vectors should be supplied (if used,
+  see UtilsProcar class).
+  
+  Members:
+
+    __init__(self, loglevel): The setup the variables internally, `loglevel` 
+      sets the verbosity level ie: `loglevel=logging.DEBUG` for debugging. Its
+      default is `logging.WARNING` 
+
+    readFile(self, procar=None, permissive=False, recLattice=None):
+      The only method of the API it load the file completely.
+
+      Arguments:
+      `procar=None`: name of the PROCAR file, can be a gzipped file (the 
+                    extension is no required). The default covers a wide range 
+                    of obvious alternatives. 
+      `permissive=False`: Set to `True` if the PROCAR file has problems reading
+                          the Kpoints (stupid Fortran), but in that case the 
+                          Kpoints mesh will be discarded. Future updates could 
+                          allow it to handle other formating/corruption issues. 
+      `recLattice`=None: Reciprical Vectors, you want to provide them since not
+                         all the paths on the BZ are the same.
+
+    Don't use the other methods beggining with underscores "_"
+
+  Example:
+  To read a PROCAR or PROCAR.gz file:
+  >>> foo = ProcarParser()
+  >>> foo.readFile()
+
+  To include the reciprocal vectors, and file name MyFirstPROCAR
+  >>> outcarparser = UtilsProcar()
+  >>> recLat = outcarparser.RecLatOutcar(args.outcar)
+  >>> foo = ProcarParser()
+  >>> foo.readFile("MyFirstPROCAR", recLat=recLat)
+ 
+  """
+
+    def __init__(self, loglevel=logging.WARNING):
+        # array with k-points, they have the following values
+        # -None: if not parsed (yet) or parsed with a `permissive` flag on
+        # -direct coordinates: if a recLattice was not supplied to the parser
+        # -cartesian coords: if a recLattice was supplied to the parser.
+        # In the later cases, self.kpoints.shape=(self.kpointsCount, 3)
+        self.kpoints = None
+        # Number of kpoints, as given by the KPOINTS header (PROCAR file)
+        self.kpointsCount = None
+
+        # bands headers present in PROCAR file.
+        # self.bands.shape=(self.kpointsCount,self.bandsCount)
+        self.bands = None
+        # Number of bands. For a spin polarized calculation the number of
+        # bands is double (spin ip + spin down). On this array there is no
+        # distinction between spin up and down
+        self.bandsCount = None
+
+        # Number of ions+1 the +1 is the 'tot' field, ie: the sum over all atoms
+        self.ionsCount = None
+
+        self.fileStr = None  # the actual file, stored in memory
+        self.spd = None  # the atom/orbital projected data
+        self.cspd = None  # spd data with the phase
+        self.orbitalName = [
+            "s",
+            "py",
+            "pz",
+            "px",
+            "dxy",
+            "dyz",
+            "dz2",
+            "dxz",
+            "dx2",
+            "tot",
+        ]
+        self.orbitalCount = None  # number of orbitals
+
+        # number of spin components (blocks of data), 1: non-magnetic non
+        # polarized, 2: spin polarized collinear, 4: non-collinear
+        # spin.
+        # NOTE: before calling to `self._readOrbital` the case '4'
+        # is marked as '1'
+        self.ispin = None
+        self.recLattice = None  # reciprocal lattice vectors
+        self.utils = UtilsProcar()
+
+        self.log = logging.getLogger("ProcarParser")
+        self.log.setLevel(loglevel)
+        self.ch = logging.StreamHandler()
+        self.ch.setFormatter(
+            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
+        )
+        self.ch.setLevel(logging.DEBUG)
+        self.log.addHandler(self.ch)
+        # At last, one message to the logger.
+        self.log.debug("Procar instanciated")
+        return
+
+    def _readKpoints(self, permissive=False):
+        """Reads the k-point headers. A typical k-point line is:
+    k-point    1 :    0.00000000 0.00000000 0.00000000  weight = 0.00003704\n
+
+    fills self.kpoint[kpointsCount][3]
+    
+    The weights are discarded (are they useful?)
+    """
+        self.log.debug("readKpoints")
+        if not self.fileStr:
+            log.warning("You should invoke `procar.readFile()` instead. Returning")
+            return
+
+        # finding all the K-points headers
+        self.kpoints = re.findall(r"k-point\s+\d+\s*:\s+([-.\d\s]+)", self.fileStr)
+        self.log.debug(str(len(self.kpoints)) + " K-point headers found")
+        self.log.debug("The first match found is: " + str(self.kpoints[0]))
+
+        # trying to build an array
+        self.kpoints = [x.split() for x in self.kpoints]
+        try:
+            self.kpoints = np.array(self.kpoints, dtype=float)
+        except ValueError:
+            self.log.error("Ill-formatted data:")
+            print("\n".join([str(x) for x in self.kpoints]))
+            if permissive is True:
+                # Discarding the kpoints list, however I need to set
+                # self.ispin beforehand.
+                if len(self.kpoints) == self.kpointsCount:
+                    self.ispin = 1
+                elif len(self.kpoints) == 2 * self.kpointsCount:
+                    self.ispin = 2
+                else:
+                    raise ValueError("Kpoints do not match with ispin=1 or 2.")
+                self.kpoints = None
+                self.log.warning("K-points list is useless, setting it to `None`")
+                return
+            else:
+                raise ValueError("Badly formated Kpoints headers, try `--permissive`")
+        # if successful, go on
+
+        # trying to identify an non-polarized or non-collinear case, a
+        # polarized case or a defective file
+
+        if len(self.kpoints) != self.kpointsCount:
+            # if they do not match, may means two things a spin polarized
+            # case or a bad file, lets check
+            self.log.debug(
+                "Number of kpoints do not match, looking for a " "spin-polarized case"
+            )
+            # lets start testing if it is spin polarized, if so, there
+            # should be 2 identical blocks of kpoints.
+            up, down = np.vsplit(self.kpoints, 2)
+            if (up == down).all():
+                self.log.info("Spin-polarized calculation found")
+                self.ispin = 2
+                # just keeping one set of kpoints (the other will be
+                # discarded)
+                self.kpoints = up
+            else:
+                self.log.error("Number of K-points do not match! check them.")
+                raise RuntimeError("Bad Kpoints list.")
+        # if ISPIN != 2 setting ISPIN=1 (later for the non-collinear case 1->4)
+        # It is unknown until parsing the projected data
+        else:
+            self.ispin = 1
+
+        # checking again, for compatibility,
+        if len(self.kpoints) != self.kpointsCount:
+            raise RuntimeError(
+                "Kpoints number do not match with metadata (header of PROCAR)"
+            )
+
+        self.log.debug(str(self.kpoints))
+        self.log.info("The kpoints shape is " + str(self.kpoints.shape))
+
+        if self.recLattice is not None:
+            self.log.info("Changing to cartesians coordinates")
+            self.kpoints = np.dot(self.kpoints, self.recLattice)
+            self.log.debug("New kpoints: \n" + str(self.kpoints))
+        return
+
+    def _readBands(self):
+        """Reads the bands header. A typical bands is:
+    band   1 # energy   -7.11986315 # occ.  1.00000000
+    
+    fills self.bands[kpointsCount][bandsCount] 
+    
+    The occupation numbers are discarded (are they useful?)"""
+        self.log.debug("readBands")
+        if not self.fileStr:
+            log.warning("You should invoke `procar.read()` instead. Returning")
+            return
+
+        # finding all bands
+        self.bands = re.findall(
+            r"band\s*(\d+)\s*#\s*energy\s*([-.\d\s]+)", self.fileStr
+        )
+        self.log.debug(
+            str(len(self.bands))
+            + " bands headers found, bands*Kpoints = "
+            + str(self.bandsCount * self.kpointsCount)
+        )
+        self.log.debug("The first match found is: " + str(self.bands[0]))
+
+        # checking if the number of bands match
+
+        if len(self.bands) != self.bandsCount * self.kpointsCount * self.ispin:
+            self.log.error("Number of bands headers do not match")
+            raise RuntimeError("Number of bands don't match")
+
+        # casting to array to manipulate the bands
+        self.bands = np.array(self.bands, dtype=float)
+        self.log.debug(str(self.bands))
+
+        # Now I will deal with the spin polarized case. The goal is join
+        # them like for a non-magnetic case
+        if self.ispin == 2:
+            # up and down are along the first axis
+            up, down = np.vsplit(self.bands, 2)
+            self.log.debug("up   , " + str(up.shape))
+            self.log.debug("down , " + str(down.shape))
+
+            # reshapping (the 2  means both band index and energy)
+            up.shape = (self.kpointsCount, self.bandsCount, 2)
+            down.shape = (self.kpointsCount, self.bandsCount, 2)
+
+            # setting the correct number of bands (up+down)
+            self.bandsCount *= 2
+            self.log.debug("New number of bands : " + str(self.bandsCount))
+
+            # and joining along the second axis (axis=1), ie: bands-like
+            self.bands = np.concatenate((up, down), axis=1)
+
+        # otherwise just reshaping is needed
+        else:
+            self.bands.shape = (self.kpointsCount, self.bandsCount, 2)
+
+        # Making a test if the broadcast is rigth, otherwise just print
+        test = [x.max() - x.min() for x in self.bands[:, :, 0].transpose()]
+        if np.array(test).any():
+            self.log.warning(
+                "The indexes of bands do not match. CHECK IT. "
+                "Likely the data was wrongly broadcasted"
+            )
+            self.log.warning(str(self.bands[:, :, 0]))
+        # Now safely removing the band index
+        self.bands = self.bands[:, :, 1]
+        self.log.info("The bands shape is " + str(self.bands.shape))
+        return
+
+    def _readOrbital(self):
+        """Reads all the spd-projected data. A typical/expected block is:
+    ion      s     py     pz     px    dxy    dyz    dz2    dxz    dx2    tot
+      1  0.079  0.000  0.001  0.000  0.000  0.000  0.000  0.000  0.000  0.079
+      2  0.152  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.152
+      3  0.079  0.000  0.001  0.000  0.000  0.000  0.000  0.000  0.000  0.079
+      4  0.188  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.188
+      5  0.188  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.000  0.188
+    tot  0.686  0.000  0.002  0.000  0.000  0.000  0.000  0.000  0.000  0.688
+    (x2 for spin-polarized -akwardkly formatted-, x4 non-collinear -nicely 
+    formatted-).
+
+    The data is stored in an array self.spd[kpoint][band][ispin][atom][orbital]
+
+    Undefined behavior in case of phase factors (LORBIT = 12). 
+    """
+        self.log.debug("readOrbital")
+        if not self.fileStr:
+            log.warning("You should invoke `procar.readFile()` instead. Returning")
+            return
+
+        # finding all orbital headers
+        self.spd = re.findall(r"ion(.+)", self.fileStr)
+        self.log.info("the first orbital match reads: " + self.spd[0])
+        self.log.debug("And I found " + str(len(self.spd)) + " orbitals headers")
+
+        # testing if the orbital names are known (the standard ones)
+        FoundOrbs = self.spd[0].split()
+        size = len(FoundOrbs)
+        # only the first 'size' orbital
+        StdOrbs = self.orbitalName[: size - 1] + self.orbitalName[-1:]
+        if FoundOrbs != (StdOrbs):
+            self.log.warning(
+                str(size) + " orbitals. (Some of) They are unknow (if "
+                "you did 'filter' them it is OK)."
+            )
+        self.orbitalCount = size
+        self.orbitalNames = self.spd[0].split()
+        self.log.debug(
+            "Anyway, I will use the following set of orbitals: "
+            + str(self.orbitalNames)
+        )
+
+        # Now reading the bulk of data
+        self.log.debug("Now searching the values")
+        # The case of just one atom is handled differently since the VASP
+        # output is a little different
+        if self.ionsCount is 1:
+            self.spd = re.findall(r"^(\s*1\s+.+)$", self.fileStr, re.MULTILINE)
+        else:
+            self.spd = re.findall(r"([-.\d\se]+tot.+)\n", self.fileStr)
+        # free the memory (could be a lot)
+        self.fileStr = None
+        self.log.debug("the first entry is \n" + self.spd[0])
+
+        # Now the method will try to find the value of self.ispin,
+        # previously it was set to either 1 or 2. If "1", it could be 1 or
+        # 4, but previously it was impossible to find the rigth value. If
+        # "2" it has to macth with the number of entries of spd data.
+
+        self.log.debug("Number of entries found: " + str(len(self.spd)))
+        expected = self.bandsCount * self.kpointsCount
+        self.log.debug(
+            "The number of entries for a non magnetic calc. is: " + str(expected)
+        )
+        if expected == len(self.spd):
+            self.log.info("Both numbers match, ok, going ahead")
+        # catching a non-collinear calc.
+        elif expected * 4 == len(self.spd):
+            self.log.info("non-collinear calculation found")
+            # testing if previous ispin value is ok
+            if self.ispin != 1:
+                self.log.warning(
+                    "Incompatible data: self.ispin= " + str(self.ispin) + ". Now is 4"
+                )
+            self.ispin = 4
+        else:
+            self.log.error("The parser or data is wrong!!!")
+            self.log.info("bandsCount: " + str(self.bandsCount))
+            self.log.info("KpointsCount: " + str(self.kpointsCount))
+            raise RuntimeError("Shit happens")
+
+        # checking for consistency
+        for line in self.spd:
+            if len(line.split()) != (self.ionsCount) * (self.orbitalCount + 1):
+                self.log.error(
+                    "Expected: "
+                    + str(self.ionsCount)
+                    + "*"
+                    + str(self.orbitalCount + 1)
+                    + " = "
+                    + str((self.ionsCount) * (self.orbitalCount + 1))
+                    + " Fields. Present block: "
+                    + str(len(line.split()))
+                )
+                print(line)
+                raise RuntimeError("Flats happens")
+
+        # replacing the "tot" string by a number, to allows a conversion
+        # to numpy
+        self.spd = [x.replace("tot", "0") for x in self.spd]
+        self.spd = [x.split() for x in self.spd]
+        self.spd = np.array(self.spd, dtype=float)
+        self.log.debug("The spd (old) array shape is:" + str(self.spd.shape))
+
+        # handling collinear polarized case
+        if self.ispin == 2:
+            self.log.debug("Handling spin-polarized collinear case...")
+            # splitting both spin components, now they are along k-points
+            # axis (1st axis) but, then should be concatenated along the
+            # bands.
+            up, down = np.vsplit(self.spd, 2)
+            # ispin = 1 for a while, we will made the distinction
+            up.shape = (
+                self.kpointsCount,
+                int(self.bandsCount / 2),
+                1,
+                self.ionsCount,
+                self.orbitalCount + 1,
+            )
+            down.shape = (
+                self.kpointsCount,
+                int(self.bandsCount / 2),
+                1,
+                self.ionsCount,
+                self.orbitalCount + 1,
+            )
+            # concatenating bandwise. Density and magntization, their
+            # meaning is obvious, and do uses 2 times more memory than
+            # required, but I *WANT* to keep it as close as possible to the
+            # non-collinear or non-polarized case
+            density = np.concatenate((up, down), axis=1)
+            magnet = np.concatenate((up, -down), axis=1)
+            # concatenated along 'ispin axis'
+            self.spd = np.concatenate((density, magnet), axis=2)
+            self.log.debug("polarized collinear spd.shape= " + str(self.spd.shape))
+
+        # otherwise, just a reshaping suffices
+        else:
+            self.spd.shape = (
+                self.kpointsCount,
+                self.bandsCount,
+                self.ispin,
+                self.ionsCount,
+                self.orbitalCount + 1,
+            )
+
+        self.log.info("spd array ready. Its shape is:" + str(self.spd.shape))
+        return
+
+    def readFile(self, procar=None, phase=False, permissive=False, recLattice=None):
+        """Reads and parses the whole PROCAR file. This method is a sort
+    of metamethod: it opens the file, reads the meta data and call the
+    respective functions for parsing kpoints, bands, and projected
+    data.
+
+    Args:
+
+    -procar: The file name, if `None` or a directory, a suitable set
+     of defaults will be used. Default=None
+    
+    -permissive: turn on (or off) some features to deal with badly
+     written PROCAR files (stupid fortran), up to now just ignores the
+     kpoints coordinates, which -as side effect- prevent he rigth
+     space between kpoints. Default=False (off)
+
+
+    -recLattice: a 3x3 array containing the reciprocal vectors, to
+     change the Kpoints from rec. coordinates to cartesians. Rarely
+     given by hand, see `UtilsProcar.RecLatProcar`. If given, the
+     kpoints will be converted from direct coordinates to cartesian
+     ones. Default=None
+
+    """
+
+        if phase == False:
+            self.log.debug("readFile...")
+
+            self.recLattice = recLattice
+
+            self.log.debug("Opening file: '" + str(procar) + "'")
+            f = self.utils.OpenFile(procar)
+            # Line 1: PROCAR lm decomposed
+            f.readline()  # throwaway
+            # Line 2: # of k-points:  816   # of bands:  52   # of ions:   8
+            metaLine = f.readline()  # metadata
+            self.log.debug("The metadata line is: " + metaLine)
+            re.findall(r"#[^:]+:([^#]+)", metaLine)
+            self.kpointsCount, self.bandsCount, self.ionsCount = list(
+                map(int, re.findall(r"#[^:]+:([^#]+)", metaLine))
+            )
+            self.log.info("kpointsCount = " + str(self.kpointsCount))
+            self.log.info("bandsCount = " + str(self.bandsCount))
+            self.log.info("ionsCount = " + str(self.ionsCount))
+            if self.ionsCount is 1:
+                self.log.warning(
+                    "Special case: only one atom found. The program may not work as expected"
+                )
+            else:
+                self.log.debug(
+                    "An extra ion representing the  total value will be added"
+                )
+                self.ionsCount = self.ionsCount + 1
+
+            # reading all the rest of the file to be parsed below
+            self.fileStr = f.read()
+            self._readKpoints(permissive)
+            self._readBands()
+            self._readOrbital()
+            self.log.debug("readfile...done")
+
+        elif phase == True:  # for LORBIT=12
+            self.recLattice = recLattice
+            f = self.utils.OpenFile(procar)
+            f.readline()  # throw away first line
+            metaLine = f.readline()  # header
+
+            # parsing header information
+            self.kpointsCount, self.bandsCount, self.ionsCount = list(
+                map(int, re.findall(r"#[^:]+:([^#]+)", metaLine))
+            )
+
+            if self.ionsCount is 1:
+                self.log.warning(
+                    "Special case: only one atom found. The program may not work as expected"
+                )
+            else:
+                self.log.debug(
+                    "An extra ion representing the  total value will be added"
+                )
+                self.ionsCount = self.ionsCount + 1
+
+            # reading all the rest of the file to be parsed below saved as spd
+            self.fileStr = f.read()
+            self._readKpoints(permissive)
+            self._readBands()
+            self._readOrbital()
+            self.log.debug("readfile...done")
+
+            # reading the complex phase data. will be saved as cspd
+            f2 = self.utils.OpenFile(procar)
+            f2.readline()  # throw away first line
+            f2.readline()  # throw away header line
+            data2 = f2.read()
+
+            # parsing
+            spd0 = re.findall(r"ion(.+)", data2)  # headers of the blocks
+            FoundOrbs = spd0[1].split()
+            size = len(FoundOrbs)
+            corbitalCount = size
+            spd_phase = re.findall(
+                r"(?<=dx2-y2)([charge0-9.\s-]*)(?=band|k-point|\Z)", data2
+            )  # for LORBIT=12
+
+            spd_new = []
+            for i in range(len(spd_phase)):
+                # get last list of original block and replace spd last line and append all to get new spd.
+                # for charge line use spd instead of spd_real
+                spd_last = spd_phase[i].split()[-(corbitalCount + 2) :]
+                result = []
+                for counter, value in enumerate(spd_last):
+                    result.append(value)
+                    result.append("0")
+                del result[1]
+                del result[-1]
+
+                # replace last line of each spd block
+                spd_block = spd_phase[i].split()
+                spd_block[-(corbitalCount + 2) :] = result
+                spd_block = [x.replace("charge", "0") for x in spd_block]
+                spd_new.append(spd_block)
+
+            # conversion to numpy
+            spd_phase = np.array(spd_new, dtype=float)
+
+            # reshaping
+            spd_phase.shape = (
+                self.kpointsCount,
+                self.bandsCount,
+                1,
+                self.ionsCount,
+                2 * corbitalCount + 2,
+            )
+
+            # matrix to hold complex values
+            self.cspd = np.zeros(
+                [
+                    self.kpointsCount,
+                    self.bandsCount,
+                    1,
+                    self.ionsCount,
+                    corbitalCount + 2,
+                ],
+                dtype="complex",
+            )
+
+            for ikpointsCount in range(self.kpointsCount):
+                for ibandsCount in range(self.bandsCount):
+                    for iionsCount in range(self.ionsCount):
+                        orbs_real = spd_phase[ikpointsCount][ibandsCount][0][
+                            iionsCount
+                        ][1:-1:2]
+                        orbs_imag = spd_phase[ikpointsCount][ibandsCount][0][
+                            iionsCount
+                        ][2::2]
+                        orbs_all = orbs_real + (1j * orbs_imag)
+                        self.cspd[
+                            ikpointsCount, ibandsCount, 0, iionsCount, :
+                        ] = np.concatenate(
+                            [
+                                [
+                                    spd_phase[ikpointsCount][ibandsCount][0][
+                                        iionsCount
+                                    ][0]
+                                ],
+                                orbs_all,
+                                [
+                                    spd_phase[ikpointsCount][ibandsCount][0][
+                                        iionsCount
+                                    ][-1]
+                                ],
+                            ]
+                        )
+
+        return
```

### Comparing `PyProcar-5.6.6/pyprocar/procarselect/procarselect.py` & `PyProcar-6.0.0/pyprocar/core/procarselect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-import logging
-import re
-import sys
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from ..utilsprocar import UtilsProcar
-
-
-class ProcarSelect:
-    """
-  Reduces the dimensionality of the data making it uselful to
-  plot bands.
-
-  The main data to manipulate is the projected electronic structure.
-  Its shape original is:
-
-  spd[kpoint][band][ispin][atom][orbital].
-
-  The selection of components should be done in order, says, first
-  "ispin", then "atom", and at last "orbital".
-
-  Note: once any selection has been performed, the data itself
-  changes. Say, if you want compare atom [0] and [1,2], you need two
-  instances of this class.
-
-
-  Example to compare the bandstructure of two set of atoms
-  >>>
-
-  """
-
-    def __init__(
-        self, ProcarData=None, deepCopy=True, loglevel=logging.WARNING, mode=None
-    ):
-
-        self.spd = None
-        self.bands = None
-        self.kpoints = None
-        # self.cspd=None
-        self.mode = mode
-
-        # We want a logging to tell us what is happening
-        self.log = logging.getLogger("ProcarSelect")
-        self.log.setLevel(loglevel)
-        self.ch = logging.StreamHandler()
-        self.ch.setFormatter(
-            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
-        )
-        self.ch.setLevel(logging.DEBUG)
-        self.log.addHandler(self.ch)
-        # At last, one message to the logger.
-        self.log.debug("ProcarSelect: instanciated")
-
-        if ProcarData is not None:
-            self.setData(ProcarData, deepCopy)
-        return
-
-    def setData(self, ProcarData, deepCopy=True):
-        """
-    The data from ProcarData is deepCopy-ed by default (ie: their
-    elements are not modified by this class.
-
-    Args:
-
-    -ProcarData: is a ProcarParser instance (or anything with similar
-     functionality, duck typing)
-
-    -deepCopy=True: If false a shallow copy will be made (saves memory).
-    """
-        self.log.debug("setData: ...")
-        if deepCopy is True:
-            self.spd = ProcarData.spd.copy()
-            self.bands = ProcarData.bands.copy()
-            self.kpoints = ProcarData.kpoints.copy()
-            # self.cspd = ProcarData.cspd.copy()
-        else:
-            self.spd = ProcarData.spd
-            self.bands = ProcarData.bands
-            self.kpoints = ProcarData.kpoints
-            # self.cspd = ProcarData.cspd
-
-        self.numspin = self.spd.shape[2]  # Number of spins
-        self.log.debug("setData: ... Done")
-        print(
-            "spd shape      :  %s [kpoints, bands, spins, atoms+1, orbitals+2]"
-            % str(self.spd.shape)
-        )
-
-        return
-
-    def selectIspin(self, value=None, separate=False):
-        """
-    value is a list with the values of Ispin to select.
-
-    UPDATE:
-        if separate == true, then spin = 0 corresponds to spin up
-        and spin = 1 corresponds to spin down. If not, they give
-        spin density and spin magnetization, respectively.
-
-    Example:
-    >>> foo = ProcarParser()
-    >>> foo.readFile("PROCAR")
-    >>> bar = ProcarSelect(foo)
-    >>> bar.selectIspin([0]) #just the density
-    """
-        # all kpoint, all bands, VALUE spin, all the rest
-        self.log.debug("selectIspin: ...")
-        self.log.debug("old spd shape =" + str(self.spd.shape))
-        # first, testing if the domensionaluty is rigth:
-        dimen = len(self.spd.shape)
-        if dimen != 5:
-            self.log.error(
-                "The array is " + str(dimen) + " dimensional, expecting a"
-                " 5 dimensional array."
-            )
-            self.log.error(
-                "You should call selectIspin->selecAtom->selectOrbitals, "
-                "in this order."
-            )
-            raise RuntimeError("Wrong dimensionality of the array")
-        self.log.debug("ispin value = " + str(value))
-
-        numofbands = int(self.spd.shape[1] / 2)
-
-        if separate == False:
-            # spin density or magnetization
-            self.spd = self.spd[:, :, value]
-            self.spd = self.spd.sum(axis=2)
-            self.log.info("new spd shape =" + str(self.spd.shape))
-            self.log.debug("selectIspin: ...Done")
-            if self.mode == "parametric":
-                if self.numspin > 1:
-                    if value == [0]:
-                        print("Plotting spin density...")
-                    elif value == [1]:
-                        print("Plotting spin magnetization...")
-
-        else:
-            # spin up (spin = 0) and spin down (spin = 1) separately.
-            if value == [0]:
-                # select spin up block
-                self.spd = self.spd[:, :numofbands, 0]
-
-            elif value == [1]:
-                # select spin down block
-                self.spd = self.spd[:, numofbands:, 0]
-
-        return
-
-    def selectAtoms(self, value=None, fortran=False):
-        """
-    value is a list with the values of Atoms to select. The optional
-    `fortran` argument indicates whether a c-like 0-based indexing
-    (`=False`, default) or a fortran-like 1-based (`=True`) is
-    provided in `value`.
-
-    Example:
-    >>> foo = ProcarParser()
-    >>> foo.readFile("PROCAR")
-    >>> bar = ProcarSelect(foo)
-    >>> bar.selectIspin([...])
-    >>> bar.selectAtoms([0,1,2]) #atom0+atom1+atom2
-
-    Note: this method should be called after select.Ispin
-    """
-        self.log.debug("selectAtoms: ...")
-
-        # taking care about stupid fortran indexing
-        if fortran is True:
-            value = [x - 1 for x in value]
-
-        # all kpoint, all bands, VALUE atoms, all the rest
-        self.log.debug("old shape =" + str(self.spd.shape))
-
-        # testing if the dimensionaluty is rigth:
-        dimen = len(self.spd.shape)
-        if dimen != 4:
-            self.log.error(
-                "The array is " + str(dimen) + " dimensional, expecting a"
-                " 4 dimensional array."
-            )
-            self.log.error(
-                "You should call selectIspin->selecAtom->selectOrbitals, "
-                "in this order."
-            )
-            raise RuntimeError("Wrong dimensionality of the array")
-        self.spd = self.spd[:, :, value]
-        self.spd = self.spd.sum(axis=2)
-        # self.cspd = self.cspd[:,:,value]
-        # self.cspd = self.cspd.sum(axis=2)
-        self.log.info("new shape =" + str(self.spd.shape))
-        self.log.debug("selectAtoms: ...Done")
-        return
-
-    def selectOrbital(self, value):
-        """
-    value is a list with the values of orbital to select.
-
-    Example:
-    >>> foo = ProcarParser()
-    >>> foo.readFile("PROCAR")
-    >>> bar = ProcarSelect(foo)
-    >>> bar.selectIspin([...])
-    >>> bar.selectAtoms([...])
-    >>> bar.selectOrbital([-1]) #the last (`tot`) field
-
-    to select "p" orbitals just change the argument in the last line
-    to [2,3,4] or as needed
-
-    Note: this method should be called after `select.Ispin` and
-    `select.Atoms`
-    """
-        self.log.debug("selectOrbital: ...")
-        self.log.debug("Changing the orbital `values` to have a 0-based indexes")
-        # Mind: the first orbital field is the atoms number, which is not
-        # an orbital, therefore the orbital index is an affective 1-based
-        # therefore all `value` indexes += 1 (well, negative values do not
-        # change )
-        for i in range(len(value)):
-            if value[i] >= 0:
-                value[i] += 1
-
-        self.log.debug("New values (indexes to select) :" + str(value))
-
-        # all kpoint, all bands, VALUE orbitals, nothing else?
-        self.spd = self.spd[:, :, value]
-        # self.cspd = self.cspd[:,:,value]
-        self.log.debug("old shape =" + str(self.spd.shape))
-
-        # testing if the dimensionaluty is rigth:
-        dimen = len(self.spd.shape)
-        if dimen != 3:
-            self.log.error(
-                "The array is " + str(dimen) + " dimensional, expecting a"
-                " 3 dimensional array."
-            )
-            self.log.error(
-                "You should call selectIspin->selecAtom->selectOrbitals, "
-                "in this order."
-            )
-            raise RuntimeError("Wrong dimensionality of the array")
-
-        self.spd = self.spd.sum(axis=2)
-        # self.cspd=self.cspd.sum(axis=2)
-        self.log.info("new shape =" + str(self.spd.shape))
-        self.log.debug("selectOrbital: ...Done")
-        return
+import logging
+import re
+import sys
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from ..utils import UtilsProcar
+
+
+class ProcarSelect:
+    """
+  Reduces the dimensionality of the data making it uselful to
+  plot bands.
+
+  The main data to manipulate is the projected electronic structure.
+  Its shape original is:
+
+  spd[kpoint][band][ispin][atom][orbital].
+
+  The selection of components should be done in order, says, first
+  "ispin", then "atom", and at last "orbital".
+
+  Note: once any selection has been performed, the data itself
+  changes. Say, if you want compare atom [0] and [1,2], you need two
+  instances of this class.
+
+
+  Example to compare the bandstructure of two set of atoms
+  >>>
+
+  """
+
+    def __init__(
+        self, ProcarData=None, deepCopy=True, loglevel=logging.WARNING, mode=None
+    ):
+
+        self.spd = None
+        self.bands = None
+        self.kpoints = None
+        # self.cspd=None
+        self.mode = mode
+
+        # We want a logging to tell us what is happening
+        self.log = logging.getLogger("ProcarSelect")
+        self.log.setLevel(loglevel)
+        self.ch = logging.StreamHandler()
+        self.ch.setFormatter(
+            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
+        )
+        self.ch.setLevel(logging.DEBUG)
+        self.log.addHandler(self.ch)
+        # At last, one message to the logger.
+        self.log.debug("ProcarSelect: instanciated")
+
+        if ProcarData is not None:
+            self.setData(ProcarData, deepCopy)
+        return
+
+    def setData(self, ProcarData, deepCopy=True):
+        """
+    The data from ProcarData is deepCopy-ed by default (ie: their
+    elements are not modified by this class.
+
+    Args:
+
+    -ProcarData: is a ProcarParser instance (or anything with similar
+     functionality, duck typing)
+
+    -deepCopy=True: If false a shallow copy will be made (saves memory).
+    """
+        self.log.debug("setData: ...")
+        if deepCopy is True:
+            self.spd = ProcarData.spd.copy()
+            self.bands = ProcarData.bands.copy()
+            self.kpoints = ProcarData.kpoints.copy()
+            # self.cspd = ProcarData.cspd.copy()
+        else:
+            self.spd = ProcarData.spd
+            self.bands = ProcarData.bands
+            self.kpoints = ProcarData.kpoints
+            # self.cspd = ProcarData.cspd
+
+        self.numspin = self.spd.shape[2]  # Number of spins
+        self.log.debug("setData: ... Done")
+        print(
+            "spd shape      :  %s [kpoints, bands, spins, atoms+1, orbitals+2]"
+            % str(self.spd.shape)
+        )
+
+        return
+
+    def selectIspin(self, value=None, separate=False):
+        """
+    value is a list with the values of Ispin to select.
+
+    UPDATE:
+        if separate == true, then spin = 0 corresponds to spin up
+        and spin = 1 corresponds to spin down. If not, they give
+        spin density and spin magnetization, respectively.
+
+    Example:
+    >>> foo = ProcarParser()
+    >>> foo.readFile("PROCAR")
+    >>> bar = ProcarSelect(foo)
+    >>> bar.selectIspin([0]) #just the density
+    """
+        # all kpoint, all bands, VALUE spin, all the rest
+        self.log.debug("selectIspin: ...")
+        self.log.debug("old spd shape =" + str(self.spd.shape))
+        # first, testing if the domensionaluty is rigth:
+        dimen = len(self.spd.shape)
+        if dimen != 5:
+            self.log.error(
+                "The array is " + str(dimen) + " dimensional, expecting a"
+                " 5 dimensional array."
+            )
+            self.log.error(
+                "You should call selectIspin->selecAtom->selectOrbitals, "
+                "in this order."
+            )
+            raise RuntimeError("Wrong dimensionality of the array")
+        self.log.debug("ispin value = " + str(value))
+
+        numofbands = int(self.spd.shape[1] / 2)
+
+        if separate == False:
+            # spin density or magnetization
+            self.spd = self.spd[:, :, value]
+            self.spd = self.spd.sum(axis=2)
+            self.log.info("new spd shape =" + str(self.spd.shape))
+            self.log.debug("selectIspin: ...Done")
+            if self.mode == "parametric":
+                if self.numspin > 1:
+                    if value == [0]:
+                        print("Plotting spin density...")
+                    elif value == [1]:
+                        print("Plotting spin magnetization...")
+
+        else:
+            # spin up (spin = 0) and spin down (spin = 1) separately.
+            if value == [0]:
+                # select spin up block
+                self.spd = self.spd[:, :numofbands, 0]
+
+            elif value == [1]:
+                # select spin down block
+                self.spd = self.spd[:, numofbands:, 0]
+
+        return
+
+    def selectAtoms(self, value=None, fortran=False):
+        """
+    value is a list with the values of Atoms to select. The optional
+    `fortran` argument indicates whether a c-like 0-based indexing
+    (`=False`, default) or a fortran-like 1-based (`=True`) is
+    provided in `value`.
+
+    Example:
+    >>> foo = ProcarParser()
+    >>> foo.readFile("PROCAR")
+    >>> bar = ProcarSelect(foo)
+    >>> bar.selectIspin([...])
+    >>> bar.selectAtoms([0,1,2]) #atom0+atom1+atom2
+
+    Note: this method should be called after select.Ispin
+    """
+        self.log.debug("selectAtoms: ...")
+
+        # taking care about stupid fortran indexing
+        if fortran is True:
+            value = [x - 1 for x in value]
+
+        # all kpoint, all bands, VALUE atoms, all the rest
+        self.log.debug("old shape =" + str(self.spd.shape))
+
+        # testing if the dimensionaluty is rigth:
+        dimen = len(self.spd.shape)
+        if dimen != 4:
+            self.log.error(
+                "The array is " + str(dimen) + " dimensional, expecting a"
+                " 4 dimensional array."
+            )
+            self.log.error(
+                "You should call selectIspin->selecAtom->selectOrbitals, "
+                "in this order."
+            )
+            raise RuntimeError("Wrong dimensionality of the array")
+        self.spd = self.spd[:, :, value]
+        self.spd = self.spd.sum(axis=2)
+        # self.cspd = self.cspd[:,:,value]
+        # self.cspd = self.cspd.sum(axis=2)
+        self.log.info("new shape =" + str(self.spd.shape))
+        self.log.debug("selectAtoms: ...Done")
+        return
+
+    def selectOrbital(self, value):
+        """
+    value is a list with the values of orbital to select.
+
+    Example:
+    >>> foo = ProcarParser()
+    >>> foo.readFile("PROCAR")
+    >>> bar = ProcarSelect(foo)
+    >>> bar.selectIspin([...])
+    >>> bar.selectAtoms([...])
+    >>> bar.selectOrbital([-1]) #the last (`tot`) field
+
+    to select "p" orbitals just change the argument in the last line
+    to [2,3,4] or as needed
+
+    Note: this method should be called after `select.Ispin` and
+    `select.Atoms`
+    """
+        self.log.debug("selectOrbital: ...")
+        self.log.debug("Changing the orbital `values` to have a 0-based indexes")
+        # Mind: the first orbital field is the atoms number, which is not
+        # an orbital, therefore the orbital index is an affective 1-based
+        # therefore all `value` indexes += 1 (well, negative values do not
+        # change )
+        for i in range(len(value)):
+            if value[i] >= 0:
+                value[i] += 1
+
+        self.log.debug("New values (indexes to select) :" + str(value))
+
+        # all kpoint, all bands, VALUE orbitals, nothing else?
+        self.spd = self.spd[:, :, value]
+        # self.cspd = self.cspd[:,:,value]
+        self.log.debug("old shape =" + str(self.spd.shape))
+
+        # testing if the dimensionaluty is rigth:
+        dimen = len(self.spd.shape)
+        if dimen != 3:
+            self.log.error(
+                "The array is " + str(dimen) + " dimensional, expecting a"
+                " 3 dimensional array."
+            )
+            self.log.error(
+                "You should call selectIspin->selecAtom->selectOrbitals, "
+                "in this order."
+            )
+            raise RuntimeError("Wrong dimensionality of the array")
+
+        self.spd = self.spd.sum(axis=2)
+        # self.cspd=self.cspd.sum(axis=2)
+        self.log.info("new shape =" + str(self.spd.shape))
+        self.log.debug("selectOrbital: ...Done")
+        return
```

### Comparing `PyProcar-5.6.6/pyprocar/procarsymmetry/procarsymmetry.py` & `PyProcar-6.0.0/pyprocar/core/procarsymmetry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-import numpy as np
-import re
-import logging
-import matplotlib.pyplot as plt
-import sys
-
-
-class ProcarSymmetry:
-    def __init__(
-        self,
-        kpoints,
-        bands,
-        character=None,
-        sx=None,
-        sy=None,
-        sz=None,
-        loglevel=logging.WARNING,
-    ):
-        self.log = logging.getLogger("ProcarSymmetry")
-        self.log.setLevel(loglevel)
-        self.ch = logging.StreamHandler()
-        self.ch.setFormatter(
-            logging.Formatter("%(name)s::%(levelname)s: " "%(message)s")
-        )
-        self.ch.setLevel(logging.DEBUG)
-        self.log.addHandler(self.ch)
-        self.log.debug("ProcarSymmetry.__init__: ...")
-
-        self.kpoints = kpoints
-        self.bands = bands
-        # optional arguments when not given will False, but they can still
-        # be treated like arrays
-        self.character = np.array([])
-        if character is not None:
-            self.character = character
-        self.sx = np.array([])
-        if sx is not None:
-            self.sx = sx
-        self.sy = np.array([])
-        if sy is not None:
-            self.sy = sy
-        self.sz = np.array([])
-        if sz is not None:
-            self.sz = sz
-
-        self.log.info("Kpoints : " + str(self.kpoints.shape))
-        self.log.info("bands   : " + str(self.bands.shape))
-        self.log.info("character  : " + str(self.character.shape))
-        self.log.info("sx      : " + str(self.sx.shape))
-        self.log.info("sy      : " + str(self.sy.shape))
-        self.log.info("sz      : " + str(self.sz.shape))
-        self.log.debug("ProcarSymmetry.__init__: ...Done")
-
-        return
-
-    def _q_mult(self, q1, q2):
-        """
-    Multiplication of quaternions, it doesn't fit in any other place
-    """
-        w1, x1, y1, z1 = q1
-        w2, x2, y2, z2 = q2
-        w = w1 * w2 - x1 * x2 - y1 * y2 - z1 * z2
-        x = w1 * x2 + x1 * w2 + y1 * z2 - z1 * y2
-        y = w1 * y2 + y1 * w2 + z1 * x2 - x1 * z2
-        z = w1 * z2 + z1 * w2 + x1 * y2 - y1 * x2
-        return np.array((w, x, y, z))
-
-    def GeneralRotation(self, angle, rotAxis=[0, 0, 1], store=True):
-        """Apply a rotation defined by an angle and an axis.
-    
-    Returning value: (Kpoints, sx,sy,sz), the rotated Kpoints and spin
-                     vectors (if not the case, they will be empty
-                     arrays).
-
-    Arguments
-    angle: the rotation angle, must be in degrees!
-
-    rotAxis : a fixed Axis when applying the symmetry, usually it is
-    from Gamma to another point). It doesn't need to be normalized. 
-    The RotAxis can be:
-       [x,y,z] : a cartesian vector in k-space.
-       'x': [1,0,0], a rotation in the yz plane. 
-       'y': [0,1,0], a rotation in the zx plane.
-       'z': [0,0,1], a rotation in the xy plane
-
-    """
-        if rotAxis == "x" or rotAxis == "X":
-            rotAxis = [1, 0, 0]
-        if rotAxis == "y" or rotAxis == "Y":
-            rotAxis = [0, 1, 0]
-        if rotAxis == "z" or rotAxis == "Z":
-            rotAxis = [0, 0, 1]
-        rotAxis = np.array(rotAxis, dtype=float)
-        self.log.debug("rotAxis : " + str(rotAxis))
-        rotAxis = rotAxis / np.linalg.norm(rotAxis)
-        self.log.debug("rotAxis Normalized : " + str(rotAxis))
-        self.log.debug("Angle : " + str(angle))
-        angle = angle * np.pi / 180
-        # defining a quaternion for rotatoin
-        angle = angle / 2
-        rotAxis = rotAxis * np.sin(angle)
-        qRot = np.array((np.cos(angle), rotAxis[0], rotAxis[1], rotAxis[2]))
-        qRotI = np.array((np.cos(angle), -rotAxis[0], -rotAxis[1], -rotAxis[2]))
-        self.log.debug("Rot. quaternion : " + str(qRot))
-        self.log.debug("Rot. quaternion conjugate : " + str(qRotI))
-        # converting self.kpoints into quaternions
-        w = np.zeros((len(self.kpoints), 1))
-        qvectors = np.column_stack((w, self.kpoints)).transpose()
-        self.log.debug(
-            "Kpoints-> quaternions (transposed):\n" + str(qvectors.transpose())
-        )
-        qvectors = self._q_mult(qRot, qvectors)
-        qvectors = self._q_mult(qvectors, qRotI).transpose()
-        kpoints = qvectors[:, 1:]
-        self.log.debug("Rotated kpoints :\n" + str(qvectors))
-
-        # rotating the spin vector (if exist)
-        sxShape, syShape, szShape = self.sx.shape, self.sy.shape, self.sz.shape
-        self.log.debug("Spin vector Shapes : " + str((sxShape, syShape, szShape)))
-        # The first entry has to be an array of 0s, w could do the work,
-        # but if len(self.sx)==0 qvectors will have a non-defined length
-        qvectors = (
-            0 * self.sx.flatten(),
-            self.sx.flatten(),
-            self.sy.flatten(),
-            self.sz.flatten(),
-        )
-        self.log.debug("Spin vector quaternions: \n" + str(qvectors))
-        qvectors = self._q_mult(qRot, qvectors)
-        qvectors = self._q_mult(qvectors, qRotI)
-        self.log.debug("Spin quaternions after rotation:\n" + str(qvectors))
-        sx, sy, sz = qvectors[1], qvectors[2], qvectors[3]
-        sx.shape, sy.shape, sz.shape = sxShape, syShape, szShape
-
-        if store is True:
-            self.kpoints, self.sx, self.sy, self.sz = kpoints, sx, sy, sz
-        self.log.debug("GeneralRotation: ...Done")
-        return (kpoints, sx, sy, sz)
-
-    def RotSymmetryZ(self, order):
-        """Applies the given rotational crystal symmetry to the current
-    system. ie: to unfold the irreductible BZ to the full BZ.
-
-    Only rotations along z-axis are performed, you can use
-    self.GeneralRotation first. 
-
-    The user is responsible of provide a useful input. The method
-    doesn't check the physics.
-
-    """
-        self.log.debug("RotSymmetryZ:...")
-        rotations = [
-            self.GeneralRotation(360 * i / order, store=False) for i in range(order)
-        ]
-        rotations = list(zip(*rotations))
-        self.log.debug(
-            "self.kpoints.shape (before concat.): " + str(self.kpoints.shape)
-        )
-        self.kpoints = np.concatenate(rotations[0], axis=0)
-        self.log.debug("self.kpoints.shape (after concat.): " + str(self.kpoints.shape))
-        self.sx = np.concatenate(rotations[1], axis=0)
-        self.sy = np.concatenate(rotations[2], axis=0)
-        self.sz = np.concatenate(rotations[3], axis=0)
-        # the bands and proj. character also need to be enlarged
-        bandsChar = [(self.bands, self.character) for i in range(order)]
-        bandsChar = list(zip(*bandsChar))
-        self.bands = np.concatenate(bandsChar[0], axis=0)
-        self.character = np.concatenate(bandsChar[1], axis=0)
-        self.log.debug("RotSymmZ:...Done")
-
-        return
-
-    def MirrorX(self):
-        """Applies the given rotational crystal symmetry to the current
-    system. ie: to unfold the irreductible BZ to the full BZ.
-
-    """
-        self.log.debug("Mirror:...")
-        newK = self.kpoints * np.array([1, -1, 1])
-        self.kpoints = np.concatenate((self.kpoints, newK), axis=0)
-        self.log.debug("self.kpoints.shape (after concat.): " + str(self.kpoints.shape))
-        newSx = -1 * self.sx
-        newSy = 1 * self.sy
-        newSz = 1 * self.sz
-        self.sx = np.concatenate((self.sx, newSx), axis=0)
-        self.sy = np.concatenate((self.sy, newSy), axis=0)
-        self.sz = np.concatenate((self.sz, newSz), axis=0)
-        print("self.sx", self.sx.shape)
-        print("self.sy", self.sy.shape)
-        print("self.sz", self.sz.shape)
-        # the bands and proj. character also need to be enlarged
-        self.bands = np.concatenate((self.bands, self.bands), axis=0)
-        self.character = np.concatenate((self.character, self.character), axis=0)
-        print("self.character", self.character.shape)
-        print("self.bands", self.bands.shape)
-        self.log.debug("Mirror:...Done")
-
-        return
-
-    def Translate(self, newOrigin):
-        """Centers the Kpoints at newOrigin, newOrigin is either and index (of
-   some Kpoint) or the cartesian coordinates of one point in the
-   reciprocal space.
-
-    """
-        self.log.debug("Translate():  ...")
-        if len(newOrigin) == 1:
-            newOrigin = int(newOrigin[0])
-            newOrigin = self.kpoints[newOrigin]
-        # Make sure newOrigin is a numpy array
-        newOrigin = np.array(newOrigin, dtype=float)
-        self.log.debug("newOrigin: " + str(newOrigin))
-        self.kpoints = self.kpoints - newOrigin
-        self.log.debug("new Kpoints:\n" + str(self.kpoints))
-        self.log.debug("Translate(): ...Done")
-        return
+import numpy as np
+import re
+import logging
+import matplotlib.pyplot as plt
+import sys
+
+
+class ProcarSymmetry:
+    def __init__(
+        self,
+        kpoints,
+        bands,
+        character=None,
+        sx=None,
+        sy=None,
+        sz=None,
+        loglevel=logging.WARNING,
+    ):
+        self.log = logging.getLogger("ProcarSymmetry")
+        self.log.setLevel(loglevel)
+        self.ch = logging.StreamHandler()
+        self.ch.setFormatter(
+            logging.Formatter("%(name)s::%(levelname)s: " "%(message)s")
+        )
+        self.ch.setLevel(logging.DEBUG)
+        self.log.addHandler(self.ch)
+        self.log.debug("ProcarSymmetry.__init__: ...")
+
+        self.kpoints = kpoints
+        self.bands = bands
+        # optional arguments when not given will False, but they can still
+        # be treated like arrays
+        self.character = np.array([])
+        if character is not None:
+            self.character = character
+        self.sx = np.array([])
+        if sx is not None:
+            self.sx = sx
+        self.sy = np.array([])
+        if sy is not None:
+            self.sy = sy
+        self.sz = np.array([])
+        if sz is not None:
+            self.sz = sz
+
+        self.log.info("Kpoints : " + str(self.kpoints.shape))
+        self.log.info("bands   : " + str(self.bands.shape))
+        self.log.info("character  : " + str(self.character.shape))
+        self.log.info("sx      : " + str(self.sx.shape))
+        self.log.info("sy      : " + str(self.sy.shape))
+        self.log.info("sz      : " + str(self.sz.shape))
+        self.log.debug("ProcarSymmetry.__init__: ...Done")
+
+        return
+
+    def _q_mult(self, q1, q2):
+        """
+    Multiplication of quaternions, it doesn't fit in any other place
+    """
+        w1, x1, y1, z1 = q1
+        w2, x2, y2, z2 = q2
+        w = w1 * w2 - x1 * x2 - y1 * y2 - z1 * z2
+        x = w1 * x2 + x1 * w2 + y1 * z2 - z1 * y2
+        y = w1 * y2 + y1 * w2 + z1 * x2 - x1 * z2
+        z = w1 * z2 + z1 * w2 + x1 * y2 - y1 * x2
+        return np.array((w, x, y, z))
+
+    def general_rotation(self, angle, rotAxis=[0, 0, 1], store=True):
+        """Apply a rotation defined by an angle and an axis.
+    
+    Returning value: (Kpoints, sx,sy,sz), the rotated Kpoints and spin
+                     vectors (if not the case, they will be empty
+                     arrays).
+
+    Arguments
+    angle: the rotation angle, must be in degrees!
+
+    rotAxis : a fixed Axis when applying the symmetry, usually it is
+    from Gamma to another point). It doesn't need to be normalized. 
+    The RotAxis can be:
+       [x,y,z] : a cartesian vector in k-space.
+       'x': [1,0,0], a rotation in the yz plane. 
+       'y': [0,1,0], a rotation in the zx plane.
+       'z': [0,0,1], a rotation in the xy plane
+
+    """
+        if rotAxis == "x" or rotAxis == "X":
+            rotAxis = [1, 0, 0]
+        if rotAxis == "y" or rotAxis == "Y":
+            rotAxis = [0, 1, 0]
+        if rotAxis == "z" or rotAxis == "Z":
+            rotAxis = [0, 0, 1]
+        rotAxis = np.array(rotAxis, dtype=float)
+        self.log.debug("rotAxis : " + str(rotAxis))
+        rotAxis = rotAxis / np.linalg.norm(rotAxis)
+        self.log.debug("rotAxis Normalized : " + str(rotAxis))
+        self.log.debug("Angle : " + str(angle))
+        angle = angle * np.pi / 180
+        # defining a quaternion for rotatoin
+        angle = angle / 2
+        rotAxis = rotAxis * np.sin(angle)
+        qRot = np.array((np.cos(angle), rotAxis[0], rotAxis[1], rotAxis[2]))
+        qRotI = np.array((np.cos(angle), -rotAxis[0], -rotAxis[1], -rotAxis[2]))
+        self.log.debug("Rot. quaternion : " + str(qRot))
+        self.log.debug("Rot. quaternion conjugate : " + str(qRotI))
+        # converting self.kpoints into quaternions
+        w = np.zeros((len(self.kpoints), 1))
+        qvectors = np.column_stack((w, self.kpoints)).transpose()
+        self.log.debug(
+            "Kpoints-> quaternions (transposed):\n" + str(qvectors.transpose())
+        )
+        qvectors = self._q_mult(qRot, qvectors)
+        qvectors = self._q_mult(qvectors, qRotI).transpose()
+        kpoints = qvectors[:, 1:]
+        self.log.debug("Rotated kpoints :\n" + str(qvectors))
+
+        # rotating the spin vector (if exist)
+        sxShape, syShape, szShape = self.sx.shape, self.sy.shape, self.sz.shape
+        self.log.debug("Spin vector Shapes : " + str((sxShape, syShape, szShape)))
+        # The first entry has to be an array of 0s, w could do the work,
+        # but if len(self.sx)==0 qvectors will have a non-defined length
+        qvectors = (
+            0 * self.sx.flatten(),
+            self.sx.flatten(),
+            self.sy.flatten(),
+            self.sz.flatten(),
+        )
+        self.log.debug("Spin vector quaternions: \n" + str(qvectors))
+        qvectors = self._q_mult(qRot, qvectors)
+        qvectors = self._q_mult(qvectors, qRotI)
+        self.log.debug("Spin quaternions after rotation:\n" + str(qvectors))
+        sx, sy, sz = qvectors[1], qvectors[2], qvectors[3]
+        sx.shape, sy.shape, sz.shape = sxShape, syShape, szShape
+
+        if store is True:
+            self.kpoints, self.sx, self.sy, self.sz = kpoints, sx, sy, sz
+        self.log.debug("GeneralRotation: ...Done")
+        return (kpoints, sx, sy, sz)
+
+    def rot_symmetry_z(self, order):
+        """Applies the given rotational crystal symmetry to the current
+    system. ie: to unfold the irreductible BZ to the full BZ.
+
+    Only rotations along z-axis are performed, you can use
+    self.GeneralRotation first. 
+
+    The user is responsible of provide a useful input. The method
+    doesn't check the physics.
+
+    """
+        self.log.debug("RotSymmetryZ:...")
+        rotations = [
+            self.general_rotation(360 * i / order, store=False) for i in range(order)
+        ]
+        rotations = list(zip(*rotations))
+        self.log.debug(
+            "self.kpoints.shape (before concat.): " + str(self.kpoints.shape)
+        )
+        self.kpoints = np.concatenate(rotations[0], axis=0)
+        self.log.debug("self.kpoints.shape (after concat.): " + str(self.kpoints.shape))
+        self.sx = np.concatenate(rotations[1], axis=0)
+        self.sy = np.concatenate(rotations[2], axis=0)
+        self.sz = np.concatenate(rotations[3], axis=0)
+        # the bands and proj. character also need to be enlarged
+        bandsChar = [(self.bands, self.character) for i in range(order)]
+        bandsChar = list(zip(*bandsChar))
+        self.bands = np.concatenate(bandsChar[0], axis=0)
+        self.character = np.concatenate(bandsChar[1], axis=0)
+        self.log.debug("RotSymmZ:...Done")
+
+        return
+
+    def mirror_x(self):
+        """Applies the given rotational crystal symmetry to the current
+    system. ie: to unfold the irreductible BZ to the full BZ.
+
+    """
+        self.log.debug("Mirror:...")
+        newK = self.kpoints * np.array([1, -1, 1])
+        self.kpoints = np.concatenate((self.kpoints, newK), axis=0)
+        self.log.debug("self.kpoints.shape (after concat.): " + str(self.kpoints.shape))
+        newSx = -1 * self.sx
+        newSy = 1 * self.sy
+        newSz = 1 * self.sz
+        self.sx = np.concatenate((self.sx, newSx), axis=0)
+        self.sy = np.concatenate((self.sy, newSy), axis=0)
+        self.sz = np.concatenate((self.sz, newSz), axis=0)
+        print("self.sx", self.sx.shape)
+        print("self.sy", self.sy.shape)
+        print("self.sz", self.sz.shape)
+        # the bands and proj. character also need to be enlarged
+        self.bands = np.concatenate((self.bands, self.bands), axis=0)
+        self.character = np.concatenate((self.character, self.character), axis=0)
+        print("self.character", self.character.shape)
+        print("self.bands", self.bands.shape)
+        self.log.debug("Mirror:...Done")
+
+        return
+
+    def translate(self, newOrigin):
+        """Centers the Kpoints at newOrigin, newOrigin is either and index (of
+   some Kpoint) or the cartesian coordinates of one point in the
+   reciprocal space.
+
+    """
+        self.log.debug("Translate():  ...")
+        if len(newOrigin) == 1:
+            newOrigin = int(newOrigin[0])
+            newOrigin = self.kpoints[newOrigin]
+        # Make sure newOrigin is a numpy array
+        newOrigin = np.array(newOrigin, dtype=float)
+        self.log.debug("newOrigin: " + str(newOrigin))
+        self.kpoints = self.kpoints - newOrigin
+        self.log.debug("new Kpoints:\n" + str(self.kpoints))
+        self.log.debug("Translate(): ...Done")
+        return
```

### Comparing `PyProcar-5.6.6/pyprocar/procarunfold/fatband.py` & `PyProcar-6.0.0/pyprocar/core/procarunfold/fatband.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-#!/usr/bin/env python
-import matplotlib as mpl
-import matplotlib.pyplot as plt
-from matplotlib.collections import LineCollection
-from matplotlib.colors import colorConverter
-import numpy as np
-import argparse
-import os.path
-
-
-def plot_band_weight(
-        kslist,
-        ekslist,
-        wkslist=None,
-        efermi=None,
-        shift_efermi=False,
-        yrange=None,
-        output=None,
-        style="alpha",
-        color="blue",
-        axis=None,
-        width=10,
-        fatness=4,
-        xticks=None,
-        cmap=mpl.cm.bwr,
-        weight_min=-0.1,
-        weight_max=0.6,
-):
-    if axis is None:
-        fig, a = plt.subplots()
-    else:
-        a = axis
-    if efermi is not None and shift_efermi:
-        ekslist = np.array(ekslist) - efermi
-    else:
-        ekslist = np.array(ekslist)
-
-    xmax = max(kslist[0])
-    if yrange is None:
-        yrange = (
-            np.array(ekslist).flatten().min() - 0.66,
-            np.array(ekslist).flatten().max() + 0.66,
-        )
-    if wkslist is not None:
-        for i in range(len(kslist)):
-            x = kslist[i]
-            y = ekslist[i]
-            # lwidths=np.ones(len(x))
-            points = np.array([x, y]).T.reshape(-1, 1, 2)
-            segments = np.concatenate([points[:-1], points[1:]], axis=1)
-            if style == "width":
-                lwidths = np.array(wkslist[i]) * width
-                lc = LineCollection(segments, linewidths=lwidths, colors=color)
-            elif style == "alpha":
-                lwidths = np.array(wkslist[i]) * width
-
-                # The alpha values sometimes goes above 1 so in those cases we will normalize
-                # the alpha values. -Uthpala
-                alpha_values = [lwidth / (width + 0.05) for lwidth in lwidths]
-
-                if max(alpha_values) > 1:
-                    print("alpha is larger than 1. Renormalizing values.")
-                    alpha_values = [
-                        alpha_i / max(alpha_values) for alpha_i in alpha_values
-                    ]
-
-                lc = LineCollection(
-                    segments,
-                    linewidths=[fatness] * len(x),
-                    colors=[
-                        colorConverter.to_rgba(color, alpha=alpha_i)
-                        for alpha_i in alpha_values
-                    ],
-                )
-
-            elif style == "color" or style == "colormap":
-                lwidths = np.array(wkslist[i]) * width
-                norm = mpl.colors.Normalize(vmin=weight_min, vmax=weight_max)
-                # norm = mpl.colors.SymLogNorm(linthresh=0.03,vmin=weight_min, vmax=weight_max)
-                m = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
-                # lc = LineCollection(segments,linewidths=np.abs(norm(lwidths)-0.5)*1, colors=[m.to_rgba(lwidth) for lwidth in lwidths])
-                lc = LineCollection(
-                    segments,
-                    linewidths=lwidths,
-                    colors=[m.to_rgba(lwidth) for lwidth in lwidths],
-                )
-            a.add_collection(lc)
-    if axis is None:
-        for ks, eks in zip(kslist, ekslist):
-            a.plot(ks, eks, color="gray", linewidth=0.01)
-        # a.set_xlim(0, xmax)
-        # a.set_ylim(yrange)
-        if xticks is not None:
-            a.set_xticks(xticks[1])
-            a.set_xticklabels(xticks[0])
-            for x in xticks[1]:
-                a.axvline(x, alpha=0.6, color="black", linewidth=0.7)
-        if efermi is not None:
-            if shift_efermi:
-                a.axhline(linestyle="--", color="black")
-            else:
-                a.axhline(efermi, linestyle="--", color="black")
-
-    return a
-
-
-def main():
-    parser = argparse.ArgumentParser(description="plot wannier bands.")
-    parser.add_argument("fname", type=str, help="dat filename")
-    parser.add_argument("-e",
-                        "--efermi",
-                        type=float,
-                        help="Fermi energy",
-                        default=None)
-    parser.add_argument("-o",
-                        "--output",
-                        type=str,
-                        help="output filename",
-                        default=None)
-    parser.add_argument("-w",
-                        "--weight",
-                        action="store_true",
-                        help="use -w to plot weighted band.")
-    parser.add_argument("-y",
-                        "--yrange",
-                        type=float,
-                        nargs="+",
-                        help="range of yticks",
-                        default=None)
-    parser.add_argument("-s",
-                        "--style",
-                        type=str,
-                        help="style of line, width | alpha",
-                        default="width")
-    args = parser.parse_args()
-    if args.output is None:
-        output = os.path.splitext(args.fname)[0] + ".png"
-    if args.efermi is None:
-        efermi = get_fermi("SCF/OUTCAR")
-    plot_band_weight_file(
-        fname=args.fname,
-        efermi=efermi,
-        weight=args.weight,
-        yrange=args.yrange,
-        style=args.style,
-    )
-    if output is not None:
-        plt.savefig(output)
-
-    plt.show()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+from matplotlib.collections import LineCollection
+from matplotlib.colors import colorConverter
+import numpy as np
+import argparse
+import os.path
+
+
+def plot_band_weight(
+        kslist,
+        ekslist,
+        wkslist=None,
+        efermi=None,
+        shift_efermi=False,
+        yrange=None,
+        output=None,
+        style="alpha",
+        color="blue",
+        axis=None,
+        width=10,
+        fatness=4,
+        xticks=None,
+        cmap=mpl.cm.bwr,
+        weight_min=-0.1,
+        weight_max=0.6,
+):
+    if axis is None:
+        fig, a = plt.subplots()
+    else:
+        a = axis
+    if efermi is not None and shift_efermi:
+        ekslist = np.array(ekslist) - efermi
+    else:
+        ekslist = np.array(ekslist)
+
+    xmax = max(kslist[0])
+    if yrange is None:
+        yrange = (
+            np.array(ekslist).flatten().min() - 0.66,
+            np.array(ekslist).flatten().max() + 0.66,
+        )
+    if wkslist is not None:
+        for i in range(len(kslist)):
+            x = kslist[i]
+            y = ekslist[i]
+            # lwidths=np.ones(len(x))
+            points = np.array([x, y]).T.reshape(-1, 1, 2)
+            segments = np.concatenate([points[:-1], points[1:]], axis=1)
+            if style == "width":
+                lwidths = np.array(wkslist[i]) * width
+                lc = LineCollection(segments, linewidths=lwidths, colors=color)
+            elif style == "alpha":
+                lwidths = np.array(wkslist[i]) * width
+
+                # The alpha values sometimes goes above 1 so in those cases we will normalize
+                # the alpha values. -Uthpala
+                alpha_values = [lwidth / (width + 0.05) for lwidth in lwidths]
+
+                if max(alpha_values) > 1:
+                    print("alpha is larger than 1. Renormalizing values.")
+                    alpha_values = [
+                        alpha_i / max(alpha_values) for alpha_i in alpha_values
+                    ]
+
+                lc = LineCollection(
+                    segments,
+                    linewidths=[fatness] * len(x),
+                    colors=[
+                        colorConverter.to_rgba(color, alpha=alpha_i)
+                        for alpha_i in alpha_values
+                    ],
+                )
+
+            elif style == "color" or style == "colormap":
+                lwidths = np.array(wkslist[i]) * width
+                norm = mpl.colors.Normalize(vmin=weight_min, vmax=weight_max)
+                # norm = mpl.colors.SymLogNorm(linthresh=0.03,vmin=weight_min, vmax=weight_max)
+                m = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+                # lc = LineCollection(segments,linewidths=np.abs(norm(lwidths)-0.5)*1, colors=[m.to_rgba(lwidth) for lwidth in lwidths])
+                lc = LineCollection(
+                    segments,
+                    linewidths=lwidths,
+                    colors=[m.to_rgba(lwidth) for lwidth in lwidths],
+                )
+            a.add_collection(lc)
+    if axis is None:
+        for ks, eks in zip(kslist, ekslist):
+            a.plot(ks, eks, color="gray", linewidth=0.01)
+        # a.set_xlim(0, xmax)
+        # a.set_ylim(yrange)
+        if xticks is not None:
+            a.set_xticks(xticks[1])
+            a.set_xticklabels(xticks[0])
+            for x in xticks[1]:
+                a.axvline(x, alpha=0.6, color="black", linewidth=0.7)
+        if efermi is not None:
+            if shift_efermi:
+                a.axhline(linestyle="--", color="black")
+            else:
+                a.axhline(efermi, linestyle="--", color="black")
+
+    return a
+
+
+def main():
+    parser = argparse.ArgumentParser(description="plot wannier bands.")
+    parser.add_argument("fname", type=str, help="dat filename")
+    parser.add_argument("-e",
+                        "--efermi",
+                        type=float,
+                        help="Fermi energy",
+                        default=None)
+    parser.add_argument("-o",
+                        "--output",
+                        type=str,
+                        help="output filename",
+                        default=None)
+    parser.add_argument("-w",
+                        "--weight",
+                        action="store_true",
+                        help="use -w to plot weighted band.")
+    parser.add_argument("-y",
+                        "--yrange",
+                        type=float,
+                        nargs="+",
+                        help="range of yticks",
+                        default=None)
+    parser.add_argument("-s",
+                        "--style",
+                        type=str,
+                        help="style of line, width | alpha",
+                        default="width")
+    args = parser.parse_args()
+    if args.output is None:
+        output = os.path.splitext(args.fname)[0] + ".png"
+    if args.efermi is None:
+        efermi = get_fermi("SCF/OUTCAR")
+    plot_band_weight_file(
+        fname=args.fname,
+        efermi=efermi,
+        weight=args.weight,
+        yrange=args.yrange,
+        style=args.style,
+    )
+    if output is not None:
+        plt.savefig(output)
+
+    plt.show()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `PyProcar-5.6.6/pyprocar/procarunfold/procar_unfolder.py` & `PyProcar-6.0.0/pyprocar/core/procarunfold/procar_unfolder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import numpy as np
-from ase.io import read
-from .unfolder import Unfolder
-import matplotlib.pyplot as plt
-from .fatband import plot_band_weight
-from ..procarparser import ProcarParser
-
-
-class ProcarUnfolder(object):
-    def __init__(self, procar, poscar, supercell_matrix, ispin=None):
-        self.fname = procar
-        self.supercell_matrix = supercell_matrix
-        self._parse_procar(ispin=ispin)
-        self.atoms = read(poscar)
-        self.basis = []
-        self.positions = []
-
-    def _parse_procar(self, ispin=None):
-        self.procar = ProcarParser()
-        self.procar.readFile2(self.fname, phase=True, ispin=ispin)
-
-        
-
-    def _prepare_unfold_basis(self, ispin=None):
-        # basis, which are the name of the bands e.g. 'Ti|dxy|0'
-        # self.eigenvectors = np.zeros(
-        #    (self.procar.kpointsCount, self.procar.bandsCount,
-        #     (self.procar.orbitalCount - 1) * (self.procar.ionsCount - 1) *
-        #     self.procar.ispin), dtype='complex')
-        if ispin is None:
-            iispin = 0
-        else:
-            ispin -= 1
-        self.eigenvectors = np.reshape(
-            self.procar.carray[:, :, ispin, :, :],
-            (
-                self.procar.kpointsCount,
-                self.procar.bandsCount,
-                self.procar.ionsCount * self.procar.orbitalCount,
-            ),
-        )
-        norm = np.linalg.norm(self.eigenvectors, ord=2, axis=2)
-        self.eigenvectors /= norm[:, :, None]
-
-        for iatom, chem in enumerate(self.atoms.get_chemical_symbols()):
-            for iorb, orb in enumerate(self.procar.orbitalName):
-                for spin in range(self.procar.nspin):
-                    # todo: what about spin?
-                    self.basis.append("%s|%s|%s" % (None, orb, spin))
-                    self.positions.append(
-                        self.atoms.get_scaled_positions()[iatom])
-            
-            
-            
-    def unfold(self, ispin=None):
-        # spd: spd[kpoint][band][ispin][atom][orbital]
-        # bands[kpt][iband]
-        # to unfold,
-        # unfolder:
-        # def __init__(self, cell, basis, positions , supercell_matrix, eigenvectors, qpoints, tol_r=0.1, compare=None):
-        self._prepare_unfold_basis(ispin=ispin)
-        self.unfolder = Unfolder(
-            self.atoms.cell,
-            self.basis,
-            self.positions,
-            self.supercell_matrix,
-            self.eigenvectors,
-            self.procar.kpoints,
-            phase=False,
-        )
-        w = self.unfolder.get_weights()
-        return w # , self.unfolder
-
-    def plot(
-            self,
-            efermi=5.46,
-            ispin=None,
-            ylim=(-5, 10),
-            ktick=[0, 41, 83, 125, 200],
-            kname=["$\Gamma$", "X", "M", "R", "$\Gamma$"],
-            show_band=True,
-            shift_efermi=True,
-            width=4.0,
-            color="blue",
-            axis=None,
-            savetab=None,
-    ):
-        iispin = 0
-        if ispin is not None:
-            iispin = ispin - 1
-        xlist = [list(range(self.procar.kpointsCount))]
-        uf = self.unfold(ispin=ispin)
-        if savetab is not False:
-            nk, nb = uf.shape
-            tab = np.zeros((nb, nk * 2), dtype=float)
-            tab[:, ::2] = self.procar.bands[iispin].T
-            tab[:, 1::2] = uf.T
-            np.savetxt(
-                savetab,
-                tab,
-                delimiter=",",
-                fmt="%10.4f",
-                header=
-                "# nkpoints: %s   nbands:%s \n#E(k1) w(k1) E(k2) w(k2) E(k3) w(k3)..."
-                % (nk, nb),
-            )
-        axes = plot_band_weight(
-            xlist * self.procar.bandsCount,
-            self.procar.bands[iispin].T,
-            np.abs(uf.T),
-            xticks=[kname, ktick],
-            efermi=efermi,
-            shift_efermi=shift_efermi,
-            fatness=width,
-            color=color,
-            axis=axis,
-        )
-        axes.set_ylim(ylim)
-        axes.set_xlim(0, self.procar.kpointsCount - 1)
-        if shift_efermi:
-            shift = -efermi
-        else:
-            shift = 0.0
-        if show_band:
-            for i in range(self.procar.bandsCount):
-                axes.plot(
-                    self.procar.bands[iispin, :, i] + shift,
-                    color="gray",
-                    linewidth=1,
-                    alpha=0.3,
-                )
-        return axes
+import numpy as np
+from ase.io import read
+from .unfolder import Unfolder
+import matplotlib.pyplot as plt
+from .fatband import plot_band_weight
+from ...io import ProcarParser
+
+
+class ProcarUnfolder(object):
+    def __init__(self, procar, poscar, supercell_matrix, ispin=None):
+        self.fname = procar
+        self.supercell_matrix = supercell_matrix
+        self._parse_procar(ispin=ispin)
+        self.atoms = read(poscar)
+        self.basis = []
+        self.positions = []
+
+    def _parse_procar(self, ispin=None):
+        self.procar = ProcarParser()
+        self.procar.readFile2(self.fname, phase=True, ispin=ispin)
+
+        
+
+    def _prepare_unfold_basis(self, ispin=None):
+        # basis, which are the name of the bands e.g. 'Ti|dxy|0'
+        # self.eigenvectors = np.zeros(
+        #    (self.procar.kpointsCount, self.procar.bandsCount,
+        #     (self.procar.orbitalCount - 1) * (self.procar.ionsCount - 1) *
+        #     self.procar.ispin), dtype='complex')
+        if ispin is None:
+            iispin = 0
+        else:
+            ispin -= 1
+        self.eigenvectors = np.reshape(
+            self.procar.carray[:, :, ispin, :, :],
+            (
+                self.procar.kpointsCount,
+                self.procar.bandsCount,
+                self.procar.ionsCount * self.procar.orbitalCount,
+            ),
+        )
+        norm = np.linalg.norm(self.eigenvectors, ord=2, axis=2)
+        self.eigenvectors /= norm[:, :, None]
+
+        for iatom, chem in enumerate(self.atoms.get_chemical_symbols()):
+            for iorb, orb in enumerate(self.procar.orbitalName):
+                for spin in range(self.procar.nspin):
+                    # todo: what about spin?
+                    self.basis.append("%s|%s|%s" % (None, orb, spin))
+                    self.positions.append(
+                        self.atoms.get_scaled_positions()[iatom])
+            
+            
+            
+    def unfold(self, ispin=None):
+        # spd: spd[kpoint][band][ispin][atom][orbital]
+        # bands[kpt][iband]
+        # to unfold,
+        # unfolder:
+        # def __init__(self, cell, basis, positions , supercell_matrix, eigenvectors, qpoints, tol_r=0.1, compare=None):
+        self._prepare_unfold_basis(ispin=ispin)
+        self.unfolder = Unfolder(
+            self.atoms.cell,
+            self.basis,
+            self.positions,
+            self.supercell_matrix,
+            self.eigenvectors,
+            self.procar.kpoints,
+            phase=False,
+        )
+        w = self.unfolder.get_weights()
+        return w # , self.unfolder
+
+    def plot(
+            self,
+            efermi=5.46,
+            ispin=None,
+            ylim=(-5, 10),
+            ktick=[0, 41, 83, 125, 200],
+            kname=["$\Gamma$", "X", "M", "R", "$\Gamma$"],
+            show_band=True,
+            shift_efermi=True,
+            width=4.0,
+            color="blue",
+            axis=None,
+            savetab=None,
+    ):
+        iispin = 0
+        if ispin is not None:
+            iispin = ispin - 1
+        xlist = [list(range(self.procar.kpointsCount))]
+        uf = self.unfold(ispin=ispin)
+        if savetab is not False:
+            nk, nb = uf.shape
+            tab = np.zeros((nb, nk * 2), dtype=float)
+            tab[:, ::2] = self.procar.bands[iispin].T
+            tab[:, 1::2] = uf.T
+            np.savetxt(
+                savetab,
+                tab,
+                delimiter=",",
+                fmt="%10.4f",
+                header=
+                "# nkpoints: %s   nbands:%s \n#E(k1) w(k1) E(k2) w(k2) E(k3) w(k3)..."
+                % (nk, nb),
+            )
+        axes = plot_band_weight(
+            xlist * self.procar.bandsCount,
+            self.procar.bands[iispin].T,
+            np.abs(uf.T),
+            xticks=[kname, ktick],
+            efermi=efermi,
+            shift_efermi=shift_efermi,
+            fatness=width,
+            color=color,
+            axis=axis,
+        )
+        axes.set_ylim(ylim)
+        axes.set_xlim(0, self.procar.kpointsCount - 1)
+        if shift_efermi:
+            shift = -efermi
+        else:
+            shift = 0.0
+        if show_band:
+            for i in range(self.procar.bandsCount):
+                axes.plot(
+                    self.procar.bands[iispin, :, i] + shift,
+                    color="gray",
+                    linewidth=1,
+                    alpha=0.3,
+                )
+        return axes
```

### Comparing `PyProcar-5.6.6/pyprocar/procarunfold/unfolder.py` & `PyProcar-6.0.0/pyprocar/core/procarunfold/unfolder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,142 @@
-"""
-Phonon unfolding: Reciprocal space method. The method is described in
-P. B. Allen et al. Phys Rev B 87, 085322 (2013).
-This method should be also applicable to other bloch waves on discrete grid, eg. electrons wave function in wannier basis set, magnons, etc. Now only phonon istested.
-"""
-from ase.build import make_supercell
-from ase.atoms import Atoms
-import numpy as np
-
-
-class Unfolder:
-    """ phonon unfolding class"""
-    def __init__(
-            self,
-            cell,
-            basis,
-            positions,
-            supercell_matrix,
-            eigenvectors,
-            qpoints,
-            tol_r=0.1,
-            compare=None,
-            phase=True,
-    ):
-        """
-        Params:
-        ===================
-        cell: cell matrix. [a,b,c]
-        basis: name of the basis. It's used to decide if two basis can
-        be identical by translation. eg. for phonons, the basis can be
-        ['x','y','z']*natoms, for electrons, it can be
-        ['Ni|dxy','Mn|dxy'] if the two dxy are seen as different, or
-        ['dxy','dxy'] if they are seen as the same.
-
-        positions: positions(->basis).
-        supercell matrix: The matrix that convert the primitive cell
-        to supercell.
-
-        eigenvectors: The phonon eigenvectors. format np.array()
-        index=[ikpts, ifreq, 3*iatoms+j]. j=0..2
-
-        qpoints: list of q-points.
-        tol_r: tolerance. If abs(a-b) <r, they are seen as the same atom.
-        """
-        self._cell = cell
-        self._basis = basis
-        self._positions = positions
-        self._scmat = supercell_matrix
-        self._evecs = eigenvectors
-        self._qpts = qpoints
-        self._tol_r = tol_r
-        self._trans_rs = None
-        self._trans_indices = None
-        self._make_translate_maps()
-        self._phase = phase
-        return
-
-    def _translate(self, evec, r):
-        """
-        T(r) psi: r is integer numbers of primitive cell lattice matrix.
-        Params:
-        =================
-        evec: an eigen vector of supercell
-        r: The translate vector
-        
-        Returns:
-        ================
-         tevec: translated vector.
-        """
-        pass
-
-    def _make_translate_maps(self):
-        """
-        find the mapping between supercell and translated cell.
-        Returns:
-        ===============
-        A N * nbasis array.
-        index[i] is the mapping from supercell to translated supercell so that
-        T(r_i) psi = psi[indices[i]].
-        
-        TODO: vacancies/add_atoms not supported. How to do it? For
-        vacancies, a ghost atom can be added. For add_atom, maybe we
-        can just ignore them? Will it change the energy spectrum?
-
-        """  
-        a1 = Atoms(symbols="H", positions=[(0, 0, 0)], cell=[1, 1, 1])
-        sc = make_supercell(a1, self._scmat)
-        rs = sc.get_scaled_positions()
-
-        positions = self._positions
-        indices = np.zeros([len(rs), len(positions)], dtype="int32")
-        for i, ri in enumerate(rs):
-            inds = []
-            Tpositions = positions + np.array(ri)
-            close_to_int = lambda x: np.all(
-                np.abs(x - np.round(x)) < self._tol_r)
-            for i_basis, pos in enumerate(positions):
-                for j_basis, Tpos in enumerate(Tpositions):
-                    dpos = Tpos - pos
-                    if close_to_int(dpos) and (
-                            self._basis[i_basis] == self._basis[j_basis]):
-                        # indices[i, j_atom * self._ndim:j_atom * self._ndim + self._ndim] = np.arange(i_atom * self._ndim, i_atom * self._ndim + self._ndim)
-                        indices[i, j_basis] = i_basis
-
-        self._trans_rs = rs
-        self._trans_indices = indices
-        # print(indices)
-
-    def get_weight(self, evec, qpt, G=None):
-        """
-        get the weight of a mode which has the wave vector of qpt and
-        eigenvector of evec.
-
-        W= sum_1^N < evec| T(r_i)exp(-I (K+G) * r_i| evec>, here
-        G=0. T(r_i)exp(-I K r_i)| evec> = evec[indices[i]]
-
-        """
-        if G is None:
-            G = np.zeros_like(qpt)
-        weight = 0j
-        N = len(self._trans_rs)
-        for r_i, ind in zip(self._trans_rs, self._trans_indices):
-            if self._phase:
-                weight += (np.vdot(evec, evec[ind]) *
-                           np.exp(1j * 2 * np.pi * np.dot(qpt + G, r_i)) / N)
-            else:
-                weight += (np.vdot(evec, evec[ind]) / N *
-                           np.exp(-1j * 2 * np.pi * np.dot(G, r_i)))
-        return weight.real
-
-    def get_weights(self):
-        """
-        Get the weight for all the modes.
-        """
-        nqpts, nfreqs = self._evecs.shape[0], self._evecs.shape[1]
-        weights = np.zeros([nqpts, nfreqs])
-        for iqpt in range(nqpts):
-            for ifreq in range(nfreqs):
-                weights[iqpt, ifreq] = self.get_weight(
-                    self._evecs[iqpt, ifreq, :], self._qpts[iqpt])
-
-        self._weights = weights
-        return self._weights
+"""
+Phonon unfolding: Reciprocal space method. The method is described in
+P. B. Allen et al. Phys Rev B 87, 085322 (2013).
+This method should be also applicable to other bloch waves on discrete grid, eg. electrons wave function in wannier basis set, magnons, etc. Now only phonon istested.
+"""
+from ase.build import make_supercell
+from ase.atoms import Atoms
+import numpy as np
+
+
+class Unfolder:
+    """ phonon unfolding class"""
+    def __init__(
+            self,
+            cell,
+            basis,
+            positions,
+            supercell_matrix,
+            eigenvectors,
+            qpoints,
+            tol_r=0.1,
+            compare=None,
+            phase=True,
+    ):
+        """
+        Params:
+        ===================
+        cell: cell matrix. [a,b,c]
+        basis: name of the basis. It's used to decide if two basis can
+        be identical by translation. eg. for phonons, the basis can be
+        ['x','y','z']*natoms, for electrons, it can be
+        ['Ni|dxy','Mn|dxy'] if the two dxy are seen as different, or
+        ['dxy','dxy'] if they are seen as the same.
+
+        positions: positions(->basis).
+        supercell matrix: The matrix that convert the primitive cell
+        to supercell.
+
+        eigenvectors: The phonon eigenvectors. format np.array()
+        index=[ikpts, ifreq, 3*iatoms+j]. j=0..2
+
+        qpoints: list of q-points.
+        tol_r: tolerance. If abs(a-b) <r, they are seen as the same atom.
+        """
+        self._cell = cell
+        self._basis = basis
+        self._positions = positions
+        self._scmat = supercell_matrix
+        self._evecs = eigenvectors
+        self._qpts = qpoints
+        self._tol_r = tol_r
+        self._trans_rs = None
+        self._trans_indices = None
+        self._make_translate_maps()
+        self._phase = phase
+        return
+
+    def _translate(self, evec, r):
+        """
+        T(r) psi: r is integer numbers of primitive cell lattice matrix.
+        Params:
+        =================
+        evec: an eigen vector of supercell
+        r: The translate vector
+        
+        Returns:
+        ================
+         tevec: translated vector.
+        """
+        pass
+
+    def _make_translate_maps(self):
+        """
+        find the mapping between supercell and translated cell.
+        Returns:
+        ===============
+        A N * nbasis array.
+        index[i] is the mapping from supercell to translated supercell so that
+        T(r_i) psi = psi[indices[i]].
+        
+        TODO: vacancies/add_atoms not supported. How to do it? For
+        vacancies, a ghost atom can be added. For add_atom, maybe we
+        can just ignore them? Will it change the energy spectrum?
+
+        """  
+        a1 = Atoms(symbols="H", positions=[(0, 0, 0)], cell=[1, 1, 1])
+        sc = make_supercell(a1, self._scmat)
+        rs = sc.get_scaled_positions()
+
+        positions = self._positions
+        indices = np.zeros([len(rs), len(positions)], dtype="int32")
+        for i, ri in enumerate(rs):
+            inds = []
+            Tpositions = positions + np.array(ri)
+            close_to_int = lambda x: np.all(
+                np.abs(x - np.round(x)) < self._tol_r)
+            for i_basis, pos in enumerate(positions):
+                for j_basis, Tpos in enumerate(Tpositions):
+                    dpos = Tpos - pos
+                    if close_to_int(dpos) and (
+                            self._basis[i_basis] == self._basis[j_basis]):
+                        # indices[i, j_atom * self._ndim:j_atom * self._ndim + self._ndim] = np.arange(i_atom * self._ndim, i_atom * self._ndim + self._ndim)
+                        indices[i, j_basis] = i_basis
+
+        self._trans_rs = rs
+        self._trans_indices = indices
+        # print(indices)
+
+    def get_weight(self, evec, qpt, G=None):
+        """
+        get the weight of a mode which has the wave vector of qpt and
+        eigenvector of evec.
+
+        W= sum_1^N < evec| T(r_i)exp(-I (K+G) * r_i| evec>, here
+        G=0. T(r_i)exp(-I K r_i)| evec> = evec[indices[i]]
+        """
+        if G is None:
+            G = np.zeros_like(qpt)
+        weight = 0j
+        N = len(self._trans_rs)
+        for r_i, ind in zip(self._trans_rs, self._trans_indices):
+            if self._phase:
+                weight += (np.vdot(evec, evec[ind]) *
+                           np.exp(1j * 2 * np.pi * np.dot(qpt + G, r_i)) / N)
+            else:
+                weight += (np.vdot(evec, evec[ind]) / N *
+                           np.exp(-1j * 2 * np.pi * np.dot(G, r_i)))
+        return weight.real
+
+    def get_weights(self):
+        """
+        Get the weight for all the modes.
+        """
+        nqpts, nfreqs = self._evecs.shape[0], self._evecs.shape[1]
+        weights = np.zeros([nqpts, nfreqs])
+        for iqpt in range(nqpts):
+            for ifreq in range(nfreqs):
+                weights[iqpt, ifreq] = self.get_weight(
+                    self._evecs[iqpt, ifreq, :], self._qpts[iqpt])
+
+        self._weights = weights
+        return self._weights
```

### Comparing `PyProcar-5.6.6/pyprocar/scriptCat.py` & `PyProcar-6.0.0/pyprocar/scripts/scriptCat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,288 @@
-import os
-import re
-import glob
-
-import numpy as np
-
-from .splash import welcome
-from .utilsprocar import UtilsProcar
-from .abinitparser import AbinitParser
-
-
-def cat(
-    inFiles=None,
-    outFile="PROCAR_merged",
-    gz=False,
-    mergeparallel=False,
-    fixformat=False,
-    nspin=1,
-    abinit_output=None,
-):
-    """
-    This module concatenates multiple PROCARs.
-    If a list of input PROCAR files is not provided it will merge all the PROCAR_*
-    files in the directory.
-    set mergeparallel = True for merging PROCARs generated from
-    parallel Abinit calculations. Set fixformat = True to fix formatting issues
-    in the Abinit PROCAR file.
-    To detect if the calculation is spin-colinear it checks for the nsppol flag
-    in the Abinit output file as set in abinit_output. If not present, set nspin.
-    """
-    welcome()
-
-    # reading in all PROCAR_* files and putting it into a list if not provided.
-    if inFiles is None:
-        inFiles = sorted(glob.glob("PROCAR_*"))
-    else:
-        pass
-
-    print("Concatenating...")
-    print("Input         : ", inFiles)  # ', '.join(inFiles)
-    print("Output        : ", outFile)
-
-    if mergeparallel == False and fixformat == False:
-
-        if gz == True:
-            print("out compressed: true")
-
-        if gz == True and outFile[-3:] != ".gz":
-            outFile += ".gz"
-            print(".gz extension appended to the outfile")
-
-        handler = UtilsProcar()
-        handler.MergeFiles(inFiles, outFile, gzipOut=gz)
-        return
-
-    elif mergeparallel == True and fixformat == False:
-        _mergeparallel(inFiles, outFile, nspin, abinit_output)
-
-    elif mergeparallel == True and fixformat == True:
-        outFile_temp = "outFile.tmp"
-        _mergeparallel(inFiles, outFile_temp, nspin, abinit_output)
-        _fixformat(outFile_temp, outFile)
-        if os.path.exists(outFile_temp):
-            os.remove(outFile_temp)
-
-    elif mergeparallel == False and fixformat == True:
-        print("Using fixformat = True without mergeparallel. Input a single PROCAR.")
-        _fixformat(inFiles, outFile)
-
-
-def _mergeparallel(inputfiles=None, outputfile=None, nspin=1, abinit_output=None):
-    """ This merges Procar files seperated between k-point ranges.
-    Happens with parallel Abinit runs.
-    """
-    print("Merging parallel files...")
-    filenames = sorted(inputfiles)
-
-    # creating an instance of the AbinitParser class
-    if abinit_output:
-        abinitparserobject = AbinitParser(abinit_output=abinit_output)
-        nspin = int(abinitparserobject.nspin)
-    else:
-        nspin = int(nspin)
-
-    if nspin != 2:
-        with open(outputfile, "w") as outfile:
-            for fname in filenames:
-                with open(fname) as infile:
-                    for line in infile:
-                        outfile.write(line)
-
-    elif nspin == 2:
-        # for spin polarized calculations the spin down segments are saved in the
-        # second half of the PROCAR's but in reverse k-point order. So we have to
-        # fix the order and merge the second half of the PROCAR's.
-        spinup_list = filenames[: int(len(filenames) / 2)]
-        spindown_list = filenames[int(len(filenames) / 2) :]
-
-        # reading the second line of the header to set as the separating line
-        # in the colinear spin PROCAR.
-        fp = open(spinup_list[0], "r")
-        header1 = fp.readline()
-        header2 = fp.readline()
-        fp.close()
-
-        # second half of PROCAR files in reverse order.
-        spindown_list.reverse()
-
-        # Writing new PROCAR with first spin up, header2 and then
-        # spin down (reversed).
-        with open(outputfile, "w") as outfile:
-            for spinupfile in spinup_list:
-                with open(spinupfile) as infile:
-                    for line in infile:
-                        outfile.write(line)
-            outfile.write("\n")
-            outfile.write(header2)
-            outfile.write("\n")
-            for spindownfile in spindown_list:
-                with open(spindownfile) as infile:
-                    for line in infile:
-                        outfile.write(line)
-
-
-def _fixformat(inputfile=None, outputfile=None):
-
-    """Fixes the formatting of Abinit's Procar
-    when the tot projection is not summed and spin directions
-    not seperated.
-    """
-    print("Fixing formatting errors...")
-    # removing existing temporary fixed file
-    if os.path.exists(outputfile):
-        os.remove(outputfile)
-
-    ####### Fixing the parallel PROCARs from Abinit ##########
-
-    rf = open(inputfile, "r")
-    data = rf.read()
-    rf.close()
-
-    # reading headers
-    rffl = open(inputfile, "r")
-    first_line = rffl.readline()
-    rffl.close()
-
-    # header
-    header = re.findall("#\sof\s.*", data)[0]
-
-    # writing to PROCAR
-    fp = open(outputfile, "a")
-    fp.write(first_line)
-    fp.write(str(header) + "\n\n")
-
-    # get all the k-point line headers
-    kpoints_raw = re.findall("k-point\s*[0-9]\s*:*.*", data)
-
-    for kpoint_counter in range(len(kpoints_raw)):
-
-        if kpoint_counter == (len(kpoints_raw) - 1):
-            # get bands of last k point
-            bands_raw = re.findall(
-                kpoints_raw[kpoint_counter] + "([a-z0-9\s\n.+#-]*)", data
-            )[0]
-
-        else:
-            # get bands between k point n and n+1
-            bands_raw = re.findall(
-                kpoints_raw[kpoint_counter]
-                + "([a-z0-9\s\n.+#-]*)"
-                + kpoints_raw[kpoint_counter + 1],
-                data,
-            )[0]
-
-        # get the bands headers for a certain k point
-        raw_bands = re.findall("band\s*[0-9]*.*", bands_raw)
-
-        # writing k point header to file
-        fp.write(kpoints_raw[kpoint_counter] + "\n\n")
-
-        for band_counter in range(len(raw_bands)):
-
-            if band_counter == (len(raw_bands) - 1):
-                # the last band
-                single_band = re.findall(
-                    raw_bands[band_counter] + "([a-z0-9.+\s\n-]*)", bands_raw
-                )[0]
-
-            else:
-                # get a single band
-                single_band = re.findall(
-                    raw_bands[band_counter]
-                    + "([a-z0-9.+\s\n-]*)"
-                    + raw_bands[band_counter + 1],
-                    bands_raw,
-                )[0]
-
-            # get the column headers for ion, orbitals and total
-            column_header = re.findall("ion\s.*tot", single_band)[0]
-
-            # get number of ions using PROCAR file
-            nion_raw = re.findall("#\s*of\s*ions:\s*[0-9]*", data)[0]
-            nion = int(nion_raw.split(" ")[-1])
-
-            # the first column of the band. Same as ions
-            first_column = []
-            for x in single_band.split("\n"):
-                if x != "":
-                    if x != " ":
-                        if x.split()[0] != "ion":
-                            first_column.append(x.split()[0])
-
-            # number of spin orientations
-            norient = int(len(first_column) / nion)
-
-            # calculate the number of orbital headers (s,p,d etc.)
-            for x in single_band.split("\n"):
-                if x != "":
-                    if x != " ":
-                        if x.split()[0] == "ion":
-                            norbital = len(x.split()) - 2
-
-            # array to store a single band data as seperate lines
-            single_band_lines = []
-            for x in single_band.split("\n"):
-                if x != "":
-                    if x != " ":
-                        if x.split()[0] != "ion":
-                            single_band_lines.append(x)
-
-            # create empty array to store data (the orbitals + tot)
-            bands_orb = np.zeros(shape=(norient, nion, norbital + 1))
-
-            # enter data into bands_orb
-            iion = 0
-            iorient = 0
-            for x in single_band.split("\n"):
-                if x != "" and x != " " and x.split()[0] != "ion":
-                    iline = x.split()
-                    if iion > 1:
-                        iion = 0
-                        iorient += 1
-                    for iorb in range(0, norbital + 1):
-                        bands_orb[iorient, iion, iorb] = float(iline[iorb + 1])
-                    iion += 1
-
-            # create an array to store the total values
-            tot = np.zeros(shape=(norient, norbital + 1))
-
-            # entering data into tot array
-            for iorient in range(norient):
-                tot[iorient, :] = np.sum(bands_orb[iorient, :, :], axis=0)
-
-            # writing data
-            fp.write(raw_bands[band_counter] + "\n\n")
-            fp.write(column_header + "\n")
-
-            band_iterator = 0
-            total_count = 0
-            for orientations_count in range(norient):
-                for ions_count in range(nion):
-                    fp.write(single_band_lines[band_iterator] + "\n")
-                    band_iterator += 1
-                fp.write("tot  " + " ".join(map(str, tot[total_count, :])) + "\n\n")
-                total_count += 1
-    fp.close()
+__author__ = "Pedram Tavadze and Logan Lang"
+__maintainer__ = "Pedram Tavadze and Logan Lang"
+__email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
+__date__ = "March 31, 2020"
+
+
+import os
+from typing import List
+import re
+import glob
+
+import numpy as np
+
+from ..utils import welcome
+from ..utils import UtilsProcar
+from ..io import AbinitParser
+
+def cat(
+    inFiles:List[str]=None,
+    outFile:str="PROCAR_merged",
+    gz:bool=False,
+    mergeparallel:bool=False,
+    fixformat:bool=False,
+    nspin:int=1,
+    abinit_output:str=None,
+    ):
+    """
+    This module concatenates multiple PROCARs.
+    If a list of input PROCAR files is not provided it will merge all the PROCAR_*
+    files in the directory.
+
+    Parameters
+    ----------
+    inFiles : List[str], optional
+        A list of PROCAR files to concatenate, by default None
+    outFile : str, optional
+        String for the output, by default "PROCAR_merged"
+    gz : bool, optional
+        Boolean if output should be compressed to .gz file, by default False
+    mergeparallel : bool, optional
+        Boolean for merging PROCARs generated 
+        from parallel Abinit calculations., by default False
+    fixformat : bool, optional
+        Boolean to fix formatting issues
+        in the Abinit PROCAR file., by default False
+    nspin : int, optional
+        To detect if the calculation is spin-colinear it checks for the nsppol flag
+        in the Abinit output file as set in abinit_output. If not present, set nspin., by default 1
+    abinit_output : str, optional
+        The abinit output file, by default None
+    """
+
+    welcome()
+
+    # reading in all PROCAR_* files and putting it into a list if not provided.
+    if inFiles is None:
+        inFiles = sorted(glob.glob("PROCAR_*"))
+    else:
+        pass
+
+    print("Concatenating...")
+    print("Input         : ", inFiles)  # ', '.join(inFiles)
+    print("Output        : ", outFile)
+
+    if mergeparallel == False and fixformat == False:
+
+        if gz == True:
+            print("out compressed: true")
+
+        if gz == True and outFile[-3:] != ".gz":
+            outFile += ".gz"
+            print(".gz extension appended to the outfile")
+
+        handler = UtilsProcar()
+        handler.MergeFiles(inFiles, outFile, gzipOut=gz)
+        return
+
+    elif mergeparallel == True and fixformat == False:
+        _mergeparallel(inFiles, outFile, nspin, abinit_output)
+
+    elif mergeparallel == True and fixformat == True:
+        outFile_temp = "outFile.tmp"
+        _mergeparallel(inFiles, outFile_temp, nspin, abinit_output)
+        _fixformat(outFile_temp, outFile)
+        if os.path.exists(outFile_temp):
+            os.remove(outFile_temp)
+
+    elif mergeparallel == False and fixformat == True:
+        print("Using fixformat = True without mergeparallel. Input a single PROCAR.")
+        _fixformat(inFiles, outFile)
+
+
+def _mergeparallel(inputfiles=None, outputfile=None, nspin=1, abinit_output=None):
+    """ This merges Procar files seperated between k-point ranges.
+    Happens with parallel Abinit runs.
+    """
+    print("Merging parallel files...")
+    filenames = sorted(inputfiles)
+
+    # creating an instance of the AbinitParser class
+    if abinit_output:
+        abinitparserobject = AbinitParser(abinit_output=abinit_output)
+        nspin = int(abinitparserobject.nspin)
+    else:
+        nspin = int(nspin)
+
+    if nspin != 2:
+        with open(outputfile, "w") as outfile:
+            for fname in filenames:
+                with open(fname) as infile:
+                    for line in infile:
+                        outfile.write(line)
+
+    elif nspin == 2:
+        # for spin polarized calculations the spin down segments are saved in the
+        # second half of the PROCAR's but in reverse k-point order. So we have to
+        # fix the order and merge the second half of the PROCAR's.
+        spinup_list = filenames[: int(len(filenames) / 2)]
+        spindown_list = filenames[int(len(filenames) / 2) :]
+
+        # reading the second line of the header to set as the separating line
+        # in the colinear spin PROCAR.
+        fp = open(spinup_list[0], "r")
+        header1 = fp.readline()
+        header2 = fp.readline()
+        fp.close()
+
+        # second half of PROCAR files in reverse order.
+        spindown_list.reverse()
+
+        # Writing new PROCAR with first spin up, header2 and then
+        # spin down (reversed).
+        with open(outputfile, "w") as outfile:
+            for spinupfile in spinup_list:
+                with open(spinupfile) as infile:
+                    for line in infile:
+                        outfile.write(line)
+            outfile.write("\n")
+            outfile.write(header2)
+            outfile.write("\n")
+            for spindownfile in spindown_list:
+                with open(spindownfile) as infile:
+                    for line in infile:
+                        outfile.write(line)
+
+
+def _fixformat(inputfile=None, outputfile=None):
+
+    """Fixes the formatting of Abinit's Procar
+    when the tot projection is not summed and spin directions
+    not seperated.
+    """
+    print("Fixing formatting errors...")
+    # removing existing temporary fixed file
+    if os.path.exists(outputfile):
+        os.remove(outputfile)
+
+    ####### Fixing the parallel PROCARs from Abinit ##########
+
+    rf = open(inputfile, "r")
+    data = rf.read()
+    rf.close()
+
+    # reading headers
+    rffl = open(inputfile, "r")
+    first_line = rffl.readline()
+    rffl.close()
+
+    # header
+    header = re.findall("#\sof\s.*", data)[0]
+
+    # writing to PROCAR
+    fp = open(outputfile, "a")
+    fp.write(first_line)
+    fp.write(str(header) + "\n\n")
+
+    # get all the k-point line headers
+    kpoints_raw = re.findall("k-point\s*[0-9]\s*:*.*", data)
+
+    for kpoint_counter in range(len(kpoints_raw)):
+
+        if kpoint_counter == (len(kpoints_raw) - 1):
+            # get bands of last k point
+            bands_raw = re.findall(
+                kpoints_raw[kpoint_counter] + "([a-z0-9\s\n.+#-]*)", data
+            )[0]
+
+        else:
+            # get bands between k point n and n+1
+            bands_raw = re.findall(
+                kpoints_raw[kpoint_counter]
+                + "([a-z0-9\s\n.+#-]*)"
+                + kpoints_raw[kpoint_counter + 1],
+                data,
+            )[0]
+
+        # get the bands headers for a certain k point
+        raw_bands = re.findall("band\s*[0-9]*.*", bands_raw)
+
+        # writing k point header to file
+        fp.write(kpoints_raw[kpoint_counter] + "\n\n")
+
+        for band_counter in range(len(raw_bands)):
+
+            if band_counter == (len(raw_bands) - 1):
+                # the last band
+                single_band = re.findall(
+                    raw_bands[band_counter] + "([a-z0-9.+\s\n-]*)", bands_raw
+                )[0]
+
+            else:
+                # get a single band
+                single_band = re.findall(
+                    raw_bands[band_counter]
+                    + "([a-z0-9.+\s\n-]*)"
+                    + raw_bands[band_counter + 1],
+                    bands_raw,
+                )[0]
+
+            # get the column headers for ion, orbitals and total
+            column_header = re.findall("ion\s.*tot", single_band)[0]
+
+            # get number of ions using PROCAR file
+            nion_raw = re.findall("#\s*of\s*ions:\s*[0-9]*", data)[0]
+            nion = int(nion_raw.split(" ")[-1])
+
+            # the first column of the band. Same as ions
+            first_column = []
+            for x in single_band.split("\n"):
+                if x != "":
+                    if x != " ":
+                        if x.split()[0] != "ion":
+                            first_column.append(x.split()[0])
+
+            # number of spin orientations
+            norient = int(len(first_column) / nion)
+
+            # calculate the number of orbital headers (s,p,d etc.)
+            for x in single_band.split("\n"):
+                if x != "":
+                    if x != " ":
+                        if x.split()[0] == "ion":
+                            norbital = len(x.split()) - 2
+
+            # array to store a single band data as seperate lines
+            single_band_lines = []
+            for x in single_band.split("\n"):
+                if x != "":
+                    if x != " ":
+                        if x.split()[0] != "ion":
+                            single_band_lines.append(x)
+
+            # create empty array to store data (the orbitals + tot)
+            bands_orb = np.zeros(shape=(norient, nion, norbital + 1))
+
+            # enter data into bands_orb
+            iion = 0
+            iorient = 0
+            for x in single_band.split("\n"):
+                if x != "" and x != " " and x.split()[0] != "ion":
+                    iline = x.split()
+                    if iion > 1:
+                        iion = 0
+                        iorient += 1
+                    for iorb in range(0, norbital + 1):
+                        bands_orb[iorient, iion, iorb] = float(iline[iorb + 1])
+                    iion += 1
+
+            # create an array to store the total values
+            tot = np.zeros(shape=(norient, norbital + 1))
+
+            # entering data into tot array
+            for iorient in range(norient):
+                tot[iorient, :] = np.sum(bands_orb[iorient, :, :], axis=0)
+
+            # writing data
+            fp.write(raw_bands[band_counter] + "\n\n")
+            fp.write(column_header + "\n")
+
+            band_iterator = 0
+            total_count = 0
+            for orientations_count in range(norient):
+                for ions_count in range(nion):
+                    fp.write(single_band_lines[band_iterator] + "\n")
+                    band_iterator += 1
+                fp.write("tot  " + " ".join(map(str, tot[total_count, :])) + "\n\n")
+                total_count += 1
+    fp.close()
```

### Comparing `PyProcar-5.6.6/pyprocar/scriptFermi3D.py` & `PyProcar-6.0.0/pyprocar/scripts/scriptFermi3D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,848 +1,755 @@
-# -*- coding: utf-8 -*-
-
-import numpy as np
-import pyvista
-
-from matplotlib import colors as mpcolors
-from matplotlib import cm
-from .core.surface import boolean_add
-from .fermisurface3d import FermiSurface3D
-from .splash import welcome
-from .utilsprocar import UtilsProcar
-from .procarparser import ProcarParser
-from .procarselect import ProcarSelect
-from .bxsfparser import BxsfParser
-from .frmsfparser import FrmsfParser
-from .qeparser import QEFermiParser
-from .lobsterparser import LobsterFermiParser
-from .abinitparser import AbinitParser
-
-
-
-import vtk
-from pyvista.utilities import NORMALS, generate_plane, get_array, try_callback
-def fermi3D(
-    procar="PROCAR",
-    outcar="OUTCAR",
-    infile="in.bxsf",
-    abinit_output=None,
-    fermi=None,
-    bands=None,
-    interpolation_factor=1,
-    mode="plain",
-    supercell=[1, 1, 1],
-    extended_zone_directions = None,
-    colors=None,
-    background_color="white",
-    save_colors=False,
-    cmap="jet",
-    atoms=None,
-    orbitals=None,
-    fermi_velocity = False,
-    fermi_velocity_vector = False,
-    effective_mass = False,
-    spin=None,
-    spin_texture=False,
-    arrow_color=None,
-    arrow_size=0.015,
-    only_spin=False,
-    fermi_shift=0,
-    projection_accuracy="normal",
-    code="vasp",
-    vmin=0,
-    vmax=1,
-    savegif=None,
-    savemp4=None,
-    save3d=None,
-    save_meshio= False,
-    perspective=True,
-    save2d=False,
-    show_curvature = False,
-    curvature_type = 'mean',
-    show_slice = False,
-    slice_normal = (1,0,0),
-    slice_origin = (0,0,0),
-    show_cross_section_area= False,
-    iso_slider = False,
-    iso_range = 2,
-    iso_surfaces = 10,
-    camera_pos=[1, 1, 1],
-    widget=False,
-    show=True,
-    repair=True,
-):
-    """
-    Parameters
-    ----------
-    procar : str, optional (default ``'PROCAR'``)
-        Path to the PROCAR file of the simulation
-        e.g. ``procar='~/MgB2/fermi/PROCAR'``
-    outcar : str, optional (default ``'OUTCAR'``)
-        Path to the OUTCAR file of the simulation
-        e.g. ``outcar='~/MgB2/fermi/OUTCAR'``
-    abinit_output : str, optional (default ``None``)
-        Path to the Abinit output file
-        e.g. ``outcar='~/MgB2/abinit.out'``
-    infile : str, optional (default ``infile = in.bxsf'``)
-        This is the path in the input bxsf file
-        e.g. ``infile = ni_fs.bxsf'``
-    fermi : float, optional (default ``None``)
-        Fermi energy at which the fermi surface is created. In other
-        words fermi is the isovalue at which the fermi surface is
-        created. If not defined it is read from the OUTCAR file.
-        e.g. ``fermi=-5.49``
-    bands : list int, optional
-        Which bands are going to be plotted in the fermi surface. The
-        numbering is based on vasp outputs. If nothing is selected,
-        this function will iterate over all the bands and plots the
-        ones that cross fermi.
-        e.g. ``bands=[14, 15, 16, 17]``
-    interpolation_factor : int, optional
-        The kpoints grid will increase by this factor and interpolated
-        at the new points using Fourier interpolation.
-        e.g. If the kgrid is 5x5x5, ``interpolation_factor=4`` will
-        lead to a kgrid of 20x20x20
-    mode : str, optional (default ``mode='plain'``)
-        Defines If the fermi surface will have any projection using
-        colormaps or is a plotted with a uniform plain color.
-        e.g. ``mode='plain'``, ``mode='parametric'``
-    supercell : list int, optional (default ``[1, 1, 1]``)
-        If one wants plot more than the 1st brillouin zone, this
-        parameter can be used.
-        e.g. ``supercell=[2, 2, 2]``
-    extended_zone_directions : list of list of size 3, optional (default ``None``)
-        If one wants plot more than  brillouin zones in a particular direection, this
-        parameter can be used.
-        e.g. ``extended_zone_directions=[[1,0,0],[0,1,0],[0,0,1]]``
-    colors : list str, optional
-        List of colors for each band. This argument does not work when
-        a 3d file is saved. The colors for when ``save3d`` is used, we
-        recomend using qualitative colormaps, as this function will
-        automatically choose colors from the colormaps.
-        e.g. ``colors=['red', 'blue', 'green']``
-    background_color : str, optional (default ``white``)
-        Defines the background color.
-        e.g. ``background_color='gray'``
-    save_colors : bool, optional (default ``False``)
-        In case the plot is saved in 3D and some property of the
-        material is projected on the fermi surface, this argument
-        allows the projection to be stored in the 3D file.
-        e.g. ``save_colors=True``
-    cmap : str, optional (default ``jet``)
-        The color map used for color coding the projections. ``cmap``
-        is only relevant in ``mode='parametric'``. A full list of
-        color maps in matplotlib are provided in this web
-        page. `https://matplotlib.org/2.0.1/users/colormaps.html
-        <https://matplotlib.org/2.0.1/users/colormaps.html>`_
-    atoms : list int, optional
-        ``atoms`` define the projection of the atoms on the fermi
-        surfcae . In other words it selects only the contribution of the
-        atoms provided. Atoms has to be a python list(or numpy array)
-        containing the atom indices. Atom indices has to be order of
-        the input files of DFT package. ``atoms`` is only relevant in
-        ``mode='parametric'``. keep in mind that python counting
-        starts from zero.
-        e.g. for SrVO\ :sub:`3`\  we are choosing only the oxygen
-        atoms. ``atoms=[2, 3, 4]``, keep in mind that python counting
-        starts from zero, for a **POSCAR** similar to following::
-            Sr1 V1 O3
-            1.0
-            3.900891 0.000000 0.000000
-            0.000000 3.900891 0.000000
-            0.000000 0.000000 3.900891
-            Sr V O
-            1 1 3
-            direct
-            0.500000 0.500000 0.500000 Sr atom 0
-            0.000000 0.000000 0.000000 V  atom 1
-            0.000000 0.500000 0.000000 O  atom 2
-            0.000000 0.000000 0.500000 O  atom 3
-            0.500000 0.000000 0.000000 O  atom 4
-        if nothing is specified this parameter will consider all the
-        atoms present.
-    orbitals : list int, optional
-        ``orbitals`` define the projection of orbitals on the fermi
-        surface. In other words it selects only the contribution of
-        the orbitals provided. Orbitals has to be a python list(or
-        numpy array) containing the Orbital indices. Orbitals indices
-        has to be order of the input files of DFT package. The
-        following table represents the indecies for different orbitals
-        in **VASP**.
-            +-----+-----+----+----+-----+-----+-----+-----+-------+
-            |  s  | py  | pz | px | dxy | dyz | dz2 | dxz | x2-y2 |
-            +-----+-----+----+----+-----+-----+-----+-----+-------+
-            |  0  |  1  |  2 |  3 |  4  |  5  |  6  |  7  |   8   |
-            +-----+-----+----+----+-----+-----+-----+-----+-------+
-        ``orbitals`` is only relavent in ``mode='parametric'``
-        e.g. ``orbitals=[1,2,3]`` will only select the p orbitals
-        while ``orbitals=[4,5,6,7,8]`` will select the d orbitals.
-        If nothing is specified pyprocar will select all the present
-        orbitals.
-    fermi_velocity_vector : bool, optional (default False)
-            Boolean value to calculate fermi velocity vectors on the fermi surface. 
-            Must be used with mode= "property_projection".
-            e.g. ``fermi_velocity_vector=True``
-    fermi_velocity : bool, optional (default False)
-        Boolean value to calculate magnitude of the fermi velocity on the fermi surface.
-        Must be used with mode= "property_projection".
-        e.g. ``fermi_velocity=True``
-    effective_mass : bool, optional (default False)
-        Boolean value to calculate the harmonic mean of the effective mass on the fermi surface.
-        Must be used with mode= "property_projection".
-        e.g. ``effective_mass=True``
-    spin : list int, optional
-        e.g. ``spin=[0]``
-    spin_texture : bool, optional (default False)
-        In non collinear calculation one can choose to plot the spin
-        texture on the fermi surface.
-        e.g. ``spin_texture=True``
-    arrow_color : str, optional
-        Defines the color of the arrows when
-        ``spin_texture=True``. The default will select the colors
-        based on the color map specified. If arrow_color is selected,
-        all arrows will have the same color.
-        e.g. ``arrow_color='red'``
-    arrow_size : int, optional
-        As the name suggests defines the size of the arrows, when spin
-        texture is selected.
-        e.g. ``arrow_size=3``
-    only_spin : bool, optional
-        If ``only_spin=True`` is selected, the fermi surface is not
-        plotted and only the spins in the spin texture is plotted.
-    fermi_shift : float, optional
-        This parameter is useful when one wants to plot the iso-surface
-        above or belove the fermi level.
-        e.g. ``fermi_shift=0.6``
-    projection_accuracy : str, optional (default ``'normal'``)
-        Selected the accuracy of projected properties. ``'normal'`` and
-        ``'high'`` are the only two options. ``'normal'`` uses the fast
-        but rather inaccurate nearest neighbor interpolation, while
-        ``'high'`` uses the more accurate linear interpolation for the
-        projection of the properties.
-        e.g. ``projection_accuracy='high'``
-    code : str, optional (default ``'vasp'``)
-        The DFT code in which the calculation is performed with.
-        Also, if you want to read a .bxsf file set code ="bxsf"
-        e.g. ``code='vasp'``
-    vmin : float, optional
-        The maximum value in the color bar. cmap is only relevant in
-        ``mode='parametric'``.
-        e.g. vmin=-1.0
-    vmax : float, optional
-        The maximum value in the color bar. cmap is only relevant in
-        ``mode='parametric'``.
-        e.g. vmax=1.0
-    savegif : str, optional
-        pyprocar can save the fermi surface in a gif
-        format. ``savegif`` is the path to which the gif is saved.
-        e.g. ``savegif='fermi.gif'`` or ``savegif='~/MgB2/fermi.gif'``
-    savemp4 : str, optional
-        pyprocar can save the fermi surface in a mp4 video format.
-        ``savemp4`` is the path to which the video is saved.
-        e.g. ``savegif='fermi.mp4'`` or ``savegif='~/MgB2/fermi.mp4'``
-    save3d : str, optional
-        pyprocar can save the fermi surface in a 3d file format.
-        pyprocar uses the `trimesh <https://github.com/mikedh/trimesh>`_
-        to save the 3d file. trimesh can export files with the
-        following formats STL, binary PLY, ASCII OFF, OBJ, GLTF/GLB
-        2.0, COLLADA. ``save3d`` is the path to which the file is saved.
-        e.g. ``save3d='fermi.glb'``
-    save_meshio : bool, optional
-        pyprocar can use meshio to save any 3d format supported by it.
-    perspective : bool, optional
-        To create the illusion of depth, perspective is used in 2d
-        graphics. One can turn this feature off by ``perspective=False``
-        e.g.  ``perspective=False``
-    save2d : str, optional
-        The fermi surface can be saved as a 2D image. This parameter
-        turns this feature on and selects the path at which the file
-        is going to be saved.
-        e.g. ``save2d='fermi.png'``
-    show_slice : bool, optional
-        Creates a widget which slices the fermi surface
-    slice_origin : tuple, optional
-        Origin to put the plane widget
-    slice_normal : bool, optional
-        Normal of the plane widget
-    show_cross_section_area : bool, optional
-        Shows the largest cross sectional area
-    show_curvature : bool, optional
-        plots the curvature of the fermi surface
-    curvature_type : str, optional
-        If show_curvature is True, this option chooses the type of curvature 
-        availible in Pyvista. ('mean', 'gaussian', 'maximum', 'minimum')
-    iso_slider : bool, optional
-        plots a slider widget which controls which iso_energy value viewed
-    iso_range : float, optional
-        If iso_slider is True, this specifies the energy range 
-        around the fermi surface to view
-    iso_surfaces : int, optional
-        If iso_slider is True, this specifies how many surfaces to 
-        generate in the range specified around the fermi surface
-    camera_pos : list float, optional (default ``[1, 1, 1]``)
-        This parameter defines the position of the camera where it is
-        looking at the fermi surface. This feature is important when
-        one chooses to use the ``save2d``, ``savegif`` or ``savemp4``
-        option.
-        e.g. ``camera_pos=[0.5, 1, -1]``
-    widget : , optional
-        .. todo::
-    show : bool, optional (default ``True``)
-        If set to ``False`` it will not show the 3D plot.
-    Returns
-    -------
-    s : pyprocar surface object
-        The whole fermi surface added bands
-    surfaces : list pyprocar surface objects
-        list of fermi surface of each band
-    """
-
-    welcome()
-    ##########################################################################
-    # Code dependencies
-    ##########################################################################
-    if code == "vasp" or code == "abinit":
-        if repair:
-            repairhandle = UtilsProcar()
-            repairhandle.ProcarRepair(procar, procar)
-            print("PROCAR repaired. Run with repair=False next time.")
-
-    if show:
-        p = pyvista.Plotter()
-
-    if code == "vasp":
-        outcarparser = UtilsProcar()
-        if fermi is None:
-            e_fermi = outcarparser.FermiOutcar(outcar)
-        else:
-            e_fermi = fermi
-        reciprocal_lattice = outcarparser.RecLatOutcar(outcar)
-        procarFile = ProcarParser()
-        procarFile.readFile(procar, False)
-        data = ProcarSelect(procarFile, deepCopy=True)
-
-    elif code == "abinit":
-        procarFile = ProcarParser()
-        procarFile.readFile(procar, False)
-        abinitFile = AbinitParser(abinit_output=abinit_output)
-        if fermi is None:
-            e_fermi = abinitFile.fermi
-        else:
-            e_fermi = fermi
-        reciprocal_lattice = abinitFile.reclat
-        data = ProcarSelect(procarFile, deepCopy=True)
-
-        # Converting Ha to eV
-        data.bands = 27.211396641308 * data.bands
-
-    elif code == "qe":
-        procarFile = QEFermiParser()
-        reciprocal_lattice = procarFile.reclat
-        data = ProcarSelect(procarFile, deepCopy=True)
-        if fermi is None:
-            e_fermi = procarFile.fermi
-        else:
-            e_fermi = fermi
-
-    elif code == "lobster":
-        procarFile = LobsterFermiParser()
-        reciprocal_lattice = procarFile.reclat
-        data = ProcarSelect(procarFile, deepCopy=True)
-        if fermi is None:
-            e_fermi = 0
-        else:
-            e_fermi = fermi
-
-
-    elif code == "bxsf":
-        e_fermi = fermi
-        data = BxsfParser(infile= infile)
-        reciprocal_lattice = data.reclat
-
-    elif code == "frmsf":
-        e_fermi = fermi
-        data = FrmsfParser(infile=infile)
-        reciprocal_lattice = data.rec_lattice
-        bands = np.arange(len(data.bands[0, :]))
-
-
-    ##########################################################################
-    # Data Formating
-    ##########################################################################
-
-
-    band_numbers = bands
-    if band_numbers is None:
-        band_numbers = np.arange(len(data.bands[0, :]))
-
-
-    spd = []
-    if mode == "parametric":
-        if orbitals is None:
-            orbitals = [-1]
-        if atoms is None:
-            atoms = [-1]
-        if spin is None:
-            spin = [0]
-        data.selectIspin(spin)
-        data.selectAtoms(atoms, fortran=False)
-        data.selectOrbital(orbitals)
-
-        for iband in band_numbers:
-            spd.append(data.spd[:, iband])
-    elif mode == "property_projection":
-        for iband in band_numbers:
-            spd.append(None)
-    else:
-        for iband in band_numbers:
-            spd.append(None)
-
-    spd_spin = []
-
-    if spin_texture:
-        dataX = ProcarSelect(procarFile, deepCopy=True)
-        dataY = ProcarSelect(procarFile, deepCopy=True)
-        dataZ = ProcarSelect(procarFile, deepCopy=True)
-
-        dataX.kpoints = data.kpoints
-        dataY.kpoints = data.kpoints
-        dataZ.kpoints = data.kpoints
-
-        dataX.spd = data.spd
-        dataY.spd = data.spd
-        dataZ.spd = data.spd
-
-        dataX.bands = data.bands
-        dataY.bands = data.bands
-        dataZ.bands = data.bands
-
-        dataX.selectIspin([1])
-        dataY.selectIspin([2])
-        dataZ.selectIspin([3])
-
-        dataX.selectAtoms(atoms, fortran=False)
-        dataY.selectAtoms(atoms, fortran=False)
-        dataZ.selectAtoms(atoms, fortran=False)
-
-        dataX.selectOrbital(orbitals)
-        dataY.selectOrbital(orbitals)
-        dataZ.selectOrbital(orbitals)
-        for iband in band_numbers:
-            spd_spin.append(
-                [dataX.spd[:, iband], dataY.spd[:, iband], dataZ.spd[:, iband]]
-            )
-    else:
-        for iband in band_numbers:
-            spd_spin.append(None)
-
-
-    ##########################################################################
-    # Initialization of the Fermi Surface
-    ##########################################################################
-    if iso_slider == False:
-        fermi_surface3D = FermiSurface3D(
-                                        kpoints=data.kpoints,
-                                        bands=data.bands,
-                                        band_numbers = band_numbers,
-                                        spd=spd,
-                                        spd_spin=spd_spin,
-                                        fermi_velocity = fermi_velocity,
-                                        fermi_velocity_vector = fermi_velocity_vector,
-                                        effective_mass = effective_mass,
-                                        fermi=e_fermi,
-                                        fermi_shift = fermi_shift,
-                                        reciprocal_lattice=reciprocal_lattice,
-                                        interpolation_factor=interpolation_factor,
-                                        projection_accuracy=projection_accuracy,
-                                        supercell=supercell,
-                                        cmap=cmap,
-                                        vmin = vmin,
-                                        vmax=vmax,
-                                        extended_zone_directions = extended_zone_directions,
-                                        curvature_type = curvature_type,
-                                    )
-        
-        band_surfaces = fermi_surface3D.band_surfaces
-        fermi_surface = fermi_surface3D.fermi_surface
-        colors = fermi_surface3D.colors
-        brillouin_zone = fermi_surface3D.brillouin_zone
-        
-        fermi_surface_area = fermi_surface3D.fermi_surface_area
-        band_surfaces_area = fermi_surface3D.band_surfaces_area
-        
-        fermi_surface_curvature = fermi_surface3D.fermi_surface_curvature
-        band_surfaces_curvature = fermi_surface3D.band_surfaces_curvature
-    
-        test = fermi_surface_curvature
-    
-        # coloring variables
-        nsurface = len(band_surfaces)
-        # # norm = mpcolors.Normalize(vmin=vmin, vmax=vmax)
-        cmap = cm.get_cmap(cmap)
-        scalars = np.arange(nsurface + 1) / nsurface
-    
-        if save_colors is not False or save3d is not None and len(bands)!=1:
-            for i in range(nsurface):
-                if band_surfaces[i].scalars is None:
-                    band_surfaces[i].set_scalars([scalars[i]] * band_surfaces[i].nfaces)
-    
-    
-    
-        fermi_surfaces = band_surfaces.copy()
-        
-    elif iso_slider == True:
-       
-    
-        energy_values = np.linspace(e_fermi-iso_range/2,e_fermi+iso_range/2,iso_surfaces)
-        e_surfaces = []
-        
-        
-        for e_value in energy_values:
-            fermi_surface3D = FermiSurface3D(
-                                            kpoints=data.kpoints,
-                                            bands=data.bands,
-                                            band_numbers = band_numbers,
-                                            spd=spd,
-                                            spd_spin=spd_spin,
-                                            fermi_velocity = fermi_velocity,
-                                            fermi_velocity_vector = fermi_velocity_vector,
-                                            effective_mass = effective_mass,
-                                            fermi=e_value,
-                                            fermi_shift = fermi_shift,
-                                            reciprocal_lattice=reciprocal_lattice,
-                                            interpolation_factor=interpolation_factor,
-                                            projection_accuracy=projection_accuracy,
-                                            supercell=supercell,
-                                            cmap=cmap,
-                                            vmin = vmin,
-                                            vmax=vmax,
-                                            extended_zone_directions = extended_zone_directions
-                                        )
-            brillouin_zone = fermi_surface3D.brillouin_zone
-            e_surfaces.append(fermi_surface3D.fermi_surface)
-       
-    
-    ##########################################################################
-    # Plotting the surface
-    ##########################################################################
-
-
-    if show or save2d:
-        # sargs = dict(interactive=True)
-
-
-        p.add_mesh(
-            brillouin_zone.pyvista_obj,
-            style="wireframe",
-            line_width=3.5,
-            color="black",
-        )
-        
-                
-        if show_slice == True:
-            text = mode
-            if show_cross_section_area == True and bands != None:
-                if len(bands) == 1:
-                    add_mesh_slice_w_cross_sectional_area(plotter = p, mesh=fermi_surface, normal =slice_normal,origin = slice_origin, cmap=cmap, clim=[vmin, vmax])
-                    p.remove_scalar_bar()
-                else:
-                    print('---------------------------------------------')
-                    print("Can only show area of one band at a time")
-                    print('---------------------------------------------')
-            else:
-                if mode == "plain":
-                    text = "Plain"
-                    add_custom_mesh_slice(plotter = p, mesh=fermi_surface, normal =slice_normal,origin = slice_origin, cmap=cmap, clim=[vmin, vmax])
-                    p.remove_scalar_bar()
-                elif mode == "parametric":
-                    text = "Projection"
-                    add_custom_mesh_slice(plotter = p, mesh=fermi_surface, normal =slice_normal,origin = slice_origin, cmap=cmap, clim=[vmin, vmax])
-                    p.remove_scalar_bar()
-
-     
-        elif show_curvature == True:
-            text = 'Curvature'
-            class MyCustomRoutine():
-                def __init__(self, actor):
-                    self.actor = actor # Expected PyVista mesh type
-                    # default parameters
-                    self.kwargs = {
-                        'lower_percentile': 10,
-                        'upper_percentile': 90,
-                    }
-            
-                def __call__(self, param, value):
-                    self.kwargs[param] = value
-                    self.update()
-            
-                def update(self):
-                    # This is where you call your simulation
-                    p.remove_actor(actor)
-                    
-                    cmin = np.percentile(fermi_surface_curvature, self.kwargs['lower_percentile'])
-                    cmax = np.percentile(fermi_surface_curvature, self.kwargs['upper_percentile'])
-                    p.add_mesh(fermi_surface, scalars = fermi_surface_curvature,  cmap=cmap, clim=[cmin,  cmax])
-                    
-                    return
-                
-            cmin = np.percentile(fermi_surface_curvature, 10)
-            cmax = np.percentile(fermi_surface_curvature, 90)
-            actor = p.add_mesh(fermi_surface, scalars = fermi_surface_curvature,  cmap=cmap, clim=[cmin,  cmax])
-
-            engine = MyCustomRoutine(actor)
-            p.add_slider_widget(
-                            callback=lambda value: engine('lower_percentile', int(value)),
-                            rng=[0, 100],
-                            value=10,
-                            title="Lower Percentile Curvature",
-                            pointa=(.025, .90), pointb=(.31, .90),
-                            style='modern',
-                            color = 'black'
-                        )
-            p.add_slider_widget(
-                            callback=lambda value: engine('upper_percentile', int(value)),
-                            rng=[0, 100],
-                            value=90,
-                            title="Upper Percentile Curvature",
-                            pointa=(.67, 0.90), pointb=(.98, 0.90),
-                            style='modern',
-                            color = 'black'
-                        )
-            
-
-            
-            
-        elif iso_slider == True:
-            def create_mesh(value):
-                res = int(value)
-                closest_idx = find_nearest(energy_values, res)
-                p.add_mesh(e_surfaces[closest_idx], name='iso_surface')
-                p.remove_scalar_bar()
-                return
-            if mode == "plain":
-                text = "Plain"
-            elif mode == "parametric":
-                text = "Projection"
-            elif mode == "property_projection":
-                if fermi_velocity == True:
-                    text = "Projection"
-            else:
-                text = "Spin Texture"
-            p.add_slider_widget(create_mesh, [np.amin(energy_values), np.amax(energy_values)], title='Energy iso-value',style='modern',color = 'black')
-            
-            
-        else:
-            for isurface in range(nsurface):
-                if not only_spin:
-                    if mode == "plain":
-                        p.add_mesh(band_surfaces[isurface], color=colors[isurface])
-                        text = "Plain"
-                    elif mode == "parametric":
-                        p.add_mesh(
-                            band_surfaces[isurface], cmap=cmap, clim=[vmin, vmax]
-                        )
-                        p.remove_scalar_bar()
-                        text = "Projection"
-                    elif mode == "property_projection":
-                       
-                        
-                        if fermi_velocity == True:
-                            text = "Fermi Velocity"
-                            p.add_mesh(band_surfaces[isurface], cmap=cmap)
-                        if effective_mass == True:
-                            text = "Effective Mass"
-                            p.add_mesh(band_surfaces[isurface], cmap=cmap)
-                            
-                        if fermi_velocity_vector == True:
-                            text = "Fermi Velocity"
-                            arrows = band_surfaces[isurface].glyph(
-                            orient="vectors",scale=False ,factor=arrow_size)
-                            p.add_mesh(band_surfaces[isurface], cmap=cmap)
-                            p.remove_scalar_bar()
-                            if arrow_color is None:
-                                p.add_mesh(arrows, cmap=cmap)
-                            else:
-                                p.add_mesh(arrows, color=arrow_color)
-                        p.remove_scalar_bar()
-                else:
-                    text = "Spin Texture"
-
-                if spin_texture:
-                    # Example dataset with normals
-                    # create a subset of arrows using the glyph filter
-                    arrows = band_surfaces[isurface].glyph(
-                    orient="vectors",scale=False ,factor=arrow_size)
-
-                    if arrow_color is None:
-                        p.add_mesh(arrows, cmap=cmap, clim=[vmin, vmax])
-                        p.remove_scalar_bar()
-                    else:
-                        p.add_mesh(arrows, color=arrow_color)
-
-        
-        if mode != "plain" or spin_texture:
-            p.add_scalar_bar(
-                title=text,
-                n_labels=6,
-                italic=False,
-                bold=False,
-                title_font_size=None,
-                label_font_size=None,
-                position_x=0.4,
-                position_y=0.01,
-                color="black",
-            )
-
-        p.add_axes(
-            xlabel="Kx", ylabel="Ky", zlabel="Kz", line_width=6, labels_off=False
-        )
-
-        if not perspective:
-            p.enable_parallel_projection()
-
-        p.set_background(background_color)
-        # p.set_position(camera_pos)
-        if not widget:
-            p.show(cpos=camera_pos, screenshot=save2d)
-        # p.screenshot('1.png')
-        # p.save_graphic('1.pdf')
-        if savegif is not None:
-            path = p.generate_orbital_path(n_points=36)
-            p.open_gif(savegif)
-            p.orbit_on_path(path)  # ,viewup=camera_pos)
-        if savemp4:
-            path = p.generate_orbital_path(n_points=36)
-            p.open_movie(savemp4)
-            p.orbit_on_path(path)  # ,viewup=camera_pos)
-            # p.close()
-    # p.show()
-    if iso_slider == False:
-        s = boolean_add(band_surfaces)
-    # s.set_color_with_cmap(cmap=cmap, vmin=vmin, vmax=vmax)
-    # s.pyvista_obj.plot()
-    # s.trimesh_obj.show()
-
-    if save3d is not None:
-        if save_meshio == True:
-            pyvista.save_meshio(save3d,  fermi_surface)
-        else:
-            extention = save3d.split(".")[-1]
-            s.export(save3d, extention)
-    if iso_slider == False:
-        return s, fermi_surfaces, fermi_surface
-    
-
-def add_mesh_slice_w_cross_sectional_area(plotter, mesh, normal='x', generate_triangles=False,
-                       widget_color=None, assign_to_axis=None,
-                       tubing=False, origin_translation=True,origin = (0,0,0),
-                       outline_translation=False, implicit=True,
-                       normal_rotation=True, **kwargs):
-
-        name = kwargs.get('name', mesh.memory_address)
-        rng = mesh.get_data_range(kwargs.get('scalars', None))
-        kwargs.setdefault('clim', kwargs.pop('rng', rng))
-        mesh.set_active_scalars(kwargs.get('scalars', mesh.active_scalars_name))
-
-        plotter.add_mesh(mesh.outline(), name=name+"outline", opacity=0.0)
-
-        alg = vtk.vtkCutter() # Construct the cutter object
-        alg.SetInputDataObject(mesh) # Use the grid as the data we desire to cut
-        if not generate_triangles:
-            alg.GenerateTrianglesOff()
-
-        # if not hasattr(self, "plane_sliced_meshes"):
-        plotter.plane_sliced_meshes = []
-        plane_sliced_mesh = pyvista.wrap(alg.GetOutput())
-        plotter.plane_sliced_meshes.append(plane_sliced_mesh)
-        
-        user_slice = plotter.plane_sliced_meshes[0]
-        surface = user_slice.delaunay_2d()
-        plotter.add_text(f'Cross sectional area : {surface.area}', color = 'black')
-        def callback(normal, origin):
-            # create the plane for clipping
-            
-            plane = generate_plane(normal, origin)
-            
-            alg.SetCutFunction(plane) # the cutter to use the plane we made
-            alg.Update() # Perform the Cut
-            
-            plane_sliced_mesh.shallow_copy(alg.GetOutput())
-            
-            user_slice = plotter.plane_sliced_meshes[0]
-            surface = user_slice.delaunay_2d()
-            text = f'Cross sectional area : {surface.area}'
-            plotter.textActor.SetText(2, text)
-
-
-        plotter.add_plane_widget(callback=callback, bounds=mesh.bounds,
-                              factor=1.25, normal='x',
-                              color=widget_color, tubing=tubing,
-                              assign_to_axis=assign_to_axis,
-                              origin_translation=origin_translation,
-                              outline_translation=outline_translation,
-                              implicit=implicit, origin=origin,
-                              normal_rotation=normal_rotation)
-    
-        actor = plotter.add_mesh(plane_sliced_mesh, **kwargs)
-        
-        plotter.plane_widgets[0].SetNormal(normal)
-
-        return actor
-    
-def add_custom_mesh_slice(plotter, mesh, normal='x', generate_triangles=False,
-                       widget_color=None, assign_to_axis=None,
-                       tubing=False, origin_translation=True,origin = (0,0,0),
-                       outline_translation=False, implicit=True,
-                       normal_rotation=True, **kwargs):
-
-        name = kwargs.get('name', mesh.memory_address)
-        rng = mesh.get_data_range(kwargs.get('scalars', None))
-        kwargs.setdefault('clim', kwargs.pop('rng', rng))
-        mesh.set_active_scalars(kwargs.get('scalars', mesh.active_scalars_name))
-
-        plotter.add_mesh(mesh.outline(), name=name+"outline", opacity=0.0)
-
-        alg = vtk.vtkCutter() # Construct the cutter object
-        alg.SetInputDataObject(mesh) # Use the grid as the data we desire to cut
-        if not generate_triangles:
-            alg.GenerateTrianglesOff()
-
-        # if not hasattr(self, "plane_sliced_meshes"):
-        plotter.plane_sliced_meshes = []
-        plane_sliced_mesh = pyvista.wrap(alg.GetOutput())
-        plotter.plane_sliced_meshes.append(plane_sliced_mesh)
-        
-
-        def callback(normal, origin):
-            # create the plane for clipping
-            
-            plane = generate_plane(normal, origin)
-            
-            alg.SetCutFunction(plane) # the cutter to use the plane we made
-            alg.Update() # Perform the Cut
-            
-            plane_sliced_mesh.shallow_copy(alg.GetOutput())
-            
-
-
-
-        plotter.add_plane_widget(callback=callback, bounds=mesh.bounds,
-                              factor=1.25, normal='x',
-                              color=widget_color, tubing=tubing,
-                              assign_to_axis=assign_to_axis,
-                              origin_translation=origin_translation,
-                              outline_translation=outline_translation,
-                              implicit=implicit, origin=origin,
-                              normal_rotation=normal_rotation)
-    
-        actor = plotter.add_mesh(plane_sliced_mesh, **kwargs)
-        
-        plotter.plane_widgets[0].SetNormal(normal)
-
-        return actor
-
-
-def find_nearest(array, value):
-    array = np.asarray(array)
-    idx = (np.abs(array - value)).argmin()
-    return idx
+__author__ = "Pedram Tavadze and Logan Lang"
+__maintainer__ = "Pedram Tavadze and Logan Lang"
+__email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
+__date__ = "March 31, 2020"
+
+import sys
+from typing import List, Tuple
+import copy
+
+import numpy as np
+from matplotlib import colors as mpcolors
+from matplotlib import cm
+import vtk
+import pyvista
+from pyvista.utilities import NORMALS, generate_plane, get_array, try_callback
+
+
+from ..core import FermiSurface3D
+from ..utils import welcome
+from ..utils import UtilsProcar
+from ..io.procarparser import ProcarParser
+from ..io.lobsterparser import LobsterFermiParser
+from ..io.abinitparser import AbinitParser
+from .. import io
+
+np.set_printoptions(threshold=sys.maxsize)
+
+# TODO update the parsing section
+# TODO separate slicing functionality to new function
+# TODO separate iso-slider functionality to new function. isoslider still experimental
+
+def fermi3D(
+    procar:str="PROCAR",
+    outcar:str="OUTCAR",
+    poscar:str="POSCAR",
+    dirname:str="",
+    infile:str="in.bxsf",
+    abinit_output:str=None,
+    fermi:float=None,
+    bands:List[int]=None,
+    interpolation_factor:int=1,
+    mode:str="plain",
+    supercell:List[int]=[1, 1, 1],
+    extended_zone_directions:List[List[int]] = None,
+    colors: List[str] or List[Tuple[float,float,float]]=None,
+    background_color:str="white",
+    save_colors:bool=False,
+    cmap:str="jet",
+    atoms:List[int]=None,
+    orbitals:List[int]=None,
+    calculate_fermi_speed: bool=False,
+    calculate_fermi_velocity: bool=False,
+    calculate_effective_mass: bool=False,
+    spins:List[int]=None,
+    spin_texture: bool=False,
+    arrow_color=None,
+    arrow_size: float=0.015,
+    only_spin: bool=False,
+    fermi_shift:float=0,
+    fermi_tolerance:float=0.1,
+    projection_accuracy:str="normal",
+    code:str="vasp",
+    vmin:float=0,
+    vmax:float=1,
+    savegif:str=None,
+    savemp4:str=None,
+    save3d:str=None,
+    save_meshio:bool=False,
+    perspective:bool=True,
+    save2d:bool=False,
+    show_slice:bool=False,
+    slice_normal: Tuple[float,float,float]=(1,0,0),
+    slice_origin: Tuple[float,float,float]=(0,0,0),
+    show_cross_section_area: bool=False,
+    iso_slider: bool=False,
+    iso_range: float=2,
+    iso_surfaces: int=10,
+    camera_pos:List[float]=[1, 1, 1],
+    widget:bool=False,
+    show:bool=True,
+    repair:bool=True,
+    ):
+    """
+    This function plots the fermi surface
+
+    Parameters
+    ----------
+    procar : str, optional (default ``'PROCAR'``)
+        Path to the PROCAR file of the simulation
+        e.g. ``procar='~/MgB2/fermi/PROCAR'``
+    outcar : str, optional (default ``'OUTCAR'``)
+        Path to the OUTCAR file of the simulation
+        e.g. ``outcar='~/MgB2/fermi/OUTCAR'``
+    abinit_output : str, optional (default ``None``)
+        Path to the Abinit output file
+        e.g. ``outcar='~/MgB2/abinit.out'``
+    infile : str, optional (default ``infile = in.bxsf'``)
+        This is the path in the input bxsf file
+        e.g. ``infile = ni_fs.bxsf'``
+    fermi : float, optional (default ``None``)
+        Fermi energy at which the fermi surface is created. In other
+        words fermi is the isovalue at which the fermi surface is
+        created. If not defined it is read from the OUTCAR file.
+        e.g. ``fermi=-5.49``
+    bands : list int, optional
+        Which bands are going to be plotted in the fermi surface. The
+        numbering is based on vasp outputs. If nothing is selected,
+        this function will iterate over all the bands and plots the
+        ones that cross fermi.
+        e.g. ``bands=[14, 15, 16, 17]``
+    interpolation_factor : int, optional
+        The kpoints grid will increase by this factor and interpolated
+        at the new points using Fourier interpolation.
+        e.g. If the kgrid is 5x5x5, ``interpolation_factor=4`` will
+        lead to a kgrid of 20x20x20
+    mode : str, optional (default ``mode='plain'``)
+        Defines If the fermi surface will have any projection using
+        colormaps or is a plotted with a uniform plain color.
+        e.g. ``mode='plain'``, ``mode='parametric'``
+    supercell : list int, optional (default ``[1, 1, 1]``)
+        If one wants plot more than the 1st brillouin zone, this
+        parameter can be used.
+        e.g. ``supercell=[2, 2, 2]``
+    extended_zone_directions : list of list of size 3, optional (default ``None``)
+        If one wants plot more than  brillouin zones in a particular direection, this
+        parameter can be used.
+        e.g. ``extended_zone_directions=[[1,0,0],[0,1,0],[0,0,1]]``
+    colors : list str or list tuples of size 4, optional
+        List of colors for each band. If you use tuple, it represents rgba values
+        This argument does not work whena 3d file is saved. 
+        The colors for when ``save3d`` is used, we
+        recomend using qualitative colormaps, as this function will
+        automatically choose colors from the colormaps.
+        e.g. ``colors=['red', 'blue', 'green']``
+        ``colors=[(1,0,0,1), (0,1,0,1), (0,0,1,1)]``
+    background_color : str, optional (default ``white``)
+        Defines the background color.
+        e.g. ``background_color='gray'``
+    save_colors : bool, optional (default ``False``)
+        In case the plot is saved in 3D and some property of the
+        material is projected on the fermi surface, this argument
+        allows the projection to be stored in the 3D file.
+        e.g. ``save_colors=True``
+    cmap : str, optional (default ``jet``)
+        The color map used for color coding the projections. ``cmap``
+        is only relevant in ``mode='parametric'``. A full list of
+        color maps in matplotlib are provided in this web
+        page. `https://matplotlib.org/2.0.1/users/colormaps.html
+        <https://matplotlib.org/2.0.1/users/colormaps.html>`_
+    atoms : list int, optional
+        ``atoms`` define the projection of the atoms on the fermi
+        surfcae . In other words it selects only the contribution of the
+        atoms provided. Atoms has to be a python list(or numpy array)
+        containing the atom indices. Atom indices has to be order of
+        the input files of DFT package. ``atoms`` is only relevant in
+        ``mode='parametric'``. keep in mind that python counting
+        starts from zero.
+        e.g. for SrVO\ :sub:`3`\  we are choosing only the oxygen
+        atoms. ``atoms=[2, 3, 4]``, keep in mind that python counting
+        starts from zero, for a **POSCAR** similar to following::
+
+            Sr1 V1 O3
+            1.0
+            3.900891 0.000000 0.000000
+            0.000000 3.900891 0.000000
+            0.000000 0.000000 3.900891
+            Sr V O
+            1 1 3
+            direct
+            0.500000 0.500000 0.500000 Sr atom 0
+            0.000000 0.000000 0.000000 V  atom 1
+            0.000000 0.500000 0.000000 O  atom 2
+            0.000000 0.000000 0.500000 O  atom 3
+            0.500000 0.000000 0.000000 O  atom 4
+
+        if nothing is specified this parameter will consider all the
+        atoms present.
+    orbitals : list int, optional
+        ``orbitals`` define the projection of orbitals on the fermi
+        surface. In other words it selects only the contribution of
+        the orbitals provided. Orbitals has to be a python list(or
+        numpy array) containing the Orbital indices. Orbitals indices
+        has to be order of the input files of DFT package. The
+        following table represents the indecies for different orbitals
+        in **VASP**.::
+
+            +-----+-----+----+----+-----+-----+-----+-----+-------+
+            |  s  | py  | pz | px | dxy | dyz | dz2 | dxz | x2-y2 |
+            +-----+-----+----+----+-----+-----+-----+-----+-------+
+            |  0  |  1  |  2 |  3 |  4  |  5  |  6  |  7  |   8   |
+            +-----+-----+----+----+-----+-----+-----+-----+-------+
+
+        ``orbitals`` is only relavent in ``mode='parametric'``
+        e.g. ``orbitals=[1,2,3]`` will only select the p orbitals
+        while ``orbitals=[4,5,6,7,8]`` will select the d orbitals.
+        If nothing is specified pyprocar will select all the present
+        orbitals.
+    calculate_fermi_velocity : bool, optional (default False)
+            Boolean value to calculate fermi velocity vectors on the fermi surface. 
+            Must be used with mode= "property_projection".
+            e.g. ``fermi_velocity_vector=True``
+    calculate_fermi_speed : bool, optional (default False)
+        Boolean value to calculate magnitude of the fermi velocity on the fermi surface.
+        Must be used with mode= "property_projection".
+        e.g. ``fermi_velocity=True``
+    calculate_effective_mass : bool, optional (default False)
+        Boolean value to calculate the harmonic mean of the effective mass on the fermi surface.
+        Must be used with mode= "property_projection".
+        e.g. ``effective_mass=True``
+    spins : list int, optional
+        e.g. ``spins=[0]``
+    spin_texture : bool, optional (default False)
+        In non collinear calculation one can choose to plot the spin
+        texture on the fermi surface.
+        e.g. ``spin_texture=True``
+    arrow_color : str, optional
+        Defines the color of the arrows when
+        ``spin_texture=True``. The default will select the colors
+        based on the color map specified. If arrow_color is selected,
+        all arrows will have the same color.
+        e.g. ``arrow_color='red'``
+    arrow_size : int, optional
+        As the name suggests defines the size of the arrows, when spin
+        texture is selected.
+        e.g. ``arrow_size=3``
+    only_spin : bool, optional
+        If ``only_spin=True`` is selected, the fermi surface is not
+        plotted and only the spins in the spin texture is plotted.
+    fermi_shift : float, optional
+        This parameter is useful when one wants to plot the iso-surface
+        above or belove the fermi level.
+        e.g. ``fermi_shift=0.6``
+    fermi_tolerance : float = 0.1
+        This is used to improve search effiency by doing a prior search selecting band within a tolerance of the fermi energy
+    projection_accuracy : str, optional (default ``'normal'``)
+        Selected the accuracy of projected properties. ``'normal'`` and
+        ``'high'`` are the only two options. ``'normal'`` uses the fast
+        but rather inaccurate nearest neighbor interpolation, while
+        ``'high'`` uses the more accurate linear interpolation for the
+        projection of the properties.
+        e.g. ``projection_accuracy='high'``
+    code : str, optional (default ``'vasp'``)
+        The DFT code in which the calculation is performed with.
+        Also, if you want to read a .bxsf file set code ="bxsf"
+        e.g. ``code='vasp'``
+    vmin : float, optional
+        The maximum value in the color bar. cmap is only relevant in
+        ``mode='parametric'``.
+        e.g. vmin=-1.0
+    vmax : float, optional
+        The maximum value in the color bar. cmap is only relevant in
+        ``mode='parametric'``.
+        e.g. vmax=1.0
+    savegif : str, optional
+        pyprocar can save the fermi surface in a gif
+        format. ``savegif`` is the path to which the gif is saved.
+        e.g. ``savegif='fermi.gif'`` or ``savegif='~/MgB2/fermi.gif'``
+    savemp4 : str, optional
+        pyprocar can save the fermi surface in a mp4 video format.
+        ``savemp4`` is the path to which the video is saved.
+        e.g. ``savegif='fermi.mp4'`` or ``savegif='~/MgB2/fermi.mp4'``
+    save3d : str, optional
+        pyprocar can save the fermi surface in a 3d file format.
+        pyprocar uses the `trimesh <https://github.com/mikedh/trimesh>`_
+        to save the 3d file. trimesh can export files with the
+        following formats STL, binary PLY, ASCII OFF, OBJ, GLTF/GLB
+        2.0, COLLADA. ``save3d`` is the path to which the file is saved.
+        e.g. ``save3d='fermi.glb'``
+    save_meshio : bool, optional
+        pyprocar can use meshio to save any 3d format supported by it.
+    perspective : bool, optional
+        To create the illusion of depth, perspective is used in 2d
+        graphics. One can turn this feature off by ``perspective=False``
+        e.g.  ``perspective=False``
+    save2d : str, optional
+        The fermi surface can be saved as a 2D image. This parameter
+        turns this feature on and selects the path at which the file
+        is going to be saved.
+        e.g. ``save2d='fermi.png'``
+    show_slice : bool, optional
+        Creates a widget which slices the fermi surface
+    slice_origin : tuple, optional
+        Origin to put the plane widget
+    slice_normal : bool, optional
+        Normal of the plane widget
+    show_cross_section_area : bool, optional
+        Shows the largest cross sectional area
+    show_curvature : bool, optional
+        plots the curvature of the fermi surface
+    curvature_type : str, optional
+        If show_curvature is True, this option chooses the type of curvature 
+        availible in Pyvista. ('mean', 'gaussian', 'maximum', 'minimum')
+    iso_slider : bool, optional
+        plots a slider widget which controls which iso_energy value viewed
+    iso_range : float, optional
+        If iso_slider is True, this specifies the energy range 
+        around the fermi surface to view
+    iso_surfaces : int, optional
+        If iso_slider is True, this specifies how many surfaces to 
+        generate in the range specified around the fermi surface
+    camera_pos : list float, optional (default ``[1, 1, 1]``)
+        This parameter defines the position of the camera where it is
+        looking at the fermi surface. This feature is important when
+        one chooses to use the ``save2d``, ``savegif`` or ``savemp4``
+        option.
+        e.g. ``camera_pos=[0.5, 1, -1]``
+    widget : bool, optional
+        boolean argument to use
+    show : bool, optional (default ``True``)
+        If set to ``False`` it will not show the 3D plot.
+
+    Returns
+    -------
+    s : pyprocar surface object
+        The whole fermi surface added bands
+    surfaces : list pyprocar surface objects
+        list of fermi surface of each band
+
+    """
+
+    welcome()
+    ##########################################################################
+    # Code dependencies
+    ##########################################################################
+    parser = io.Parser(code = code, dir = dirname)
+    ebs = parser.ebs
+    reciprocal_lattice = parser.ebs.reciprocal_lattice
+    if fermi is None:
+        e_fermi = ebs.efermi
+    ##########################################################################
+    # Data Formating
+    ##########################################################################
+
+    bands_to_keep = bands
+    if bands_to_keep is None:
+        bands_to_keep = np.arange(len(bands[0, :]))
+
+
+    spd = []
+    
+    if mode == "parametric":
+        if orbitals is None:
+            orbitals = np.arange(ebs.norbitals, dtype=int)
+        if atoms is None:
+            atoms = np.arange(ebs.natoms, dtype=int)
+        if spins is None:
+            spins = [0]
+
+        # data.selectIspin(spins)
+        # data.selectAtoms(atoms, fortran=False)
+        # data.selectOrbital(orbitals)
+
+        projected = ebs.ebs_sum(spins=spins , atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
+        projected = projected[:,:,spins[0]]
+
+        for iband in bands_to_keep:
+            spd.append(projected[:,iband] )
+    elif mode == "property_projection":
+        for iband in bands_to_keep:
+            spd.append(None)
+    else:
+        for iband in bands_to_keep:
+            spd.append(None)
+   
+    spd_spin = []
+
+    if spin_texture:
+        ebsX = copy.deepcopy(ebs)
+        ebsY = copy.deepcopy(ebs)
+        ebsZ = copy.deepcopy(ebs)
+
+        ebsX.projected = ebsX.ebs_sum(spins=spins, atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
+        ebsY.projected = ebsY.ebs_sum(spins=spins, atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
+        ebsZ.projected = ebsZ.ebs_sum(spins=spins, atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
+
+        ebsX.projected = ebsX.projected[:,:,[0]]
+        ebsY.projected = ebsY.projected[:,:,[1]]
+        ebsZ.projected = ebsZ.projected[:,:,[2]]
+
+        for iband in bands_to_keep:
+            spd_spin.append(
+                [ebsX.projected[:, iband], ebsY.projected[:, iband], ebsZ.projected[:, iband]]
+            )
+    else:
+        for iband in bands_to_keep:
+            spd_spin.append(None)
+
+
+
+    ##########################################################################
+    # Initialization of the Fermi Surface
+    ##########################################################################
+    if iso_slider == False:
+        fermi_surface3D = FermiSurface3D(
+                                        kpoints=ebs.kpoints,
+                                        bands=ebs.bands,
+                                        bands_to_keep = bands_to_keep,
+                                        spd=spd,
+                                        spd_spin=spd_spin,
+                                        colors = colors,
+                                        calculate_fermi_speed = calculate_fermi_speed,
+                                        calculate_fermi_velocity = calculate_fermi_velocity,
+                                        calculate_effective_mass = calculate_effective_mass,
+                                        fermi=e_fermi,
+                                        fermi_shift = fermi_shift,
+                                        fermi_tolerance=fermi_tolerance,
+                                        reciprocal_lattice=reciprocal_lattice,
+                                        interpolation_factor=interpolation_factor,
+                                        projection_accuracy=projection_accuracy,
+                                        supercell=supercell,
+                                        cmap=cmap,
+                                        vmin = vmin,
+                                        vmax=vmax,
+                                        extended_zone_directions = extended_zone_directions,
+                                        # curvature_type = curvature_type,
+                                    )
+        
+
+        brillouin_zone = fermi_surface3D.brillouin_zone
+
+        # fermi_surface_area = fermi_surface3D.fermi_surface_area
+        # band_surfaces_area = fermi_surface3D.band_surfaces_area
+        
+        # fermi_surface_curvature = fermi_surface3D.fermi_surface_curvature
+        # band_surfaces_curvature = fermi_surface3D.band_surfaces_curvature
+    
+        
+    elif iso_slider == True:
+       
+        energy_values = np.linspace(e_fermi-iso_range/2,e_fermi+iso_range/2,iso_surfaces)
+        e_surfaces = []
+        
+    
+        for e_value in energy_values:
+            fermi_surface3D = FermiSurface3D(
+                                            kpoints=ebs.kpoints,
+                                            bands_to_keep = bands_to_keep,
+                                            bands=ebs.bands,
+                                            spd=spd,
+                                            spd_spin=spd_spin,
+                                            calculate_fermi_speed = calculate_fermi_speed,
+                                            calculate_fermi_velocity = calculate_fermi_velocity,
+                                            calculate_effective_mass = calculate_effective_mass,
+                                            fermi=e_value,
+                                            fermi_shift = fermi_shift,
+                                            fermi_tolerance=fermi_tolerance,
+                                            reciprocal_lattice=reciprocal_lattice,
+                                            interpolation_factor=interpolation_factor,
+                                            projection_accuracy=projection_accuracy,
+                                            supercell=supercell,
+                                            cmap=cmap,
+                                            vmin = vmin,
+                                            vmax=vmax,
+                                            extended_zone_directions = extended_zone_directions
+                                        )
+            brillouin_zone = fermi_surface3D.brillouin_zone
+            e_surfaces.append(fermi_surface3D)
+       
+    
+    ##########################################################################
+    # Plotting the surface
+    ##########################################################################
+    if show:
+        p = pyvista.Plotter()
+
+    if show or save2d:
+
+        # sargs = dict(interactive=True)
+
+
+        p.add_mesh(
+            brillouin_zone,
+            style="wireframe",
+            line_width=3.5,
+            color="black",
+        )
+        
+                
+        if show_slice == True:
+            text = mode
+            if show_cross_section_area == True and bands != None:
+                if len(bands) == 1:
+                    add_mesh_slice_w_cross_sectional_area(plotter = p, mesh=fermi_surface3D, normal =slice_normal,origin = slice_origin, scalars = "scalars")
+                    p.remove_scalar_bar()
+                else:
+                    print('---------------------------------------------')
+                    print("Can only show area of one band at a time")
+                    print('---------------------------------------------')
+            else:
+                if mode == "plain":
+                    text = "Plain"
+                    add_custom_mesh_slice(plotter = p, mesh=fermi_surface3D, normal =slice_normal,origin = slice_origin,  scalars = "scalars")
+                    p.remove_scalar_bar()
+                elif mode == "parametric":
+                    text = "Projection"
+                    add_custom_mesh_slice(plotter = p, mesh=fermi_surface3D, normal =slice_normal,origin = slice_origin,  scalars = "scalars")
+
+                    p.remove_scalar_bar()
+                    
+        elif iso_slider == True:
+            def create_mesh(value):
+                res = int(value)
+                closest_idx = find_nearest(energy_values, res)
+                if mode == "plain":
+                    scalars = "bands"
+                elif mode == "parametric":
+                    scalars = "scalars"
+                elif mode == "property_projection":
+                    if calculate_fermi_speed == True:
+                        scalars = "Fermi Speed"
+                    elif calculate_fermi_velocity == True:
+                        scalars = "Fermi Velocity Vector"
+                        
+                    elif calculate_effective_mass == True:
+                        scalars = "Geometric Average Effective Mass"
+                else:
+                    text = "Spin Texture"
+                    scalars = "spin"
+                    
+                    
+                p.add_mesh(e_surfaces[closest_idx], name='iso_surface', scalars = scalars)
+                arrows =e_surfaces[closest_idx].glyph(
+                orient=scalars,scale=False ,factor=arrow_size)
+                p.remove_scalar_bar()
+                
+                if arrow_color is None:
+                    p.add_mesh(arrows, scalars = "Fermi Velocity Vector_magnitude" ,cmap=cmap)
+                else:
+                    p.add_mesh(arrows, color=arrow_color)
+                p.remove_scalar_bar()
+                
+                return
+            if mode == "plain":
+                text = "Plain"
+            elif mode == "parametric":
+                text = "Projection"
+            elif mode == "property_projection":
+                if calculate_fermi_speed == True:
+                    text = "Projection"
+            else:
+                text = "Spin Texture"
+                
+                    
+            p.add_slider_widget(create_mesh, [np.amin(energy_values), np.amax(energy_values)], title='Energy iso-value',style='modern',color = 'black')
+            
+            
+            
+        else:
+
+            if not spin_texture:
+                if mode == "plain":
+                    p.add_mesh(fermi_surface3D, scalars = "bands",cmap = cmap, rgba = True)
+                    text = "Plain"
+                elif mode == "parametric":
+                    p.add_mesh(fermi_surface3D, scalars = "scalars", cmap=cmap)
+                    p.remove_scalar_bar()
+                    text = "Projection"
+                elif mode == "property_projection":
+                    if calculate_fermi_speed == True:
+                        text = "Fermi Speed"
+                        p.add_mesh(fermi_surface3D,scalars = "Fermi Speed", cmap=cmap)
+                    if calculate_effective_mass == True:
+                        text = "Effective Mass"
+                        p.add_mesh(fermi_surface3D,scalars =  "Geometric Average Effective Mass", cmap=cmap)
+                        
+                    if calculate_fermi_velocity == True:
+                        text = "Fermi Velocity"
+
+                        arrows = fermi_surface3D.glyph(
+                        orient="Fermi Velocity Vector",scale=False ,factor=arrow_size)
+                        p.add_mesh(fermi_surface3D, scalars = "Fermi Velocity Vector_magnitude" , cmap=cmap)
+                        p.remove_scalar_bar()
+                        if arrow_color is None:
+                            p.add_mesh(arrows, scalars = "Fermi Velocity Vector_magnitude" ,cmap=cmap)
+                        else:
+                            p.add_mesh(arrows, color=arrow_color)
+                    p.remove_scalar_bar()
+            else:
+                text = "Spin Texture"
+                # Example dataset with normals
+                # create a subset of arrows using the glyph filter
+                arrows = fermi_surface3D.glyph(
+                orient="spin",scale=False ,factor=arrow_size)
+
+                if arrow_color is None:
+                    p.add_mesh(arrows, cmap=cmap, clim=[vmin, vmax])
+                    p.remove_scalar_bar()
+                else:
+                    p.add_mesh(arrows, color=arrow_color)
+
+        
+        if mode != "plain" or spin_texture:
+            p.add_scalar_bar(
+                title=text,
+                n_labels=6,
+                italic=False,
+                bold=False,
+                title_font_size=None,
+                label_font_size=None,
+                position_x=0.4,
+                position_y=0.01,
+                color="black",
+            )
+
+        p.add_axes(
+            xlabel="Kx", ylabel="Ky", zlabel="Kz", line_width=6, labels_off=False
+        )
+
+        if not perspective:
+            p.enable_parallel_projection()
+
+        p.set_background(background_color)
+        if not widget:
+            p.show(cpos=camera_pos, screenshot=save2d)
+        if savegif is not None:
+            path = p.generate_orbital_path(n_points=36)
+            p.open_gif(savegif)
+            p.orbit_on_path(path) 
+        if savemp4:
+            path = p.generate_orbital_path(n_points=36)
+            p.open_movie(savemp4)
+            p.orbit_on_path(path) 
+            # p.close()
+    # p.show()
+    # if iso_slider == False:
+    #     s = boolean_add(fermi_surface3D)
+    # s.set_color_with_cmap(cmap=cmap, vmin=vmin, vmax=vmax)
+    # s.pyvista_obj.plot()
+    # s.trimesh_obj.show()
+
+    if save3d is not None:
+        if save_meshio == True:
+            pyvista.save_meshio(save3d,  fermi_surface3D)
+        else:
+            extention = save3d.split(".")[-1]
+    #         s.export(save3d, extention)
+    # if iso_slider == False:
+    #     return s, fermi_surface3D
+    
+
+def add_mesh_slice_w_cross_sectional_area(plotter, mesh, normal='x', generate_triangles=False,
+                                        widget_color=None, assign_to_axis=None,
+                                        tubing=False, origin_translation=True,origin = (0,0,0),
+                                        outline_translation=False, implicit=True,
+                                        normal_rotation=True, **kwargs):
+
+        name = kwargs.get('name', mesh.memory_address)
+        rng = mesh.get_data_range(kwargs.get('scalars', None))
+        kwargs.setdefault('clim', kwargs.pop('rng', rng))
+        mesh.set_active_scalars(kwargs.get('scalars', mesh.active_scalars_name))
+
+        plotter.add_mesh(mesh.outline(), name=name+"outline", opacity=0.0)
+
+        alg = vtk.vtkCutter() # Construct the cutter object
+        alg.SetInputDataObject(mesh) # Use the grid as the data we desire to cut
+        if not generate_triangles:
+            alg.GenerateTrianglesOff()
+
+        # if not hasattr(self, "plane_sliced_meshes"):
+        plotter.plane_sliced_meshes = []
+        plane_sliced_mesh = pyvista.wrap(alg.GetOutput())
+        plotter.plane_sliced_meshes.append(plane_sliced_mesh)
+        
+        user_slice = plotter.plane_sliced_meshes[0]
+        surface = user_slice.delaunay_2d()
+        plotter.add_text(f'Cross sectional area : {surface.area}', color = 'black')
+        def callback(normal, origin):
+            # create the plane for clipping
+            
+            plane = generate_plane(normal, origin)
+            
+            alg.SetCutFunction(plane) # the cutter to use the plane we made
+            alg.Update() # Perform the Cut
+            
+            plane_sliced_mesh.shallow_copy(alg.GetOutput())
+            
+            user_slice = plotter.plane_sliced_meshes[0]
+            surface = user_slice.delaunay_2d()
+            text = f'Cross sectional area : {surface.area}'
+            plotter.textActor.SetText(2, text)
+
+
+        plotter.add_plane_widget(callback=callback, bounds=mesh.bounds,
+                              factor=1.25, normal='x',
+                              color=widget_color, tubing=tubing,
+                              assign_to_axis=assign_to_axis,
+                              origin_translation=origin_translation,
+                              outline_translation=outline_translation,
+                              implicit=implicit, origin=origin,
+                              normal_rotation=normal_rotation)
+    
+        actor = plotter.add_mesh(plane_sliced_mesh, **kwargs)
+        
+        plotter.plane_widgets[0].SetNormal(normal)
+
+        return actor
+    
+def add_custom_mesh_slice(plotter, mesh, normal='x', generate_triangles=False,
+                       widget_color=None, assign_to_axis=None,
+                       tubing=False, origin_translation=True,origin = (0,0,0),
+                       outline_translation=False, implicit=True,
+                       normal_rotation=True, **kwargs):
+
+        name = kwargs.get('name', mesh.memory_address)
+        rng = mesh.get_data_range(kwargs.get('scalars', None))
+        kwargs.setdefault('clim', kwargs.pop('rng', rng))
+        mesh.set_active_scalars(kwargs.get('scalars', mesh.active_scalars_name))
+
+        plotter.add_mesh(mesh.outline(), name=name+"outline", opacity=0.0)
+
+        alg = vtk.vtkCutter() # Construct the cutter object
+        alg.SetInputDataObject(mesh) # Use the grid as the data we desire to cut
+        if not generate_triangles:
+            alg.GenerateTrianglesOff()
+
+        # if not hasattr(self, "plane_sliced_meshes"):
+        plotter.plane_sliced_meshes = []
+        plane_sliced_mesh = pyvista.wrap(alg.GetOutput())
+        plotter.plane_sliced_meshes.append(plane_sliced_mesh)
+        
+
+        def callback(normal, origin):
+            # create the plane for clipping
+            
+            plane = generate_plane(normal, origin)
+            
+            alg.SetCutFunction(plane) # the cutter to use the plane we made
+            alg.Update() # Perform the Cut
+            
+            plane_sliced_mesh.shallow_copy(alg.GetOutput())
+            
+
+
+
+        plotter.add_plane_widget(callback=callback, bounds=mesh.bounds,
+                              factor=1.25, normal='x',
+                              color=widget_color, tubing=tubing,
+                              assign_to_axis=assign_to_axis,
+                              origin_translation=origin_translation,
+                              outline_translation=outline_translation,
+                              implicit=implicit, origin=origin,
+                              normal_rotation=normal_rotation)
+    
+        actor = plotter.add_mesh(plane_sliced_mesh, **kwargs)
+        
+        plotter.plane_widgets[0].SetNormal(normal)
+
+        return actor
+
+
+def find_nearest(array, value):
+    array = np.asarray(array)
+    idx = (np.abs(array - value)).argmin()
+    return idx
+
```

### Comparing `PyProcar-5.6.6/pyprocar/scriptSpin_asymmetry.py` & `PyProcar-6.0.0/pyprocar/scripts/scriptSpin_asymmetry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,234 +1,233 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Aug 18 11:14:17 2020
-
-@author: petavazohi
-"""
-
-import numpy as np
-import pyvista
-from matplotlib import colors as mpcolors
-from matplotlib import cm
-from .fermisurface3d import boolean_add
-from .fermisurface3d import FermiSurface3D
-from .splash import welcome
-from .fermisurface3d import FermiSurface3D
-from .utilsprocar import UtilsProcar
-from .procarparser import ProcarParser
-from .procarselect import ProcarSelect
-
-def spin_asymmetry(procar='PROCAR',
-                   outcar='OUTCAR',
-                   fermi=None,
-                   bands=None, 
-                   interpolation_factor=1,
-                   mode="plain",
-                   supercell=[1,1,1],
-                   colors=None,
-                   background_color='white',
-                   save_colors=None,
-                   cmap='viridis',
-                   atoms=None,
-                   orbitals=None,
-                   spin=None,
-                   spin_texture=False,
-                   arrow_color=None,
-                   arrow_size=0.015,
-                   only_spin=False,
-                   fermi_shift=0,
-                   projection_accuracy='normal',
-                   code='vasp',
-                   vmin=0, 
-                   vmax=1,
-                   savegif=None,
-                   savemp4=None,
-                   save3d=None,
-                   perspective=True,
-                   save2d=False,
-                   camera_pos=[1,1,1],
-                   widget=None,
-                   show=True,
-            ):
-    
-    
-    
-    
-    welcome()
-    
-    
-    if show:
-        p = pyvista.Plotter()
-    
-    if code=='vasp':
-        outcarparser = UtilsProcar()
-        if fermi is None:
-            e_fermi = outcarparser.FermiOutcar(outcar)
-        else:
-            e_fermi = fermi
-        reciprocal_lattice = outcarparser.RecLatOutcar(outcar)
-        procarFile = ProcarParser()
-        procarFile.readFile(procar, False)
-        data = ProcarSelect(procarFile, deepCopy=True)
-    if bands is None:
-        bands = np.arange(len(data.bands[0,:]))
-    surfaces = []
-    
-        
-        
-    spd = []        
-    if mode == 'parametric':
-        if orbitals is None:
-            orbitals = [-1]
-        if atoms is None:
-            atoms = [-1]
-        
-        spin = [0,1]
-        data.selectIspin(spin)
-        data.selectAtoms(atoms, fortran=False)
-        data.selectOrbital(orbitals)
-
-        for iband in bands:
-            spd.append(data.spd[:,iband])
-    else :
-        for iband in bands:
-            spd.append(None)
-
-    spd_spin=[]
-    
-    if spin_texture:
-        dataX = ProcarSelect(procarFile, deepCopy=True)
-        dataY = ProcarSelect(procarFile, deepCopy=True)
-        dataZ = ProcarSelect(procarFile, deepCopy=True)
-
-        dataX.kpoints = data.kpoints
-        dataY.kpoints = data.kpoints
-        dataZ.kpoints = data.kpoints
-
-        dataX.spd = data.spd
-        dataY.spd = data.spd
-        dataZ.spd = data.spd
-
-        dataX.bands = data.bands
-        dataY.bands = data.bands
-        dataZ.bands = data.bands
-
-        dataX.selectIspin([1])
-        dataY.selectIspin([2])
-        dataZ.selectIspin([3])
-
-        dataX.selectAtoms(atoms, fortran=False)
-        dataY.selectAtoms(atoms, fortran=False)
-        dataZ.selectAtoms(atoms, fortran=False)
-
-        dataX.selectOrbital(orbitals)
-        dataY.selectOrbital(orbitals)
-        dataZ.selectOrbital(orbitals)
-        for iband in bands:
-            spd_spin.append([dataX.spd[:,iband],dataY.spd[:,iband],dataZ.spd[:,iband]])
-    else:
-        for iband in bands:
-            spd_spin.append(None)
-    counter = 0
-    for iband in bands:
-        print("Trying to extract isosurface for band %d"%iband)
-        surface = FermiSurface3D(kpoints=data.kpoints,
-                                 band=data.bands[:,iband],
-                                 spd=spd[counter],
-                                 spd_spin=spd_spin[counter],
-                                 fermi=e_fermi+fermi_shift,
-                                 reciprocal_lattice=reciprocal_lattice,
-                                 interpolation_factor=interpolation_factor,
-                                 projection_accuracy=projection_accuracy,
-                                 supercell=supercell)
-        if surface.verts is not None:
-            surfaces.append(surface)       
-        counter+=1
-
-        
-        
-    nsurface = len(surfaces)
-    norm = mpcolors.Normalize(vmin=vmin, vmax=vmax)
-    cmap = cm.get_cmap(cmap)
-    scalars = np.arange(nsurface+1)/nsurface
-    if colors is None:
-        colors = np.array([cmap(norm(x)) for x in (scalars)]).reshape(-1,4)
-    
-    
-    if show or save2d:
-        # sargs = dict(interactive=True) 
-        p.add_mesh(surfaces[0].brillouin_zone.pyvista_obj,
-                    style='wireframe',line_width=3.5,color='black')
-        for isurface in range(nsurface):
-            if not only_spin:
-                if mode == 'plain':
-                    p.add_mesh(surfaces[isurface].pyvista_obj,
-                               color=colors[isurface])
-                    text='Colors'
-                elif mode =='parametric':
-                    p.add_mesh(surfaces[isurface].pyvista_obj,
-                               cmap=cmap,
-                               clim=[vmin,vmax])
-                    p.remove_scalar_bar()
-                    text='Projection'
-            else:
-                text='Spin Texture'
-            if spin_texture:
-                # Example dataset with normals
-                # create a subset of arrows using the glyph filter
-                arrows = surfaces[isurface].pyvista_obj.glyph(orient="vectors",factor=arrow_size)
-
-                if arrow_color is None:
-                    p.add_mesh(arrows,
-                               cmap=cmap,
-                               clim=[vmin,vmax])
-                    p.remove_scalar_bar()
-                else:
-                    p.add_mesh(arrows,
-                               color=arrow_color)
-
-        p.add_scalar_bar(title=text,
-                         n_labels=6,
-                         italic=False,
-                         bold=False,
-                         title_font_size=None,
-                         label_font_size=None,
-                         position_x=0.9,
-                         position_y=0.01,
-                         color='black')
-                
-        p.add_axes(xlabel='Kx',
-                   ylabel='Ky',
-                   zlabel='Kz',
-                   line_width=6,
-                   labels_off=False)
-
-        if not perspective :
-            p.enable_parallel_projection()
-        p.set_background(background_color)
-        p.set_position(camera_pos)
-        p.show(cpos=camera_pos,screenshot=save2d)
-        # p.screenshot('1.png')
-        # p.save_graphic('1.pdf')
-        if savegif is not None:
-            path = p.generate_orbital_path(n_points=36)
-            p.open_gif(savegif)
-            p.orbit_on_path(path)#,viewup=camera_pos)
-        if savemp4:
-            path = p.generate_orbital_path(n_points=36)
-            p.open_movie(savemp4)
-            p.orbit_on_path(path)#,viewup=camera_pos)
-            # p.close()        
-    if save_colors is None:
-        for i in range(nsurface):
-            if surfaces[i].scalars is None:
-                surfaces[i].set_scalars([scalars[i]]*surfaces[i].nfaces)
-    s = boolean_add(surfaces)
-    s.set_color_with_cmap(cmap=cmap,vmin=vmin,vmax=vmax)
-    # s.pyvista_obj.plot()
-    # s.trimesh_obj.show()
-    
-    if save3d is not None:
-        extention=save3d.split('.')[-1]
-        s.export(save3d,extention)
-    return s,surfaces
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Aug 18 11:14:17 2020
+
+@author: petavazohi
+"""
+
+import numpy as np
+import pyvista
+from matplotlib import colors as mpcolors
+from matplotlib import cm
+from ..core import boolean_add
+from ..core import FermiSurface3D
+from ..utils import welcome
+from ..utils import UtilsProcar
+from ..io import ProcarParser
+from ..core import ProcarSelect
+
+def spin_asymmetry(procar='PROCAR',
+                   outcar='OUTCAR',
+                   fermi=None,
+                   bands=None, 
+                   interpolation_factor=1,
+                   mode="plain",
+                   supercell=[1,1,1],
+                   colors=None,
+                   background_color='white',
+                   save_colors=None,
+                   cmap='viridis',
+                   atoms=None,
+                   orbitals=None,
+                   spin=None,
+                   spin_texture=False,
+                   arrow_color=None,
+                   arrow_size=0.015,
+                   only_spin=False,
+                   fermi_shift=0,
+                   projection_accuracy='normal',
+                   code='vasp',
+                   vmin=0, 
+                   vmax=1,
+                   savegif=None,
+                   savemp4=None,
+                   save3d=None,
+                   perspective=True,
+                   save2d=False,
+                   camera_pos=[1,1,1],
+                   widget=None,
+                   show=True,
+            ):
+    
+    
+    
+    
+    welcome()
+    
+    
+    if show:
+        p = pyvista.Plotter()
+    
+    if code=='vasp':
+        outcarparser = UtilsProcar()
+        if fermi is None:
+            e_fermi = outcarparser.FermiOutcar(outcar)
+        else:
+            e_fermi = fermi
+        reciprocal_lattice = outcarparser.RecLatOutcar(outcar)
+        procarFile = ProcarParser()
+        procarFile.readFile(procar, False)
+        data = ProcarSelect(procarFile, deepCopy=True)
+    if bands is None:
+        bands = np.arange(len(data.bands[0,:]))
+    surfaces = []
+    
+        
+        
+    spd = []        
+    if mode == 'parametric':
+        if orbitals is None:
+            orbitals = [-1]
+        if atoms is None:
+            atoms = [-1]
+        
+        spin = [0,1]
+        data.selectIspin(spin)
+        data.selectAtoms(atoms, fortran=False)
+        data.selectOrbital(orbitals)
+
+        for iband in bands:
+            spd.append(data.spd[:,iband])
+    else :
+        for iband in bands:
+            spd.append(None)
+
+    spd_spin=[]
+    
+    if spin_texture:
+        dataX = ProcarSelect(procarFile, deepCopy=True)
+        dataY = ProcarSelect(procarFile, deepCopy=True)
+        dataZ = ProcarSelect(procarFile, deepCopy=True)
+
+        dataX.kpoints = data.kpoints
+        dataY.kpoints = data.kpoints
+        dataZ.kpoints = data.kpoints
+
+        dataX.spd = data.spd
+        dataY.spd = data.spd
+        dataZ.spd = data.spd
+
+        dataX.bands = data.bands
+        dataY.bands = data.bands
+        dataZ.bands = data.bands
+
+        dataX.selectIspin([1])
+        dataY.selectIspin([2])
+        dataZ.selectIspin([3])
+
+        dataX.selectAtoms(atoms, fortran=False)
+        dataY.selectAtoms(atoms, fortran=False)
+        dataZ.selectAtoms(atoms, fortran=False)
+
+        dataX.selectOrbital(orbitals)
+        dataY.selectOrbital(orbitals)
+        dataZ.selectOrbital(orbitals)
+        for iband in bands:
+            spd_spin.append([dataX.spd[:,iband],dataY.spd[:,iband],dataZ.spd[:,iband]])
+    else:
+        for iband in bands:
+            spd_spin.append(None)
+    counter = 0
+    for iband in bands:
+        print("Trying to extract isosurface for band %d"%iband)
+        surface = FermiSurface3D(kpoints=data.kpoints,
+                                 band=data.bands[:,iband],
+                                 spd=spd[counter],
+                                 spd_spin=spd_spin[counter],
+                                 fermi=e_fermi+fermi_shift,
+                                 reciprocal_lattice=reciprocal_lattice,
+                                 interpolation_factor=interpolation_factor,
+                                 projection_accuracy=projection_accuracy,
+                                 supercell=supercell)
+        if surface.verts is not None:
+            surfaces.append(surface)       
+        counter+=1
+
+        
+        
+    nsurface = len(surfaces)
+    norm = mpcolors.Normalize(vmin=vmin, vmax=vmax)
+    cmap = cm.get_cmap(cmap)
+    scalars = np.arange(nsurface+1)/nsurface
+    if colors is None:
+        colors = np.array([cmap(norm(x)) for x in (scalars)]).reshape(-1,4)
+    
+    
+    if show or save2d:
+        # sargs = dict(interactive=True) 
+        p.add_mesh(surfaces[0].brillouin_zone.pyvista_obj,
+                    style='wireframe',line_width=3.5,color='black')
+        for isurface in range(nsurface):
+            if not only_spin:
+                if mode == 'plain':
+                    p.add_mesh(surfaces[isurface].pyvista_obj,
+                               color=colors[isurface])
+                    text='Colors'
+                elif mode =='parametric':
+                    p.add_mesh(surfaces[isurface].pyvista_obj,
+                               cmap=cmap,
+                               clim=[vmin,vmax])
+                    p.remove_scalar_bar()
+                    text='Projection'
+            else:
+                text='Spin Texture'
+            if spin_texture:
+                # Example dataset with normals
+                # create a subset of arrows using the glyph filter
+                arrows = surfaces[isurface].pyvista_obj.glyph(orient="vectors",factor=arrow_size)
+
+                if arrow_color is None:
+                    p.add_mesh(arrows,
+                               cmap=cmap,
+                               clim=[vmin,vmax])
+                    p.remove_scalar_bar()
+                else:
+                    p.add_mesh(arrows,
+                               color=arrow_color)
+
+        p.add_scalar_bar(title=text,
+                         n_labels=6,
+                         italic=False,
+                         bold=False,
+                         title_font_size=None,
+                         label_font_size=None,
+                         position_x=0.9,
+                         position_y=0.01,
+                         color='black')
+                
+        p.add_axes(xlabel='Kx',
+                   ylabel='Ky',
+                   zlabel='Kz',
+                   line_width=6,
+                   labels_off=False)
+
+        if not perspective :
+            p.enable_parallel_projection()
+        p.set_background(background_color)
+        p.set_position(camera_pos)
+        p.show(cpos=camera_pos,screenshot=save2d)
+        # p.screenshot('1.png')
+        # p.save_graphic('1.pdf')
+        if savegif is not None:
+            path = p.generate_orbital_path(n_points=36)
+            p.open_gif(savegif)
+            p.orbit_on_path(path)#,viewup=camera_pos)
+        if savemp4:
+            path = p.generate_orbital_path(n_points=36)
+            p.open_movie(savemp4)
+            p.orbit_on_path(path)#,viewup=camera_pos)
+            # p.close()        
+    if save_colors is None:
+        for i in range(nsurface):
+            if surfaces[i].scalars is None:
+                surfaces[i].set_scalars([scalars[i]]*surfaces[i].nfaces)
+    s = boolean_add(surfaces)
+    s.set_color_with_cmap(cmap=cmap,vmin=vmin,vmax=vmax)
+    # s.pyvista_obj.plot()
+    # s.trimesh_obj.show()
+    
+    if save3d is not None:
+        extention=save3d.split('.')[-1]
+        s.export(save3d,extention)
+    return s,surfaces
```

### Comparing `PyProcar-5.6.6/pyprocar/scriptVector.py` & `PyProcar-6.0.0/pyprocar/scripts/scriptVector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from .utilsprocar import UtilsProcar
-from .procarparser import ProcarParser
-from .procarselect import ProcarSelect
-from .procarplot import ProcarPlot
-from .fermisurface import FermiSurface
-from .splash import welcome
-
-
-def Vector(
-    infile,
-    bands=None,
-    energy=None,
-    fermi=None,
-    atoms=None,
-    orbitals=None,
-    outcar=None,
-    scale=0.1,
-    code="vasp",
-    repair=True,
-):
-
-    welcome()
-
-    if code == "vasp" or code == "abinit":
-        if repair:
-            repairhandle = UtilsProcar()
-            repairhandle.ProcarRepair(infile, infile)
-            print("PROCAR repaired. Run with repair=False next time.")
-
-    print("Input File    : ", infile)
-    print("Bands         : ", bands)
-    print("Energy        : ", energy)
-    print("Fermi         : ", fermi)
-    print("outcar        : ", outcar)
-    print("atoms         : ", atoms)
-    print("orbitals      : ", orbitals)
-    print("scale factor  : ", scale)
-
-    if bands is [] and energy is None:
-        raise RuntimeError("You must provide the bands or energy.")
-    if fermi == None and outcar == None:
-        print("WARNING: Fermi's Energy not set")
-
-    # first parse the outcar if given
-    recLat = None  # Will contain reciprocal vectors, if necessary
-    if outcar:
-        outcarparser = UtilsProcar()
-        if fermi is None:
-            fermi = outcarparser.FermiOutcar(outcar)
-            # if quiet is False:
-            print("Fermi energy found in outcar file = " + str(fermi))
-        recLat = outcarparser.RecLatOutcar(outcar)
-
-    if atoms is None:
-        atoms = [-1]
-    if orbitals is None:
-        orbitals = [-1]
-
-    # parsing the file
-    procarFile = ProcarParser()
-    procarFile.readFile(infile, recLattice=recLat)
-
-    # processing the data
-    sx = ProcarSelect(procarFile, deepCopy=True)
-    sx.selectIspin([1])
-    sx.selectAtoms(atoms)
-    sx.selectOrbital(orbitals)
-
-    sy = ProcarSelect(procarFile, deepCopy=True)
-    sy.selectIspin([2])
-    sy.selectAtoms(atoms)
-    sy.selectOrbital(orbitals)
-
-    sz = ProcarSelect(procarFile, deepCopy=True)
-    sz.selectIspin([3])
-    sz.selectAtoms(atoms)
-    sz.selectOrbital(orbitals)
-
-    x = sx.kpoints[:, 0]
-    y = sx.kpoints[:, 1]
-    z = sx.kpoints[:, 2]
-
-    # if energy was given I need to find the bands indexes crossing it
-    if energy != None:
-        FerSurf = FermiSurface(sx.kpoints, sx.bands - fermi, sx.spd)
-        FerSurf.FindEnergy(energy)
-        bands = list(FerSurf.useful[0])
-        print("Bands indexes crossing Energy  ", energy, ", are: ", bands)
-
-    from mayavi import mlab
-
-    fig = mlab.figure(bgcolor=(1, 1, 1))
-
-    for band in bands:
-        # z = sx.bands[:,band]-fermi
-        u = sx.spd[:, band]
-        v = sy.spd[:, band]
-        w = sz.spd[:, band]
-        scalar = w
-
-        vect = mlab.quiver3d(
-            x,
-            y,
-            z,
-            u,
-            v,
-            w,
-            scale_factor=scale,
-            scale_mode="vector",
-            scalars=scalar,
-            mode="arrow",
-            colormap="jet",
-        )
-        vect.glyph.color_mode = "color_by_scalar"
-        vect.scene.parallel_projection = True
-        vect.scene.z_plus_view()
-
-        # tube= mlab.plot3d(x,y,z, tube_radius=0.0050, color=(0.5,0.5,0.5))
-    mlab.show()
+from ..utils import UtilsProcar
+from ..io import ProcarParser
+from ..core import ProcarSelect
+from ..plotter import ProcarPlot
+from ..core.fermisurface import FermiSurface
+from ..utils import welcome
+
+
+def Vector(
+    infile,
+    bands=None,
+    energy=None,
+    fermi=None,
+    atoms=None,
+    orbitals=None,
+    outcar=None,
+    scale=0.1,
+    code="vasp",
+    repair=True,
+):
+
+    welcome()
+
+    if code == "vasp" or code == "abinit":
+        if repair:
+            repairhandle = UtilsProcar()
+            repairhandle.ProcarRepair(infile, infile)
+            print("PROCAR repaired. Run with repair=False next time.")
+
+    print("Input File    : ", infile)
+    print("Bands         : ", bands)
+    print("Energy        : ", energy)
+    print("Fermi         : ", fermi)
+    print("outcar        : ", outcar)
+    print("atoms         : ", atoms)
+    print("orbitals      : ", orbitals)
+    print("scale factor  : ", scale)
+
+    if bands is [] and energy is None:
+        raise RuntimeError("You must provide the bands or energy.")
+    if fermi == None and outcar == None:
+        print("WARNING: Fermi's Energy not set")
+
+    # first parse the outcar if given
+    recLat = None  # Will contain reciprocal vectors, if necessary
+    if outcar:
+        outcarparser = UtilsProcar()
+        if fermi is None:
+            fermi = outcarparser.FermiOutcar(outcar)
+            # if quiet is False:
+            print("Fermi energy found in outcar file = " + str(fermi))
+        recLat = outcarparser.RecLatOutcar(outcar)
+
+    if atoms is None:
+        atoms = [-1]
+    if orbitals is None:
+        orbitals = [-1]
+
+    # parsing the file
+    procarFile = ProcarParser()
+    procarFile.readFile(infile, recLattice=recLat)
+
+    # processing the data
+    sx = ProcarSelect(procarFile, deepCopy=True)
+    sx.selectIspin([1])
+    sx.selectAtoms(atoms)
+    sx.selectOrbital(orbitals)
+
+    sy = ProcarSelect(procarFile, deepCopy=True)
+    sy.selectIspin([2])
+    sy.selectAtoms(atoms)
+    sy.selectOrbital(orbitals)
+
+    sz = ProcarSelect(procarFile, deepCopy=True)
+    sz.selectIspin([3])
+    sz.selectAtoms(atoms)
+    sz.selectOrbital(orbitals)
+
+    x = sx.kpoints[:, 0]
+    y = sx.kpoints[:, 1]
+    z = sx.kpoints[:, 2]
+
+    # if energy was given I need to find the bands indexes crossing it
+    if energy != None:
+        FerSurf = FermiSurface(sx.kpoints, sx.bands - fermi, sx.spd)
+        FerSurf.FindEnergy(energy)
+        bands = list(FerSurf.useful[0])
+        print("Bands indexes crossing Energy  ", energy, ", are: ", bands)
+
+    from mayavi import mlab
+
+    fig = mlab.figure(bgcolor=(1, 1, 1))
+
+    for band in bands:
+        # z = sx.bands[:,band]-fermi
+        u = sx.spd[:, band]
+        v = sy.spd[:, band]
+        w = sz.spd[:, band]
+        scalar = w
+
+        vect = mlab.quiver3d(
+            x,
+            y,
+            z,
+            u,
+            v,
+            w,
+            scale_factor=scale,
+            scale_mode="vector",
+            scalars=scalar,
+            mode="arrow",
+            colormap="jet",
+        )
+        vect.glyph.color_mode = "color_by_scalar"
+        vect.scene.parallel_projection = True
+        vect.scene.z_plus_view()
+
+        # tube= mlab.plot3d(x,y,z, tube_radius=0.0050, color=(0.5,0.5,0.5))
+    mlab.show()
```

### Comparing `PyProcar-5.6.6/pyprocar/splash.py` & `PyProcar-6.0.0/pyprocar/utils/splash.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import pyprocar
-
-
-def welcome():
-    print(
-        " ____        ____\n|  _ \ _   _|  _ \ _ __ ___   ___ __ _ _ __ \n| |_) | | | | |_) | '__/ _ \ / __/ _` | '__|\n|  __/| |_| |  __/| | | (_) | (_| (_| | |   \n|_|    \__, |_|   |_|  \___/ \___\__,_|_|\n       |___/"
-    )
-    print("A Python library for electronic structure pre/post-processing.\n")
-    print("Version %s created on %s\n" % (pyprocar.__version__, pyprocar.__date__))
-    print(
-        "Please cite:\n \
-Uthpala Herath, Pedram Tavadze, Xu He, Eric Bousquet, Sobhit Singh, Francisco Muñoz and Aldo Romero.,\n \
-PyProcar: A Python library for electronic structure pre/post-processing.,\n \
-Computer Physics Communications 251 (2020):107080.\n"
-    )
-
-    dev_string = """
-Developers:
-- Francisco Muñoz
-- Aldo Romero
-- Sobhit Singh
-- Uthpala Herath
-- Pedram Tavadze
-- Eric Bousquet
-- Xu He
-- Reese Boucher
-- Logan Lang
-- Freddy Farah
-    """
-    print(dev_string)
-
-    return
+import pyprocar
+
+
+def welcome():
+    print(
+        " ____        ____\n|  _ \ _   _|  _ \ _ __ ___   ___ __ _ _ __ \n| |_) | | | | |_) | '__/ _ \ / __/ _` | '__|\n|  __/| |_| |  __/| | | (_) | (_| (_| | |   \n|_|    \__, |_|   |_|  \___/ \___\__,_|_|\n       |___/"
+    )
+    print("A Python library for electronic structure pre/post-processing.\n")
+    print("Version %s created on %s\n" % (pyprocar.__version__, pyprocar.__date__))
+    print(
+        "Please cite:\n \
+Uthpala Herath, Pedram Tavadze, Xu He, Eric Bousquet, Sobhit Singh, Francisco Muñoz and Aldo Romero.,\n \
+PyProcar: A Python library for electronic structure pre/post-processing.,\n \
+Computer Physics Communications 251 (2020):107080.\n"
+    )
+
+    dev_string = """
+Developers:
+- Francisco Muñoz
+- Aldo Romero
+- Sobhit Singh
+- Uthpala Herath
+- Pedram Tavadze
+- Eric Bousquet
+- Xu He
+- Reese Boucher
+- Logan Lang
+- Freddy Farah
+    """
+    print(dev_string)
+
+    return
```

### Comparing `PyProcar-5.6.6/pyprocar/utils/mathematics.py` & `PyProcar-6.0.0/pyprocar/utils/mathematics.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-# -*- coding: utf-8 -*-
-
-import numpy as np
-
-
-def get_angle(v, w, radians=False):
-    """
-    Calculates angle between two vectors
-
-    Parameters
-    ----------
-    v : float
-        vector 1.
-    w : float
-        vector 1.
-    radians : bool, optional
-        To return the result in radians or degrees. The default is False.
-
-    Returns
-    -------
-    float
-        Angle between v and w.
-
-    """
-
-    if np.linalg.norm(v) == 0 or np.linalg.norm(w) == 0 or np.all(v == w):
-        return 0
-    cosine = np.dot(v, w) / (np.linalg.norm(v) * np.linalg.norm(w))
-
-    if radians:
-        return np.arccos(cosine)
-    else:
-        return np.rad2deg(np.arccos(cosine))
-
-
-
-def fft_interpolate(function, interpolation_factor=2, axis=None):
-    """
-
-
-    Parameters
-    ----------
-    function : TYPE
-        DESCRIPTION.
-    interpolation_factor : TYPE, optional
-        DESCRIPTION. The default is 2.
-    axis : TYPE, optional
-        DESCRIPTION. The default is None.
-
-    Returns
-    -------
-    interpolated : TYPE
-        DESCRIPTION.
-
-    """
-
-    if axis is None:
-        axis = np.arange(function.ndim)
-    if type(axis) is int:
-        axis = [axis]
-    function = np.array(function)
-    eigen_fft = np.fft.fftn(function)
-    shifted_fft = np.fft.fftshift(eigen_fft)
-    pad_width = []
-    factor = 0
-    for idim in range(function.ndim):
-        if idim in axis:
-            n = shifted_fft.shape[idim]
-            pad = n * (interpolation_factor - 1) // 2
-            factor += 1
-        else:
-            pad = 0
-        pad_width.append([pad, pad])
-    new_matrix = np.pad(shifted_fft, pad_width, "constant", constant_values=0)
-    new_matrix = np.fft.ifftshift(new_matrix)
-    if "complex" in function.dtype.name:
-        interpolated = np.fft.ifftn(new_matrix) * (interpolation_factor * factor)
-    else:
-        interpolated = np.real(np.fft.ifftn(new_matrix)) * (
-            interpolation_factor * factor
-        )
-    return interpolated
+# -*- coding: utf-8 -*-
+
+import numpy as np
+
+
+def get_angle(v, w, radians=False):
+    """
+    Calculates angle between two vectors
+
+    Parameters
+    ----------
+    v : float
+        vector 1.
+    w : float
+        vector 1.
+    radians : bool, optional
+        To return the result in radians or degrees. The default is False.
+
+    Returns
+    -------
+    float
+        Angle between v and w.
+
+    """
+
+    if np.linalg.norm(v) == 0 or np.linalg.norm(w) == 0 or np.all(v == w):
+        return 0
+    cosine = np.dot(v, w) / (np.linalg.norm(v) * np.linalg.norm(w))
+
+    if radians:
+        return np.arccos(cosine)
+    else:
+        return np.rad2deg(np.arccos(cosine))
+
+
+
+def fft_interpolate(function, interpolation_factor=2, axis=None):
+    """
+
+
+    Parameters
+    ----------
+    function : TYPE
+        DESCRIPTION.
+    interpolation_factor : TYPE, optional
+        DESCRIPTION. The default is 2.
+    axis : TYPE, optional
+        DESCRIPTION. The default is None.
+
+    Returns
+    -------
+    interpolated : TYPE
+        DESCRIPTION.
+
+    """
+
+    if axis is None:
+        axis = np.arange(function.ndim)
+    if type(axis) is int:
+        axis = [axis]
+    function = np.array(function)
+    eigen_fft = np.fft.fftn(function)
+    shifted_fft = np.fft.fftshift(eigen_fft)
+    pad_width = []
+    factor = 0
+    for idim in range(function.ndim):
+        if idim in axis:
+            n = shifted_fft.shape[idim]
+            pad = n * (interpolation_factor - 1) // 2
+            factor += 1
+        else:
+            pad = 0
+        pad_width.append([pad, pad])
+    new_matrix = np.pad(shifted_fft, pad_width, "constant", constant_values=0)
+    new_matrix = np.fft.ifftshift(new_matrix)
+    if "complex" in function.dtype.name:
+        interpolated = np.fft.ifftn(new_matrix) * (interpolation_factor * factor)
+    else:
+        interpolated = np.real(np.fft.ifftn(new_matrix)) * (
+            interpolation_factor * factor
+        )
+    return interpolated
```

### Comparing `PyProcar-5.6.6/pyprocar/utilsprocar/scriptFermi3D.py` & `PyProcar-6.0.0/pyprocar/utils/scriptFermi3D.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,786 +1,786 @@
-"""
-Created on Fri May 10 16:23:30 2019
-
-@author: Pedram Tavadze
-
-"""
-
-from .utilsprocar import UtilsProcar
-from .procarparser import ProcarParser
-from .procarselect import ProcarSelect
-import numpy as np
-from scipy.spatial import ConvexHull
-from scipy.spatial import Voronoi
-from skimage import measure
-from multiprocessing import Pool
-import scipy.interpolate as interpolate
-from .splash import welcome
-
-
-def get_wigner_seitz(recLat):
-    kpoints = []
-    for i in range(-1, 2):
-        for j in range(-1, 2):
-            for k in range(-1, 2):
-                vec = i * recLat[0] + j * recLat[1] + k * recLat[2]
-                kpoints.append(vec)
-    brill = Voronoi(np.array(kpoints))
-    faces = []
-    for idict in brill.ridge_dict:
-        if idict[0] == 13 or idict[1] == 13:
-            faces.append(brill.ridge_dict[idict])
-    verts = brill.vertices
-    poly = []
-    for ix in range(len(faces)):
-        temp = []
-        for iy in range(len(faces[ix])):
-            temp.append(verts[faces[ix][iy]])
-        poly.append(np.array(temp))
-    return np.array(poly)
-
-
-def mapping_func(kpoints, bands):
-    kx = np.unique(kpoints[:, 0])
-    ky = np.unique(kpoints[:, 1])
-    kz = np.unique(kpoints[:, 2])
-    mapped_func = np.zeros(shape=(len(kx), len(ky), len(kz)))
-    kpoint_matrix = np.zeros(shape=(len(kx), len(ky), len(kz), 3))
-    for ikx in range(len(kx)):
-        cond1 = kpoints[:, 0] == kx[ikx]
-        for iky in range(len(ky)):
-            cond2 = kpoints[:, 1] == ky[iky]
-            for ikz in range(len(kz)):
-                cond3 = kpoints[:, 2] == kz[ikz]
-                tot_cond = np.all([cond1, cond2, cond3], axis=0)
-                if len(bands[tot_cond]) != 0:
-                    mapped_func[ikx, iky, ikz] = bands[tot_cond][0]
-                    kpoint_matrix[ikx, iky, ikz] = [kx[ikx], ky[iky], kz[ikz]]
-                else:
-                    mapped_func[ikx, iky, ikz] = np.nan
-                    kpoint_matrix[ikx, iky, ikz] = [np.nan, np.nan, np.nan]
-
-    return mapped_func, kpoint_matrix
-
-
-# if the grid is gamma centered the gird would be something like [-0.45,-0.35,...,0,...,0.5]
-# using FFT interpolate we will loose center. The fermi surface will not be symmetric with
-# respect to the center. To avoid this we will add the points from 0.5 to -0.5 so the mesh will be like
-# [-0.5,-0.45,..,0,...,0.45,0.5]
-def symmetrize(data):
-    # kpoints with one 0.5
-    idx = (data.kpoints == 0.5).sum(axis=1) == 1
-    #    idx = np.any(data.kpoints == 0.5,axis=1)
-    kpoints_toAdd = data.kpoints[idx] + (data.kpoints[idx] == 0.5).astype(int) * -1
-    bands_toAdd = data.bands[idx]
-    spd_toAdd = data.spd[idx]
-    # kpoints with two 0.5
-    # -0.5,-0.5
-    idx = (data.kpoints == 0.5).sum(axis=1) == 2
-    kpoints_temp = data.kpoints[idx] + (data.kpoints[idx] == 0.5).astype(int) * -1
-    bands_temp = data.bands[idx]
-    spd_temp = data.spd[idx]
-
-    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
-    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
-    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
-    # [0.5,:,:]
-    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 0])] - [1, 0, 0]
-    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 0])]
-    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 0])]
-    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
-    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
-    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
-    # [:,0.5,:]
-    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 1])] - [0, 1, 0]
-    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 1])]
-    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 1])]
-    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
-    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
-    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
-    # [:,:,0.5]
-    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 2])] - [0, 0, 1]
-    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 2])]
-    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 2])]
-    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
-    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
-    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
-    # kpoints with three 0.5
-    idx = (data.kpoints == 0.5).sum(axis=1) == 3
-    kpoints_temp = np.array(
-        [(x, y, z) for x in [-0.5, 0.5] for y in [-0.5, 0.5] for z in [-0.5, 0.5]]
-    )[:-1]
-    bands_temp = np.repeat(data.bands[idx], 7, axis=0)
-    spd_temp = np.repeat(data.spd[idx], 7, axis=0)
-    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
-    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
-    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
-
-    data.kpoints = np.append(data.kpoints, kpoints_toAdd, axis=0)
-    data.bands = np.append(data.bands, bands_toAdd, axis=0)
-    data.spd = np.append(data.spd, spd_toAdd, axis=0)
-    return data
-
-
-def bring_pnts_to_BZ(recLat, kvector_cart, kvector_red, br_points):
-    outsides = []
-    directions = []
-    # This section finds points that are outside of the 1st BZ and and creates those points in the 1st BZ
-    movements = np.array(
-        [
-            recLat[0],
-            recLat[1],
-            recLat[2],
-            -1 * recLat[0],
-            -1 * recLat[1],
-            -1 * recLat[2],
-        ]
-    )
-    for ik in range(len(kvector_cart)):
-        ik_copy = kvector_cart[ik][:]
-        idirection = 0
-        was_outside = False
-        while is_outside([br_points, ik_copy]) and idirection < 6:
-            ik_copy = kvector_cart[ik] + movements[idirection]
-            idirection += 1
-            was_outside = True
-        if was_outside:
-            outsides.append(kvector_red[ik])
-            directions.append(
-                np.dot(movements[idirection - 1], np.linalg.pinv(recLat)).round(2)
-            )
-        kvector_cart[ik] = ik_copy[:]
-        kvector_red[ik] = np.dot(ik_copy, np.linalg.pinv(recLat)).round(2)
-    if len(outsides):
-        has_points_out = True
-    else:
-        has_points_out = False
-    return kvector_cart, kvector_red, has_points_out
-
-
-def fft_interpolate(function, scale):
-    eigen_fft = np.fft.fftn(function)
-    shifted_fft = np.fft.fftshift(eigen_fft)
-    nx, ny, nz = np.array(shifted_fft.shape)
-    pad_x = nx * (scale - 1) // 2
-    pad_y = ny * (scale - 1) // 2
-    pad_z = nz * (scale - 1) // 2
-    new_matrix = np.pad(
-        shifted_fft,
-        ((pad_x, pad_x), (pad_y, pad_y), (pad_z, pad_z)),
-        "constant",
-        constant_values=0,
-    )
-
-    new_matrix = np.fft.ifftshift(new_matrix)
-    interpolated = np.real(np.fft.ifftn(new_matrix)) * (scale ** 3)
-    return interpolated
-
-
-def is_outside(args):
-    br_points = args[0]
-    point = args[1]
-    Hull1 = ConvexHull(br_points)
-    added_points = np.append(br_points, [point], axis=0)
-    Hull2 = ConvexHull(added_points)
-    if len(Hull2.vertices) == len(Hull1.vertices):
-        if sum(Hull2.vertices - Hull1.vertices) != 0:
-            return True
-    else:
-        return True
-    return False
-
-
-def to_remove(args):
-    faces = args[0]
-    vert = args[1]
-    return np.any(faces == vert, axis=1)
-
-
-def fermi3D(procar, outcar, bands=-1, scale=1, mode="plain", st=False, **kwargs):
-    """
-    This function plots 3d fermi surface
-    list of acceptable kwargs :
-        plotting_package
-        nprocess
-        face_colors
-        arrow_colors 
-        arrow_spin
-        atom
-        orbital
-        spin
-        
-    """
-    welcome()
-
-    # Initilizing the arguments :
-
-    if "plotting_package" in kwargs:
-        plotting_package = kwargs["plotting_package"]
-    else:
-        plotting_package = "mayavi"
-
-    if "nprocess" in kwargs:
-        nprocess = kwargs["nprocess"]
-    else:
-        nprocess = 2
-
-    if "face_colors" in kwargs:
-        face_colors = kwargs["face_colors"]
-    else:
-        face_colors = None
-    if "cmap" in kwargs:
-        cmap = kwargs["cmap"]
-    else:
-        cmap = "jet"
-    if "atoms" in kwargs:
-        atoms = kwargs["atoms"]
-    else:
-        atoms = [-1]  # project all atoms
-    if "orbitals" in kwargs:
-        orbitals = kwargs["orbitals"]
-    else:
-        orbitals = [-1]
-
-    if "spin" in kwargs:
-        spin = kwargs["spin"]
-    else:
-        spin = [0]
-    if "mask_points" in kwargs:
-        mask_points = kwargs["mask_points"]
-    else:
-        mask_points = 1
-    if "energy" in kwargs:
-        energy = kwargs["energy"]
-    else:
-        energy = 0
-    if "transparent" in kwargs:
-        transparent = kwargs["transparent"]
-    else:
-        transparent = False
-
-    if "arrow_projection" in kwargs:
-        arrow_projection = kwargs["arrow_projection"]
-    else:
-        arrow_projection = 2
-
-    if plotting_package == "mayavi":
-        try:
-            from mayavi import mlab
-            from tvtk.api import tvtk
-        except:
-            print(
-                "You have selected mayavi as plottin package. please install mayavi and tvtk or choose a different package"
-            )
-            return
-    elif plotting_package == "plotly":
-        try:
-            import plotly.plotly as py
-            import plotly.figure_factory as ff
-            import plotly.graph_objs as go
-            
-            cmap = mpl.cm.get_cmap(cmap)
-            figs = []
-
-        except:
-            print(
-                "You have selected plotly as plottin package. please install plotly or choose a different package"
-            )
-            return
-    elif plotting_package == "matplotlib":
-        try:
-            import matplotlib.pylab as plt
-            from mpl_toolkits.mplot3d.art3d import Poly3DCollection
-        except:
-            print(
-                "You have selected matplotlib as plotting package. please install matplotlib or choose a different package"
-            )
-            return
-    elif plotting_package == "ipyvolume":
-        try:
-            import ipyvolume.pylab as ipv
-        except:
-            print(
-                "You have selected ipyvolume as plotting package. please install ipyvolume or choose a different package"
-            )
-            return
-    if mode == 'colorful' :
-        face_colors = [(1, 0, 0),
-                       (0, 1, 0),
-                       (0, 0, 1),
-                       (1, 1, 0),
-                       (0, 1, 1),
-                       (1, 0, 1),
-                       (192/255, 192/255, 192/255),
-                       (128/255, 128/255, 128/255),
-                       (128/255, 0, 0),
-                       (128/255, 128/255, 0),
-                       (0, 128/255, 0),
-                       (128/255, 0, 128/255),
-                       (0, 128/255, 128/255),
-                       (0, 0, 128/255)]
-
-    permissive = False
-
-    # get fermi from outcar
-    outcarparser = UtilsProcar()
-    e_fermi = outcarparser.FermiOutcar(outcar)
-    print("Fermi=", e_fermi)
-    e_fermi += energy
-    # get reciprocal lattice from outcar
-    recLat = outcarparser.RecLatOutcar(outcar)
-
-    # parsing the Procar file
-    procarFile = ProcarParser()
-    procarFile.readFile(procar, permissive)
-
-    poly = get_wigner_seitz(recLat)
-    # plot brilliouin zone
-    if plotting_package == "mayavi":
-        brillouin_point = []
-        brillouin_faces = []
-        point_count = 0
-        for iface in poly:
-            single_face = []
-            for ipoint in iface:
-                single_face.append(point_count)
-                brillouin_point.append(list(ipoint))
-                point_count += 1
-            brillouin_faces.append(single_face)
-        polydata_br = tvtk.PolyData(points=brillouin_point, polys=brillouin_faces)
-        mlab.figure(figure=None, bgcolor=(1,1,1), fgcolor=None, engine=None, size=(400, 350))
-        mlab.pipeline.surface(
-            polydata_br,
-            representation="wireframe",
-            color=(0, 0, 0),
-            line_width=4,
-            name="BRZ",
-        )
-    elif plotting_package == "plotly":
-
-        for iface in poly:
-            iface = np.pad(iface, ((0, 1), (0, 0)), "wrap")
-            x, y, z = iface[:, 0], iface[:, 1], iface[:, 2]
-            plane = go.Scatter3d(
-                x=x, y=y, z=z, mode="lines", line=dict(color="black", width=4)
-            )
-            figs.append(plane)
-
-    elif plotting_package == "matplotlib":
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection="3d")
-        brillouin_zone = Poly3DCollection(
-            poly, facecolors=["None"] * len(poly), alpha=1, linewidth=4
-        )
-        brillouin_zone.set_edgecolor("k")
-        ax.add_collection3d(brillouin_zone, zs=0, zdir="z")
-
-    br_points = []
-    for iface in poly:
-        for ipoint in iface:
-            br_points.append(ipoint)
-    br_points = np.unique(br_points, axis=0)
-    print("Number of bands: %d" % procarFile.bandsCount)
-    print("Number of koints %d" % procarFile.kpointsCount)
-    print("Number of ions: %d" % procarFile.ionsCount)
-    print("Number of orbitals: %d" % procarFile.orbitalCount)
-    print("Number of spins: %d" % procarFile.ispin)
-
-    # selecting the data
-    data = ProcarSelect(procarFile, deepCopy=True)
-    if bands == -1:
-        bands = range(data.bands.shape[1])
-
-    kvector = data.kpoints
-    kmax = np.max(kvector)
-    kmin = np.min(kvector)
-
-    if abs(kmax) != abs(kmin):
-        print("The mesh provided is gamma center, symmetrizing data")
-        print("For a better fermi surface, use a non-gamma centered k-mesh")
-        data = symmetrize(data)
-        kvector = data.kpoints
-
-    kvector_red = data.kpoints.copy()
-    kvector_cart = np.dot(kvector_red, recLat)
-
-    # This section finds points that are outside of the 1st BZ and and creates those points in the 1st BZ
-    kvector_cart, kvector_red, has_points_out = bring_pnts_to_BZ(
-        recLat, kvector_cart, kvector_red, br_points
-    )
-    #    has_points_out = False
-
-    # getting the mesh grid in each dirrection
-    kx_red = np.unique(kvector_red[:, 0])
-    ky_red = np.unique(kvector_red[:, 1])
-    kz_red = np.unique(kvector_red[:, 2])
-
-    # getting the lengths between kpoints in each direction
-    klength_x = np.abs(kx_red[-1] - kx_red[-2])
-    klength_y = np.abs(ky_red[-1] - ky_red[-2])
-    klength_z = np.abs(kz_red[-1] - kz_red[-2])
-    klengths = [klength_x, klength_y, klength_z]
-
-    # getting number of kpoints in each direction with the addition of kpoints needed to sample the 1st BZ fully (in reduced)
-    nkx_red = kx_red.shape[0]
-    nky_red = ky_red.shape[0]
-    nkz_red = kz_red.shape[0]
-
-    # getting numner of kpoints in each direction provided by vasp
-    nkx_orig = np.unique(kvector[:, 0]).shape[0]
-    nky_orig = np.unique(kvector[:, 1]).shape[0]
-    nkz_orig = np.unique(kvector[:, 2]).shape[0]
-
-    # Amount of kpoints needed to add on to fully sample 1st BZ
-    padding_x = (nkx_red - nkx_orig) // 2
-    padding_y = (nky_red - nky_orig) // 2
-    padding_z = (nkz_red - nkz_orig) // 2
-
-    if mode == "parametric":
-        data.selectIspin(spin)
-        data.selectAtoms(atoms, fortran=False)
-        data.selectOrbital(orbitals)
-    elif mode == "external":
-        if "color_file" in kwargs:
-            rf = open(kwargs["color_file"])
-
-            lines = rf.readlines()
-            counter = 0
-            color_kvector = []
-            color_eigen = []
-            for iline in lines:
-                if counter < 2:
-                    if "band" in iline:
-                        counter += 1
-                        continue
-                    temp = [float(x) for x in iline.split()]
-                    color_kvector.append([temp[0], temp[1], temp[2]])
-            counter = -1
-            for iline in lines:
-                if "band" in iline:
-                    counter += 1
-                    iband = int(iline.split()[-1])
-                    color_eigen.append([])
-                    continue
-                color_eigen[counter].append(float(iline.split()[-1]))
-            rf.close()
-
-            color_kvector = np.array(color_kvector)
-            color_kvector_red = color_kvector.copy()
-            color_kvector_cart = np.dot(color_kvector, recLat)
-            if has_points_out:
-
-                color_kvector_cart, color_kvector_red, temp = bring_pnts_to_BZ(
-                    recLat, color_kvector_cart, color_kvector_red, br_points
-                )
-        else:
-            print("mode selected was external, but no color_file name was provided")
-            return
-    if st:
-
-        dataX = ProcarSelect(procarFile, deepCopy=True)
-        dataY = ProcarSelect(procarFile, deepCopy=True)
-        dataZ = ProcarSelect(procarFile, deepCopy=True)
-
-        dataX.kpoints = data.kpoints
-        dataY.kpoints = data.kpoints
-        dataZ.kpoints = data.kpoints
-
-        dataX.spd = data.spd
-        dataY.spd = data.spd
-        dataZ.spd = data.spd
-
-        dataX.bands = data.bands
-        dataY.bands = data.bands
-        dataZ.bands = data.bands
-
-        dataX.selectIspin([1])
-        dataY.selectIspin([2])
-        dataZ.selectIspin([3])
-
-        dataX.selectAtoms(atoms, fortran=False)
-        dataY.selectAtoms(atoms, fortran=False)
-        dataZ.selectAtoms(atoms, fortran=False)
-
-        dataX.selectOrbital(orbitals)
-        dataY.selectOrbital(orbitals)
-        dataZ.selectOrbital(orbitals)
-    ic = 0
-    for iband in bands:
-
-        print("Plotting band %d" % iband)
-
-        eigen = data.bands[:, iband]
-
-        # mapping the eigen values on the mesh grid to a matrix
-        mapped_func, kpoint_matrix = mapping_func(kvector, eigen)
-
-        # adding the points from the 2nd BZ to 1st BZ to fully sample the BZ. Check np.pad("wrap") for more information
-        mapped_func = np.pad(
-            mapped_func,
-            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
-            "wrap",
-        )
-
-        # Fourier interpolate the mapped function E(x,y,z)
-        surf_equation = fft_interpolate(mapped_func, scale)
-
-        # after the FFT we loose the center of the BZ, using numpy roll we bring back the center of the BZ
-        surf_equation = np.roll(surf_equation, (scale) // 2, axis=[0, 1, 2])
-
-        try:
-            # creating the isosurface if possible
-            verts, faces, normals, values = measure.marching_cubes_lewiner(
-                surf_equation, e_fermi
-            )
-
-        except:
-
-            print("No isosurface for this band")
-            continue
-        # the vertices provided are scaled and shifted to start from zero
-        # we center them to zero, and rescale them to fit the real BZ by multiplying by the klength in each direction
-        for ix in range(3):
-            verts[:, ix] -= verts[:, ix].min()
-            verts[:, ix] -= (verts[:, ix].max() - verts[:, ix].min()) / 2
-            verts[:, ix] *= klengths[ix] / scale
-
-        # the vertices need to be transformed to reciprocal spcae from recuded space, to find the points that are
-        # in 2nd BZ, to be removed
-        verts = np.dot(verts, recLat)
-
-        # identifying the points in 2nd BZ and removing them
-        if has_points_out:
-            args = []
-            for ivert in range(len(verts)):
-                args.append([br_points, verts[ivert]])
-
-            p = Pool(nprocess)
-            results = np.array(p.map(is_outside, args))
-            p.close()
-            out_verts = np.arange(0, len(results))[results]
-            new_faces = []
-            #            outs_bool_mat = np.zeros(shape=faces.shape,dtype=np.bool)
-
-            for iface in faces:
-                remove = False
-                for ivert in iface:
-                    if ivert in out_verts:
-                        remove = True
-
-                        continue
-
-                if not remove:
-                    new_faces.append(iface)
-            faces = np.array(new_faces)
-
-        print("done removing")
-        # At this point we have the plain Fermi surface, we can color the surface depending on the projection
-        # We create the center of faces by averaging coordinates of corners
-
-        if mode == "parametric":
-
-            character = data.spd[:, iband]
-
-            centers = np.zeros(shape=(len(faces), 3))
-            for iface in range(len(faces)):
-                centers[iface, 0:3] = np.average(verts[faces[iface]], axis=0)
-
-            colors = interpolate.griddata(
-                kvector_cart, character, centers, method="nearest"
-            )
-        elif mode == "external":
-            character = np.array(color_eigen[ic])
-            ic += 1
-            centers = np.zeros(shape=(len(faces), 3))
-            for iface in range(len(faces)):
-                centers[iface, 0:3] = np.average(verts[faces[iface]], axis=0)
-
-            colors = interpolate.griddata(
-                color_kvector_cart, character, centers, method="nearest"
-            )
-
-        if st:
-            projection_x = dataX.spd[:, iband]
-            projection_y = dataY.spd[:, iband]
-            projection_z = dataZ.spd[:, iband]
-
-            verts_spin, faces_spin, normals, values = measure.marching_cubes_lewiner(
-                mapped_func, e_fermi
-            )
-
-            for ix in range(3):
-                verts_spin[:, ix] -= verts_spin[:, ix].min()
-                verts_spin[:, ix] -= (
-                    verts_spin[:, ix].max() - verts_spin[:, ix].min()
-                ) / 2
-                verts_spin[:, ix] *= klengths[ix]
-            verts_spin = np.dot(verts_spin, recLat)
-
-            if has_points_out:
-                args = []
-                for ivert in range(len(verts_spin)):
-                    args.append([br_points, verts_spin[ivert]])
-
-                p = Pool(nprocess)
-                results = np.array(p.map(is_outside, args))
-                p.close()
-                out_verts = np.arange(0, len(results))[results]
-
-                new_faces = []
-                for iface in faces_spin:
-                    remove = False
-                    for ivert in iface:
-                        if ivert in out_verts:
-                            remove = True
-                            continue
-                    if not remove:
-                        new_faces.append(iface)
-                faces_spin = np.array(new_faces)
-
-            centers = np.zeros(shape=(len(faces_spin), 3))
-            for iface in range(len(faces_spin)):
-                centers[iface, 0:3] = np.average(verts_spin[faces_spin[iface]], axis=0)
-
-            colors1 = interpolate.griddata(
-                kvector_cart, projection_x, centers, method="linear"
-            )
-            colors2 = interpolate.griddata(
-                kvector_cart, projection_y, centers, method="linear"
-            )
-            colors3 = interpolate.griddata(
-                kvector_cart, projection_z, centers, method="linear"
-            )
-            spin_arrows = np.vstack((colors1, colors2, colors3)).T
-
-        if plotting_package == "mayavi":
-            polydata = tvtk.PolyData(points=verts, polys=faces)
-
-            if face_colors != None:
-                mlab.pipeline.surface(
-                    polydata,
-                    representation="surface",
-                    color=face_colors[ic],
-                    opacity=1,
-                    name="band-" + str(iband),
-                )
-                ic += 1
-            else:
-                if mode == "plain":
-                    if not (transparent):
-                        s = mlab.pipeline.surface(
-                            polydata,
-                            representation="surface",
-                            color=(0, 0.5, 1),
-                            opacity=1,
-                            name="band-" + str(iband),
-                        )
-
-
-                elif mode == "parametric" or mode == "external":
-
-                    polydata.cell_data.scalars = colors
-                    polydata.cell_data.scalars.name = "celldata"
-                    mlab.pipeline.surface(
-                        polydata, vmin=0, vmax=colors.max(), colormap=cmap
-                    )
-                    cb = mlab.colorbar(orientation="vertical")
-
-            if st:
-                x, y, z = list(zip(*centers))
-                u, v, w = list(zip(*spin_arrows))
-
-                pnts = mlab.quiver3d(
-                    x,
-                    y,
-                    z,
-                    u,
-                    v,
-                    w,
-                    line_width=5,
-                    mode="arrow",
-                    resolution=25,
-                    reset_zoom=False,
-                    name="spin-" + str(iband),
-                    mask_points=mask_points,
-                    scalars=spin_arrows[:, arrow_projection],
-                    vmin=-1,
-                    vmax=1,
-                    colormap=cmap,
-                )
-                pnts.glyph.color_mode = "color_by_scalar"
-                pnts.glyph.glyph_source.glyph_source.shaft_radius = 0.05
-                pnts.glyph.glyph_source.glyph_source.tip_radius = 0.1
-
-        elif plotting_package == "plotly":
-            if mode == "plain":
-                if not (transparent):
-                    x, y, z = zip(*verts)
-                    fig = ff.create_trisurf(
-                        x=x,
-                        y=y,
-                        z=z,
-                        plot_edges=False,
-                        simplices=faces,
-                        title="band-%d" % ic,
-                    )
-
-                    figs.append(fig["data"][0])
-
-            elif mode == "parametric" or mode == "external":
-
-                face_colors = cmap(colors)
-                colormap = [
-                    "rgb(%i,%i,%i)" % (x[0], x[1], x[2])
-                    for x in (face_colors * 255).round()
-                ]
-                x, y, z = zip(*verts)
-                fig = ff.create_trisurf(
-                    x=x,
-                    y=y,
-                    z=z,
-                    plot_edges=False,
-                    colormap=colormap,
-                    simplices=faces,
-                    show_colorbar=True,
-                    title="band-%d" % ic,
-                )
-
-                figs.append(fig["data"][0])
-        elif plotting_package == "matplotlib":
-            if mode == "plain":
-                x, y, z = zip(*verts)
-                ax.plot_trisurf(x, y, faces, z, linewidth=0.2, antialiased=True)
-            elif mode == "parametric" or mode == "external":
-                print(
-                    "coloring the faces is not implemented in matplot lib, please use another plotting package.we recomend mayavi."
-                )
-        elif plotting_package == "ipyvolume":
-            if mode == "plain":
-                ipv.figure()
-                ipv.plot_trisurf(verts[:, 0], verts[:, 1], verts[:, 2], triangles=faces)
-
-            elif mode == "paramteric" or mode == "external":
-                face_colors = cmap(colors)
-                colormap = [
-                    "rgb(%i,%i,%i)" % (x[0], x[1], x[2])
-                    for x in (face_colors * 255).round()
-                ]
-                ipv.figure()
-                ipv.plot_trisurf(
-                    verts[:, 0], verts[:, 1], verts[:, 2], triangles=faces, color=cmap
-                )
-
-    # if plotting_package == "mayavi":
-    #     mlab.colorbar(orientation="vertical") 
-    #     mlab.show()
-    # elif plotting_package == "plotly":
-    #     layout = go.Layout(showlegend=False)
-
-    #     fig = go.Figure(data=figs, layout=layout)
-    #     py.iplot(fig)
-    # elif plotting_package == "matplotlib":
-    #     plt.show()
-    # elif plotting_package == "ipyvolume":
-    #     ipv.show()
-
-    return
+"""
+Created on Fri May 10 16:23:30 2019
+
+@author: Pedram Tavadze
+
+"""
+
+from ..utils import UtilsProcar
+from ..io import ProcarParser
+from ..core import ProcarSelect
+import numpy as np
+from scipy.spatial import ConvexHull
+from scipy.spatial import Voronoi
+from skimage import measure
+from multiprocessing import Pool
+import scipy.interpolate as interpolate
+from .splash import welcome
+
+
+def get_wigner_seitz(recLat):
+    kpoints = []
+    for i in range(-1, 2):
+        for j in range(-1, 2):
+            for k in range(-1, 2):
+                vec = i * recLat[0] + j * recLat[1] + k * recLat[2]
+                kpoints.append(vec)
+    brill = Voronoi(np.array(kpoints))
+    faces = []
+    for idict in brill.ridge_dict:
+        if idict[0] == 13 or idict[1] == 13:
+            faces.append(brill.ridge_dict[idict])
+    verts = brill.vertices
+    poly = []
+    for ix in range(len(faces)):
+        temp = []
+        for iy in range(len(faces[ix])):
+            temp.append(verts[faces[ix][iy]])
+        poly.append(np.array(temp))
+    return np.array(poly)
+
+
+def mapping_func(kpoints, bands):
+    kx = np.unique(kpoints[:, 0])
+    ky = np.unique(kpoints[:, 1])
+    kz = np.unique(kpoints[:, 2])
+    mapped_func = np.zeros(shape=(len(kx), len(ky), len(kz)))
+    kpoint_matrix = np.zeros(shape=(len(kx), len(ky), len(kz), 3))
+    for ikx in range(len(kx)):
+        cond1 = kpoints[:, 0] == kx[ikx]
+        for iky in range(len(ky)):
+            cond2 = kpoints[:, 1] == ky[iky]
+            for ikz in range(len(kz)):
+                cond3 = kpoints[:, 2] == kz[ikz]
+                tot_cond = np.all([cond1, cond2, cond3], axis=0)
+                if len(bands[tot_cond]) != 0:
+                    mapped_func[ikx, iky, ikz] = bands[tot_cond][0]
+                    kpoint_matrix[ikx, iky, ikz] = [kx[ikx], ky[iky], kz[ikz]]
+                else:
+                    mapped_func[ikx, iky, ikz] = np.nan
+                    kpoint_matrix[ikx, iky, ikz] = [np.nan, np.nan, np.nan]
+
+    return mapped_func, kpoint_matrix
+
+
+# if the grid is gamma centered the gird would be something like [-0.45,-0.35,...,0,...,0.5]
+# using FFT interpolate we will loose center. The fermi surface will not be symmetric with
+# respect to the center. To avoid this we will add the points from 0.5 to -0.5 so the mesh will be like
+# [-0.5,-0.45,..,0,...,0.45,0.5]
+def symmetrize(data):
+    # kpoints with one 0.5
+    idx = (data.kpoints == 0.5).sum(axis=1) == 1
+    #    idx = np.any(data.kpoints == 0.5,axis=1)
+    kpoints_toAdd = data.kpoints[idx] + (data.kpoints[idx] == 0.5).astype(int) * -1
+    bands_toAdd = data.bands[idx]
+    spd_toAdd = data.spd[idx]
+    # kpoints with two 0.5
+    # -0.5,-0.5
+    idx = (data.kpoints == 0.5).sum(axis=1) == 2
+    kpoints_temp = data.kpoints[idx] + (data.kpoints[idx] == 0.5).astype(int) * -1
+    bands_temp = data.bands[idx]
+    spd_temp = data.spd[idx]
+
+    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
+    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
+    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
+    # [0.5,:,:]
+    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 0])] - [1, 0, 0]
+    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 0])]
+    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 0])]
+    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
+    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
+    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
+    # [:,0.5,:]
+    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 1])] - [0, 1, 0]
+    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 1])]
+    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 1])]
+    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
+    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
+    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
+    # [:,:,0.5]
+    kpoints_temp = data.kpoints[idx][((data.kpoints[idx] == 0.5)[:, 2])] - [0, 0, 1]
+    bands_temp = data.bands[idx][((data.kpoints[idx] == 0.5)[:, 2])]
+    spd_temp = data.spd[idx][((data.kpoints[idx] == 0.5)[:, 2])]
+    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
+    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
+    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
+    # kpoints with three 0.5
+    idx = (data.kpoints == 0.5).sum(axis=1) == 3
+    kpoints_temp = np.array(
+        [(x, y, z) for x in [-0.5, 0.5] for y in [-0.5, 0.5] for z in [-0.5, 0.5]]
+    )[:-1]
+    bands_temp = np.repeat(data.bands[idx], 7, axis=0)
+    spd_temp = np.repeat(data.spd[idx], 7, axis=0)
+    kpoints_toAdd = np.append(kpoints_toAdd, kpoints_temp, axis=0)
+    bands_toAdd = np.append(bands_toAdd, bands_temp, axis=0)
+    spd_toAdd = np.append(spd_toAdd, spd_temp, axis=0)
+
+    data.kpoints = np.append(data.kpoints, kpoints_toAdd, axis=0)
+    data.bands = np.append(data.bands, bands_toAdd, axis=0)
+    data.spd = np.append(data.spd, spd_toAdd, axis=0)
+    return data
+
+
+def bring_pnts_to_BZ(recLat, kvector_cart, kvector_red, br_points):
+    outsides = []
+    directions = []
+    # This section finds points that are outside of the 1st BZ and and creates those points in the 1st BZ
+    movements = np.array(
+        [
+            recLat[0],
+            recLat[1],
+            recLat[2],
+            -1 * recLat[0],
+            -1 * recLat[1],
+            -1 * recLat[2],
+        ]
+    )
+    for ik in range(len(kvector_cart)):
+        ik_copy = kvector_cart[ik][:]
+        idirection = 0
+        was_outside = False
+        while is_outside([br_points, ik_copy]) and idirection < 6:
+            ik_copy = kvector_cart[ik] + movements[idirection]
+            idirection += 1
+            was_outside = True
+        if was_outside:
+            outsides.append(kvector_red[ik])
+            directions.append(
+                np.dot(movements[idirection - 1], np.linalg.pinv(recLat)).round(2)
+            )
+        kvector_cart[ik] = ik_copy[:]
+        kvector_red[ik] = np.dot(ik_copy, np.linalg.pinv(recLat)).round(2)
+    if len(outsides):
+        has_points_out = True
+    else:
+        has_points_out = False
+    return kvector_cart, kvector_red, has_points_out
+
+
+def fft_interpolate(function, scale):
+    eigen_fft = np.fft.fftn(function)
+    shifted_fft = np.fft.fftshift(eigen_fft)
+    nx, ny, nz = np.array(shifted_fft.shape)
+    pad_x = nx * (scale - 1) // 2
+    pad_y = ny * (scale - 1) // 2
+    pad_z = nz * (scale - 1) // 2
+    new_matrix = np.pad(
+        shifted_fft,
+        ((pad_x, pad_x), (pad_y, pad_y), (pad_z, pad_z)),
+        "constant",
+        constant_values=0,
+    )
+
+    new_matrix = np.fft.ifftshift(new_matrix)
+    interpolated = np.real(np.fft.ifftn(new_matrix)) * (scale ** 3)
+    return interpolated
+
+
+def is_outside(args):
+    br_points = args[0]
+    point = args[1]
+    Hull1 = ConvexHull(br_points)
+    added_points = np.append(br_points, [point], axis=0)
+    Hull2 = ConvexHull(added_points)
+    if len(Hull2.vertices) == len(Hull1.vertices):
+        if sum(Hull2.vertices - Hull1.vertices) != 0:
+            return True
+    else:
+        return True
+    return False
+
+
+def to_remove(args):
+    faces = args[0]
+    vert = args[1]
+    return np.any(faces == vert, axis=1)
+
+
+def fermi3D(procar, outcar, bands=-1, scale=1, mode="plain", st=False, **kwargs):
+    """
+    This function plots 3d fermi surface
+    list of acceptable kwargs :
+        plotting_package
+        nprocess
+        face_colors
+        arrow_colors 
+        arrow_spin
+        atom
+        orbital
+        spin
+        
+    """
+    welcome()
+
+    # Initilizing the arguments :
+
+    if "plotting_package" in kwargs:
+        plotting_package = kwargs["plotting_package"]
+    else:
+        plotting_package = "mayavi"
+
+    if "nprocess" in kwargs:
+        nprocess = kwargs["nprocess"]
+    else:
+        nprocess = 2
+
+    if "face_colors" in kwargs:
+        face_colors = kwargs["face_colors"]
+    else:
+        face_colors = None
+    if "cmap" in kwargs:
+        cmap = kwargs["cmap"]
+    else:
+        cmap = "jet"
+    if "atoms" in kwargs:
+        atoms = kwargs["atoms"]
+    else:
+        atoms = [-1]  # project all atoms
+    if "orbitals" in kwargs:
+        orbitals = kwargs["orbitals"]
+    else:
+        orbitals = [-1]
+
+    if "spin" in kwargs:
+        spin = kwargs["spin"]
+    else:
+        spin = [0]
+    if "mask_points" in kwargs:
+        mask_points = kwargs["mask_points"]
+    else:
+        mask_points = 1
+    if "energy" in kwargs:
+        energy = kwargs["energy"]
+    else:
+        energy = 0
+    if "transparent" in kwargs:
+        transparent = kwargs["transparent"]
+    else:
+        transparent = False
+
+    if "arrow_projection" in kwargs:
+        arrow_projection = kwargs["arrow_projection"]
+    else:
+        arrow_projection = 2
+
+    if plotting_package == "mayavi":
+        try:
+            from mayavi import mlab
+            from tvtk.api import tvtk
+        except:
+            print(
+                "You have selected mayavi as plottin package. please install mayavi and tvtk or choose a different package"
+            )
+            return
+    elif plotting_package == "plotly":
+        try:
+            import plotly.plotly as py
+            import plotly.figure_factory as ff
+            import plotly.graph_objs as go
+            
+            cmap = mpl.cm.get_cmap(cmap)
+            figs = []
+
+        except:
+            print(
+                "You have selected plotly as plottin package. please install plotly or choose a different package"
+            )
+            return
+    elif plotting_package == "matplotlib":
+        try:
+            import matplotlib.pylab as plt
+            from mpl_toolkits.mplot3d.art3d import Poly3DCollection
+        except:
+            print(
+                "You have selected matplotlib as plotting package. please install matplotlib or choose a different package"
+            )
+            return
+    elif plotting_package == "ipyvolume":
+        try:
+            import ipyvolume.pylab as ipv
+        except:
+            print(
+                "You have selected ipyvolume as plotting package. please install ipyvolume or choose a different package"
+            )
+            return
+    if mode == 'colorful' :
+        face_colors = [(1, 0, 0),
+                       (0, 1, 0),
+                       (0, 0, 1),
+                       (1, 1, 0),
+                       (0, 1, 1),
+                       (1, 0, 1),
+                       (192/255, 192/255, 192/255),
+                       (128/255, 128/255, 128/255),
+                       (128/255, 0, 0),
+                       (128/255, 128/255, 0),
+                       (0, 128/255, 0),
+                       (128/255, 0, 128/255),
+                       (0, 128/255, 128/255),
+                       (0, 0, 128/255)]
+
+    permissive = False
+
+    # get fermi from outcar
+    outcarparser = UtilsProcar()
+    e_fermi = outcarparser.FermiOutcar(outcar)
+    print("Fermi=", e_fermi)
+    e_fermi += energy
+    # get reciprocal lattice from outcar
+    recLat = outcarparser.RecLatOutcar(outcar)
+
+    # parsing the Procar file
+    procarFile = ProcarParser()
+    procarFile.readFile(procar, permissive)
+
+    poly = get_wigner_seitz(recLat)
+    # plot brilliouin zone
+    if plotting_package == "mayavi":
+        brillouin_point = []
+        brillouin_faces = []
+        point_count = 0
+        for iface in poly:
+            single_face = []
+            for ipoint in iface:
+                single_face.append(point_count)
+                brillouin_point.append(list(ipoint))
+                point_count += 1
+            brillouin_faces.append(single_face)
+        polydata_br = tvtk.PolyData(points=brillouin_point, polys=brillouin_faces)
+        mlab.figure(figure=None, bgcolor=(1,1,1), fgcolor=None, engine=None, size=(400, 350))
+        mlab.pipeline.surface(
+            polydata_br,
+            representation="wireframe",
+            color=(0, 0, 0),
+            line_width=4,
+            name="BRZ",
+        )
+    elif plotting_package == "plotly":
+
+        for iface in poly:
+            iface = np.pad(iface, ((0, 1), (0, 0)), "wrap")
+            x, y, z = iface[:, 0], iface[:, 1], iface[:, 2]
+            plane = go.Scatter3d(
+                x=x, y=y, z=z, mode="lines", line=dict(color="black", width=4)
+            )
+            figs.append(plane)
+
+    elif plotting_package == "matplotlib":
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection="3d")
+        brillouin_zone = Poly3DCollection(
+            poly, facecolors=["None"] * len(poly), alpha=1, linewidth=4
+        )
+        brillouin_zone.set_edgecolor("k")
+        ax.add_collection3d(brillouin_zone, zs=0, zdir="z")
+
+    br_points = []
+    for iface in poly:
+        for ipoint in iface:
+            br_points.append(ipoint)
+    br_points = np.unique(br_points, axis=0)
+    print("Number of bands: %d" % procarFile.bandsCount)
+    print("Number of koints %d" % procarFile.kpointsCount)
+    print("Number of ions: %d" % procarFile.ionsCount)
+    print("Number of orbitals: %d" % procarFile.orbitalCount)
+    print("Number of spins: %d" % procarFile.ispin)
+
+    # selecting the data
+    data = ProcarSelect(procarFile, deepCopy=True)
+    if bands == -1:
+        bands = range(data.bands.shape[1])
+
+    kvector = data.kpoints
+    kmax = np.max(kvector)
+    kmin = np.min(kvector)
+
+    if abs(kmax) != abs(kmin):
+        print("The mesh provided is gamma center, symmetrizing data")
+        print("For a better fermi surface, use a non-gamma centered k-mesh")
+        data = symmetrize(data)
+        kvector = data.kpoints
+
+    kvector_red = data.kpoints.copy()
+    kvector_cart = np.dot(kvector_red, recLat)
+
+    # This section finds points that are outside of the 1st BZ and and creates those points in the 1st BZ
+    kvector_cart, kvector_red, has_points_out = bring_pnts_to_BZ(
+        recLat, kvector_cart, kvector_red, br_points
+    )
+    #    has_points_out = False
+
+    # getting the mesh grid in each dirrection
+    kx_red = np.unique(kvector_red[:, 0])
+    ky_red = np.unique(kvector_red[:, 1])
+    kz_red = np.unique(kvector_red[:, 2])
+
+    # getting the lengths between kpoints in each direction
+    klength_x = np.abs(kx_red[-1] - kx_red[-2])
+    klength_y = np.abs(ky_red[-1] - ky_red[-2])
+    klength_z = np.abs(kz_red[-1] - kz_red[-2])
+    klengths = [klength_x, klength_y, klength_z]
+
+    # getting number of kpoints in each direction with the addition of kpoints needed to sample the 1st BZ fully (in reduced)
+    nkx_red = kx_red.shape[0]
+    nky_red = ky_red.shape[0]
+    nkz_red = kz_red.shape[0]
+
+    # getting numner of kpoints in each direction provided by vasp
+    nkx_orig = np.unique(kvector[:, 0]).shape[0]
+    nky_orig = np.unique(kvector[:, 1]).shape[0]
+    nkz_orig = np.unique(kvector[:, 2]).shape[0]
+
+    # Amount of kpoints needed to add on to fully sample 1st BZ
+    padding_x = (nkx_red - nkx_orig) // 2
+    padding_y = (nky_red - nky_orig) // 2
+    padding_z = (nkz_red - nkz_orig) // 2
+
+    if mode == "parametric":
+        data.selectIspin(spin)
+        data.selectAtoms(atoms, fortran=False)
+        data.selectOrbital(orbitals)
+    elif mode == "external":
+        if "color_file" in kwargs:
+            rf = open(kwargs["color_file"])
+
+            lines = rf.readlines()
+            counter = 0
+            color_kvector = []
+            color_eigen = []
+            for iline in lines:
+                if counter < 2:
+                    if "band" in iline:
+                        counter += 1
+                        continue
+                    temp = [float(x) for x in iline.split()]
+                    color_kvector.append([temp[0], temp[1], temp[2]])
+            counter = -1
+            for iline in lines:
+                if "band" in iline:
+                    counter += 1
+                    iband = int(iline.split()[-1])
+                    color_eigen.append([])
+                    continue
+                color_eigen[counter].append(float(iline.split()[-1]))
+            rf.close()
+
+            color_kvector = np.array(color_kvector)
+            color_kvector_red = color_kvector.copy()
+            color_kvector_cart = np.dot(color_kvector, recLat)
+            if has_points_out:
+
+                color_kvector_cart, color_kvector_red, temp = bring_pnts_to_BZ(
+                    recLat, color_kvector_cart, color_kvector_red, br_points
+                )
+        else:
+            print("mode selected was external, but no color_file name was provided")
+            return
+    if st:
+
+        dataX = ProcarSelect(procarFile, deepCopy=True)
+        dataY = ProcarSelect(procarFile, deepCopy=True)
+        dataZ = ProcarSelect(procarFile, deepCopy=True)
+
+        dataX.kpoints = data.kpoints
+        dataY.kpoints = data.kpoints
+        dataZ.kpoints = data.kpoints
+
+        dataX.spd = data.spd
+        dataY.spd = data.spd
+        dataZ.spd = data.spd
+
+        dataX.bands = data.bands
+        dataY.bands = data.bands
+        dataZ.bands = data.bands
+
+        dataX.selectIspin([1])
+        dataY.selectIspin([2])
+        dataZ.selectIspin([3])
+
+        dataX.selectAtoms(atoms, fortran=False)
+        dataY.selectAtoms(atoms, fortran=False)
+        dataZ.selectAtoms(atoms, fortran=False)
+
+        dataX.selectOrbital(orbitals)
+        dataY.selectOrbital(orbitals)
+        dataZ.selectOrbital(orbitals)
+    ic = 0
+    for iband in bands:
+
+        print("Plotting band %d" % iband)
+
+        eigen = data.bands[:, iband]
+
+        # mapping the eigen values on the mesh grid to a matrix
+        mapped_func, kpoint_matrix = mapping_func(kvector, eigen)
+
+        # adding the points from the 2nd BZ to 1st BZ to fully sample the BZ. Check np.pad("wrap") for more information
+        mapped_func = np.pad(
+            mapped_func,
+            ((padding_x, padding_x), (padding_y, padding_y), (padding_z, padding_z)),
+            "wrap",
+        )
+
+        # Fourier interpolate the mapped function E(x,y,z)
+        surf_equation = fft_interpolate(mapped_func, scale)
+
+        # after the FFT we loose the center of the BZ, using numpy roll we bring back the center of the BZ
+        surf_equation = np.roll(surf_equation, (scale) // 2, axis=[0, 1, 2])
+
+        try:
+            # creating the isosurface if possible
+            verts, faces, normals, values = measure.marching_cubes_lewiner(
+                surf_equation, e_fermi
+            )
+
+        except:
+
+            print("No isosurface for this band")
+            continue
+        # the vertices provided are scaled and shifted to start from zero
+        # we center them to zero, and rescale them to fit the real BZ by multiplying by the klength in each direction
+        for ix in range(3):
+            verts[:, ix] -= verts[:, ix].min()
+            verts[:, ix] -= (verts[:, ix].max() - verts[:, ix].min()) / 2
+            verts[:, ix] *= klengths[ix] / scale
+
+        # the vertices need to be transformed to reciprocal spcae from recuded space, to find the points that are
+        # in 2nd BZ, to be removed
+        verts = np.dot(verts, recLat)
+
+        # identifying the points in 2nd BZ and removing them
+        if has_points_out:
+            args = []
+            for ivert in range(len(verts)):
+                args.append([br_points, verts[ivert]])
+
+            p = Pool(nprocess)
+            results = np.array(p.map(is_outside, args))
+            p.close()
+            out_verts = np.arange(0, len(results))[results]
+            new_faces = []
+            #            outs_bool_mat = np.zeros(shape=faces.shape,dtype=np.bool)
+
+            for iface in faces:
+                remove = False
+                for ivert in iface:
+                    if ivert in out_verts:
+                        remove = True
+
+                        continue
+
+                if not remove:
+                    new_faces.append(iface)
+            faces = np.array(new_faces)
+
+        print("done removing")
+        # At this point we have the plain Fermi surface, we can color the surface depending on the projection
+        # We create the center of faces by averaging coordinates of corners
+
+        if mode == "parametric":
+
+            character = data.spd[:, iband]
+
+            centers = np.zeros(shape=(len(faces), 3))
+            for iface in range(len(faces)):
+                centers[iface, 0:3] = np.average(verts[faces[iface]], axis=0)
+
+            colors = interpolate.griddata(
+                kvector_cart, character, centers, method="nearest"
+            )
+        elif mode == "external":
+            character = np.array(color_eigen[ic])
+            ic += 1
+            centers = np.zeros(shape=(len(faces), 3))
+            for iface in range(len(faces)):
+                centers[iface, 0:3] = np.average(verts[faces[iface]], axis=0)
+
+            colors = interpolate.griddata(
+                color_kvector_cart, character, centers, method="nearest"
+            )
+
+        if st:
+            projection_x = dataX.spd[:, iband]
+            projection_y = dataY.spd[:, iband]
+            projection_z = dataZ.spd[:, iband]
+
+            verts_spin, faces_spin, normals, values = measure.marching_cubes_lewiner(
+                mapped_func, e_fermi
+            )
+
+            for ix in range(3):
+                verts_spin[:, ix] -= verts_spin[:, ix].min()
+                verts_spin[:, ix] -= (
+                    verts_spin[:, ix].max() - verts_spin[:, ix].min()
+                ) / 2
+                verts_spin[:, ix] *= klengths[ix]
+            verts_spin = np.dot(verts_spin, recLat)
+
+            if has_points_out:
+                args = []
+                for ivert in range(len(verts_spin)):
+                    args.append([br_points, verts_spin[ivert]])
+
+                p = Pool(nprocess)
+                results = np.array(p.map(is_outside, args))
+                p.close()
+                out_verts = np.arange(0, len(results))[results]
+
+                new_faces = []
+                for iface in faces_spin:
+                    remove = False
+                    for ivert in iface:
+                        if ivert in out_verts:
+                            remove = True
+                            continue
+                    if not remove:
+                        new_faces.append(iface)
+                faces_spin = np.array(new_faces)
+
+            centers = np.zeros(shape=(len(faces_spin), 3))
+            for iface in range(len(faces_spin)):
+                centers[iface, 0:3] = np.average(verts_spin[faces_spin[iface]], axis=0)
+
+            colors1 = interpolate.griddata(
+                kvector_cart, projection_x, centers, method="linear"
+            )
+            colors2 = interpolate.griddata(
+                kvector_cart, projection_y, centers, method="linear"
+            )
+            colors3 = interpolate.griddata(
+                kvector_cart, projection_z, centers, method="linear"
+            )
+            spin_arrows = np.vstack((colors1, colors2, colors3)).T
+
+        if plotting_package == "mayavi":
+            polydata = tvtk.PolyData(points=verts, polys=faces)
+
+            if face_colors != None:
+                mlab.pipeline.surface(
+                    polydata,
+                    representation="surface",
+                    color=face_colors[ic],
+                    opacity=1,
+                    name="band-" + str(iband),
+                )
+                ic += 1
+            else:
+                if mode == "plain":
+                    if not (transparent):
+                        s = mlab.pipeline.surface(
+                            polydata,
+                            representation="surface",
+                            color=(0, 0.5, 1),
+                            opacity=1,
+                            name="band-" + str(iband),
+                        )
+
+
+                elif mode == "parametric" or mode == "external":
+
+                    polydata.cell_data.scalars = colors
+                    polydata.cell_data.scalars.name = "celldata"
+                    mlab.pipeline.surface(
+                        polydata, vmin=0, vmax=colors.max(), colormap=cmap
+                    )
+                    cb = mlab.colorbar(orientation="vertical")
+
+            if st:
+                x, y, z = list(zip(*centers))
+                u, v, w = list(zip(*spin_arrows))
+
+                pnts = mlab.quiver3d(
+                    x,
+                    y,
+                    z,
+                    u,
+                    v,
+                    w,
+                    line_width=5,
+                    mode="arrow",
+                    resolution=25,
+                    reset_zoom=False,
+                    name="spin-" + str(iband),
+                    mask_points=mask_points,
+                    scalars=spin_arrows[:, arrow_projection],
+                    vmin=-1,
+                    vmax=1,
+                    colormap=cmap,
+                )
+                pnts.glyph.color_mode = "color_by_scalar"
+                pnts.glyph.glyph_source.glyph_source.shaft_radius = 0.05
+                pnts.glyph.glyph_source.glyph_source.tip_radius = 0.1
+
+        elif plotting_package == "plotly":
+            if mode == "plain":
+                if not (transparent):
+                    x, y, z = zip(*verts)
+                    fig = ff.create_trisurf(
+                        x=x,
+                        y=y,
+                        z=z,
+                        plot_edges=False,
+                        simplices=faces,
+                        title="band-%d" % ic,
+                    )
+
+                    figs.append(fig["data"][0])
+
+            elif mode == "parametric" or mode == "external":
+
+                face_colors = cmap(colors)
+                colormap = [
+                    "rgb(%i,%i,%i)" % (x[0], x[1], x[2])
+                    for x in (face_colors * 255).round()
+                ]
+                x, y, z = zip(*verts)
+                fig = ff.create_trisurf(
+                    x=x,
+                    y=y,
+                    z=z,
+                    plot_edges=False,
+                    colormap=colormap,
+                    simplices=faces,
+                    show_colorbar=True,
+                    title="band-%d" % ic,
+                )
+
+                figs.append(fig["data"][0])
+        elif plotting_package == "matplotlib":
+            if mode == "plain":
+                x, y, z = zip(*verts)
+                ax.plot_trisurf(x, y, faces, z, linewidth=0.2, antialiased=True)
+            elif mode == "parametric" or mode == "external":
+                print(
+                    "coloring the faces is not implemented in matplot lib, please use another plotting package.we recomend mayavi."
+                )
+        elif plotting_package == "ipyvolume":
+            if mode == "plain":
+                ipv.figure()
+                ipv.plot_trisurf(verts[:, 0], verts[:, 1], verts[:, 2], triangles=faces)
+
+            elif mode == "paramteric" or mode == "external":
+                face_colors = cmap(colors)
+                colormap = [
+                    "rgb(%i,%i,%i)" % (x[0], x[1], x[2])
+                    for x in (face_colors * 255).round()
+                ]
+                ipv.figure()
+                ipv.plot_trisurf(
+                    verts[:, 0], verts[:, 1], verts[:, 2], triangles=faces, color=cmap
+                )
+
+    # if plotting_package == "mayavi":
+    #     mlab.colorbar(orientation="vertical") 
+    #     mlab.show()
+    # elif plotting_package == "plotly":
+    #     layout = go.Layout(showlegend=False)
+
+    #     fig = go.Figure(data=figs, layout=layout)
+    #     py.iplot(fig)
+    # elif plotting_package == "matplotlib":
+    #     plt.show()
+    # elif plotting_package == "ipyvolume":
+    #     ipv.show()
+
+    return
```

### Comparing `PyProcar-5.6.6/pyprocar/utilsprocar/utilsprocar.py` & `PyProcar-6.0.0/pyprocar/utils/utilsprocar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,310 +1,310 @@
-import logging
-import re
-import sys
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-
-class UtilsProcar:
-    """
-  This class store handy methods that do not fit any other place
-
-  members:
-
-  -Openfile: Tries to open a File, it has suitable values for PROCARs
-   and can handle gzipped files
-
-  -MergeFiles: concatenate two or more PROCAR files taking care of
-   metadata and kpoint indexes. Useful for splitted bandstructures
-   calculation.
-
-  -FermiOutcar: it greps the Fermi Energy from a given outcar file.
-
-  -RecLatOutcar: it greps the reciprocal lattice from the outcar.
-
-  """
-
-    def __init__(self, loglevel=logging.WARNING):
-        self.log = logging.getLogger("UtilsProcar")
-        self.log.setLevel(loglevel)
-        self.ch = logging.StreamHandler()
-        self.ch.setFormatter(
-            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
-        )
-        self.ch.setLevel(logging.DEBUG)
-        self.log.addHandler(self.ch)
-        self.log.debug("UtilsProcar()")
-        self.log.debug("UtilsProcar()...done")
-        return
-
-    ###############################SCRIPTS####################################################################
-
-    # #calls ProcarRepair
-    # def scriptRepair(self,infile,outfile):
-
-    #   print "Input File    : ", infile
-    #   print "Output File   : ", outfile
-
-    #   #parsing the file
-    #   handler = UtilsProcar()
-    #   handler.ProcarRepair(infile,outfile)
-
-    # calls MergeFiles
-    # inFiles should be a list of the PROCAR files that require concatenation
-    # def scriptCat(self,inFiles,outFile,gz=False):
-    #   print   "Concatenating:"
-    #   print   "Input         : ", ', '.join(inFiles)
-    #   print   "Output        : ", outFile
-    #   if gz==True:
-    #       print "out compressed: True"
-
-    #   if gz=="True" and outFile[-3:] is not '.gz':
-    #     outFile += '.gz'
-    #     print ".gz extension appended to the outFile"
-
-    #   handler = UtilsProcar()
-    #   handler.MergeFiles(inFiles,outFile, gzipOut=gz)
-    #   return
-
-    ####################################################################################################################################################
-
-    def OpenFile(self, FileName=None):
-        """
-    Tries to open a File, it has suitable values for PROCAR and can
-    handle gzipped files
-
-    Example:
-
-    >>> foo =  UtilsProcar.Openfile()
-    Tries to open "PROCAR", then "PROCAR.gz"
-
-    >>> foo = UtilsProcar.Openfile("../bar")
-    Tries to open "../bar". If it is a directory, it will try to open
-    "../bar/PROCAR" and if fails again "../bar/PROCAR.gz"
-
-    >>> foo = UtilsProcar.Openfile("PROCAR-spd.gz")
-    Tries to open a gzipped file "PROCAR-spd.gz"
-
-    If unable to open a file, it raises a "IOError" exception.
-"""
-        import os
-        import gzip
-
-        self.log.debug("OpenFile()")
-        self.log.debug("Filename :" + FileName)
-
-        if FileName is None:
-            FileName = "PROCAR"
-            self.log.debug("Input was None, now is: " + FileName)
-
-        # checking if fileName is just a path and needs a "PROCAR to " be
-        # appended
-        elif os.path.isdir(FileName):
-            self.log.info("The filename is a directory")
-            if FileName[-1] != r"/":
-                FileName += "/"
-            FileName += "PROCAR"
-            self.log.debug("I will try  to open :" + FileName)
-
-        # checking that the file exist
-        if os.path.isfile(FileName):
-            self.log.debug("The File does exist")
-            # Checking if compressed
-            if FileName[-2:] == "gz":
-                self.log.info("A gzipped file found")
-                inFile = gzip.open(FileName, mode="rt")
-            else:
-                self.log.debug("A normal file found")
-                inFile = open(FileName, "r")
-            return inFile
-
-        # otherwise a gzipped version may exist
-        elif os.path.isfile(FileName + ".gz"):
-            self.log.info(
-                "File not found, however a .gz version does exist and will" " be used"
-            )
-            inFile = gzip.open(FileName + ".gz", mode="rt")
-
-        else:
-            self.log.debug("File not exist, neither a gzipped version")
-            print(FileName)
-            raise IOError("File not found")
-
-        self.log.debug("OpenFile()...done")
-        return inFile
-
-    def MergeFiles(self, inFiles, outFile, gzipOut=False):
-        """
-    Concatenate two or more PROCAR files. This methods
-    takes care of the k-indexes.
-
-    Useful when large number of K points have been calculated in
-    different PROCARs.
-
-    Args:
-    -inFiles: an iterable with files to be concatenated
-
-    -outFile: a string with the outfile name.
-
-    -gzipOut: whether gzip or not the outout file.
-
-    Warning: spin polarized case is not Ok!
-
-    """
-        import gzip
-
-        self.log.debug("MergeFiles()")
-        self.log.debug("infiles: " " ,".join(inFiles))
-
-        inFiles = [self.OpenFile(x) for x in inFiles]
-        header = [x.readline() for x in inFiles]
-        self.log.debug("All the input headers are: \n" + "".join(header))
-        metas = [x.readline() for x in inFiles]
-        self.log.debug("All the input metalines are:\n " + "".join(metas))
-        # parsing metalines
-
-        parsedMeta = [list(map(int, re.findall(r"#[^:]+:([^#]+)", x))) for x in metas]
-        kpoints = [x[0] for x in parsedMeta]
-        bands = set([x[1] for x in parsedMeta])
-        ions = set([x[2] for x in parsedMeta])
-
-        # checking that bands and ions match (mind: bands & ions are 'sets'):
-        if len(bands) != 1 or len(ions) != 1:
-            self.log.error("Number of bands/ions  do not match")
-            raise RuntimeError("Files are incompatible")
-
-        newKpoints = np.array(kpoints, dtype=int).sum()
-        self.log.info("New number of Kpoints: " + str(newKpoints))
-        newMeta = metas[0].replace(str(kpoints[0]), str(newKpoints), 1)
-        self.log.debug("New meta line:\n" + newMeta)
-
-        if gzipOut:
-            self.log.debug("gzipped output")
-            outFile = gzip.open(outFile, mode="wt")
-        else:
-            self.log.debug("normal output")
-            outFile = open(outFile, "w")
-        outFile.write(header[0])
-        outFile.write(newMeta)
-
-        # embedded function to change old k-point indexes by the correct
-        # ones. The `kreplace.k` syntax is for making the variable 'static'
-        def kreplace(matchobj):
-            # self.log.debug(print matchobj.group(0))
-            kreplace.k += 1
-            kreplace.localCounter += 1
-            return matchobj.group(0).replace(
-                str(kreplace.localCounter), str(kreplace.k)
-            )
-
-        kreplace.k = 0
-        down = []  # to handle spin-down (if found)
-        self.log.debug("Going to replace K-points indexes")
-        for inFile in inFiles:
-            lines = inFile.read()
-            # looking for an extra metada line, if found the file is
-            # spin-polarized
-            p = re.compile(
-                r"#[\s\w]+k-points:[\s\d]+#[\s\w]+bands:[\s\d]+#[\w\s]+ions:\s*\d+\s*"
-            )
-            lines = p.split(lines)
-            up = lines[0]
-            if len(lines) == 2:
-                down.append(lines[1])
-                self.log.info("Spin-polarized PROCAR!")
-            # closing inFile
-            inFile.close()
-            kreplace.localCounter = 0
-            up = re.sub("(\s+k-point\s*\d+\s*:)", kreplace, up)
-            outFile.write(up)
-
-        # handling the spin-down channel, if present
-        if down:
-            self.log.debug("writing spin down metadata")
-            outFile.write("\n")
-            outFile.write(newMeta)
-        kreplace.k = 0
-        for group in down:
-            kreplace.localCounter = 0
-            group = re.sub("(\s+k-point\s*\d+\s*:)", kreplace, group)
-            outFile.write(group)
-
-        self.log.debug("Closing output file")
-        outFile.close()
-        self.log.debug("MergeFiles()...done")
-        return
-
-    def FermiOutcar(self, filename):
-        """Just finds all E-fermi fields in the outcar file and keeps the
-    last one (if more than one found).
-
-    Args:
-    -filename: the file name of the outcar to be readed
-
-    """
-        self.log.debug("FermiOutcar(): ...")
-        self.log.debug("Input filename : " + filename)
-
-        outcar = open(filename, "r").read()
-        match = re.findall(r"E-fermi\s*:\s*(-?\d+.\d+)", outcar)[-1]
-        self.log.info("Fermi Energy found : " + match)
-        self.log.debug("FermiOutcar(): ...Done")
-        return float(match)
-
-    def RecLatOutcar(self, filename):
-        """Finds and return the reciprocal lattice vectors, if more than
-    one set present, it return just the last one.
-
-    Args:
-    -filename: the name of the outcar file  to be read
-
-    """
-        self.log.debug("RecLatOutcar(): ...")
-        self.log.debug("Input filename : " + filename)
-
-        outcar = open(filename, "r").read()
-        # just keeping the last component
-        recLat = re.findall(r"reciprocal\s*lattice\s*vectors\s*([-.\s\d]*)", outcar)[-1]
-        self.log.debug("the match is : " + recLat)
-        recLat = recLat.split()
-        recLat = np.array(recLat, dtype=float)
-        # up to now I have, both direct and rec. lattices (3+3=6 columns)
-        recLat.shape = (3, 6)
-        recLat = recLat[:, 3:]
-        self.log.info("Reciprocal Lattice found :\n" + str(recLat))
-        self.log.debug("RecLatOutcar(): ...Done")
-        return recLat
-
-    def ProcarRepair(self, infilename, outfilename):
-        """It Tries to repair some stupid problems due the stupid fixed
-    format of the stupid fortran.
-
-    Up to now it only separes k-points as the following:
-    k-point    61 :    0.00000000-0.50000000 0.00000000 ...
-    to
-    k-point    61 :    0.00000000 -0.50000000 0.00000000 ...
-
-    But as I found new stupid errors they should be fixed here.
-    """
-        self.log.debug("ProcarRepair(): ...")
-        infile = self.OpenFile(infilename)
-        fileStr = infile.read()
-        infile.close()
-
-        # Fixing bands issues (when there are more than 999 bands)
-        # band *** # energy    6.49554019 # occ.  0.00000000
-        fileStr = re.sub(r"(band\s)(\*\*\*)", r"\1 1000", fileStr)
-
-        # Fixing k-point issues
-        fileStr = re.sub(r"(\.\d{8})(\d{2}\.)", r"\1 \2", fileStr)
-        fileStr = re.sub(r"(\d)-(\d)", r"\1 -\2", fileStr)
-
-        fileStr = re.sub(r"\*+", r" -10.0000 ", fileStr)
-
-        outfile = open(outfilename, "w")
-        outfile.write(fileStr)
-        outfile.close()
-
-        self.log.debug("ProcarRepair(): ...Done")
-        return
+import logging
+import re
+import sys
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+
+class UtilsProcar:
+    """
+  This class store handy methods that do not fit any other place
+
+  members:
+
+  -Openfile: Tries to open a File, it has suitable values for PROCARs
+   and can handle gzipped files
+
+  -MergeFiles: concatenate two or more PROCAR files taking care of
+   metadata and kpoint indexes. Useful for splitted bandstructures
+   calculation.
+
+  -FermiOutcar: it greps the Fermi Energy from a given outcar file.
+
+  -RecLatOutcar: it greps the reciprocal lattice from the outcar.
+
+  """
+
+    def __init__(self, loglevel=logging.WARNING):
+        self.log = logging.getLogger("UtilsProcar")
+        self.log.setLevel(loglevel)
+        self.ch = logging.StreamHandler()
+        self.ch.setFormatter(
+            logging.Formatter("%(name)s::%(levelname)s:" " %(message)s")
+        )
+        self.ch.setLevel(logging.DEBUG)
+        self.log.addHandler(self.ch)
+        self.log.debug("UtilsProcar()")
+        self.log.debug("UtilsProcar()...done")
+        return
+
+    ###############################SCRIPTS####################################################################
+
+    # #calls ProcarRepair
+    # def scriptRepair(self,infile,outfile):
+
+    #   print "Input File    : ", infile
+    #   print "Output File   : ", outfile
+
+    #   #parsing the file
+    #   handler = UtilsProcar()
+    #   handler.ProcarRepair(infile,outfile)
+
+    # calls MergeFiles
+    # inFiles should be a list of the PROCAR files that require concatenation
+    # def scriptCat(self,inFiles,outFile,gz=False):
+    #   print   "Concatenating:"
+    #   print   "Input         : ", ', '.join(inFiles)
+    #   print   "Output        : ", outFile
+    #   if gz==True:
+    #       print "out compressed: True"
+
+    #   if gz=="True" and outFile[-3:] is not '.gz':
+    #     outFile += '.gz'
+    #     print ".gz extension appended to the outFile"
+
+    #   handler = UtilsProcar()
+    #   handler.MergeFiles(inFiles,outFile, gzipOut=gz)
+    #   return
+
+    ####################################################################################################################################################
+
+    def OpenFile(self, FileName=None):
+        """
+    Tries to open a File, it has suitable values for PROCAR and can
+    handle gzipped files
+
+    Example:
+
+    >>> foo =  UtilsProcar.Openfile()
+    Tries to open "PROCAR", then "PROCAR.gz"
+
+    >>> foo = UtilsProcar.Openfile("../bar")
+    Tries to open "../bar". If it is a directory, it will try to open
+    "../bar/PROCAR" and if fails again "../bar/PROCAR.gz"
+
+    >>> foo = UtilsProcar.Openfile("PROCAR-spd.gz")
+    Tries to open a gzipped file "PROCAR-spd.gz"
+
+    If unable to open a file, it raises a "IOError" exception.
+"""
+        import os
+        import gzip
+
+        self.log.debug("OpenFile()")
+        self.log.debug("Filename :" + FileName)
+
+        if FileName is None:
+            FileName = "PROCAR"
+            self.log.debug("Input was None, now is: " + FileName)
+
+        # checking if fileName is just a path and needs a "PROCAR to " be
+        # appended
+        elif os.path.isdir(FileName):
+            self.log.info("The filename is a directory")
+            if FileName[-1] != r"/":
+                FileName += "/"
+            FileName += "PROCAR"
+            self.log.debug("I will try  to open :" + FileName)
+
+        # checking that the file exist
+        if os.path.isfile(FileName):
+            self.log.debug("The File does exist")
+            # Checking if compressed
+            if FileName[-2:] == "gz":
+                self.log.info("A gzipped file found")
+                inFile = gzip.open(FileName, mode="rt")
+            else:
+                self.log.debug("A normal file found")
+                inFile = open(FileName, "r")
+            return inFile
+
+        # otherwise a gzipped version may exist
+        elif os.path.isfile(FileName + ".gz"):
+            self.log.info(
+                "File not found, however a .gz version does exist and will" " be used"
+            )
+            inFile = gzip.open(FileName + ".gz", mode="rt")
+
+        else:
+            self.log.debug("File not exist, neither a gzipped version")
+            print(FileName)
+            raise IOError(f"File not found : {FileName}")
+
+        self.log.debug("OpenFile()...done")
+        return inFile
+
+    def MergeFiles(self, inFiles, outFile, gzipOut=False):
+        """
+    Concatenate two or more PROCAR files. This methods
+    takes care of the k-indexes.
+
+    Useful when large number of K points have been calculated in
+    different PROCARs.
+
+    Args:
+    -inFiles: an iterable with files to be concatenated
+
+    -outFile: a string with the outfile name.
+
+    -gzipOut: whether gzip or not the outout file.
+
+    Warning: spin polarized case is not Ok!
+
+    """
+        import gzip
+
+        self.log.debug("MergeFiles()")
+        self.log.debug("infiles: " " ,".join(inFiles))
+
+        inFiles = [self.OpenFile(x) for x in inFiles]
+        header = [x.readline() for x in inFiles]
+        self.log.debug("All the input headers are: \n" + "".join(header))
+        metas = [x.readline() for x in inFiles]
+        self.log.debug("All the input metalines are:\n " + "".join(metas))
+        # parsing metalines
+
+        parsedMeta = [list(map(int, re.findall(r"#[^:]+:([^#]+)", x))) for x in metas]
+        kpoints = [x[0] for x in parsedMeta]
+        bands = set([x[1] for x in parsedMeta])
+        ions = set([x[2] for x in parsedMeta])
+
+        # checking that bands and ions match (mind: bands & ions are 'sets'):
+        if len(bands) != 1 or len(ions) != 1:
+            self.log.error("Number of bands/ions  do not match")
+            raise RuntimeError("Files are incompatible")
+
+        newKpoints = np.array(kpoints, dtype=int).sum()
+        self.log.info("New number of Kpoints: " + str(newKpoints))
+        newMeta = metas[0].replace(str(kpoints[0]), str(newKpoints), 1)
+        self.log.debug("New meta line:\n" + newMeta)
+
+        if gzipOut:
+            self.log.debug("gzipped output")
+            outFile = gzip.open(outFile, mode="wt")
+        else:
+            self.log.debug("normal output")
+            outFile = open(outFile, "w")
+        outFile.write(header[0])
+        outFile.write(newMeta)
+
+        # embedded function to change old k-point indexes by the correct
+        # ones. The `kreplace.k` syntax is for making the variable 'static'
+        def kreplace(matchobj):
+            # self.log.debug(print matchobj.group(0))
+            kreplace.k += 1
+            kreplace.localCounter += 1
+            return matchobj.group(0).replace(
+                str(kreplace.localCounter), str(kreplace.k)
+            )
+
+        kreplace.k = 0
+        down = []  # to handle spin-down (if found)
+        self.log.debug("Going to replace K-points indexes")
+        for inFile in inFiles:
+            lines = inFile.read()
+            # looking for an extra metada line, if found the file is
+            # spin-polarized
+            p = re.compile(
+                r"#[\s\w]+k-points:[\s\d]+#[\s\w]+bands:[\s\d]+#[\w\s]+ions:\s*\d+\s*"
+            )
+            lines = p.split(lines)
+            up = lines[0]
+            if len(lines) == 2:
+                down.append(lines[1])
+                self.log.info("Spin-polarized PROCAR!")
+            # closing inFile
+            inFile.close()
+            kreplace.localCounter = 0
+            up = re.sub("(\s+k-point\s*\d+\s*:)", kreplace, up)
+            outFile.write(up)
+
+        # handling the spin-down channel, if present
+        if down:
+            self.log.debug("writing spin down metadata")
+            outFile.write("\n")
+            outFile.write(newMeta)
+        kreplace.k = 0
+        for group in down:
+            kreplace.localCounter = 0
+            group = re.sub("(\s+k-point\s*\d+\s*:)", kreplace, group)
+            outFile.write(group)
+
+        self.log.debug("Closing output file")
+        outFile.close()
+        self.log.debug("MergeFiles()...done")
+        return
+
+    def FermiOutcar(self, filename):
+        """Just finds all E-fermi fields in the outcar file and keeps the
+    last one (if more than one found).
+
+    Args:
+    -filename: the file name of the outcar to be readed
+
+    """
+        self.log.debug("FermiOutcar(): ...")
+        self.log.debug("Input filename : " + filename)
+
+        outcar = open(filename, "r").read()
+        match = re.findall(r"E-fermi\s*:\s*(-?\d+.\d+)", outcar)[-1]
+        self.log.info("Fermi Energy found : " + match)
+        self.log.debug("FermiOutcar(): ...Done")
+        return float(match)
+
+    def RecLatOutcar(self, filename):
+        """Finds and return the reciprocal lattice vectors, if more than
+    one set present, it return just the last one.
+
+    Args:
+    -filename: the name of the outcar file  to be read
+
+    """
+        self.log.debug("RecLatOutcar(): ...")
+        self.log.debug("Input filename : " + filename)
+
+        outcar = open(filename, "r").read()
+        # just keeping the last component
+        recLat = re.findall(r"reciprocal\s*lattice\s*vectors\s*([-.\s\d]*)", outcar)[-1]
+        self.log.debug("the match is : " + recLat)
+        recLat = recLat.split()
+        recLat = np.array(recLat, dtype=float)
+        # up to now I have, both direct and rec. lattices (3+3=6 columns)
+        recLat.shape = (3, 6)
+        recLat = recLat[:, 3:]
+        self.log.info("Reciprocal Lattice found :\n" + str(recLat))
+        self.log.debug("RecLatOutcar(): ...Done")
+        return recLat
+
+    def ProcarRepair(self, infilename, outfilename):
+        """It Tries to repair some stupid problems due the stupid fixed
+    format of the stupid fortran.
+
+    Up to now it only separes k-points as the following:
+    k-point    61 :    0.00000000-0.50000000 0.00000000 ...
+    to
+    k-point    61 :    0.00000000 -0.50000000 0.00000000 ...
+
+    But as I found new stupid errors they should be fixed here.
+    """
+        self.log.debug("ProcarRepair(): ...")
+        infile = self.OpenFile(infilename)
+        fileStr = infile.read()
+        infile.close()
+
+        # Fixing bands issues (when there are more than 999 bands)
+        # band *** # energy    6.49554019 # occ.  0.00000000
+        fileStr = re.sub(r"(band\s)(\*\*\*)", r"\1 1000", fileStr)
+
+        # Fixing k-point issues
+        fileStr = re.sub(r"(\.\d{8})(\d{2}\.)", r"\1 \2", fileStr)
+        fileStr = re.sub(r"(\d)-(\d)", r"\1 -\2", fileStr)
+
+        fileStr = re.sub(r"\*+", r" -10.0000 ", fileStr)
+
+        outfile = open(outfilename, "w")
+        outfile.write(fileStr)
+        outfile.close()
+
+        self.log.debug("ProcarRepair(): ...Done")
+        return
```

### Comparing `PyProcar-5.6.6/pyprocar/vaspxml/vaspxml.py` & `PyProcar-6.0.0/pyprocar/io/vaspxml/vaspxml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,696 +1,696 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Aug 19 20:49:03 2020
-
-@author: Pedram Tavadze, Logan Lang
-"""
-
-from ..core import Structure, DensityOfStates
-from numpy import array
-import xml.etree.ElementTree as ET
-import os
-import numpy as np
-import collections
-
-
-class VaspXML(collections.abc.Mapping):
-    """contains."""
-    def __init__(self, filename='vasprun.xml', dos_interpolation_factor=None):
-
-        self.variables = {}
-        self.dos_interpolation_factor = dos_interpolation_factor
-
-        if not os.path.isfile(filename):
-            raise ValueError('File not found ' + filename)
-        else:
-            self.filename = filename
-
-        self.spins_dict = {'spin 1': 'Spin-up', 'spin 2': 'Spin-down'}
-        # self.positions = None
-        # self.stress = None
-        self.bands = None
-        # self.array_sizes = {}
-        self.data = self.read()
-
-    def repair(self):
-        """
-        repairs the wrong syntaxes in vasprun.xml
-        """
-        
-        
-
-    def read(self):
-        """
-        Read and parse vasprun.xml.
-
-        Returns
-        -------
-        TYPE
-            DESCRIPTION.
-
-        """
-        return parse_vasprun(self.filename)
-
-    def _get_dos_total(self):
-
-        spins = list(
-            self.data['general']['dos']['total']['array']['data'].keys())
-        energies = np.array(self.data['general']['dos']['total']['array']
-                            ['data'][spins[0]])[:, 0]
-        dos_total = {'energies': energies}
-        for ispin in spins:
-            dos_total[self.spins_dict[ispin]] = np.array(
-                self.data['general']['dos']['total']['array']['data']
-                [ispin])[:, 1]
-
-        return dos_total, list(dos_total.keys())
-
-    def _get_dos_projected(self, atoms=[]):
-
-        if len(atoms) == 0:
-            atoms = np.arange(self.initial_structure.natoms)
-
-        if 'partial' in self.data['general']['dos']:
-            dos_projected = {}
-            ion_list = ["ion %s" % str(x + 1) for x in atoms
-                        ]  # using this name as vasrun.xml uses ion #
-            for i in range(len(ion_list)):
-                iatom = ion_list[i]
-                name = self.initial_structure.atoms[atoms[i]] + str(atoms[i])
-                spins = list(self.data['general']['dos']['partial']['array']
-                             ['data'][iatom].keys())
-                energies = np.array(
-                    self.data['general']['dos']['partial']['array']['data']
-                    [iatom][spins[0]][spins[0]])[:, 0]
-                dos_projected[name] = {'energies': energies}
-                for ispin in spins:
-                    dos_projected[name][self.spins_dict[ispin]] = np.array(
-                        self.data['general']['dos']['partial']['array']['data']
-                        [iatom][ispin][ispin])[:, 1:]
-            return dos_projected, self.data['general']['dos']['partial'][
-                'array']['info']
-        else:
-            print(
-                "This calculation does not include partial density of states")
-            return None, None
-
-    @property
-    def dos(self):
-        energies = self.dos_total['energies']
-        total = []
-        for ispin in self.dos_total:
-            if ispin == 'energies':
-                continue
-            total.append(self.dos_total[ispin])
-        # total = np.array(total).T
-        return DensityOfStates(
-            energies=energies,
-            total=total,
-            projected=self.dos_projected,
-            interpolation_factor=self.dos_interpolation_factor)
-
-    @property
-    def dos_to_dict(self):
-        """
-        Returns the complete density (total,projected) of states as a python dictionary
-        """
-        return {
-            'total': self._get_dos_total(),
-            'projected': self._get_dos_projected()
-        }
-
-    @property
-    def dos_total(self):
-        """
-        Returns the total density of states as a pychemia.visual.DensityOfSates object
-        """
-        dos_total, labels = self._get_dos_total()
-        dos_total['energies'] -= self.fermi
-
-        return dos_total
-
-    @property
-    def dos_projected(self):
-        """
-        Returns the projected DOS as a multi-dimentional array, to be used in the
-        pyprocar.core.dos object
-        """
-        ret = []
-        dos_projected, info = self._get_dos_projected()
-        if dos_projected is None:
-            return None
-        norbitals = len(info) - 1
-        info[0] = info[0].capitalize()
-        labels = []
-        labels.append(info[0])
-        ret = []
-        for iatom in dos_projected:
-            temp_atom = []
-            for iorbital in range(norbitals):
-                temp_spin = []
-                for key in dos_projected[iatom]:
-                    if key == 'energies':
-                        continue
-                    temp_spin.append(dos_projected[iatom][key][:, iorbital])
-                temp_atom.append(temp_spin)
-            ret.append([temp_atom])
-        return ret
-
-    @property
-    def kpoints(self):
-        """
-        Returns the kpoints used in the calculation in form of a pychemia.core.KPoints object
-        """
-
-        if self.data['kpoints_info']['mode'] == 'listgenerated':
-            kpoints = dict(
-                mode='path',
-                kvertices=self.data['kpoints_info']['kpoint_vertices'])
-        else:
-            kpoints = dict(mode=self.data['kpoints_info']['mode'].lower(),
-                           grid=self.data['kpoints_info']['kgrid'],
-                           shifts=self.data['kpoints_info']['user_shift'])
-        return kpoints
-
-    @property
-    def kpoints_list(self):
-        """
-        Returns the list of kpoints and weights used in the calculation in form of a pychemia.core.KPoints object
-        """
-        return dict(mode='reduced',
-                    kpoints_list=self.data['kpoints']['kpoints_list'],
-                    weights=self.data['kpoints']['k_weights'])
-
-    @property
-    def incar(self):
-        """
-        Returns the incar parameters used in the calculation as pychemia.code.vasp.VaspIncar object
-        """
-        return self.data['incar']
-
-    @property
-    def vasp_parameters(self):
-        """
-        Returns all of the parameters vasp has used in this calculation
-        """
-        return self.data['vasp_params']
-
-    @property
-    def potcar_info(self):
-        """
-        Returns the information about pseudopotentials(POTCAR) used in this calculation
-        """
-        return self.data['atom_info']['atom_types']
-
-    @property
-    def fermi(self):
-        """
-        Returns the fermi energy
-        """
-        return self.data['general']['dos']['efermi']
-
-    @property
-    def species(self):
-        """
-        Returns the species in POSCAR
-        """
-        return self.initial_structure.species
-
-    @property
-    def structures(self):
-        """
-        Returns a list of pychemia.core.Structure representing all the ionic step structures
-        """
-        symbols = [x.strip() for x in self.data['atom_info']['symbols']]
-        structures = []
-        for ist in self.data['structures']:
-
-            st = Structure(atoms=symbols,
-                           fractional_coordinates=ist['reduced'],
-                           lattice=ist['cell'])
-            structures.append(st)
-        return structures
-
-    @property
-    def structure(self):
-        """
-        crystal structure of the last step
-        """
-        return self.structures[-1]
-
-    @property
-    def forces(self):
-        """
-        Returns all the forces in ionic steps
-        """
-        return self.data['forces']
-
-    @property
-    def initial_structure(self):
-        """
-        Returns the initial Structure as a pychemia structure
-        """
-        return self.structures[0]
-
-    @property
-    def final_structure(self):
-        """
-        Returns the final Structure as a pychemia structure
-        """
-
-        return self.structures[-1]
-
-    @property
-    def iteration_data(self):
-        """
-        Returns a list of information in each electronic and ionic step of calculation
-        """
-        return self.data['calculation']
-
-    @property
-    def energies(self):
-        """
-        Returns a list of energies in each electronic and ionic step [ionic step,electronic step, energy]
-        """
-        scf_step = 0
-        ion_step = 0
-        double_counter = 1
-        energies = []
-        for calc in self.data['calculation']:
-            if 'ewald' in calc['energy']:
-                if double_counter == 0:
-                    double_counter += 1
-                    scf_step += 1
-                elif double_counter == 1:
-                    double_counter = 0
-                    ion_step += 1
-                    scf_step = 1
-            else:
-                scf_step += 1
-            energies.append([ion_step, scf_step, calc['energy']['e_0_energy']])
-        return energies
-
-    @property
-    def last_energy(self):
-        """
-        Returns the last calculated energy of the system
-        """
-        return self.energies[-1][-1]
-
-    @property
-    def energy(self):
-        """
-        Returns the last calculated energy of the system
-        """
-        return self.last_energy
-
-    @property
-    def convergence_electronic(self):
-        """
-        Returns a boolian representing if the last electronic self-consistent
-        calculation converged
-        """
-        ediff = self.vasp_parameters['electronic']['EDIFF']
-        last_dE = abs(self.energies[-1][-1] - self.energies[-2][-1])
-        if last_dE < ediff:
-            return True
-        else:
-            return False
-
-    @property
-    def convergence_ionic(self):
-        """
-        Returns a boolian representing if the ionic part of the
-        calculation converged
-        """
-        energies = np.array(self.energies)
-        nsteps = len(np.unique(np.array(self.energies)[:, 0]))
-        if nsteps == 1:
-            print('This calculation does not have ionic steps')
-            return True
-        else:
-            ediffg = self.vasp_parameters['ionic']['EDIFFG']
-            if ediffg < 0:
-                last_forces_abs = np.abs(np.array(self.forces[-1]))
-                return not (np.any(last_forces_abs > abs(ediffg)))
-            else:
-                last_ionic_energy = energies[(
-                    energies[:, 0] == nsteps)][-1][-1]
-                penultimate_ionic_energy = energies[(energies[:, 0] == (
-                    nsteps - 1))][-1][-1]
-                last_dE = abs(last_ionic_energy - penultimate_ionic_energy)
-                if last_dE < ediffg:
-                    return True
-        return False
-
-    @property
-    def convergence(self):
-        """
-        Returns a boolian representing if the the electronic self-consistent
-        and ionic calculation converged
-        """
-        return (self.convergence_electronic and self.convergence_ionic)
-
-    @property
-    def is_finished(self):
-        """
-        Always returns True, need to fix this according to reading the xml as if the calc is
-        not finished we will have errors in xml parser
-        """
-        # if vasprun.xml is read the calculation is finished
-        return True
-
-    def __contains__(self, x):
-        return x in self.variables
-
-    def __getitem__(self, x):
-        return self.variables.__getitem__(x)
-
-    def __iter__(self):
-        return self.variables.__iter__()
-
-    def __len__(self):
-        return self.variables.__len__()
-
-
-def text_to_bool(text):
-    """boolians in vaspxml are stores as T or F in str format, this function coverts them to python boolians """
-    text = text.strip(' ')
-    if text == 'T' or text == '.True.' or text == '.TRUE.':
-        return True
-    else:
-        return False
-
-
-def conv(ele, _type):
-    """This function converts the xml text to the type specified in the attrib of xml tree """
-
-    if _type == 'string':
-        return ele.strip()
-    elif _type == 'int':
-        return int(ele)
-    elif _type == 'logical':
-        return text_to_bool(ele)
-    elif _type == 'float':
-        if '*' in ele:
-            return np.nan
-        else:
-            return float(ele)
-
-
-def get_varray(xml_tree):
-    """Returns an array for each varray tag in vaspxml """
-    ret = []
-    for ielement in xml_tree:
-        ret.append([float(x) for x in ielement.text.split()])
-    return ret
-
-
-def get_params(xml_tree, dest):
-    """dest should be a dictionary
-    This function is recurcive #check spelling"""
-    for ielement in xml_tree:
-        if ielement.tag == 'separator':
-            dest[ielement.attrib['name'].strip()] = {}
-            dest[ielement.attrib['name'].strip()] = get_params(
-                ielement, dest[ielement.attrib['name']])
-        else:
-            if 'type' in ielement.attrib:
-                _type = ielement.attrib['type']
-            else:
-                _type = 'float'
-            if ielement.text is None:
-                dest[ielement.attrib['name'].strip()] = None
-
-            elif len(ielement.text.split()) > 1:
-                dest[ielement.attrib['name'].strip()] = [
-                    conv(x, _type) for x in ielement.text.split()
-                ]
-            else:
-                dest[ielement.attrib['name'].strip()] = conv(
-                    ielement.text, _type)
-
-    return dest
-
-
-def get_structure(xml_tree):
-    """Returns a dictionary of the structure """
-    ret = {}
-    for ielement in xml_tree:
-        if ielement.tag == 'crystal':
-            for isub in ielement:
-                if isub.attrib['name'] == 'basis':
-                    ret['cell'] = get_varray(isub)
-                elif isub.attrib['name'] == 'volume':
-                    ret['volume'] = float(isub.text)
-                elif isub.attrib['name'] == 'rec_basis':
-                    ret['rec_cell'] = get_varray(isub)
-        elif ielement.tag == 'varray':
-            if ielement.attrib['name'] == 'positions':
-                ret['reduced'] = get_varray(ielement)
-    return ret
-
-
-def get_scstep(xml_tree):
-    """This function extracts the self-consistent step information """
-    scstep = {'time': {}, 'energy': {}}
-    for isub in xml_tree:
-        if isub.tag == 'time':
-            scstep['time'][isub.attrib['name']] = [
-                float(x) for x in isub.text.split()
-            ]
-        elif isub.tag == 'energy':
-            for ienergy in isub:
-                scstep['energy'][ienergy.attrib['name']] = float(ienergy.text)
-    return scstep
-
-
-def get_set(xml_tree, ret):
-    """ This function will extract any element taged set recurcively"""
-    if xml_tree[0].tag == 'r':
-        ret[xml_tree.attrib['comment']] = get_varray(xml_tree)
-        return ret
-    else:
-        ret[xml_tree.attrib['comment']] = {}
-        for ielement in xml_tree:
-
-            if ielement.tag == 'set':
-                ret[xml_tree.attrib['comment']][
-                    ielement.attrib['comment']] = {}
-                ret[xml_tree.attrib['comment']][
-                    ielement.attrib['comment']] = get_set(
-                        ielement, ret[xml_tree.attrib['comment']][
-                            ielement.attrib['comment']])
-        return ret
-
-
-def get_general(xml_tree, ret):
-    """ This function will parse any element in calculatio other than the structures, scsteps"""
-    if 'dimension' in [x.tag for x in xml_tree]:
-        ret['info'] = []
-        ret['data'] = {}
-        for ielement in xml_tree:
-            if ielement.tag == 'field':
-                ret['info'].append(ielement.text.strip(' '))
-            elif ielement.tag == 'set':
-                for iset in ielement:
-                    ret['data'] = get_set(iset, ret['data'])
-        return ret
-    else:
-        for ielement in xml_tree:
-            if ielement.tag == 'i':
-                if 'name' in ielement.attrib:
-                    if ielement.attrib['name'] == 'efermi':
-                        ret['efermi'] = float(ielement.text)
-                continue
-            ret[ielement.tag] = {}
-            ret[ielement.tag] = get_general(ielement, ret[ielement.tag])
-        return ret
-
-
-def parse_vasprun(vasprun):
-    tree = ET.parse(vasprun)
-    root = tree.getroot()
-
-    calculation = []
-    structures = []
-    forces = []
-    stresses = []
-    orbital_magnetization = {}
-    run_info = {}
-    incar = {}
-    general = {}
-    kpoints_info = {}
-    vasp_params = {}
-    kpoints_list = []
-    k_weights = []
-    atom_info = {}
-    for ichild in root:
-
-        if ichild.tag == 'generator':
-            for ielement in ichild:
-                run_info[ielement.attrib['name']] = ielement.text
-
-        elif ichild.tag == 'incar':
-            incar = get_params(ichild, incar)
-
-        # Skipping 1st structure which is primitive cell
-        elif ichild.tag == 'kpoints':
-
-            for ielement in ichild:
-                if ielement.items()[0][0] == 'param':
-                    kpoints_info['mode'] = ielement.items()[0][1]
-                    if kpoints_info['mode'] == 'listgenerated':
-                        kpoints_info['kpoint_vertices'] = []
-                        for isub in ielement:
-
-                            if isub.attrib == 'divisions':
-                                kpoints_info['ndivision'] = int(isub.text)
-                            else:
-                                if len(isub.text.split()) != 3:
-                                    continue
-                                kpoints_info['kpoint_vertices'].append(
-                                    [float(x) for x in isub.text.split()])
-                    else:
-                        for isub in ielement:
-                            if isub.attrib['name'] == 'divisions':
-                                kpoints_info['kgrid'] = [
-                                    int(x) for x in isub.text.split()
-                                ]
-                            elif isub.attrib['name'] == 'usershift':
-                                kpoints_info['user_shift'] = [
-                                    float(x) for x in isub.text.split()
-                                ]
-                            elif isub.attrib['name'] == 'genvec1':
-                                kpoints_info['genvec1'] = [
-                                    float(x) for x in isub.text.split()
-                                ]
-                            elif isub.attrib['name'] == 'genvec2':
-                                kpoints_info['genvec2'] = [
-                                    float(x) for x in isub.text.split()
-                                ]
-                            elif isub.attrib['name'] == 'genvec3':
-                                kpoints_info['genvec3'] = [
-                                    float(x) for x in isub.text.split()
-                                ]
-                            elif isub.attrib['name'] == 'shift':
-                                kpoints_info['shift'] = [
-                                    float(x) for x in isub.text.split()
-                                ]
-
-                elif ielement.items()[0][1] == 'kpointlist':
-                    for ik in ielement:
-                        kpoints_list.append(
-                            [float(x) for x in ik.text.split()])
-                    kpoints_list = array(kpoints_list)
-                elif ielement.items()[0][1] == 'weights':
-                    for ik in ielement:
-                        k_weights.append(float(ik.text))
-                    k_weights = array(k_weights)
-
-        # Vasp Parameters
-        elif ichild.tag == 'parameters':
-            vasp_params = get_params(ichild, vasp_params)
-
-        # Atom info
-        elif ichild.tag == 'atominfo':
-
-            for ielement in ichild:
-                if ielement.tag == 'atoms':
-                    atom_info['natom'] = int(ielement.text)
-                elif ielement.tag == 'types':
-                    atom_info['nspecies'] = int(ielement.text)
-                elif ielement.tag == 'array':
-                    if ielement.attrib['name'] == 'atoms':
-                        for isub in ielement:
-                            if isub.tag == 'set':
-                                atom_info['symbols'] = []
-                                for isym in isub:
-                                    atom_info['symbols'].append(isym[0].text)
-                    elif ielement.attrib['name'] == 'atomtypes':
-                        atom_info['atom_types'] = {}
-                        for isub in ielement:
-                            if isub.tag == 'set':
-                                for iatom in isub:
-                                    atom_info['atom_types'][iatom[1].text] = {}
-                                    atom_info['atom_types'][iatom[1].text][
-                                        'natom_per_specie'] = int(
-                                            iatom[0].text)
-                                    atom_info['atom_types'][
-                                        iatom[1].text]['mass'] = float(
-                                            iatom[2].text)
-                                    atom_info['atom_types'][
-                                        iatom[1].text]['valance'] = float(
-                                            iatom[3].text)
-                                    atom_info['atom_types'][iatom[1].text][
-                                        'pseudopotential'] = iatom[
-                                            4].text.strip()
-
-        elif ichild.tag == 'structure':
-            if ichild.attrib['name'] == 'initialpos':
-                initial_pos = get_structure(ichild)
-            elif ichild.attrib['name'] == 'finalpos':
-                final_pos = get_structure(ichild)
-
-        elif ichild.tag == 'calculation':
-            for ielement in ichild:
-                if ielement.tag == 'scstep':
-                    calculation.append(get_scstep(ielement))
-                elif ielement.tag == 'structure':
-                    structures.append(get_structure(ielement))
-                elif ielement.tag == 'varray':
-                    if ielement.attrib['name'] == 'forces':
-                        forces.append(get_varray(ielement))
-                    elif ielement.attrib['name'] == 'stress':
-                        stresses.append(get_varray(ielement))
-
-                # elif ielement.tag == 'eigenvalues':
-                #     for isub in ielement[0] :
-                #         if isub.tag == 'set':
-                #             for iset in isub :
-                #                 eigen_values[iset.attrib['comment']] = {}
-                #                 for ikpt in iset :
-                #                     eigen_values[iset.attrib['comment']][ikpt.attrib['comment']] = get_varray(ikpt)
-
-                elif ielement.tag == 'separator':
-                    if ielement.attrib['name'] == "orbital magnetization":
-                        for isub in ielement:
-                            orbital_magnetization[isub.attrib['name']] = [
-                                float(x) for x in isub.text.split()
-                            ]
-
-                # elif ielement.tag == 'dos':
-                #     for isub in ielement :
-                #         if 'name' in isub.attrib:
-                #             if isub.attrib['name'] == 'efermi' :
-                #                 dos['efermi'] = float(isub.text)
-                #             else :
-                #                 dos[isub.tag] = {}
-                #                 dos[isub.tag]['info'] = []
-                #               for iset in isub[0]  :
-                #                   if iset.tag == 'set' :
-                #                       for isub_set in iset:
-                #                           dos[isub.tag] = get_set(isub_set,dos[isub.tag])
-                #                   elif iset.tag == 'field' :
-                #                       dos[isub.tag]['info'].append(iset.text.strip(' '))
-                else:
-                    general[ielement.tag] = {}
-                    general[ielement.tag] = get_general(
-                        ielement, general[ielement.tag])
-        # NEED TO ADD ORBITAL MAGNETIZATION
-
-    return {
-        'calculation': calculation,
-        'structures': structures,
-        'forces': forces,
-        'run_info': run_info,
-        'incar': incar,
-        'general': general,
-        'kpoints_info': kpoints_info,
-        'vasp_params': vasp_params,
-        'kpoints': {
-            'kpoints_list': kpoints_list,
-            'k_weights': k_weights
-        },
-        'atom_info': atom_info
-    }
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Aug 19 20:49:03 2020
+
+@author: Pedram Tavadze, Logan Lang
+"""
+
+from ...core import Structure, DensityOfStates
+from numpy import array
+import xml.etree.ElementTree as ET
+import os
+import numpy as np
+import collections
+
+
+class VaspXML(collections.abc.Mapping):
+    """contains."""
+    def __init__(self, filename='vasprun.xml', dos_interpolation_factor=None):
+
+        self.variables = {}
+        self.dos_interpolation_factor = dos_interpolation_factor
+
+        if not os.path.isfile(filename):
+            raise ValueError('File not found ' + filename)
+        else:
+            self.filename = filename
+
+        self.spins_dict = {'spin 1': 'Spin-up', 'spin 2': 'Spin-down'}
+        # self.positions = None
+        # self.stress = None
+        self.bands = None
+        # self.array_sizes = {}
+        self.data = self.read()
+
+    def repair(self):
+        """
+        repairs the wrong syntaxes in vasprun.xml
+        """
+        
+        
+
+    def read(self):
+        """
+        Read and parse vasprun.xml.
+
+        Returns
+        -------
+        TYPE
+            DESCRIPTION.
+
+        """
+        return parse_vasprun(self.filename)
+
+    def _get_dos_total(self):
+
+        spins = list(
+            self.data['general']['dos']['total']['array']['data'].keys())
+        energies = np.array(self.data['general']['dos']['total']['array']
+                            ['data'][spins[0]])[:, 0]
+        dos_total = {'energies': energies}
+        for ispin in spins:
+            dos_total[self.spins_dict[ispin]] = np.array(
+                self.data['general']['dos']['total']['array']['data']
+                [ispin])[:, 1]
+
+        return dos_total, list(dos_total.keys())
+
+    def _get_dos_projected(self, atoms=[]):
+
+        if len(atoms) == 0:
+            atoms = np.arange(self.initial_structure.natoms)
+
+        if 'partial' in self.data['general']['dos']:
+            dos_projected = {}
+            ion_list = ["ion %s" % str(x + 1) for x in atoms
+                        ]  # using this name as vasrun.xml uses ion #
+            for i in range(len(ion_list)):
+                iatom = ion_list[i]
+                name = self.initial_structure.atoms[atoms[i]] + str(atoms[i])
+                spins = list(self.data['general']['dos']['partial']['array']
+                             ['data'][iatom].keys())
+                energies = np.array(
+                    self.data['general']['dos']['partial']['array']['data']
+                    [iatom][spins[0]][spins[0]])[:, 0]
+                dos_projected[name] = {'energies': energies}
+                for ispin in spins:
+                    dos_projected[name][self.spins_dict[ispin]] = np.array(
+                        self.data['general']['dos']['partial']['array']['data']
+                        [iatom][ispin][ispin])[:, 1:]
+            return dos_projected, self.data['general']['dos']['partial'][
+                'array']['info']
+        else:
+            print(
+                "This calculation does not include partial density of states")
+            return None, None
+
+    @property
+    def dos(self):
+        energies = self.dos_total['energies']
+        total = []
+        for ispin in self.dos_total:
+            if ispin == 'energies':
+                continue
+            total.append(self.dos_total[ispin])
+        # total = np.array(total).T
+        return DensityOfStates(
+            energies=energies,
+            total=total,
+            projected=self.dos_projected,
+            interpolation_factor=self.dos_interpolation_factor)
+
+    @property
+    def dos_to_dict(self):
+        """
+        Returns the complete density (total,projected) of states as a python dictionary
+        """
+        return {
+            'total': self._get_dos_total(),
+            'projected': self._get_dos_projected()
+        }
+
+    @property
+    def dos_total(self):
+        """
+        Returns the total density of states as a pychemia.visual.DensityOfSates object
+        """
+        dos_total, labels = self._get_dos_total()
+        dos_total['energies'] -= self.fermi
+
+        return dos_total
+
+    @property
+    def dos_projected(self):
+        """
+        Returns the projected DOS as a multi-dimentional array, to be used in the
+        pyprocar.core.dos object
+        """
+        ret = []
+        dos_projected, info = self._get_dos_projected()
+        if dos_projected is None:
+            return None
+        norbitals = len(info) - 1
+        info[0] = info[0].capitalize()
+        labels = []
+        labels.append(info[0])
+        ret = []
+        for iatom in dos_projected:
+            temp_atom = []
+            for iorbital in range(norbitals):
+                temp_spin = []
+                for key in dos_projected[iatom]:
+                    if key == 'energies':
+                        continue
+                    temp_spin.append(dos_projected[iatom][key][:, iorbital])
+                temp_atom.append(temp_spin)
+            ret.append([temp_atom])
+        return ret
+
+    @property
+    def kpoints(self):
+        """
+        Returns the kpoints used in the calculation in form of a pychemia.core.KPoints object
+        """
+
+        if self.data['kpoints_info']['mode'] == 'listgenerated':
+            kpoints = dict(
+                mode='path',
+                kvertices=self.data['kpoints_info']['kpoint_vertices'])
+        else:
+            kpoints = dict(mode=self.data['kpoints_info']['mode'].lower(),
+                           grid=self.data['kpoints_info']['kgrid'],
+                           shifts=self.data['kpoints_info']['user_shift'])
+        return kpoints
+
+    @property
+    def kpoints_list(self):
+        """
+        Returns the list of kpoints and weights used in the calculation in form of a pychemia.core.KPoints object
+        """
+        return dict(mode='reduced',
+                    kpoints_list=self.data['kpoints']['kpoints_list'],
+                    weights=self.data['kpoints']['k_weights'])
+
+    @property
+    def incar(self):
+        """
+        Returns the incar parameters used in the calculation as pychemia.code.vasp.VaspIncar object
+        """
+        return self.data['incar']
+
+    @property
+    def vasp_parameters(self):
+        """
+        Returns all of the parameters vasp has used in this calculation
+        """
+        return self.data['vasp_params']
+
+    @property
+    def potcar_info(self):
+        """
+        Returns the information about pseudopotentials(POTCAR) used in this calculation
+        """
+        return self.data['atom_info']['atom_types']
+
+    @property
+    def fermi(self):
+        """
+        Returns the fermi energy
+        """
+        return self.data['general']['dos']['efermi']
+
+    @property
+    def species(self):
+        """
+        Returns the species in POSCAR
+        """
+        return self.initial_structure.species
+
+    @property
+    def structures(self):
+        """
+        Returns a list of pychemia.core.Structure representing all the ionic step structures
+        """
+        symbols = [x.strip() for x in self.data['atom_info']['symbols']]
+        structures = []
+        for ist in self.data['structures']:
+
+            st = Structure(atoms=symbols,
+                           fractional_coordinates=ist['reduced'],
+                           lattice=ist['cell'])
+            structures.append(st)
+        return structures
+
+    @property
+    def structure(self):
+        """
+        crystal structure of the last step
+        """
+        return self.structures[-1]
+
+    @property
+    def forces(self):
+        """
+        Returns all the forces in ionic steps
+        """
+        return self.data['forces']
+
+    @property
+    def initial_structure(self):
+        """
+        Returns the initial Structure as a pychemia structure
+        """
+        return self.structures[0]
+
+    @property
+    def final_structure(self):
+        """
+        Returns the final Structure as a pychemia structure
+        """
+
+        return self.structures[-1]
+
+    @property
+    def iteration_data(self):
+        """
+        Returns a list of information in each electronic and ionic step of calculation
+        """
+        return self.data['calculation']
+
+    @property
+    def energies(self):
+        """
+        Returns a list of energies in each electronic and ionic step [ionic step,electronic step, energy]
+        """
+        scf_step = 0
+        ion_step = 0
+        double_counter = 1
+        energies = []
+        for calc in self.data['calculation']:
+            if 'ewald' in calc['energy']:
+                if double_counter == 0:
+                    double_counter += 1
+                    scf_step += 1
+                elif double_counter == 1:
+                    double_counter = 0
+                    ion_step += 1
+                    scf_step = 1
+            else:
+                scf_step += 1
+            energies.append([ion_step, scf_step, calc['energy']['e_0_energy']])
+        return energies
+
+    @property
+    def last_energy(self):
+        """
+        Returns the last calculated energy of the system
+        """
+        return self.energies[-1][-1]
+
+    @property
+    def energy(self):
+        """
+        Returns the last calculated energy of the system
+        """
+        return self.last_energy
+
+    @property
+    def convergence_electronic(self):
+        """
+        Returns a boolian representing if the last electronic self-consistent
+        calculation converged
+        """
+        ediff = self.vasp_parameters['electronic']['EDIFF']
+        last_dE = abs(self.energies[-1][-1] - self.energies[-2][-1])
+        if last_dE < ediff:
+            return True
+        else:
+            return False
+
+    @property
+    def convergence_ionic(self):
+        """
+        Returns a boolian representing if the ionic part of the
+        calculation converged
+        """
+        energies = np.array(self.energies)
+        nsteps = len(np.unique(np.array(self.energies)[:, 0]))
+        if nsteps == 1:
+            print('This calculation does not have ionic steps')
+            return True
+        else:
+            ediffg = self.vasp_parameters['ionic']['EDIFFG']
+            if ediffg < 0:
+                last_forces_abs = np.abs(np.array(self.forces[-1]))
+                return not (np.any(last_forces_abs > abs(ediffg)))
+            else:
+                last_ionic_energy = energies[(
+                    energies[:, 0] == nsteps)][-1][-1]
+                penultimate_ionic_energy = energies[(energies[:, 0] == (
+                    nsteps - 1))][-1][-1]
+                last_dE = abs(last_ionic_energy - penultimate_ionic_energy)
+                if last_dE < ediffg:
+                    return True
+        return False
+
+    @property
+    def convergence(self):
+        """
+        Returns a boolian representing if the the electronic self-consistent
+        and ionic calculation converged
+        """
+        return (self.convergence_electronic and self.convergence_ionic)
+
+    @property
+    def is_finished(self):
+        """
+        Always returns True, need to fix this according to reading the xml as if the calc is
+        not finished we will have errors in xml parser
+        """
+        # if vasprun.xml is read the calculation is finished
+        return True
+
+    def __contains__(self, x):
+        return x in self.variables
+
+    def __getitem__(self, x):
+        return self.variables.__getitem__(x)
+
+    def __iter__(self):
+        return self.variables.__iter__()
+
+    def __len__(self):
+        return self.variables.__len__()
+
+
+def text_to_bool(text):
+    """boolians in vaspxml are stores as T or F in str format, this function coverts them to python boolians """
+    text = text.strip(' ')
+    if text == 'T' or text == '.True.' or text == '.TRUE.':
+        return True
+    else:
+        return False
+
+
+def conv(ele, _type):
+    """This function converts the xml text to the type specified in the attrib of xml tree """
+
+    if _type == 'string':
+        return ele.strip()
+    elif _type == 'int':
+        return int(ele)
+    elif _type == 'logical':
+        return text_to_bool(ele)
+    elif _type == 'float':
+        if '*' in ele:
+            return np.nan
+        else:
+            return float(ele)
+
+
+def get_varray(xml_tree):
+    """Returns an array for each varray tag in vaspxml """
+    ret = []
+    for ielement in xml_tree:
+        ret.append([float(x) for x in ielement.text.split()])
+    return ret
+
+
+def get_params(xml_tree, dest):
+    """dest should be a dictionary
+    This function is recurcive #check spelling"""
+    for ielement in xml_tree:
+        if ielement.tag == 'separator':
+            dest[ielement.attrib['name'].strip()] = {}
+            dest[ielement.attrib['name'].strip()] = get_params(
+                ielement, dest[ielement.attrib['name']])
+        else:
+            if 'type' in ielement.attrib:
+                _type = ielement.attrib['type']
+            else:
+                _type = 'float'
+            if ielement.text is None:
+                dest[ielement.attrib['name'].strip()] = None
+
+            elif len(ielement.text.split()) > 1:
+                dest[ielement.attrib['name'].strip()] = [
+                    conv(x, _type) for x in ielement.text.split()
+                ]
+            else:
+                dest[ielement.attrib['name'].strip()] = conv(
+                    ielement.text, _type)
+
+    return dest
+
+
+def get_structure(xml_tree):
+    """Returns a dictionary of the structure """
+    ret = {}
+    for ielement in xml_tree:
+        if ielement.tag == 'crystal':
+            for isub in ielement:
+                if isub.attrib['name'] == 'basis':
+                    ret['cell'] = get_varray(isub)
+                elif isub.attrib['name'] == 'volume':
+                    ret['volume'] = float(isub.text)
+                elif isub.attrib['name'] == 'rec_basis':
+                    ret['rec_cell'] = get_varray(isub)
+        elif ielement.tag == 'varray':
+            if ielement.attrib['name'] == 'positions':
+                ret['reduced'] = get_varray(ielement)
+    return ret
+
+
+def get_scstep(xml_tree):
+    """This function extracts the self-consistent step information """
+    scstep = {'time': {}, 'energy': {}}
+    for isub in xml_tree:
+        if isub.tag == 'time':
+            scstep['time'][isub.attrib['name']] = [
+                float(x) for x in isub.text.split()
+            ]
+        elif isub.tag == 'energy':
+            for ienergy in isub:
+                scstep['energy'][ienergy.attrib['name']] = float(ienergy.text)
+    return scstep
+
+
+def get_set(xml_tree, ret):
+    """ This function will extract any element taged set recurcively"""
+    if xml_tree[0].tag == 'r':
+        ret[xml_tree.attrib['comment']] = get_varray(xml_tree)
+        return ret
+    else:
+        ret[xml_tree.attrib['comment']] = {}
+        for ielement in xml_tree:
+
+            if ielement.tag == 'set':
+                ret[xml_tree.attrib['comment']][
+                    ielement.attrib['comment']] = {}
+                ret[xml_tree.attrib['comment']][
+                    ielement.attrib['comment']] = get_set(
+                        ielement, ret[xml_tree.attrib['comment']][
+                            ielement.attrib['comment']])
+        return ret
+
+
+def get_general(xml_tree, ret):
+    """ This function will parse any element in calculatio other than the structures, scsteps"""
+    if 'dimension' in [x.tag for x in xml_tree]:
+        ret['info'] = []
+        ret['data'] = {}
+        for ielement in xml_tree:
+            if ielement.tag == 'field':
+                ret['info'].append(ielement.text.strip(' '))
+            elif ielement.tag == 'set':
+                for iset in ielement:
+                    ret['data'] = get_set(iset, ret['data'])
+        return ret
+    else:
+        for ielement in xml_tree:
+            if ielement.tag == 'i':
+                if 'name' in ielement.attrib:
+                    if ielement.attrib['name'] == 'efermi':
+                        ret['efermi'] = float(ielement.text)
+                continue
+            ret[ielement.tag] = {}
+            ret[ielement.tag] = get_general(ielement, ret[ielement.tag])
+        return ret
+
+
+def parse_vasprun(vasprun):
+    tree = ET.parse(vasprun)
+    root = tree.getroot()
+
+    calculation = []
+    structures = []
+    forces = []
+    stresses = []
+    orbital_magnetization = {}
+    run_info = {}
+    incar = {}
+    general = {}
+    kpoints_info = {}
+    vasp_params = {}
+    kpoints_list = []
+    k_weights = []
+    atom_info = {}
+    for ichild in root:
+
+        if ichild.tag == 'generator':
+            for ielement in ichild:
+                run_info[ielement.attrib['name']] = ielement.text
+
+        elif ichild.tag == 'incar':
+            incar = get_params(ichild, incar)
+
+        # Skipping 1st structure which is primitive cell
+        elif ichild.tag == 'kpoints':
+
+            for ielement in ichild:
+                if ielement.items()[0][0] == 'param':
+                    kpoints_info['mode'] = ielement.items()[0][1]
+                    if kpoints_info['mode'] == 'listgenerated':
+                        kpoints_info['kpoint_vertices'] = []
+                        for isub in ielement:
+
+                            if isub.attrib == 'divisions':
+                                kpoints_info['ndivision'] = int(isub.text)
+                            else:
+                                if len(isub.text.split()) != 3:
+                                    continue
+                                kpoints_info['kpoint_vertices'].append(
+                                    [float(x) for x in isub.text.split()])
+                    else:
+                        for isub in ielement:
+                            if isub.attrib['name'] == 'divisions':
+                                kpoints_info['kgrid'] = [
+                                    int(x) for x in isub.text.split()
+                                ]
+                            elif isub.attrib['name'] == 'usershift':
+                                kpoints_info['user_shift'] = [
+                                    float(x) for x in isub.text.split()
+                                ]
+                            elif isub.attrib['name'] == 'genvec1':
+                                kpoints_info['genvec1'] = [
+                                    float(x) for x in isub.text.split()
+                                ]
+                            elif isub.attrib['name'] == 'genvec2':
+                                kpoints_info['genvec2'] = [
+                                    float(x) for x in isub.text.split()
+                                ]
+                            elif isub.attrib['name'] == 'genvec3':
+                                kpoints_info['genvec3'] = [
+                                    float(x) for x in isub.text.split()
+                                ]
+                            elif isub.attrib['name'] == 'shift':
+                                kpoints_info['shift'] = [
+                                    float(x) for x in isub.text.split()
+                                ]
+
+                elif ielement.items()[0][1] == 'kpointlist':
+                    for ik in ielement:
+                        kpoints_list.append(
+                            [float(x) for x in ik.text.split()])
+                    kpoints_list = array(kpoints_list)
+                elif ielement.items()[0][1] == 'weights':
+                    for ik in ielement:
+                        k_weights.append(float(ik.text))
+                    k_weights = array(k_weights)
+
+        # Vasp Parameters
+        elif ichild.tag == 'parameters':
+            vasp_params = get_params(ichild, vasp_params)
+
+        # Atom info
+        elif ichild.tag == 'atominfo':
+
+            for ielement in ichild:
+                if ielement.tag == 'atoms':
+                    atom_info['natom'] = int(ielement.text)
+                elif ielement.tag == 'types':
+                    atom_info['nspecies'] = int(ielement.text)
+                elif ielement.tag == 'array':
+                    if ielement.attrib['name'] == 'atoms':
+                        for isub in ielement:
+                            if isub.tag == 'set':
+                                atom_info['symbols'] = []
+                                for isym in isub:
+                                    atom_info['symbols'].append(isym[0].text)
+                    elif ielement.attrib['name'] == 'atomtypes':
+                        atom_info['atom_types'] = {}
+                        for isub in ielement:
+                            if isub.tag == 'set':
+                                for iatom in isub:
+                                    atom_info['atom_types'][iatom[1].text] = {}
+                                    atom_info['atom_types'][iatom[1].text][
+                                        'natom_per_specie'] = int(
+                                            iatom[0].text)
+                                    atom_info['atom_types'][
+                                        iatom[1].text]['mass'] = float(
+                                            iatom[2].text)
+                                    atom_info['atom_types'][
+                                        iatom[1].text]['valance'] = float(
+                                            iatom[3].text)
+                                    atom_info['atom_types'][iatom[1].text][
+                                        'pseudopotential'] = iatom[
+                                            4].text.strip()
+
+        elif ichild.tag == 'structure':
+            if ichild.attrib['name'] == 'initialpos':
+                initial_pos = get_structure(ichild)
+            elif ichild.attrib['name'] == 'finalpos':
+                final_pos = get_structure(ichild)
+
+        elif ichild.tag == 'calculation':
+            for ielement in ichild:
+                if ielement.tag == 'scstep':
+                    calculation.append(get_scstep(ielement))
+                elif ielement.tag == 'structure':
+                    structures.append(get_structure(ielement))
+                elif ielement.tag == 'varray':
+                    if ielement.attrib['name'] == 'forces':
+                        forces.append(get_varray(ielement))
+                    elif ielement.attrib['name'] == 'stress':
+                        stresses.append(get_varray(ielement))
+
+                # elif ielement.tag == 'eigenvalues':
+                #     for isub in ielement[0] :
+                #         if isub.tag == 'set':
+                #             for iset in isub :
+                #                 eigen_values[iset.attrib['comment']] = {}
+                #                 for ikpt in iset :
+                #                     eigen_values[iset.attrib['comment']][ikpt.attrib['comment']] = get_varray(ikpt)
+
+                elif ielement.tag == 'separator':
+                    if ielement.attrib['name'] == "orbital magnetization":
+                        for isub in ielement:
+                            orbital_magnetization[isub.attrib['name']] = [
+                                float(x) for x in isub.text.split()
+                            ]
+
+                # elif ielement.tag == 'dos':
+                #     for isub in ielement :
+                #         if 'name' in isub.attrib:
+                #             if isub.attrib['name'] == 'efermi' :
+                #                 dos['efermi'] = float(isub.text)
+                #             else :
+                #                 dos[isub.tag] = {}
+                #                 dos[isub.tag]['info'] = []
+                #               for iset in isub[0]  :
+                #                   if iset.tag == 'set' :
+                #                       for isub_set in iset:
+                #                           dos[isub.tag] = get_set(isub_set,dos[isub.tag])
+                #                   elif iset.tag == 'field' :
+                #                       dos[isub.tag]['info'].append(iset.text.strip(' '))
+                else:
+                    general[ielement.tag] = {}
+                    general[ielement.tag] = get_general(
+                        ielement, general[ielement.tag])
+        # NEED TO ADD ORBITAL MAGNETIZATION
+
+    return {
+        'calculation': calculation,
+        'structures': structures,
+        'forces': forces,
+        'run_info': run_info,
+        'incar': incar,
+        'general': general,
+        'kpoints_info': kpoints_info,
+        'vasp_params': vasp_params,
+        'kpoints': {
+            'kpoints_list': kpoints_list,
+            'k_weights': k_weights
+        },
+        'atom_info': atom_info
+    }
```

### Comparing `PyProcar-5.6.6/pyprocar/version.py` & `PyProcar-6.0.0/pyprocar/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-
-# THIS FILE IS GENERATED FROM PYPROCAR SETUP.PY.
-name = 'PyProcar'
-version = '5.6.6'
-description = 'A Python library for electronic structure pre/post-processing. '
-url = 'https://github.com/romerogroup/pyprocar'
-author = 'Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah'
-email = 'fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com'
-status = 'development'
-copyright = 'Copyright 2021'
-date = 'March 6th, 2022'
+# THIS FILE IS GENERATED FROM PYPROCAR SETUP.PY.
+name = 'PyProcar'
+version = '6.0.0'
+description = 'A Python library for electronic structure pre/post-processing. '
+author = 'Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah'
+email = 'fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com'
+url = 'https://github.com/romerogroup/pyprocar'
+download_url = 'https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz'
+status = 'development'
+copyright = 'Copyright 2021'
+date = 'Jun 10th, 2021'
```

### Comparing `PyProcar-5.6.6/scripts/procar.py` & `PyProcar-6.0.0/scripts/procar.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,816 +1,816 @@
-#!/usr/bin/env python
-
-"""
-Stand alone script for PyProcar.
-
-This calls the modules in the /pyprocar directory.
-
-Based on the original script developed by Aldo Romero (alromero@mail.wvu.edu) and
-Francisco Munoz (fvmunoz@gmail.com).
-"""
-
-import argparse
-from argparse import RawTextHelpFormatter
-import pyprocar
-import numpy as np
-
-
-def call_bandsplot(args):
-    """
-	This module calls the band structure plotting function.
-	"""
-
-    pyprocar.bandsplot(
-        args.file,
-        mode=args.mode,
-        color=args.color,
-        abinit_output=args.abinit,
-        spin=args.spin,
-        atoms=args.atoms,
-        orbitals=args.orbitals,
-        fermi=args.fermi,
-        elimit=args.elimit,
-        mask=args.mask,
-        markersize=args.markersize,
-        cmap=args.cmap,
-        vmax=args.vmax,
-        vmin=args.vmin,
-        grid=args.grid,
-        marker=args.marker,
-        permissive=args.permissive,
-        human=args.human,
-        savefig=args.savefig,
-        kticks=args.kticks,
-        knames=args.knames,
-        title=args.title,
-        outcar=args.outcar,
-        kpointsfile=args.kpointsfile,
-        kdirect=args.kdirect,
-    )
-
-
-def call_kpath(args):
-    """
-	This module calls the k-path generation function.
-	"""
-
-    pyprocar.kpath(
-        args.infile,
-        grid_size=args.grid_size,
-        with_time_reversal=args.with_time_reversal,
-        recipe=args.recipe,
-        threshold=args.threshold,
-        symprec=args.symprec,
-        angle_tolerence=args.angle_tolerence,
-        supercell_matrix=args.supercell_matrix,
-    )
-
-
-def call_repair(args):
-    """
-	This module calls the repair function.
-	"""
-    pyprocar.repair(args.infile, args.outfile)
-
-
-def call_generate2dkmesh(args):
-    """
-	This module calls the k-mesh generating function.
-	"""
-    pyprocar.generate2dkmesh(
-        args.x1, args.y1, args.x2, args.y2, args.z, args.nkx, args.nky
-    )
-
-
-def call_fermi2D(args):
-    """
-	This module calls the fermi2D plotting function.
-	"""
-    pyprocar.fermi2D(
-        args.file,
-        outcar=args.outcar,
-        spin=args.spin,
-        atoms=args.atoms,
-        orbitals=args.orbitals,
-        energy=args.energy,
-        fermi=args.fermi,
-        rec_basis=args.rec_basis,
-        rot_symm=args.rot_symm,
-        translate=args.translate,
-        rotation=args.rotation,
-        human=args.human,
-        mask=args.mask,
-        savefig=args.savefig,
-        st=args.st,
-        noarrow=args.noarrow,
-    )
-
-
-def call_fermi3D(args):
-    """
-	This module calls the fermi3D plotting function.
-	"""
-    pyprocar.fermi3D(
-        args.procar,
-        args.outcar,
-        args.bands,
-        scale=args.scale,
-        mode=args.mode,
-        st=args.st,
-        kwargs=args.kwargs,
-    )
-
-
-def call_filter(args):
-    """
-	This module calls the filter function.
-	"""
-
-    pyprocar.filter(
-        args.infile,
-        args.outfile,
-        atoms=args.atoms,
-        orbitals=args.orbitals,
-        orbital_names=args.orbital_names,
-        bands=args.bands,
-        spin=args.spin,
-        human_atoms=args.human_atoms,
-    )
-
-
-def call_cat(args):
-    """
-	This module calls the cat function.
-	"""
-    pyprocar.cat(inFiles=args.inFiles, outFile=args.outFile, gz=args.gz)
-
-
-def call_mergeabinit(args):
-    """
-	This module calls the mergeabinit function.
-	"""
-    pyprocar.mergeabinit(args.outfile)
-
-
-def call_bandgap(args):
-    """
-	This module calls the mergeabinit function.
-	"""
-    pyprocar.bandgap(args.procar, args.outcar, args.code, args.fermi)
-
-
-def call_unfold(args):
-    """
-	This module calls the band unfolding function.
-	"""
-    pyprocar.unfold(
-        fname=args.fname,
-        poscar=args.poscar,
-        outcar=args.outcar,
-        supercell_matrix=args.supercell_matrix,
-        ispin=args.ispin,
-        efermi=args.efermi,
-        shift_efermi=args.shift_efermi,
-        elimit=args.elimit,
-        kticks=args.kticks,
-        knames=args.knames,
-        print_kpts=args.print_kpts,
-        show_band=args.show_band,
-        width=args.width,
-        color=args.color,
-        savetab=args.savetab,
-        savefig=args.savefig,
-    )
-
-
-if __name__ == "__main__":
-
-    import sys
-
-    args = sys.argv[1:]
-
-    if args:
-
-        # Top level parser
-        description = "PyProcar: A Python library for analyzing PROCAR files."
-        parser = argparse.ArgumentParser(description=description)
-        subparsers = parser.add_subparsers(help="sub-command help")
-
-        ############### cat ############################################
-
-        phelp = (
-            "concatenation of PROCARs files, they should be compatible (ie: "
-            "joining parts of a large bandstructure calculation)."
-        )
-        parserCat = subparsers.add_parser("cat", help=phelp)
-
-        phelp = "Input files. They can be compressed"
-        parserCat.add_argument("inFiles", nargs="+", help=phelp)
-
-        phelp = "Output file."
-        parserCat.add_argument("outFile", help=phelp)
-
-        phelp = "Writes a gzipped outfile (if needed a .gz extension automatically will be added)"
-        parserCat.add_argument("--gz", help=phelp, action="store_true")
-
-        parserCat.set_defaults(func=call_cat)
-
-        ################ mergeabinit ##################################
-
-        parsermergeabinit = subparsers.add_parser(
-            "mergeabinit", help="Merge Abinit PROCARs."
-        )
-        parsermergeabinit.add_argument("outfile", help="Merged PROCAR")
-        parsermergeabinit.set_defaults(func=call_mergeabinit)
-
-        ############### unfold #######################################
-        parserunfold = subparsers.add_parser("unfold", help="Band unfolding.")
-        parserunfold.add_argument("-fname", help="PROCAR filename.")
-        parserunfold.add_argument("-poscar", help="POSCAR filename.")
-        parserunfold.add_argument(
-            "-outcar", help="OUTCAR filename. Used to get Fermi energy."
-        )
-        parserunfold.add_argument(
-            "-supercell_matrix",
-            help="Supercell matrix from primitive cell to supercell.",
-        )
-        parserunfold.add_argument(
-            "-ispin",
-            help="None - non spin polarized \n 1 - spin up" "\n 2 - spin down.",
-            choices=[None, 1, 2],
-        )
-        parserunfold.add_argument(
-            "-efermi", help="Fermi energy. Only when no OUTCAR is given."
-        )
-        parserunfold.add_argument("-elimit", help="Range of energy to be plotted.")
-        parserunfold.add_argument(
-            "-kticks",
-            help="The indices of k-points for labels.",
-            type=int,
-            nargs="+",
-            action="append",
-        )
-        parserunfold.add_argument(
-            "-knames", help="Labels of k-points.", type=str, nargs="+", action="append"
-        )
-        parserunfold.add_argument(
-            "-print_kpts", help="Print all the k-points to screen.", action="store_true"
-        )
-        parserunfold.add_argument(
-            "-show_band",
-            help="Whether to plot the bands before unfolding.",
-            action="store_true",
-        )
-        parserunfold.add_argument(
-            "-width", help="Width of the unfolded band.", type=float
-        )
-        parserunfold.add_argument(
-            "-color", help="Color of the unfolded band.", type=str
-        )
-        parserunfold.add_argument(
-            "-savetab",
-            help="The csv file name of which the table of unfolding result will be written into",
-        )
-        parserunfold.add_argument(
-            "-savefig", help="The file name of which the figure will be saved."
-        )
-        parserunfold.set_defaults(func=call_unfold)
-
-        ############### filter ##########################################
-        phelp = (
-            "Filters (manipulates) the data of the input file (PROCAR-like) and"
-            " it yields a new file (PROCAR-like too) with the changes. This "
-            "method can do only one manipulation at time (ie: spin, atoms, "
-            "bands or orbitals)."
-        )
-        parserFilter = subparsers.add_parser("filter", help=phelp)
-
-        phelp = "Input file. Can be compressed"
-        parserFilter.add_argument("inFile", help=phelp)
-
-        phelp = "Output file."
-        parserFilter.add_argument("outFile", help=phelp)
-
-        OptFilter = parserFilter.add_mutually_exclusive_group()
-        phelp = (
-            "List of atoms to group (add) as a new single entry. Each group of"
-            " atoms should be specified in a different `--atoms` option. "
-            "Example: `procar.py filter in out -a 0 1 -a 2` will group the 1st"
-            " and 2nd atoms, while keeping the 3rd atom in `out` (any atom "
-            "beyond the 3rd will be discarded). Mind the last atomic field "
-            "present on a PROCAR file, is not an atom, is the 'tot' value (sum"
-            " of all atoms), this field always is included in the outfile and "
-            "it always is the 'tot' value from infile, regardless the selection"
-            " of atoms."
-        )
-        OptFilter.add_argument(
-            "-a", "--atoms", type=int, nargs="+", action="append", help=phelp
-        )
-
-        phelp = (
-            "List of orbitals to group as a single entry. Each group of "
-            "orbitals needs a different `--orbitals` list. By instance, to "
-            "group orbitals in 's','p', 'd' it is needed `-o 0 -o 1 2 3 -o 4 5 "
-            "6 7 8`. Where 0=s, 1,2,3=px,py,pz, 4...9=dxx...dyz. Mind the last "
-            "value (aka) 'tot' always is written."
-        )
-        OptFilter.add_argument(
-            "-o", "--orbitals", help=phelp, type=int, nargs="+", action="append"
-        )
-
-        phelp = (
-            "Keeps only the bands between `min` and `max` indexes. To keep the "
-            "bands from 120 to 150 you should give `-b 120 150 `. It is not "
-            "obvious which indexes are in the interest region, therefore I "
-            "recommend you trial and error "
-        )
-        OptFilter.add_argument("-b", "--bands", help=phelp, type=int, nargs=2)
-
-        phelp = (
-            "Which spin components should be written: 0=density, 1,2,3=Sx,Sy,Sz."
-            " They are not averaged."
-        )
-        OptFilter.add_argument("-s", "--spin", help=phelp, type=int, nargs="+")
-
-        phelp = (
-            "enable to give atoms list in a more human, 1-based order (say the"
-            " 1st is 1, 2nd is 2 and so on ). Mind: this only holds for atoms."
-        )
-        parserFilter.add_argument("--human", help=phelp, action="store_true")
-
-        phelp = (
-            "List of names of new 'orbitals' to appear in the new file, eg. "
-            "(`--orbital_names s p d` for a 's', 'p', 'd'). Only meaningful "
-            "when manipulating the orbitals, ie: using `-o` "
-        )
-        parserFilter.add_argument("--orbital_names", help=phelp, nargs="+")
-
-        parserFilter.set_defaults(func=call_filter)
-
-        ################ fermi2D ##########################################
-        parserFermi2D = subparsers.add_parser(
-            "fermi2D",
-            help="Plot the Fermi surface for a 2D Brillouin zone (layer-wise)"
-            "along z and just perpendicular to z! (actually k_z)",
-        )
-
-        phelp = "Input file. It can be compressed"
-        parserFermi2D.add_argument("file", help=phelp)
-
-        phelp = (
-            "Spin component to be used: for non-polarized calculations density "
-            "is '-s 0'. For spin polarized case test '-s 0' (ignore the spin) or"
-            " '-s 1' (assing a sign to the spin channel). For "
-            "non-collinear stuff you can use '-s 0', '-s 1', '-s 2', -s "
-            "3 for the magnitude, x, y, z components of your spin "
-            "vector, in this case you really want to see spin textures "
-            "'--st'. Default: s=0"
-        )
-        parserFermi2D.add_argument(
-            "-s", "--spin", type=int, choices=[0, 1, 2, 3], default=0, help=phelp
-        )
-
-        phelp = (
-            "List of atoms to be used (0-based): ie. '-a 0 2' to select the 1st"
-            " and 3rd. It defaults to the last one (-a -1 the 'tot' entry)"
-        )
-        parserFermi2D.add_argument("-a", "--atoms", type=int, nargs="+", help=phelp)
-
-        phelp = (
-            "Orbital index(es) to be used 0-based. Take a look to the PROCAR "
-            "file. Its default is the last field (ie: 'tot'). From a standard "
-            "PROCAR: `-o 0`='s', `-o 1 2 3`='p', `-o 4 5 6 7 8`='d'."
-        )
-        parserFermi2D.add_argument("-o", "--orbitals", type=int, nargs="+", help=phelp)
-
-        phelp = (
-            "Energy for the surface. To plot the Fermi surface at Fermi Energy `-e 0`"
-        )
-        parserFermi2D.add_argument(
-            "-e", "--energy", help=phelp, type=float, required=True
-        )
-
-        phelp = (
-            "Set the Fermi energy (or any reference energy) as zero. To get it "
-            "you should `grep E-fermi` the self-consistent OUTCAR. See `--outcar`"
-        )
-        parserFermi2D.add_argument("-f", "--fermi", help=phelp, type=float)
-
-        phelp = (
-            "reciprocal space basis vectors. 9 number are required b1x b1y ... "
-            " b3z. This option is quite involved, so I recommend you to use `--outcar`"
-        )
-        parserFermi2D.add_argument("--rec_basis", help=phelp, type=float, nargs=9)
-
-        phelp = (
-            "Apply a rotational symmetry to unfold the Kpoints found. If your"
-            "PROCAR only has a portion of the Brillouin Zone, you may want to "
-            "plot the FULL BZ (ie: a Dirac cone at Gamma will look like a cone "
-            "and not like a segment of circle). Supported rotations are "
-            "1,2,3,4,6. All of them along Z and centered at Gamma. Consider to "
-            "'--translate' your cell to rotate with other origin. This is the "
-            "last symmetry operation to be performed."
-        )
-        parserFermi2D.add_argument("--rot_symm", help=phelp, type=int, default=1)
-
-        phelp = (
-            "Translate your mesh to the specified point. The point can be 3 "
-            "coordinates (numbers) or the index of one K-point (zero-based, as "
-            "usual). This is the first symmetry operation to be performed "
-            "(i.e. rotations will take this point as the origin)."
-        )
-        parserFermi2D.add_argument(
-            "--translate", help=phelp, nargs="+", default=[0, 0, 0]
-        )
-
-        phelp = (
-            "A general rotation is applied to the data in the PROCAR. While this "
-            " script has a large bias to work on the 'xy' plane, with this option"
-            " you can rotate your whole PROCAR to fit the 'xy' plane. A rotation "
-            "is composed by one angle plus one fixed axis, eg: '--rotation 90 1 0"
-            " 0' is 90 degrees along the x axis, this changes the 'xy'->'xz'. The"
-            " rotation is performed after the translation and before applying "
-            "rot_symm. "
-        )
-        parserFermi2D.add_argument(
-            "--rotation", help=phelp, type=float, nargs=4, default=[0, 0, 0, 1]
-        )
-
-        phelp = "enable to give atoms list in a more human, 1-based way (say the 1st is 1,2nd is 2 and so on )"
-        parserFermi2D.add_argument("-u", "--human", help=phelp, action="store_true")
-
-        phelp = "If set, masks(hides) values lowers than it. Useful to remove unwanted bands."
-        parserFermi2D.add_argument("--mask", type=float, help=phelp)
-
-        phelp = (
-            "Saves the figure, instead of display it on screen. Anyway, you can save from"
-            " the screen too. Any file extension supported by"
-            "matplotlib.savefig is valid (if you are too lazy"
-            " to google it, trial and error also works)"
-        )
-        parserFermi2D.add_argument("--savefig", help=phelp)
-
-        phelp = (
-            "OUTCAR file where to find the reciprocal lattice vectors and "
-            "perhaps E_fermi. Mind: '--fermi' has precedence, remember that the"
-            " E-fermi should correspond to a self-consistent run, not a "
-            "bandstructure! (however, this is irrelevant for basis vectors)"
-        )
-        parserFermi2D.add_argument("--outcar", help=phelp)
-
-        phelp = (
-            "Plot of the spin texture (ie: spin arrows) on the Fermi's surface."
-            " This option works quite indepentent of another options."
-        )
-        parserFermi2D.add_argument("--st", help=phelp, action="store_true")
-
-        phelp = (
-            "Plot of the spin texture without arrows (just intensity) for a "
-            "given spin direction on the Fermi's surface.  This option works"
-            "quite indepentent of another options but needs to set '--st' and '--spin'."
-        )
-        parserFermi2D.add_argument("--noarrow", help=phelp, action="store_true")
-
-        parserFermi2D.set_defaults(func=call_fermi2D)
-
-        ################ Fermi3D ##########################################
-
-        parserfermi3D = subparsers.add_parser("fermi3D", help="Plot 3D Fermi surface")
-        parserfermi3D.add_argument("procar", help="PROCAR file.")
-        parserfermi3D.add_argument("outcar", help="OUTCAR file.")
-        parserfermi3D.add_argument(
-            "bands", help="Array of bands to be included. -1 considers all.", default=-1
-        )
-        parserfermi3D.add_argument(
-            "scale", help="Interpolation factor", type=float, default=1
-        )
-        parserfermi3D.add_argument(
-            "mode", help="Plot mode.", choices=["plain", "parametric", "external"]
-        )
-        parserfermi3D.add_argument(
-            "-st", help="Flag to set spin texture on.", action="store_true"
-        )
-        parserfermi3D.add_argument("kwargs", help="Additional arguments.", nargs="*")
-        parserfermi3D.set_defaults(func=call_fermi3D)
-
-        ################# repair ##########################################
-        parserrepair = subparsers.add_parser(
-            "repair", help="Repairs formatting issues in PROCAR file."
-        )
-        parserrepair.add_argument("infile", help="Input file. Can be compressed.")
-        parserrepair.add_argument("outfile", help="Output file.")
-        parserrepair.set_defaults(func=call_repair)
-
-        ################# bandgap ##########################################
-        parserbandgap = subparsers.add_parser(
-            "bandgap",
-            help="Calculate bandgap. procar and outcar needed only for Abinit and VASP.",
-        )
-        parserbandgap.add_argument("procar", help="PROCAR file.")
-        parserbandgap.add_argument("outcar", help="OUTCAR file.")
-        parserbandgap.add_argument(
-            "code",
-            help="code",
-            choices=["vasp", "qe", "lobster", "abinit", "elk"],
-            default="vasp",
-        )
-        parserbandgap.add_argument(
-            "fermi", help="Fermi energy. Retrived from output if not provided."
-        )
-        parserbandgap.set_defaults(func=call_bandgap)
-
-        ################## k-mesh ########################################
-        parsergenerate2dkmesh = subparsers.add_parser(
-            "generate2dkmesh",
-            help="Generate a 2D k-mesh"
-            "centered at a given k-point in a given k-plane.",
-        )
-        parsergenerate2dkmesh.add_argument("x1", help="x1 coordinate")
-        parsergenerate2dkmesh.add_argument("y1", help="y1 coordinate")
-        parsergenerate2dkmesh.add_argument("x2", help="x2 coordinate")
-        parsergenerate2dkmesh.add_argument("y2", help="y2 coordinate")
-        parsergenerate2dkmesh.add_argument("z", help="z plane")
-        parsergenerate2dkmesh.add_argument(
-            "nkx", help="number of grids in the x direction"
-        )
-        parsergenerate2dkmesh.add_argument(
-            "nky", help="number of grids in the y direction"
-        )
-        parsergenerate2dkmesh.set_defaults(func=call_generate2dkmesh)
-
-        ################## k-path ####################################################
-        parserkpath = subparsers.add_parser(
-            "kpath", help="k-path generator.", formatter_class=RawTextHelpFormatter
-        )
-        parserkpath.add_argument("infile", help="POSCAR file", default="POSCAR")
-        parserkpath.add_argument("-grid_size", help="Grid size", default=40, type=int)
-        parserkpath.add_argument(
-            "-with_time_reversal",
-            help="Flag to turn on time reversal symmetry",
-            action="store_true",
-        )
-        parserkpath.add_argument(
-            "-recipe",
-            help="The algorithm that defines the special points and paths",
-            type=str,
-            default="hpkot",
-        )
-        parserkpath.add_argument(
-            "-threshold",
-            help="The threshold to use to verify if we are in an edge case",
-            type=float,
-            default=1e-07,
-        )
-        parserkpath.add_argument(
-            "-symprec",
-            help="The symmetry precision used internally by SPGLIB",
-            type=float,
-            default=1e-05,
-        )
-        parserkpath.add_argument(
-            "-angle_tolerence",
-            help="Angle_tolerance used internally by SPGLIB",
-            type=float,
-            default=-1.0,
-        )
-        parserkpath.add_argument(
-            "-supercell_matrix",
-            help="The super cell for band unfolding. Default 3x3 identity matrix.",
-            type=int,
-            default=np.eye(3),
-        )
-        parserkpath.set_defaults(func=call_kpath)
-
-        ################### bandstructure ######################################################
-        parserBandsplot = subparsers.add_parser(
-            "bandsplot",
-            help="Bandstructure plot.",
-            formatter_class=RawTextHelpFormatter,
-        )
-
-        phelp = "Input file. It can be compressed"
-        parserBandsplot.add_argument("file", help=phelp)
-
-        phelp = (
-            "Plot mode:\n"
-            "-m  scatter : is a points plot with the color given by the chosen\n"
-            "  projection. It produces a rather heavy pdf file.\n\n"
-            "-m  parametric : like scatter, but with lines instead of points \n"
-            "  (bands crossings are not handled, and some  unphysical 'jumps' \n"
-            " can be present). Sligthy smaller PDF size.\n\n"
-            "-m plain : is a featureless bandstructure ignoring all data about\n"
-            "  projections. Rather light-weight\n\n"
-            "-m atomic : For non-periodic system, like molecules, rather ugly \n"
-            "  but useful to visualize energy level. Only 1 K-point!\n\n"
-        )
-        choices = ["scatter", "plain", "parametric", "atomic"]
-        parserBandsplot.add_argument(
-            "-m", "--mode", help=phelp, default="plain", choices=choices
-        )
-
-        phelp = "Color of the bands for plain mode."
-        parserBandsplot.add_argument("-color", help=phelp, default="blue")
-
-        phelp = "Name of Abinit output file if used."
-        parserBandsplot.add_argument("-abinit", help=phelp, default=None)
-
-        phelp = (
-            "Spin component to be used (default -s 0): \n\n"
-            "Non-polarized calculations density is '-s 0', just ignore it.\n\n"
-            "Spin-Polarized (collinear) calculation: \n"
-            "-s 0 are the unpolarized bands, the spin-polarization is ignored.\n"
-            "-s 1 'spin-polarized' bands, the character of 'up' bands positive,\n"
-            "  but negative for 'down' bands, this means that the color of \n"
-            "  'down' is negative. Useful together with '--cmap seismic'.\n\n"
-            "Non-collinear calculation: \n"
-            "-s 0 : density, ie: Spin-orbit-coupling but don't care of spin.\n"
-            "-s 1 : Sx, projection along 'x' quantization axis, see SAXIS flag\n"
-            "  in the VASP manual\n"
-            "-s 2 : Sy, projection along 'y' quantization axis.\n"
-            "-s 3 : Sy, projection along 'z' quantization axis.\n"
-            "-s st : Spin-texture perpendicular in the plane (kx,ky) to each\n "
-            "(kx,ky) vector. Useful for Rashba-like states in surfaces. Use\n "
-            "'--cmap seismic'\n\n "
-        )
-        parserBandsplot.add_argument(
-            "-s", "--spin", choices=["0", "1", "2", "3", "st"], default="0", help=phelp
-        )
-
-        phelp = (
-            "List of rows (atoms) to be used. This list refers to the rows of\n"
-            "(each block of) your PROCAR file. If you haven't manipulated your\n"
-            "PROCAR (eg: with the '-a' option of 'filter' mode) each row\n"
-            "correspond to the respective atom in the POSCAR.\n\n"
-            "Mind: This list is 0-based, ie: the 1st atom is 0, the 2nd is 1,\n"
-            "  and so on. If you need to be treated like a human, specify '-u'\n"
-            "or '--human' and 1st->1, 2nd->2, etc.\n\n"
-            "Example:\n"
-            "-a 0 2 :  select the 1st  and 3rd. rows (likely 1st and 3rd atoms)"
-            "\n\n"
-        )
-        parserBandsplot.add_argument(
-            "-a", "--atoms", type=int, nargs="+", help=phelp, default=None
-        )
-
-        phelp = (
-            "Orbitals index(es) to be used, take a look to the PROCAR file, \n"
-            "they are 's py pz px ...', then s->0, py->1, pz->2 and so on. \n"
-            "Note that indexes begin at 0!. Its default is the last field (ie:\n"
-            "'tot', did you saw the PROCAR?). Some examples:\n\n"
-            "-o 0 : s-orbital (unless you modified the orbitals, eg. 'filter')\n"
-            "-o 1 2 3 : py+pz+px (unless you modified the orbitals)\n"
-            "-o 4 5 6 7 8 : all the d-orbitasl (unless...)\n"
-            "-o 2 6 : pz+dzz (did you look at the PROCAR?)\n\n "
-        )
-        parserBandsplot.add_argument(
-            "-o", "--orbitals", type=int, nargs="+", help=phelp, default=None
-        )
-
-        phelp = (
-            "Set the Fermi energy (or any reference energy) as the zero energy.\n"
-            "See '--outcar', avoids to give it explicitly. A list of \n"
-            "k-dependant 'fermi-like energies' are also accepted (useful to\n"
-            "compare different systems in one PROCAR made by hand). \n\n"
-            "Mind: The Fermi energy MUST be the one from the self-consistent\n"
-            "calculation, not from a Bandstructure calculation!\n\n"
-        )
-        parserBandsplot.add_argument(
-            "-f", "--fermi", type=float, help=phelp, nargs="+", default=None
-        )
-
-        phelp = (
-            "Min/Max energy to be ploted. Example:\n "
-            "--elimit -1 1 : From -1 to 1 around Fermi energy (if given)\n\n"
-        )
-        parserBandsplot.add_argument(
-            "--elimit", type=float, nargs=2, help=phelp, default=None
-        )
-
-        phelp = (
-            "If given, it masks(hides) bands with values lowers than 'mask'.\n"
-            "It is useful to remove 'unwanted' bands. For instance, if you\n"
-            "project the bandstructure on a 'surface' atom -with the default\n"
-            "colormap- some white points can appear, they are bands with \n"
-            "almost no contribution to the 'surface': no physics but they \n"
-            "still look ugly, to hide those bands use '--mask 0.08' (or some \n"
-            "other small value). Mind: it works with the absolute value of\n"
-            "projection (no problem with spin polarization)\n\n"
-        )
-        parserBandsplot.add_argument("--mask", type=float, help=phelp, default=None)
-
-        phelp = (
-            "Size of markers, if used. Each mode has it own scale,\n"
-            "just test them\n\n"
-        )
-        parserBandsplot.add_argument(
-            "--markersize", type=float, help=phelp, default=0.02
-        )
-
-        phelp = (
-            "Change the color scheme. Example:\n\n"
-            "--cmap  seismic : blue->white->red, useful to see the \n"
-            "  spin-polarization of a band (it will blueish or reddish)\n"
-            "  depending of spin channel\n"
-            "--cmap  seismic_r : the 'seismic' colormap, but reversed.\n\n"
-        )
-        parserBandsplot.add_argument("--cmap", help=phelp, default="jet")
-
-        phelp = (
-            "Do you want to Normalize the plots to the same scale of colors\n"
-            "(ie: the numbers on the bar at the right), just try '--vmax'\n\n"
-            "--vmax 1 : If you are looking for the s, p or d character.\n"
-            "--vmax 0.2: If you want to capture some tiny effect, eg: s-band of\n"
-            "  a impurity on a metal\n\n"
-        )
-        parserBandsplot.add_argument("--vmax", type=float, help=phelp, default=None)
-
-        phelp = (
-            "Like '--vmax' (see '--vmax'), However, for spin-polarized \n"
-            "(collinear or not) you can set it to a negative value. Actually\n"
-            "you can do it for a non-spin-polarized calculation and the \n"
-            "effect will be a 'stretching' of the color scheme, try it.\n\n"
-        )
-        parserBandsplot.add_argument("--vmin", type=float, help=phelp, default=None)
-
-        phelp = "switch on/off the grid. Default is 'on'\n\n"
-        parserBandsplot.add_argument("--grid", type=bool, help=phelp, default=True)
-
-        phelp = (
-            "set the marker shape, ie: 'o'=circle, 's'=square,\ '-'=line\n"
-            "(only mode `plain`, other symbols: google pyplot markers)\n\n"
-        )
-        parserBandsplot.add_argument("--marker", type=str, help=phelp, default="o")
-
-        phelp = (
-            "Some fault tolerance for ill-formatted files (stupid fortran)\n"
-            "But be careful, something could be messed up and don't work (at\n"
-            "least as expected). Length of K-points paths will be ignored\n\n"
-        )
-        parserBandsplot.add_argument("--permissive", help=phelp, action="store_true")
-
-        phelp = (
-            "Enable human-like 1-based order (ie 1st is 1, 2nd is 2, and so\n"
-            "on). Mind: this only works for atoms, not for orbitals or spin\n\n"
-        )
-        parserBandsplot.add_argument("-u", "--human", help=phelp, action="store_true")
-
-        phelp = (
-            "Saves the figure, instead of display it on screen. Anyway, you can\n"
-            "save from the screen too. Any file extension supported by\n "
-            "`matplotlib.savefig` is valid (if you are too lazy to google it,\n"
-            "trial and error also works fine)\n\n"
-        )
-        parserBandsplot.add_argument("--savefig", help=phelp, default=None)
-
-        phelp = (
-            "list of ticks along the kpoints axis (x axis). For instance a\n"
-            "bandstructure G-X-M with 10 point by segment should be:\n "
-            "--kticks 0 9 19\n\n"
-        )
-        parserBandsplot.add_argument("--kticks", help=phelp, nargs="+", type=int)
-
-        phelp = (
-            "Names of the points given in `--kticks`. In the `kticks` example\n"
-            'they should be `--knames "\$Gamma\$" X M`. As you can see \n'
-            "LaTeX stuff works with a minimal mess (extra \\s)\n\n"
-        )
-        parserBandsplot.add_argument(
-            "--knames", help=phelp, nargs="+", type=str, default=None
-        )
-
-        phelp = (
-            "Title, to use several words, use quotation marks\"\" or ''. Latex\n"
-            " works if you scape the special characteres, ie: $\\alpha$ -> \n"
-            "\$\\\\alpha\$"
-        )
-        parserBandsplot.add_argument(
-            "-t", "--title", help=phelp, type=str, default=None
-        )
-
-        phelp = (
-            "OUTCAR file where to find the reciprocal lattice vectors and\n "
-            "perhaps E_fermi.\n"
-            "Mind: '--fermi' has precedence, remember that the E-fermi should\n"
-            "correspond to a self-consistent run, not to a bandstructure!\n"
-            "(however, the basis and reciprocal vectors will be safe from the\n"
-            "non-self-consistentness)\n\n"
-        )
-        parserBandsplot.add_argument("--outcar", help=phelp, default=None)
-
-        phelp = "KPOINTS file for bandstructure plotting.\n"
-        parserBandsplot.add_argument("--kpointsfile", help=phelp, default=None)
-
-        phelp = "Convert k-points from reduced to cartesian for plot #1?"
-        parserBandsplot.add_argument("-kdirect", help=phelp, action="store_false")
-
-        parserBandsplot.set_defaults(func=call_bandsplot)
-
-        args = parser.parse_args()
-        args.func(args)
-
-    else:
-        print("PyProcar: A Python library for analyzing PROCAR files.\n")
-        print("Usage: procar [-h]")
-        print(
-            "{cat,mergeabinit,unfold,filter,fermi2D,fermi3D,repair,generate2dkmesh,kpath,bandsplot,bandscompare}"
-        )
+#!/usr/bin/env python
+
+"""
+Stand alone script for PyProcar.
+
+This calls the modules in the /pyprocar directory.
+
+Based on the original script developed by Aldo Romero (alromero@mail.wvu.edu) and
+Francisco Munoz (fvmunoz@gmail.com).
+"""
+
+import argparse
+from argparse import RawTextHelpFormatter
+import pyprocar
+import numpy as np
+
+
+def call_bandsplot(args):
+    """
+	This module calls the band structure plotting function.
+	"""
+
+    pyprocar.bandsplot(
+        args.file,
+        mode=args.mode,
+        color=args.color,
+        abinit_output=args.abinit,
+        spin=args.spin,
+        atoms=args.atoms,
+        orbitals=args.orbitals,
+        fermi=args.fermi,
+        elimit=args.elimit,
+        mask=args.mask,
+        markersize=args.markersize,
+        cmap=args.cmap,
+        vmax=args.vmax,
+        vmin=args.vmin,
+        grid=args.grid,
+        marker=args.marker,
+        permissive=args.permissive,
+        human=args.human,
+        savefig=args.savefig,
+        kticks=args.kticks,
+        knames=args.knames,
+        title=args.title,
+        outcar=args.outcar,
+        kpointsfile=args.kpointsfile,
+        kdirect=args.kdirect,
+    )
+
+
+def call_kpath(args):
+    """
+	This module calls the k-path generation function.
+	"""
+
+    pyprocar.kpath(
+        args.infile,
+        grid_size=args.grid_size,
+        with_time_reversal=args.with_time_reversal,
+        recipe=args.recipe,
+        threshold=args.threshold,
+        symprec=args.symprec,
+        angle_tolerence=args.angle_tolerence,
+        supercell_matrix=args.supercell_matrix,
+    )
+
+
+def call_repair(args):
+    """
+	This module calls the repair function.
+	"""
+    pyprocar.repair(args.infile, args.outfile)
+
+
+def call_generate2dkmesh(args):
+    """
+	This module calls the k-mesh generating function.
+	"""
+    pyprocar.generate2dkmesh(
+        args.x1, args.y1, args.x2, args.y2, args.z, args.nkx, args.nky
+    )
+
+
+def call_fermi2D(args):
+    """
+	This module calls the fermi2D plotting function.
+	"""
+    pyprocar.fermi2D(
+        args.file,
+        outcar=args.outcar,
+        spin=args.spin,
+        atoms=args.atoms,
+        orbitals=args.orbitals,
+        energy=args.energy,
+        fermi=args.fermi,
+        rec_basis=args.rec_basis,
+        rot_symm=args.rot_symm,
+        translate=args.translate,
+        rotation=args.rotation,
+        human=args.human,
+        mask=args.mask,
+        savefig=args.savefig,
+        st=args.st,
+        noarrow=args.noarrow,
+    )
+
+
+def call_fermi3D(args):
+    """
+	This module calls the fermi3D plotting function.
+	"""
+    pyprocar.fermi3D(
+        args.procar,
+        args.outcar,
+        args.bands,
+        scale=args.scale,
+        mode=args.mode,
+        st=args.st,
+        kwargs=args.kwargs,
+    )
+
+
+def call_filter(args):
+    """
+	This module calls the filter function.
+	"""
+
+    pyprocar.filter(
+        args.infile,
+        args.outfile,
+        atoms=args.atoms,
+        orbitals=args.orbitals,
+        orbital_names=args.orbital_names,
+        bands=args.bands,
+        spin=args.spin,
+        human_atoms=args.human_atoms,
+    )
+
+
+def call_cat(args):
+    """
+	This module calls the cat function.
+	"""
+    pyprocar.cat(inFiles=args.inFiles, outFile=args.outFile, gz=args.gz)
+
+
+def call_mergeabinit(args):
+    """
+	This module calls the mergeabinit function.
+	"""
+    pyprocar.mergeabinit(args.outfile)
+
+
+def call_bandgap(args):
+    """
+	This module calls the mergeabinit function.
+	"""
+    pyprocar.bandgap(args.procar, args.outcar, args.code, args.fermi)
+
+
+def call_unfold(args):
+    """
+	This module calls the band unfolding function.
+	"""
+    pyprocar.unfold(
+        fname=args.fname,
+        poscar=args.poscar,
+        outcar=args.outcar,
+        supercell_matrix=args.supercell_matrix,
+        ispin=args.ispin,
+        efermi=args.efermi,
+        shift_efermi=args.shift_efermi,
+        elimit=args.elimit,
+        kticks=args.kticks,
+        knames=args.knames,
+        print_kpts=args.print_kpts,
+        show_band=args.show_band,
+        width=args.width,
+        color=args.color,
+        savetab=args.savetab,
+        savefig=args.savefig,
+    )
+
+
+if __name__ == "__main__":
+
+    import sys
+
+    args = sys.argv[1:]
+
+    if args:
+
+        # Top level parser
+        description = "PyProcar: A Python library for analyzing PROCAR files."
+        parser = argparse.ArgumentParser(description=description)
+        subparsers = parser.add_subparsers(help="sub-command help")
+
+        ############### cat ############################################
+
+        phelp = (
+            "concatenation of PROCARs files, they should be compatible (ie: "
+            "joining parts of a large bandstructure calculation)."
+        )
+        parserCat = subparsers.add_parser("cat", help=phelp)
+
+        phelp = "Input files. They can be compressed"
+        parserCat.add_argument("inFiles", nargs="+", help=phelp)
+
+        phelp = "Output file."
+        parserCat.add_argument("outFile", help=phelp)
+
+        phelp = "Writes a gzipped outfile (if needed a .gz extension automatically will be added)"
+        parserCat.add_argument("--gz", help=phelp, action="store_true")
+
+        parserCat.set_defaults(func=call_cat)
+
+        ################ mergeabinit ##################################
+
+        parsermergeabinit = subparsers.add_parser(
+            "mergeabinit", help="Merge Abinit PROCARs."
+        )
+        parsermergeabinit.add_argument("outfile", help="Merged PROCAR")
+        parsermergeabinit.set_defaults(func=call_mergeabinit)
+
+        ############### unfold #######################################
+        parserunfold = subparsers.add_parser("unfold", help="Band unfolding.")
+        parserunfold.add_argument("-fname", help="PROCAR filename.")
+        parserunfold.add_argument("-poscar", help="POSCAR filename.")
+        parserunfold.add_argument(
+            "-outcar", help="OUTCAR filename. Used to get Fermi energy."
+        )
+        parserunfold.add_argument(
+            "-supercell_matrix",
+            help="Supercell matrix from primitive cell to supercell.",
+        )
+        parserunfold.add_argument(
+            "-ispin",
+            help="None - non spin polarized \n 1 - spin up" "\n 2 - spin down.",
+            choices=[None, 1, 2],
+        )
+        parserunfold.add_argument(
+            "-efermi", help="Fermi energy. Only when no OUTCAR is given."
+        )
+        parserunfold.add_argument("-elimit", help="Range of energy to be plotted.")
+        parserunfold.add_argument(
+            "-kticks",
+            help="The indices of k-points for labels.",
+            type=int,
+            nargs="+",
+            action="append",
+        )
+        parserunfold.add_argument(
+            "-knames", help="Labels of k-points.", type=str, nargs="+", action="append"
+        )
+        parserunfold.add_argument(
+            "-print_kpts", help="Print all the k-points to screen.", action="store_true"
+        )
+        parserunfold.add_argument(
+            "-show_band",
+            help="Whether to plot the bands before unfolding.",
+            action="store_true",
+        )
+        parserunfold.add_argument(
+            "-width", help="Width of the unfolded band.", type=float
+        )
+        parserunfold.add_argument(
+            "-color", help="Color of the unfolded band.", type=str
+        )
+        parserunfold.add_argument(
+            "-savetab",
+            help="The csv file name of which the table of unfolding result will be written into",
+        )
+        parserunfold.add_argument(
+            "-savefig", help="The file name of which the figure will be saved."
+        )
+        parserunfold.set_defaults(func=call_unfold)
+
+        ############### filter ##########################################
+        phelp = (
+            "Filters (manipulates) the data of the input file (PROCAR-like) and"
+            " it yields a new file (PROCAR-like too) with the changes. This "
+            "method can do only one manipulation at time (ie: spin, atoms, "
+            "bands or orbitals)."
+        )
+        parserFilter = subparsers.add_parser("filter", help=phelp)
+
+        phelp = "Input file. Can be compressed"
+        parserFilter.add_argument("inFile", help=phelp)
+
+        phelp = "Output file."
+        parserFilter.add_argument("outFile", help=phelp)
+
+        OptFilter = parserFilter.add_mutually_exclusive_group()
+        phelp = (
+            "List of atoms to group (add) as a new single entry. Each group of"
+            " atoms should be specified in a different `--atoms` option. "
+            "Example: `procar.py filter in out -a 0 1 -a 2` will group the 1st"
+            " and 2nd atoms, while keeping the 3rd atom in `out` (any atom "
+            "beyond the 3rd will be discarded). Mind the last atomic field "
+            "present on a PROCAR file, is not an atom, is the 'tot' value (sum"
+            " of all atoms), this field always is included in the outfile and "
+            "it always is the 'tot' value from infile, regardless the selection"
+            " of atoms."
+        )
+        OptFilter.add_argument(
+            "-a", "--atoms", type=int, nargs="+", action="append", help=phelp
+        )
+
+        phelp = (
+            "List of orbitals to group as a single entry. Each group of "
+            "orbitals needs a different `--orbitals` list. By instance, to "
+            "group orbitals in 's','p', 'd' it is needed `-o 0 -o 1 2 3 -o 4 5 "
+            "6 7 8`. Where 0=s, 1,2,3=px,py,pz, 4...9=dxx...dyz. Mind the last "
+            "value (aka) 'tot' always is written."
+        )
+        OptFilter.add_argument(
+            "-o", "--orbitals", help=phelp, type=int, nargs="+", action="append"
+        )
+
+        phelp = (
+            "Keeps only the bands between `min` and `max` indexes. To keep the "
+            "bands from 120 to 150 you should give `-b 120 150 `. It is not "
+            "obvious which indexes are in the interest region, therefore I "
+            "recommend you trial and error "
+        )
+        OptFilter.add_argument("-b", "--bands", help=phelp, type=int, nargs=2)
+
+        phelp = (
+            "Which spin components should be written: 0=density, 1,2,3=Sx,Sy,Sz."
+            " They are not averaged."
+        )
+        OptFilter.add_argument("-s", "--spin", help=phelp, type=int, nargs="+")
+
+        phelp = (
+            "enable to give atoms list in a more human, 1-based order (say the"
+            " 1st is 1, 2nd is 2 and so on ). Mind: this only holds for atoms."
+        )
+        parserFilter.add_argument("--human", help=phelp, action="store_true")
+
+        phelp = (
+            "List of names of new 'orbitals' to appear in the new file, eg. "
+            "(`--orbital_names s p d` for a 's', 'p', 'd'). Only meaningful "
+            "when manipulating the orbitals, ie: using `-o` "
+        )
+        parserFilter.add_argument("--orbital_names", help=phelp, nargs="+")
+
+        parserFilter.set_defaults(func=call_filter)
+
+        ################ fermi2D ##########################################
+        parserFermi2D = subparsers.add_parser(
+            "fermi2D",
+            help="Plot the Fermi surface for a 2D Brillouin zone (layer-wise)"
+            "along z and just perpendicular to z! (actually k_z)",
+        )
+
+        phelp = "Input file. It can be compressed"
+        parserFermi2D.add_argument("file", help=phelp)
+
+        phelp = (
+            "Spin component to be used: for non-polarized calculations density "
+            "is '-s 0'. For spin polarized case test '-s 0' (ignore the spin) or"
+            " '-s 1' (assing a sign to the spin channel). For "
+            "non-collinear stuff you can use '-s 0', '-s 1', '-s 2', -s "
+            "3 for the magnitude, x, y, z components of your spin "
+            "vector, in this case you really want to see spin textures "
+            "'--st'. Default: s=0"
+        )
+        parserFermi2D.add_argument(
+            "-s", "--spin", type=int, choices=[0, 1, 2, 3], default=0, help=phelp
+        )
+
+        phelp = (
+            "List of atoms to be used (0-based): ie. '-a 0 2' to select the 1st"
+            " and 3rd. It defaults to the last one (-a -1 the 'tot' entry)"
+        )
+        parserFermi2D.add_argument("-a", "--atoms", type=int, nargs="+", help=phelp)
+
+        phelp = (
+            "Orbital index(es) to be used 0-based. Take a look to the PROCAR "
+            "file. Its default is the last field (ie: 'tot'). From a standard "
+            "PROCAR: `-o 0`='s', `-o 1 2 3`='p', `-o 4 5 6 7 8`='d'."
+        )
+        parserFermi2D.add_argument("-o", "--orbitals", type=int, nargs="+", help=phelp)
+
+        phelp = (
+            "Energy for the surface. To plot the Fermi surface at Fermi Energy `-e 0`"
+        )
+        parserFermi2D.add_argument(
+            "-e", "--energy", help=phelp, type=float, required=True
+        )
+
+        phelp = (
+            "Set the Fermi energy (or any reference energy) as zero. To get it "
+            "you should `grep E-fermi` the self-consistent OUTCAR. See `--outcar`"
+        )
+        parserFermi2D.add_argument("-f", "--fermi", help=phelp, type=float)
+
+        phelp = (
+            "reciprocal space basis vectors. 9 number are required b1x b1y ... "
+            " b3z. This option is quite involved, so I recommend you to use `--outcar`"
+        )
+        parserFermi2D.add_argument("--rec_basis", help=phelp, type=float, nargs=9)
+
+        phelp = (
+            "Apply a rotational symmetry to unfold the Kpoints found. If your"
+            "PROCAR only has a portion of the Brillouin Zone, you may want to "
+            "plot the FULL BZ (ie: a Dirac cone at Gamma will look like a cone "
+            "and not like a segment of circle). Supported rotations are "
+            "1,2,3,4,6. All of them along Z and centered at Gamma. Consider to "
+            "'--translate' your cell to rotate with other origin. This is the "
+            "last symmetry operation to be performed."
+        )
+        parserFermi2D.add_argument("--rot_symm", help=phelp, type=int, default=1)
+
+        phelp = (
+            "Translate your mesh to the specified point. The point can be 3 "
+            "coordinates (numbers) or the index of one K-point (zero-based, as "
+            "usual). This is the first symmetry operation to be performed "
+            "(i.e. rotations will take this point as the origin)."
+        )
+        parserFermi2D.add_argument(
+            "--translate", help=phelp, nargs="+", default=[0, 0, 0]
+        )
+
+        phelp = (
+            "A general rotation is applied to the data in the PROCAR. While this "
+            " script has a large bias to work on the 'xy' plane, with this option"
+            " you can rotate your whole PROCAR to fit the 'xy' plane. A rotation "
+            "is composed by one angle plus one fixed axis, eg: '--rotation 90 1 0"
+            " 0' is 90 degrees along the x axis, this changes the 'xy'->'xz'. The"
+            " rotation is performed after the translation and before applying "
+            "rot_symm. "
+        )
+        parserFermi2D.add_argument(
+            "--rotation", help=phelp, type=float, nargs=4, default=[0, 0, 0, 1]
+        )
+
+        phelp = "enable to give atoms list in a more human, 1-based way (say the 1st is 1,2nd is 2 and so on )"
+        parserFermi2D.add_argument("-u", "--human", help=phelp, action="store_true")
+
+        phelp = "If set, masks(hides) values lowers than it. Useful to remove unwanted bands."
+        parserFermi2D.add_argument("--mask", type=float, help=phelp)
+
+        phelp = (
+            "Saves the figure, instead of display it on screen. Anyway, you can save from"
+            " the screen too. Any file extension supported by"
+            "matplotlib.savefig is valid (if you are too lazy"
+            " to google it, trial and error also works)"
+        )
+        parserFermi2D.add_argument("--savefig", help=phelp)
+
+        phelp = (
+            "OUTCAR file where to find the reciprocal lattice vectors and "
+            "perhaps E_fermi. Mind: '--fermi' has precedence, remember that the"
+            " E-fermi should correspond to a self-consistent run, not a "
+            "bandstructure! (however, this is irrelevant for basis vectors)"
+        )
+        parserFermi2D.add_argument("--outcar", help=phelp)
+
+        phelp = (
+            "Plot of the spin texture (ie: spin arrows) on the Fermi's surface."
+            " This option works quite indepentent of another options."
+        )
+        parserFermi2D.add_argument("--st", help=phelp, action="store_true")
+
+        phelp = (
+            "Plot of the spin texture without arrows (just intensity) for a "
+            "given spin direction on the Fermi's surface.  This option works"
+            "quite indepentent of another options but needs to set '--st' and '--spin'."
+        )
+        parserFermi2D.add_argument("--noarrow", help=phelp, action="store_true")
+
+        parserFermi2D.set_defaults(func=call_fermi2D)
+
+        ################ Fermi3D ##########################################
+
+        parserfermi3D = subparsers.add_parser("fermi3D", help="Plot 3D Fermi surface")
+        parserfermi3D.add_argument("procar", help="PROCAR file.")
+        parserfermi3D.add_argument("outcar", help="OUTCAR file.")
+        parserfermi3D.add_argument(
+            "bands", help="Array of bands to be included. -1 considers all.", default=-1
+        )
+        parserfermi3D.add_argument(
+            "scale", help="Interpolation factor", type=float, default=1
+        )
+        parserfermi3D.add_argument(
+            "mode", help="Plot mode.", choices=["plain", "parametric", "external"]
+        )
+        parserfermi3D.add_argument(
+            "-st", help="Flag to set spin texture on.", action="store_true"
+        )
+        parserfermi3D.add_argument("kwargs", help="Additional arguments.", nargs="*")
+        parserfermi3D.set_defaults(func=call_fermi3D)
+
+        ################# repair ##########################################
+        parserrepair = subparsers.add_parser(
+            "repair", help="Repairs formatting issues in PROCAR file."
+        )
+        parserrepair.add_argument("infile", help="Input file. Can be compressed.")
+        parserrepair.add_argument("outfile", help="Output file.")
+        parserrepair.set_defaults(func=call_repair)
+
+        ################# bandgap ##########################################
+        parserbandgap = subparsers.add_parser(
+            "bandgap",
+            help="Calculate bandgap. procar and outcar needed only for Abinit and VASP.",
+        )
+        parserbandgap.add_argument("procar", help="PROCAR file.")
+        parserbandgap.add_argument("outcar", help="OUTCAR file.")
+        parserbandgap.add_argument(
+            "code",
+            help="code",
+            choices=["vasp", "qe", "lobster", "abinit", "elk"],
+            default="vasp",
+        )
+        parserbandgap.add_argument(
+            "fermi", help="Fermi energy. Retrived from output if not provided."
+        )
+        parserbandgap.set_defaults(func=call_bandgap)
+
+        ################## k-mesh ########################################
+        parsergenerate2dkmesh = subparsers.add_parser(
+            "generate2dkmesh",
+            help="Generate a 2D k-mesh"
+            "centered at a given k-point in a given k-plane.",
+        )
+        parsergenerate2dkmesh.add_argument("x1", help="x1 coordinate")
+        parsergenerate2dkmesh.add_argument("y1", help="y1 coordinate")
+        parsergenerate2dkmesh.add_argument("x2", help="x2 coordinate")
+        parsergenerate2dkmesh.add_argument("y2", help="y2 coordinate")
+        parsergenerate2dkmesh.add_argument("z", help="z plane")
+        parsergenerate2dkmesh.add_argument(
+            "nkx", help="number of grids in the x direction"
+        )
+        parsergenerate2dkmesh.add_argument(
+            "nky", help="number of grids in the y direction"
+        )
+        parsergenerate2dkmesh.set_defaults(func=call_generate2dkmesh)
+
+        ################## k-path ####################################################
+        parserkpath = subparsers.add_parser(
+            "kpath", help="k-path generator.", formatter_class=RawTextHelpFormatter
+        )
+        parserkpath.add_argument("infile", help="POSCAR file", default="POSCAR")
+        parserkpath.add_argument("-grid_size", help="Grid size", default=40, type=int)
+        parserkpath.add_argument(
+            "-with_time_reversal",
+            help="Flag to turn on time reversal symmetry",
+            action="store_true",
+        )
+        parserkpath.add_argument(
+            "-recipe",
+            help="The algorithm that defines the special points and paths",
+            type=str,
+            default="hpkot",
+        )
+        parserkpath.add_argument(
+            "-threshold",
+            help="The threshold to use to verify if we are in an edge case",
+            type=float,
+            default=1e-07,
+        )
+        parserkpath.add_argument(
+            "-symprec",
+            help="The symmetry precision used internally by SPGLIB",
+            type=float,
+            default=1e-05,
+        )
+        parserkpath.add_argument(
+            "-angle_tolerence",
+            help="Angle_tolerance used internally by SPGLIB",
+            type=float,
+            default=-1.0,
+        )
+        parserkpath.add_argument(
+            "-supercell_matrix",
+            help="The super cell for band unfolding. Default 3x3 identity matrix.",
+            type=int,
+            default=np.eye(3),
+        )
+        parserkpath.set_defaults(func=call_kpath)
+
+        ################### bandstructure ######################################################
+        parserBandsplot = subparsers.add_parser(
+            "bandsplot",
+            help="Bandstructure plot.",
+            formatter_class=RawTextHelpFormatter,
+        )
+
+        phelp = "Input file. It can be compressed"
+        parserBandsplot.add_argument("file", help=phelp)
+
+        phelp = (
+            "Plot mode:\n"
+            "-m  scatter : is a points plot with the color given by the chosen\n"
+            "  projection. It produces a rather heavy pdf file.\n\n"
+            "-m  parametric : like scatter, but with lines instead of points \n"
+            "  (bands crossings are not handled, and some  unphysical 'jumps' \n"
+            " can be present). Sligthy smaller PDF size.\n\n"
+            "-m plain : is a featureless bandstructure ignoring all data about\n"
+            "  projections. Rather light-weight\n\n"
+            "-m atomic : For non-periodic system, like molecules, rather ugly \n"
+            "  but useful to visualize energy level. Only 1 K-point!\n\n"
+        )
+        choices = ["scatter", "plain", "parametric", "atomic"]
+        parserBandsplot.add_argument(
+            "-m", "--mode", help=phelp, default="plain", choices=choices
+        )
+
+        phelp = "Color of the bands for plain mode."
+        parserBandsplot.add_argument("-color", help=phelp, default="blue")
+
+        phelp = "Name of Abinit output file if used."
+        parserBandsplot.add_argument("-abinit", help=phelp, default=None)
+
+        phelp = (
+            "Spin component to be used (default -s 0): \n\n"
+            "Non-polarized calculations density is '-s 0', just ignore it.\n\n"
+            "Spin-Polarized (collinear) calculation: \n"
+            "-s 0 are the unpolarized bands, the spin-polarization is ignored.\n"
+            "-s 1 'spin-polarized' bands, the character of 'up' bands positive,\n"
+            "  but negative for 'down' bands, this means that the color of \n"
+            "  'down' is negative. Useful together with '--cmap seismic'.\n\n"
+            "Non-collinear calculation: \n"
+            "-s 0 : density, ie: Spin-orbit-coupling but don't care of spin.\n"
+            "-s 1 : Sx, projection along 'x' quantization axis, see SAXIS flag\n"
+            "  in the VASP manual\n"
+            "-s 2 : Sy, projection along 'y' quantization axis.\n"
+            "-s 3 : Sy, projection along 'z' quantization axis.\n"
+            "-s st : Spin-texture perpendicular in the plane (kx,ky) to each\n "
+            "(kx,ky) vector. Useful for Rashba-like states in surfaces. Use\n "
+            "'--cmap seismic'\n\n "
+        )
+        parserBandsplot.add_argument(
+            "-s", "--spin", choices=["0", "1", "2", "3", "st"], default="0", help=phelp
+        )
+
+        phelp = (
+            "List of rows (atoms) to be used. This list refers to the rows of\n"
+            "(each block of) your PROCAR file. If you haven't manipulated your\n"
+            "PROCAR (eg: with the '-a' option of 'filter' mode) each row\n"
+            "correspond to the respective atom in the POSCAR.\n\n"
+            "Mind: This list is 0-based, ie: the 1st atom is 0, the 2nd is 1,\n"
+            "  and so on. If you need to be treated like a human, specify '-u'\n"
+            "or '--human' and 1st->1, 2nd->2, etc.\n\n"
+            "Example:\n"
+            "-a 0 2 :  select the 1st  and 3rd. rows (likely 1st and 3rd atoms)"
+            "\n\n"
+        )
+        parserBandsplot.add_argument(
+            "-a", "--atoms", type=int, nargs="+", help=phelp, default=None
+        )
+
+        phelp = (
+            "Orbitals index(es) to be used, take a look to the PROCAR file, \n"
+            "they are 's py pz px ...', then s->0, py->1, pz->2 and so on. \n"
+            "Note that indexes begin at 0!. Its default is the last field (ie:\n"
+            "'tot', did you saw the PROCAR?). Some examples:\n\n"
+            "-o 0 : s-orbital (unless you modified the orbitals, eg. 'filter')\n"
+            "-o 1 2 3 : py+pz+px (unless you modified the orbitals)\n"
+            "-o 4 5 6 7 8 : all the d-orbitasl (unless...)\n"
+            "-o 2 6 : pz+dzz (did you look at the PROCAR?)\n\n "
+        )
+        parserBandsplot.add_argument(
+            "-o", "--orbitals", type=int, nargs="+", help=phelp, default=None
+        )
+
+        phelp = (
+            "Set the Fermi energy (or any reference energy) as the zero energy.\n"
+            "See '--outcar', avoids to give it explicitly. A list of \n"
+            "k-dependant 'fermi-like energies' are also accepted (useful to\n"
+            "compare different systems in one PROCAR made by hand). \n\n"
+            "Mind: The Fermi energy MUST be the one from the self-consistent\n"
+            "calculation, not from a Bandstructure calculation!\n\n"
+        )
+        parserBandsplot.add_argument(
+            "-f", "--fermi", type=float, help=phelp, nargs="+", default=None
+        )
+
+        phelp = (
+            "Min/Max energy to be ploted. Example:\n "
+            "--elimit -1 1 : From -1 to 1 around Fermi energy (if given)\n\n"
+        )
+        parserBandsplot.add_argument(
+            "--elimit", type=float, nargs=2, help=phelp, default=None
+        )
+
+        phelp = (
+            "If given, it masks(hides) bands with values lowers than 'mask'.\n"
+            "It is useful to remove 'unwanted' bands. For instance, if you\n"
+            "project the bandstructure on a 'surface' atom -with the default\n"
+            "colormap- some white points can appear, they are bands with \n"
+            "almost no contribution to the 'surface': no physics but they \n"
+            "still look ugly, to hide those bands use '--mask 0.08' (or some \n"
+            "other small value). Mind: it works with the absolute value of\n"
+            "projection (no problem with spin polarization)\n\n"
+        )
+        parserBandsplot.add_argument("--mask", type=float, help=phelp, default=None)
+
+        phelp = (
+            "Size of markers, if used. Each mode has it own scale,\n"
+            "just test them\n\n"
+        )
+        parserBandsplot.add_argument(
+            "--markersize", type=float, help=phelp, default=0.02
+        )
+
+        phelp = (
+            "Change the color scheme. Example:\n\n"
+            "--cmap  seismic : blue->white->red, useful to see the \n"
+            "  spin-polarization of a band (it will blueish or reddish)\n"
+            "  depending of spin channel\n"
+            "--cmap  seismic_r : the 'seismic' colormap, but reversed.\n\n"
+        )
+        parserBandsplot.add_argument("--cmap", help=phelp, default="jet")
+
+        phelp = (
+            "Do you want to Normalize the plots to the same scale of colors\n"
+            "(ie: the numbers on the bar at the right), just try '--vmax'\n\n"
+            "--vmax 1 : If you are looking for the s, p or d character.\n"
+            "--vmax 0.2: If you want to capture some tiny effect, eg: s-band of\n"
+            "  a impurity on a metal\n\n"
+        )
+        parserBandsplot.add_argument("--vmax", type=float, help=phelp, default=None)
+
+        phelp = (
+            "Like '--vmax' (see '--vmax'), However, for spin-polarized \n"
+            "(collinear or not) you can set it to a negative value. Actually\n"
+            "you can do it for a non-spin-polarized calculation and the \n"
+            "effect will be a 'stretching' of the color scheme, try it.\n\n"
+        )
+        parserBandsplot.add_argument("--vmin", type=float, help=phelp, default=None)
+
+        phelp = "switch on/off the grid. Default is 'on'\n\n"
+        parserBandsplot.add_argument("--grid", type=bool, help=phelp, default=True)
+
+        phelp = (
+            "set the marker shape, ie: 'o'=circle, 's'=square,\ '-'=line\n"
+            "(only mode `plain`, other symbols: google pyplot markers)\n\n"
+        )
+        parserBandsplot.add_argument("--marker", type=str, help=phelp, default="o")
+
+        phelp = (
+            "Some fault tolerance for ill-formatted files (stupid fortran)\n"
+            "But be careful, something could be messed up and don't work (at\n"
+            "least as expected). Length of K-points paths will be ignored\n\n"
+        )
+        parserBandsplot.add_argument("--permissive", help=phelp, action="store_true")
+
+        phelp = (
+            "Enable human-like 1-based order (ie 1st is 1, 2nd is 2, and so\n"
+            "on). Mind: this only works for atoms, not for orbitals or spin\n\n"
+        )
+        parserBandsplot.add_argument("-u", "--human", help=phelp, action="store_true")
+
+        phelp = (
+            "Saves the figure, instead of display it on screen. Anyway, you can\n"
+            "save from the screen too. Any file extension supported by\n "
+            "`matplotlib.savefig` is valid (if you are too lazy to google it,\n"
+            "trial and error also works fine)\n\n"
+        )
+        parserBandsplot.add_argument("--savefig", help=phelp, default=None)
+
+        phelp = (
+            "list of ticks along the kpoints axis (x axis). For instance a\n"
+            "bandstructure G-X-M with 10 point by segment should be:\n "
+            "--kticks 0 9 19\n\n"
+        )
+        parserBandsplot.add_argument("--kticks", help=phelp, nargs="+", type=int)
+
+        phelp = (
+            "Names of the points given in `--kticks`. In the `kticks` example\n"
+            'they should be `--knames "\$Gamma\$" X M`. As you can see \n'
+            "LaTeX stuff works with a minimal mess (extra \\s)\n\n"
+        )
+        parserBandsplot.add_argument(
+            "--knames", help=phelp, nargs="+", type=str, default=None
+        )
+
+        phelp = (
+            "Title, to use several words, use quotation marks\"\" or ''. Latex\n"
+            " works if you scape the special characteres, ie: $\\alpha$ -> \n"
+            "\$\\\\alpha\$"
+        )
+        parserBandsplot.add_argument(
+            "-t", "--title", help=phelp, type=str, default=None
+        )
+
+        phelp = (
+            "OUTCAR file where to find the reciprocal lattice vectors and\n "
+            "perhaps E_fermi.\n"
+            "Mind: '--fermi' has precedence, remember that the E-fermi should\n"
+            "correspond to a self-consistent run, not to a bandstructure!\n"
+            "(however, the basis and reciprocal vectors will be safe from the\n"
+            "non-self-consistentness)\n\n"
+        )
+        parserBandsplot.add_argument("--outcar", help=phelp, default=None)
+
+        phelp = "KPOINTS file for bandstructure plotting.\n"
+        parserBandsplot.add_argument("--kpointsfile", help=phelp, default=None)
+
+        phelp = "Convert k-points from reduced to cartesian for plot #1?"
+        parserBandsplot.add_argument("-kdirect", help=phelp, action="store_false")
+
+        parserBandsplot.set_defaults(func=call_bandsplot)
+
+        args = parser.parse_args()
+        args.func(args)
+
+    else:
+        print("PyProcar: A Python library for analyzing PROCAR files.\n")
+        print("Usage: procar [-h]")
+        print(
+            "{cat,mergeabinit,unfold,filter,fermi2D,fermi3D,repair,generate2dkmesh,kpath,bandsplot,bandscompare}"
+        )
```

### Comparing `PyProcar-5.6.6/setup.json` & `PyProcar-6.0.0/setup.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.85%*

 * *Differences: {"'date'": "'Jun 10th, 2021'",*

 * * "'download_url'": "'https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz'",*

 * * "'version'": "'6.0.0'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Francisco Mu\u00f1oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah",
     "copyright": "Copyright 2021",
-    "date": "March 6th, 2022",
+    "date": "Jun 10th, 2021",
     "description": "A Python library for electronic structure pre/post-processing. ",
-    "download_url": "https://github.com/romerogroup/pyprocar/archive/5.6.5.tar.gz",
+    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz",
     "email": "fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com",
     "name": "PyProcar",
     "status": "development",
     "url": "https://github.com/romerogroup/pyprocar",
-    "version": "5.6.6"
+    "version": "6.0.0"
 }
```

