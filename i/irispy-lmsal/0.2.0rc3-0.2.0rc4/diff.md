# Comparing `tmp/irispy-lmsal-0.2.0rc3.tar.gz` & `tmp/irispy-lmsal-0.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irispy-lmsal-0.2.0rc3.tar", last modified: Wed Jun 15 06:11:52 2022, max compression
+gzip compressed data, was "irispy-lmsal-0.2.0rc4.tar", last modified: Fri Jun  9 23:32:33 2023, max compression
```

## Comparing `irispy-lmsal-0.2.0rc3.tar` & `irispy-lmsal-0.2.0rc4.tar`

### file list

```diff
@@ -1,117 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.685405 irispy-lmsal-0.2.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/.codecov.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3636 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1220 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      363 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     1656 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     1505 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1804 2022-06-15 06:11:52.685405 irispy-lmsal-0.2.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      738 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.641402 irispy-lmsal-0.2.0rc3/changelog/
--rw-rw-rw-   0 root         (0) root         (0)     1887 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/changelog/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.644152 irispy-lmsal-0.2.0rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      162 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/changelog.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.645069 irispy-lmsal-0.2.0rc3/docs/code_api/
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/code_api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/code_api/sji.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/code_api/spectrograph.rst
--rw-rw-rw-   0 root         (0) root         (0)      116 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/code_api/utils.rst
--rw-rw-rw-   0 root         (0) root         (0)     3795 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)    18857 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/guide.rst
--rw-rw-rw-   0 root         (0) root         (0)     1762 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     4557 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4305 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     2192 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/known_issues.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/docs/rtd_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.645986 irispy-lmsal-0.2.0rc3/examples/
--rw-rw-rw-   0 root         (0) root         (0)      350 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/examples/README.txt
--rw-rw-rw-   0 root         (0) root         (0)     6556 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/examples/mg_ii_dopplergrams.py
--rw-rw-rw-   0 root         (0) root         (0)    15113 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/examples/overview.py
--rw-rw-rw-   0 root         (0) root         (0)     4708 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/examples/timeseries_analysis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.648736 irispy-lmsal-0.2.0rc3/irispy/
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2022-06-15 06:11:51.000000 irispy-lmsal-0.2.0rc3/irispy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.655153 irispy-lmsal-0.2.0rc3/irispy/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2742 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/_sample.py
--rw-rw-rw-   0 root         (0) root         (0)    15008 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sg_psfs.geny
--rw-rw-rw-   0 root         (0) root         (0)   395148 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_20130211.geny
--rw-rw-rw-   0 root         (0) root         (0)   394308 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_20130715.geny
--rw-rw-rw-   0 root         (0) root         (0)   396308 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20150331.geny
--rw-rw-rw-   0 root         (0) root         (0)   396540 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20161022.geny
--rw-rw-rw-   0 root         (0) root         (0)   396564 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20191101.geny
--rw-rw-rw-   0 root         (0) root         (0)   397016 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20200223.geny
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.676238 irispy-lmsal-0.2.0rc3/irispy/data/test/
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/compress.py
--rw-rw-rw-   0 root         (0) root         (0)   394292 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version001.sav
--rw-rw-rw-   0 root         (0) root         (0)   394320 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version002.sav
--rw-rw-rw-   0 root         (0) root         (0)   103100 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version003.sav
--rw-rw-rw-   0 root         (0) root         (0)   103096 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version004.sav
--rw-rw-rw-   0 root         (0) root         (0)   103100 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version005.sav
--rw-rw-rw-   0 root         (0) root         (0)   103100 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version006.sav
--rw-rw-rw-   0 root         (0) root         (0)   763200 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_1330_t000.fits
--rw-rw-rw-   0 root         (0) root         (0)   763200 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_1400_t000.fits
--rw-rw-rw-   0 root         (0) root         (0)   763200 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_2796_t000.fits
--rw-rw-rw-   0 root         (0) root         (0)   763200 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_2832_t000.fits
--rw-rw-rw-   0 root         (0) root         (0) 12170880 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/iris_l2_20170502_052551_3893010094_raster_t000_r00000.fits
--rwxrwxrwx   0 root         (0) root         (0)   103088 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/test/test_response.sav
--rw-rw-rw-   0 root         (0) root         (0)     9037 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v36-table10.csv
--rw-rw-rw-   0 root         (0) root         (0)     2283 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v36-table2000.csv
--rw-rw-rw-   0 root         (0) root         (0)    10865 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v38-table10.csv
--rw-rw-rw-   0 root         (0) root         (0)     2214 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v38-table2000.csv
--rw-rw-rw-   0 root         (0) root         (0)     7785 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v40-table10.csv
--rw-rw-rw-   0 root         (0) root         (0)     2206 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/data/v40-table2000.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.678071 irispy-lmsal-0.2.0rc3/irispy/io/
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/sji.py
--rw-rw-rw-   0 root         (0) root         (0)    14290 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/spectrograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.678071 irispy-lmsal-0.2.0rc3/irispy/io/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2239 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3454 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/io/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/obsid.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/sji.py
--rw-rw-rw-   0 root         (0) root         (0)    11991 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/spectrograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.679905 irispy-lmsal-0.2.0rc3/irispy/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/tests/test_obsid.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/tests/test_sji.py
--rw-rw-rw-   0 root         (0) root         (0)    10993 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/tests/test_sji_fd.py
--rw-rw-rw-   0 root         (0) root         (0)     7916 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/tests/test_spectrograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.681738 irispy-lmsal-0.2.0rc3/irispy/utils/
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    18690 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/response.py
--rw-rw-rw-   0 root         (0) root         (0)     7939 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/spectrograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.683572 irispy-lmsal-0.2.0rc3/irispy/utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7194 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2529 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_spectrograph.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1449 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_wobble.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4000 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/utils/wobble.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/irispy/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.685405 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1804 2022-06-15 06:11:51.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2967 2022-06-15 06:11:52.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-15 06:11:52.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-15 06:11:51.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      333 2022-06-15 06:11:52.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-06-15 06:11:52.000000 irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 06:11:52.685405 irispy-lmsal-0.2.0rc3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1411 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3190 2022-06-15 06:11:52.686322 irispy-lmsal-0.2.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      878 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2022-06-15 06:11:34.000000 irispy-lmsal-0.2.0rc3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.133406 irispy-lmsal-0.2.0rc4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.141407 irispy-lmsal-0.2.0rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.141407 irispy-lmsal-0.2.0rc4/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/changelog/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.145407 irispy-lmsal-0.2.0rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.145407 irispy-lmsal-0.2.0rc4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/reference/irispy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/reference/sji.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/reference/spectrograph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/docs/rtd_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.145407 irispy-lmsal-0.2.0rc4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/align_iris_aia_rolled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/mg_ii_dopplergrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/skip_umbral_flashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/examples/south_sji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.145407 irispy-lmsal-0.2.0rc4/irispy/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.145407 irispy-lmsal-0.2.0rc4/irispy/_dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/_dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/_dev/scm_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 23:32:32.000000 irispy-lmsal-0.2.0rc4/irispy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.153407 irispy-lmsal-0.2.0rc4/irispy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sg_psfs.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   395148 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_20130211.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   394308 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_20130715.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   396308 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20150331.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   396540 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20161022.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   396564 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20191101.geny
+-rw-r--r--   0 runner    (1001) docker     (123)   397016 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20200223.geny
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.161407 irispy-lmsal-0.2.0rc4/irispy/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)   394292 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version001.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   394320 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version002.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   103100 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version003.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   103096 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version004.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   103100 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version005.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   103100 2023-06-09 23:31:41.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version006.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   345600 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_1330_t000_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   408960 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_1400_t000_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   408960 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_2796_t000_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    86400 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_2832_t000_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5264640 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/iris_l2_20210905_001833_3620258102_raster_t000_r00000_test.fits
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103088 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/test/test_response.sav
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v34-table10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v34-table2000.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v36-table10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v36-table2000.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v38-table10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v38-table2000.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v40-table10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/data/v40-table2000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/sji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/spectrograph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/obsid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/sji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/spectrograph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/tests/test_obsid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/tests/test_sji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/tests/test_sji_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/tests/test_spectrograph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/spectrograph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_spectrograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_wobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/utils/wobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/irispy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-09 23:32:33.000000 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-09 23:32:33.000000 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:32:33.000000 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 23:32:33.000000 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 23:32:33.000000 irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 23:32:33.165407 irispy-lmsal-0.2.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-09 23:31:42.000000 irispy-lmsal-0.2.0rc4/tox.ini
```

### Comparing `irispy-lmsal-0.2.0rc3/.gitignore` & `irispy-lmsal-0.2.0rc4/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -216,15 +216,10 @@
 # Release script
 .github_cache
 
 # Misc Stuff
 .history
 *.orig
 .tmp
+
+# Example files
 iris_l2_20140708_114109_3824262996_raster_t000_r00000.fits
-iris_l2_20130902_163935_4000255147_SJI_1400_t000.fits.gz
-iris_l2_20130902_163935_4000255147_raster.tar.gz
-iris_l2_20130902_163935_4000255147_raster_t000_r00000.fits
-iris_l2_20140708_114109_3824262996_raster.tar.gz
-iris_l2_20140919_051712_3860608353_SJI_2832_t000.fits.gz
-iris_l2_20180102_153155_3610108077_raster.tar.gz
-iris_l2_20180102_153155_3610108077_raster_t000_r00000.fits
```

### Comparing `irispy-lmsal-0.2.0rc3/.pre-commit-config.yaml` & `irispy-lmsal-0.2.0rc4/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 repos:
   - repo: https://github.com/myint/docformatter
-    rev: v1.4
+    rev: v1.7.2-rc7
     hooks:
       - id: docformatter
         args: [--in-place, --pre-summary-newline, --make-summary-multi]
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|__init__.py|docs/conf.py)$"
+        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|docs/conf.py)$"
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.270'
+    hooks:
+      - id: ruff
+        args: ['--fix']
   -   repo: https://github.com/psf/black
-      rev: 22.3.0
+      rev: 23.3.0
       hooks:
       - id: black
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
-  -   repo: https://github.com/timothycrosley/isort
-      rev: 5.10.1
+  -   repo: https://github.com/PyCQA/isort
+      rev: 5.12.0
       hooks:
       - id: isort
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
   -   repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.2.0
+      rev: v4.4.0
       hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: mixed-line-ending
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: end-of-file-fixer
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: check-yaml
       - id: debug-statements
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
+    hooks:
+      - id: codespell
+        additional_dependencies:
+          - tomli
```

### Comparing `irispy-lmsal-0.2.0rc3/LICENSE.rst` & `irispy-lmsal-0.2.0rc4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/README.rst` & `irispy-lmsal-0.2.0rc4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-00000000: 6060 6972 6973 7079 2d6c 6d73 616c 6060  ``irispy-lmsal``
-00000010: 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  .***************
-00000020: 2a0a 0a2e 2e20 696d 6167 653a 3a20 6874  *.... image:: ht
-00000030: 7470 3a2f 2f69 7269 732e 6c6d 7361 6c2e  tp://iris.lmsal.
-00000040: 636f 6d2f 696d 6167 6573 2f69 7269 735f  com/images/iris_
-00000050: 6675 6c6c 2e6a 7067 0a20 203a 7769 6474  full.jpg.  :widt
-00000060: 683a 2034 3030 0a20 203a 616c 743a 2049  h: 400.  :alt: I
-00000070: 6d61 6765 206f 6620 7468 6520 4952 4953  mage of the IRIS
-00000080: 2073 7061 6365 6372 6166 740a 0a60 6069   spacecraft..``i
-00000090: 7269 7370 792d 6c6d 7361 6c60 6020 6973  rispy-lmsal`` is
-000000a0: 2061 206c 6962 7261 7279 2074 6861 7420   a library that 
-000000b0: 7072 6f76 6964 6573 2074 6865 2074 6f6f  provides the too
-000000c0: 6c73 2074 6f20 7265 6164 2069 6e20 616e  ls to read in an
-000000d0: 6420 616e 616c 797a 6520 6461 7461 2066  d analyze data f
-000000e0: 726f 6d20 496e 7465 7266 6163 6520 5265  rom Interface Re
-000000f0: 6769 6f6e 0a49 6d61 6769 6e67 2053 7065  gion.Imaging Spe
-00000100: 6374 726f 6772 6170 6820 2849 5249 5329  ctrograph (IRIS)
-00000110: 2e0a 0a49 5249 5320 6973 2061 204e 4153  ...IRIS is a NAS
-00000120: 412d 6675 6e64 6564 2053 6d61 6c6c 2045  A-funded Small E
-00000130: 7870 6c6f 7265 7220 7768 6963 6820 7573  xplorer which us
-00000140: 6573 2061 2068 6967 682d 6672 616d 652d  es a high-frame-
-00000150: 7261 7465 2075 6c74 7261 7669 6f6c 6574  rate ultraviolet
-00000160: 2069 6d61 6769 6e67 2073 7065 6374 726f   imaging spectro
-00000170: 6d65 7465 7220 746f 206d 616b 6520 6f62  meter to make ob
-00000180: 7365 7276 6174 696f 6e73 206f 6620 7468  servations of th
-00000190: 6520 5375 6e2e 0a46 6f72 206d 6f72 6520  e Sun..For more 
-000001a0: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
-000001b0: 7468 6520 6d69 7373 696f 6e2f 696e 7374  the mission/inst
-000001c0: 7275 6d65 6e74 2070 6170 6572 2077 6869  rument paper whi
-000001d0: 6368 2069 7320 6176 6169 6c61 626c 6520  ch is available 
-000001e0: 606f 6e6c 696e 6520 666f 7220 6672 6565  `online for free
-000001f0: 203c 6874 7470 733a 2f2f 7777 772e 6c6d   <https://www.lm
-00000200: 7361 6c2e 636f 6d2f 6972 6973 5f73 6369  sal.com/iris_sci
-00000210: 656e 6365 2f64 6f63 3f63 6d64 3d64 6375  ence/doc?cmd=dcu
-00000220: 7226 7072 6f6a 5f6e 756d 3d49 5330 3139  r&proj_num=IS019
-00000230: 3626 6669 6c65 5f74 7970 653d 7064 663e  6&file_type=pdf>
-00000240: 605f 5f2e 0a0a 6054 6865 2064 6174 6120  `__...`The data 
-00000250: 6973 2070 7562 6c69 636c 7920 6176 6169  is publicly avai
-00000260: 6c61 626c 6520 3c68 7474 7073 3a2f 2f69  lable <https://i
-00000270: 7269 732e 6c6d 7361 6c2e 636f 6d2f 6461  ris.lmsal.com/da
-00000280: 7461 2e68 746d 6c3e 605f 5f2e 0a0a 6044  ta.html>`__...`D
-00000290: 6f63 756d 656e 7461 7469 6f6e 2069 7320  ocumentation is 
-000002a0: 686f 7374 6564 206f 6e20 5254 4420 3c68  hosted on RTD <h
-000002b0: 7474 7073 3a2f 2f69 7269 7370 792d 6c6d  ttps://irispy-lm
-000002c0: 7361 6c2e 7265 6164 7468 6564 6f63 732e  sal.readthedocs.
-000002d0: 696f 2f65 6e2f 7374 6162 6c65 2f3e 605f  io/en/stable/>`_
-000002e0: 5f0a                                     _.
+00000000: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000010: 0a60 6069 7269 7370 792d 6c6d 7361 6c60  .``irispy-lmsal`
+00000020: 600a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  `.**************
+00000030: 2a2a 0a0a 2e2e 2069 6d61 6765 3a3a 2068  **.... image:: h
+00000040: 7474 703a 2f2f 6972 6973 2e6c 6d73 616c  ttp://iris.lmsal
+00000050: 2e63 6f6d 2f69 6d61 6765 732f 6972 6973  .com/images/iris
+00000060: 5f66 756c 6c2e 6a70 670a 2020 3a77 6964  _full.jpg.  :wid
+00000070: 7468 3a20 3430 300a 2020 3a61 6c74 3a20  th: 400.  :alt: 
+00000080: 496d 6167 6520 6f66 2074 6865 2049 5249  Image of the IRI
+00000090: 5320 7370 6163 6563 7261 6674 0a0a 6060  S spacecraft..``
+000000a0: 6972 6973 7079 2d6c 6d73 616c 6060 2069  irispy-lmsal`` i
+000000b0: 7320 6120 6c69 6272 6172 7920 7468 6174  s a library that
+000000c0: 2070 726f 7669 6465 7320 7468 6520 746f   provides the to
+000000d0: 6f6c 7320 746f 2072 6561 6420 696e 2061  ols to read in a
+000000e0: 6e64 2061 6e61 6c79 7a65 2064 6174 6120  nd analyze data 
+000000f0: 6672 6f6d 2049 6e74 6572 6661 6365 2052  from Interface R
+00000100: 6567 696f 6e20 496d 6167 696e 6720 5370  egion Imaging Sp
+00000110: 6563 7472 6f67 7261 7068 2028 4952 4953  ectrograph (IRIS
+00000120: 292e 0a0a 4952 4953 2069 7320 6120 4e41  )...IRIS is a NA
+00000130: 5341 2d66 756e 6465 6420 536d 616c 6c20  SA-funded Small 
+00000140: 4578 706c 6f72 6572 2077 6869 6368 2075  Explorer which u
+00000150: 7365 7320 6120 6869 6768 2d66 7261 6d65  ses a high-frame
+00000160: 2d72 6174 6520 756c 7472 6176 696f 6c65  -rate ultraviole
+00000170: 7420 696d 6167 696e 6720 7370 6563 7472  t imaging spectr
+00000180: 6f6d 6574 6572 2074 6f20 6d61 6b65 206f  ometer to make o
+00000190: 6273 6572 7661 7469 6f6e 7320 6f66 2074  bservations of t
+000001a0: 6865 2053 756e 2e0a 466f 7220 6d6f 7265  he Sun..For more
+000001b0: 2069 6e66 6f72 6d61 7469 6f6e 2073 6565   information see
+000001c0: 2074 6865 206d 6973 7369 6f6e 2f69 6e73   the mission/ins
+000001d0: 7472 756d 656e 7420 7061 7065 7220 7768  trument paper wh
+000001e0: 6963 6820 6973 2061 7661 696c 6162 6c65  ich is available
+000001f0: 2060 6f6e 6c69 6e65 2066 6f72 2066 7265   `online for fre
+00000200: 6520 3c68 7474 7073 3a2f 2f77 7777 2e6c  e <https://www.l
+00000210: 6d73 616c 2e63 6f6d 2f69 7269 735f 7363  msal.com/iris_sc
+00000220: 6965 6e63 652f 646f 633f 636d 643d 6463  ience/doc?cmd=dc
+00000230: 7572 2670 726f 6a5f 6e75 6d3d 4953 3031  ur&proj_num=IS01
+00000240: 3936 2666 696c 655f 7479 7065 3d70 6466  96&file_type=pdf
+00000250: 3e60 5f5f 2e0a 0a60 5468 6520 6461 7461  >`__...`The data
+00000260: 2069 7320 7075 626c 6963 6c79 2061 7661   is publicly ava
+00000270: 696c 6162 6c65 203c 6874 7470 733a 2f2f  ilable <https://
+00000280: 6972 6973 2e6c 6d73 616c 2e63 6f6d 2f64  iris.lmsal.com/d
+00000290: 6174 612e 6874 6d6c 3e60 5f5f 2e0a 0a60  ata.html>`__...`
+000002a0: 446f 6375 6d65 6e74 6174 696f 6e20 6973  Documentation is
+000002b0: 2068 6f73 7465 6420 6f6e 2052 5444 203c   hosted on RTD <
+000002c0: 6874 7470 733a 2f2f 6972 6973 7079 2d6c  https://irispy-l
+000002d0: 6d73 616c 2e72 6561 6474 6865 646f 6373  msal.readthedocs
+000002e0: 2e69 6f2f 656e 2f73 7461 626c 652f 3e60  .io/en/stable/>`
+000002f0: 5f5f 0a                                  __.
```

### Comparing `irispy-lmsal-0.2.0rc3/changelog/README.rst` & `irispy-lmsal-0.2.0rc4/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/docs/Makefile` & `irispy-lmsal-0.2.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/docs/contributing.rst` & `irispy-lmsal-0.2.0rc4/docs/contributing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 ********************************
 Contributing to ``irispy-lmsal``
 ********************************
 
 ``irispy-lmsal`` is open-source and community-developed and we are always glad to welcome new contributors and users.
-
-We are always enthusiastic to welcome new users and developers who want to enhance the ``irispy-lmsal``.
 You can contribute in several ways, from providing feedback, reporting bugs, contributing code, and reviewing pull requests.
 There is a role for almost any level of engagement.
 
 Providing Feedback
 ==================
 
 We could always use more voices and opinions in the discussions about ``irispy-lmsal`` and its development from both users and developers.
-There are a r of ways to make your voice heard.
+There are ways to make your voice heard.
 Whether it be constructive criticism, inquiries about current or future capabilities, or flattering praise, we would love to hear from you.
 
 Reporting Bugs
 ==============
 
 If you run into unexpected behavior or a bug please report it.
 All bugs are raised and stored on our `issue tracker`_.
@@ -27,27 +25,27 @@
 =================
 
 If you would like to contribute code, it is strongly recommended that you first discuss your aims with the ``irispy-lmsal`` community.
 We strive to be an open and welcoming community for developers of all experience levels.
 Discussing your ideas before you start can give you new insights that will make your development easier, lead to a better end product, and reduce the chances of your work being regretfully rejected because of an issue you weren't aware of, e.g. the functionality already exists elsewhere.
 
 In the rest of this section we will go through the steps needed to set up your system so you can contribute code to ``irispy-lmsal``.
-This is done using `git`_ version control software and `GitLab`_, a website that allows you to upload, update, and share code repositories (repos).
-If you are new to code development or git and GitLab you can learn more from the following guides:
+This is done using `git`_ version control software and `GitHub`_, a website that allows you to upload, update, and share code repositories (repos).
+If you are new to code development or git and GitHub you can learn more from the following guides:
 
 * `SunPy Newcomers Guide`_
-* `GitLab guide`_
+* `GitHub guide`_
 * `git guide`_
 
-The principles in the SunPy guides for contributing code and utilizing GitLab and git are exactly the same for ``irispy-lmsal`` except that we contribute to the irispy repository rather than the ``sunpy`` one.
+The principles in the SunPy guides for contributing code and utilizing GitHub and git are exactly the same for ``irispy-lmsal`` except that we contribute to the irispy repository rather than the ``sunpy`` one.
 If you are a more seasoned developer and would like to get further information, you can check out the `sunpy Developers Guide`_.
 
 Before you can contribute code to irispy, you first need to install the development version of ``irispy-lmsal``.
 To find out how, see :ref:`dev_install`.
 
-.. _issue tracker: https://gitlab.com/LMSAL_HUB/iris_hub/irispy-lmsal/issues
+.. _issue tracker: https://github.com/LM-SAL/irispy-lmsal/issues
 .. _SunPy Newcomers Guide: http://docs.sunpy.org/en/latest/dev_guide/newcomers.html
-.. _GitLab: https://about.gitlab.com/
+.. _GitHub: https://github.com/
 .. _git: https://git-scm.com/
-.. _GitLab guide: https://docs.gitlab.com/ee/gitlab-basics/
+.. _GitHub guide: https://github.com/git-guides
 .. _git guide: https://git-scm.com/book/en/v2/Getting-Started-Git-Basics
 .. _sunpy Developers Guide: http://docs.sunpy.org/en/latest/dev_guide
```

### Comparing `irispy-lmsal-0.2.0rc3/docs/guide.rst` & `irispy-lmsal-0.2.0rc4/docs/guide.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-******************************************************
-A quick guide to work with IRIS Level 2 data in Python
-******************************************************
+.. _guide:
 
-This guide is intended to help the solar community to start working with IRIS Level 2 data using Python.
-It is especially oriented to those who have a limited knowledge of Python and want to start using this language to analyze IRIS data.
+*************************
+An ``irispy-lmsal`` guide
+*************************
+
+This guide is intended to help the solar community to start working with level 2 data using Python.
+It is especially oriented to those who have a limited knowledge of Python and want to start using this language to analyze data.
 
 This guide will cover:
 
-- reading IRIS Level 2 files
+- reading level 2 files
 - load the data of any of the spectral windows
-- visualize, inspect, and interact with them
 
 In the future more features will arrive:
 
 - a GUI to interact with the data
-- analysis tools
 - a way to save and load regions of interest
-- reading of L3 IRIS data
-- Dopplergrams
+- analysis tools
 - Density Diagnostics
+- Dopplergrams
 - PSF and filter functions
-
+- reading of L3 data
 
 Currently, ``irispy-lmsal`` does not provide a way to download the data from the `IRIS archive <https://iris.lmsal.com/data.html>`__.
 We recommend you browse the catalogue using your browser.
 
 This guide uses some "sample data" from the IRIS archive that can be accessed:
 
 .. code-block:: python
 
   >>> import irispy.data.sample as sample_data  # doctest: +REMOTE_DATA
 
-Once the IRIS Level 2 data has downloaded, the next step is to read, extract, and inspect them.
+Once the level 2 data has downloaded, the next step is to read, extract, and inspect them.
 
 .. code-block:: python
 
   >>> from irispy.io import read_files  # doctest: +REMOTE_DATA
 
 The sample data is from this `observation
 <https://www.lmsal.com/hek/hcr?cmd=view-event&event-id=ivo%3A%2F%2Fsot.lmsal.com%2FVOEvent%23VOEvent_IRIS_20211001_060925_3683602040_2021-10-01T06%3A09%3A252021-10-01T06%3A09%3A25.xml>`__.
@@ -51,84 +51,77 @@
     This, by default will load the data into memory.
     You can pass ``memmap=True`` to avoid this, the data array will be a `numpy.memmap` instead.
     Thus, the data are not loaded in the memory of the system, but written in a temporary file.
 
 .. code-block:: python
 
     >>> raster  # doctest: +REMOTE_DATA
-    <irispy.spectrograph.IRISCollection object at ...>
+    <irispy.spectrograph.Collection object at ...>
     <BLANKLINE>
-    IRISCollection
-    --------------
+    Collection
+    ----------
     Cube keys: ('C II 1336', 'Si IV 1394', 'Mg II k 2796')
     Number of Cubes: 3
     Aligned dimensions: [<Quantity 5. pix> <Quantity 16. pix> <Quantity 548. pix>]
     Aligned physical types: [('meta.obs.sequence',), ...]
     <BLANKLINE>
 
 We get some basic information about the raster file from this, what spectral windows were observed
 The size of the cube, the wavelength keys as well.
 
-.. note::
-
-  Notice the raster type here, it is a `ndcube.ndcollection.NDCollection` instance.
-  In order to allow easier use o multidimensional data sets (which are common in astronomy), the SunPy-affiliated package `ndcube <https://docs.sunpy.org/projects/ndcube/en/stable/>`_  was developed.
-  This package combines N-dimensional data with their corresponding word coordinate system (WCS) information
-  allowing the data be sliced, visualized and to undergo WCS transforms to alternative coordinate systems.
-  ``irispy-lmsal`` is built upon this.
-
 If we want to check the header of the raster, we can do the following:
-
 Let us check the header of this collection, this is stored as a ``meta`` attribute:
 
 .. code-block:: python
 
     >>> raster["C II 1336"][0].meta  # doctest: +REMOTE_DATA
-    <irispy.io.spectrograph.IRISSGMeta object at ...>
+    <irispy.spectrograph.SGMeta object at ...>
     <BLANKLINE>
-    IRISMeta
-    --------
+    SGMeta
+    ------
     Observatory:     IRIS
     Instrument:      SPEC
     Detector:        FUV1
     Spectral Window: C II 1336
     Spectral Range:  [1331.70275015 1358.28579039] Angstrom
     Spectral Band:   FUV
     Dimensions:      [16, 548, 513]
     Date:            2021-10-01T06:09:25.090
     OBS ID:          3683602040
     OBS Description: Very large sparse 16-step raster 15x175 16s   Deep x 0.5 Spatial x 2
     <BLANKLINE>
 
 Note this is not on the main object but each individual element, in this case the spectral window.
-While the SJI files contain just one spectral window per file, the raster files have several spectral windows
-per file.
+While the SJI files contain just one spectral window per file, the raster files have several spectral windows per file.
 
-As the SJI IRIS Level 2 data are simpler than the raster files, since they have only one spectral window per
-file, we will start with this data instead of the raster file above.
+As the SJI level 2 data are simpler than the raster files, since they have only one spectral window per file, we will start with this data instead of the raster file above.
 
-We use the following command to read and load the data from a SJI IRIS Level 2 file:
+We use the following command to read and load the data from a SJI level 2 file:
 
 .. code-block:: python
 
     >>> iris_sji = read_files(sample_data.SJI_1330)  # doctest: +REMOTE_DATA
     >>> iris_sji  # doctest: +REMOTE_DATA
-    <irispy.sji.IRISMapCubeSequence object at ...>
+    <irispy.sji.SJICube object at ...>
     <BLANKLINE>
-    IRISMapCubeSequence
-    -------------------
-    Observatory:     IRIS
-    Instrument:      SJI
-    OBS ID:          3683602040
-    OBS Description: Very large sparse 16-step raster 15x175 16s   Deep x 0.5 Spatial x 2
-    OBS period:      2021-10-01T06:09:24.920 -- 2021-10-01T06:11:44.461
-    Sequence period: 2021-10-01T06:09:25.020 -- 2021-10-01T06:11:37.580
-    Sequence Shape:  (<Quantity 20. pix>, <Quantity 548. pix>, <Quantity 555. pix>)
-    Axis Types:      [('meta.obs.sequence',), ('custom:pos.helioprojective.lon', 'custom:pos.helioprojective.lat'), ('custom:pos.helioprojective.lon', 'custom:pos.helioprojective.lat')]
-    Roll:            0.000464606 deg
+    SJICube
+    -------
+    Observatory:           IRIS
+    Instrument:            SJI
+    Bandpass:              1330.0
+    Obs. Start:            2021-10-01T06:09:24.920
+    Obs. End:              2021-10-01T06:11:44.461
+    Instance Start:        2021-10-01T06:09:25.020
+    Instance End:          2021-10-01T06:11:37.580
+    Total Frames in Obs.:  None
+    IRIS Obs. id:          3683602040
+    IRIS Obs. Description: Very large sparse 16-step raster 15x175 16s   Deep x 0.5 Spatial x 2
+    Axis Types:            [('custom:pos.helioprojective.lon', 'custom:pos.helioprojective.lat', 'time', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM', 'custom:CUSTOM'), ('custom:pos.helioprojective.lon', 'custom:pos.helioprojective.lat'), ('custom:pos.helioprojective.lon', 'custom:pos.helioprojective.lat')]
+    Roll:                  0.000464606
+    Cube dimensions:       [ 20. 548. 555.] pix
     <BLANKLINE>
 
 Metadata
 ========
 
 Here we will highlight some of the more important metadata that is available.
 
@@ -140,107 +133,126 @@
     'Very large sparse 16-step raster 15x175 16s   Deep x 0.5 Spatial x 2'
 
 When the observation started:
 
 .. code-block:: python
 
     >>> iris_sji.meta['STARTOBS']   # doctest: +REMOTE_DATA
-    <Time object: scale='utc' format='isot' value=2021-10-01T06:09:24.920>
+    '2021-10-01T06:09:24.920'
 
 It possible it might be in a ``"DATE_OBS"`` instead.
 
 The exposure times:
 
 .. code-block:: python
 
     >>> iris_sji.exposure_time   # doctest: +REMOTE_DATA
-    <ndcube.extra_coords.extra_coords.ExtraCoords object at ...>
-    ExtraCoords(exposure time (0) None: QuantityTableCoordinate ['exposure time'] [None]:
     <Quantity [0.50031197, 0.50025398, 0.50023699, 0.50024003, 0.50023901,
                0.50028503, 0.50024903, 0.500269  , 0.50026202, 0.500247  ,
                0.50029403, 0.50021601, 0.50028402, 0.50023901, 0.50024903,
-               0.50025803, 0.500283  , 0.50029802, 0.50029498, 0.50027299] s>)
+               0.50025803, 0.500283  , 0.50029802, 0.50029498, 0.50027299] s>
 
 In most cases, the exposure times are fixed for all scans in a raster.
-However, when automatic exposure compensation (AEC) is switched on and there is a very energetic event (e.g. a
-flare), IRIS will automatically use a lower exposure time to prevent saturation in the detectors.
+However, when automatic exposure compensation (AEC) is switched on and there is a very energetic event (e.g. a flare), IRIS will automatically use a lower exposure time to prevent saturation in the detectors.
 
-If the exposure time varies, you can get the time-dependent exposure times in seconds from the auxiliary
-metadata, second to last HDU in the file with the keys ``"EXPTIMEF"`` and ``"EXPTIMEN"``.
+If the exposure time varies, you can get the time-dependent exposure times in seconds from the auxiliary metadata, second to last HDU in the file with the keys ``"EXPTIMEF"`` and ``"EXPTIMEN"``.
 
-To get arrays of timestamps, or exposure times or "xcenix", that information will be in the ``extra_coords``
-attribute.
+To get arrays of timestamps, or exposure times or "xcenix", that information will be in the ``extra_coords`` attribute.
 
 .. code-block:: python
 
     >>> iris_sji.extra_coords  # doctest: +REMOTE_DATA
     <ndcube.extra_coords.extra_coords.ExtraCoords object at ...>
-    ExtraCoords(time (0) None: TimeTableCoordinate ['time'] [None]:
-    ['2021-10-01T06:09:25.020' '2021-10-01T06:09:31.990'
-     '2021-10-01T06:09:38.950' '2021-10-01T06:09:45.920'
-     '2021-10-01T06:09:52.920' '2021-10-01T06:09:59.890'
-     '2021-10-01T06:10:06.860' '2021-10-01T06:10:13.860'
-     '2021-10-01T06:10:20.830' '2021-10-01T06:10:27.800'
-     '2021-10-01T06:10:34.800' '2021-10-01T06:10:41.770'
-     '2021-10-01T06:10:48.740' '2021-10-01T06:10:55.740'
-     '2021-10-01T06:11:02.700' '2021-10-01T06:11:09.670'
-     '2021-10-01T06:11:16.670' '2021-10-01T06:11:23.640'
-     '2021-10-01T06:11:30.610' '2021-10-01T06:11:37.580'],
-    ...
-    exposure time (0) None: QuantityTableCoordinate ['exposure time'] [None]:
+    ExtraCoords(exposure time (0) None: QuantityTableCoordinate ['exposure time'] [None]:
     <Quantity [0.50031197, 0.50025398, 0.50023699, 0.50024003, 0.50023901,
                0.50028503, 0.50024903, 0.500269  , 0.50026202, 0.500247  ,
                0.50029403, 0.50021601, 0.50028402, 0.50023901, 0.50024903,
                0.50025803, 0.500283  , 0.50029802, 0.50029498, 0.50027299] s>,
+                obs_vrix (0) None: QuantityTableCoordinate ['obs_vrix'] [None]:
+    <Quantity [-253.13569641, -242.44810486, -231.77319336, -221.11309814,
+               -210.41799927, -199.78419495, -189.16329956, -178.50950623,
+               -167.91630554, -157.33630371, -146.72239685, -136.17030334,
+               -125.63009644, -115.05719757, -104.5714035 ,  -94.14320374,
+                -83.69550323,  -73.3214035 ,  -62.97399902,  -52.65399933] m / s>,
+                ophaseix (0) None: QuantityTableCoordinate ['ophaseix'] [None]:
+    <Quantity [0.77429509, 0.77548558, 0.77667391, 0.77786386, 0.77905941,
+               0.78024989, 0.78144038, 0.78263599, 0.78382647, 0.78501666,
+               0.78621155, 0.78740203, 0.78859252, 0.78978807, 0.79097688,
+               0.79216683, 0.79336196, 0.79455239, 0.79574287, 0.79693335] arcsec>,
+                pztx (0) None: QuantityTableCoordinate ['pztx'] [None]:
+    <Quantity [-7.97803831e+00, -3.98715830e+00,  3.72256944e-03,
+                3.99460268e+00, -7.97803831e+00, -3.98715830e+00,
+                3.72256944e-03,  3.99460268e+00, -7.97803831e+00,
+               -3.98715830e+00,  3.72256944e-03,  3.99460268e+00,
+               -7.97803831e+00, -3.98715830e+00,  3.72256944e-03,
+                3.99460268e+00, -7.97803831e+00, -3.98715830e+00,
+                3.72256944e-03,  3.99460268e+00] arcsec>,
+                pzty (0) None: QuantityTableCoordinate ['pzty'] [None]:
+    <Quantity [0.6446346 , 0.66160059, 0.67856681, 0.69553316, 0.6446346 ,
+               0.66160059, 0.67856681, 0.69553316, 0.6446346 , 0.66160059,
+               0.67856681, 0.69553316, 0.6446346 , 0.66160059, 0.67856681,
+               0.69553316, 0.6446346 , 0.66160059, 0.67856681, 0.69553316] arcsec>,
                 slit x position (0) None: QuantityTableCoordinate ['slit x position'] [None]:
     <Quantity [258.75      , 270.74543085, 282.74086427, 294.73629541,
                258.75      , 270.74543085, 282.74086427, 294.73629541,
                258.75      , 270.74543085, 282.74086427, 294.73629541,
                258.75      , 270.74543085, 282.74086427, 294.73629541,
-               258.75      , 270.74543085, 282.74086427, 294.73629541] arcsec pix>,
+               258.75      , 270.74543085, 282.74086427, 294.73629541] arcsec>,
                 slit y position (0) None: QuantityTableCoordinate ['slit y position'] [None]:
     <Quantity [254.75, 254.75, 254.75, 254.75, 254.75, 254.75, 254.75, 254.75,
                254.75, 254.75, 254.75, 254.75, 254.75, 254.75, 254.75, 254.75,
-               254.75, 254.75, 254.75, 254.75] arcsec pix>)
+               254.75, 254.75, 254.75, 254.75] arcsec>,
+                xcenix (0) None: QuantityTableCoordinate ['xcenix'] [None]:
+    <Quantity [-321.64163621, -321.64154081, -321.64054553, -321.63951873,
+               -321.5924215 , -321.59850309, -321.60135777, -321.56819773,
+               -321.55565282, -321.55661478, -321.51550993, -321.5241685 ,
+               -321.4984636 , -321.49132346, -321.47172876, -321.48122647,
+               -321.46051587, -321.41851219, -321.42161527, -321.42543197] arcsec>,
+                ycenix (0) None: QuantityTableCoordinate ['ycenix'] [None]:
+    <Quantity [390.41458808, 390.43178122, 390.44696156, 390.46218927,
+               390.40669468, 390.41598631, 390.42799954, 390.43424635,
+               390.38567211, 390.39919174, 390.41787952, 390.43324879,
+               390.40355692, 390.4319302 , 390.43515948, 390.44981385,
+               390.41605352, 390.43774154, 390.45774336, 390.47763699] arcsec>)
 
-Understanding a Level 2 FITS file
+Understanding a level 2 FITS file
 =================================
 
-The structure of the IRIS Level 2 FITS data file is as follows:
+The structure of the level 2 FITS data file is as follows:
 
-The IRIS Level 2 FITS are multi-extension FITS files.
+The level 2 FITS are multi-extension FITS files.
 An extension" refers to a part of the file containing self-consistent information.
 This information may be, in the general case, a header or its corresponding data.
 The first extension is called ``primary`` and its ``extension number`` is 0.
 
-The extensions in an IRIS Level 2 SJI FITS file has the following numbers:
+The extensions in an level 2 SJI FITS file has the following numbers:
 
    - ``0``: header and data corresponding to the spectral images observed by the SJI.
    - ``1``: header and auxiliary 31 values from each exposure taken by the SJI in the spectral band of the file.
      It is an array of float values with dimensions :math:`no. images \times 31`.
    - ``2``: header and extra data from each exposure taken by the SJI in the spectral band of the file.
      It is a record array containing 5 string fields for each exposure.
      The values of each field can be access as the key in a dictionary or as an attribute.
      See example in the last code block of this section.
 
-An IRIS Level 2 raster FITS file has the following extensions:
+An level 2 raster FITS file has the following extensions:
 
    -  ``0``: main header with the main information of the observation.
       This header has information about all the spectral windows contained in the file and other relevant and
       general information.
       This extension DOES NOT have spectral data associated with the file.
    -  ``1`` to ``N``: header and data for the N spectral windows contained in the file.
    -  ``N+1``: header and auxiliary 47 values from each exposure considered in the file.
       It is an array of float values with dimensions :math:`no. acquisitions \times 47`.
    -  ``N+2``: header and extra information data from each exposure considered in the file.
       It is a record array containing 9 string fields for each exposure. The values of
       each field can be access as the key in a dictionary or as an attribute.
       See example in the last code block of this section.
 
-The function `astropy.fits.io` shows the information of the extensions contained in the IRIS Level 2 file.
+The function `astropy.fits.io` shows the information of the extensions contained in the level 2 file.
 For a SJI file:
 
 .. code-block:: python
 
    >>> from astropy.io import fits   # doctest: +REMOTE_DATA
    >>> fits.info(sample_data.SJI_1330)   # doctest: +REMOTE_DATA
     Filename: ...iris_l2_20211001_060925_3683602040_SJI_1330_t000.fits.gz
@@ -270,17 +282,14 @@
     >>> from irispy.io import fitsinfo  # doctest: +REMOTE_DATA
     >>> fitsinfo(sample_data.SJI_1330)  # doctest: +REMOTE_DATA
     Filename: ...iris_l2_20211001_060925_3683602040_SJI_1330_t000.fits.gz
     No.    Name      Ver    Type      Cards   Dimensions   Format
       0  PRIMARY       1 PrimaryHDU     162   (555, 548, 20)   int16 (rescales to float32)
       1                1 ImageHDU        38   (31, 20)   float64
       2                1 TableHDU        33   20R x 5C   [A10, A10, A4, A66, A63]
-    Observation description:  Very large sparse 16-step raster 15x175 16s   Deep x 0.5 Spatial x 2
-    <BLANKLINE>
-    Extension No. 1 stores data and header of SJI_1330: 1310.00 - 1350.00 AA
 
 .. code-block:: python
 
     >>> fitsinfo("iris_l2_20211001_060925_3683602040_raster_t000_r00000.fits") # doctest: +SKIP
     Filename: iris_l2_20211001_060925_3683602040_raster_t000_r00000.fits
     No.    Name      Ver    Type      Cards   Dimensions   Format
       0  PRIMARY       1 PrimaryHDU     215   ()
@@ -338,15 +347,15 @@
     NAXIS3  =                   16 /
     PCOUNT  =                    0 / No Group Parameters
     GCOUNT  =                    1 / One Data Group
     ...
 
 The same can be done with the data using `astropy.io.fits.getdata`.
 
-As the number of spectral windows in a raster file may vary from an observation to another, a good option to access to the last 2 extensions of the IRIS Level 2 file, is to use a negative index:
+As the number of spectral windows in a raster file may vary from an observation to another, a good option to access to the last 2 extensions of the level 2 file, is to use a negative index:
 
 .. code-block:: python
 
     # The header corresponding to the extra information extension
     >>> fits.getheader("iris_l2_20211001_060925_3683602040_raster_t000_r00000.fits", -1) # doctest: +SKIP
     XTENSION= 'TABLE   '           / ASCII table extension
     BITPIX  =                    8 / 8 bit bytes
@@ -383,8 +392,8 @@
     chararray(['/irisa/data/level1/2021/10/01/H0600/iris20211001_06092534_fuv.fits',
               '/irisa/data/level1/2021/10/01/H0600/iris20211001_06092706_fuv.fits',
               ...
               '/irisa/data/level1/2021/10/01/H0600/iris20211001_06094981_fuv.fits',
               '/irisa/data/level1/2021/10/01/H0600/iris20211001_06095140_fuv.fits'],
               dtype='<U66')
 
-`More information on the Level 2 data can be found in ITN 26. <https://iris.lmsal.com/itn26/iris_level2.html>`__
+`More information on the level 2 data can be found in ITN 26. <https://iris.lmsal.com/itn26/iris_level2.html>`__
```

### Comparing `irispy-lmsal-0.2.0rc3/docs/installation.rst` & `irispy-lmsal-0.2.0rc4/docs/installation.rst`

 * *Files 26% similar despite different names*

```diff
@@ -2,111 +2,104 @@
 
 ************
 Installation
 ************
 
 Release version
 ===============
+
 ``irispy-lmsal`` is part of the wider ecosystem of scientific Python packages for solar physics and therefore a working installation is more about installing the scientific Python ecosystem.
-If you do not currently have a working scientific Python distribution this guide will set you up with the Miniconda, which makes it easy to install and manage your scientific Python packages.
 
-To install the Miniconda Python distribution follow the `instructions <https://docs.conda.io/en/latest/miniconda.html>`__.
-Although Miniconda makes it simple to switch between Python versions, we recommend that new users install the latest Python 3.x version of Miniconda.
+To install the Minifoge Python distribution `download the executable for your Operation System <https://github.com/conda-forge/miniforge#miniforge3>`__.
 
 The reason we choose Miniconda over Anaconda, is mainly due to the size as Anaconda comes with a full install of packages you probably do not need and this way you have more direct control over what has been installed into your Python virtual environment.
-Furthermore, you bypass the need for the conda resolver to sort out your root environment which should make conda faster to use.
 
-Using Miniconda
+Using Miniforge
 ---------------
-To install, launch a system command prompt or the 'Anaconda Prompt' (under Windows).
-First configure conda for to add the `conda-forge channel <https://conda-forge.org/>`__::
 
-    conda config --add channels conda-forge
-    conda config --set channel_priority strict
+To install, launch a system command prompt or the 'Miniforge Prompt' (under Windows).
 
-and now to install ``irispy-lmasl`` within the default conda virtual environment::
+.. note::
 
-    $ conda install irispy-lmsal
+    We strongly recommend using a `conda virtual environment. <https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307>`__
 
-This will install ``irispy-lmsal`` and every package it needs to function.
+Now to install ``irispy-lmasl`` within the default conda virtual environment:
 
-.. note::
-    We strongly recommend using a `Python virtual environment <https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/>`__ or a `conda virtual environment. <https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307>`__
+.. code-block:: console
+
+    $ conda install irispy-lmsal
+
+This will install ``irispy-lmsal``.
 
 Updating
 --------
-You can update to the latest version by running::
+You can update to the latest version by running:
 
-    conda update irispy-lmsal
+.. code-block:: console
+
+    $ conda update irispy-lmsal
 
 .. _dev_install:
 
 Development version
 ===================
+
 This section outlines how to install the development version of ``irispy-lmsal``.
 
 Stable Dependencies Install
 ---------------------------
 
 Create a conda environment
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 The first step is to create a conda environment (let's call it ``irispy-dev``) in which to install the development version of ``irispy-lmsal``.
 This will allow you to keep your root environment clean of development packages.
 From the command line, type:
 
 .. code-block:: console
 
-    conda create -n irispy-dev pip
+    $ conda create -n irispy-dev pip
 
 This creates the ``irispy-dev`` conda environment with just ``pip``.
 Next, you must activate that environment, i.e., switch into it.
 
 .. code-block:: console
 
-    conda activate irispy-dev
+    $ conda activate irispy-dev
 
 Clone ``irispy-lmsal`` repository
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Now we need to clone the `irispy repository`_ from `GitLab`_ into a directory called ``irispy-git``.
-From the directory in which you want ``irispy-git`` to reside, type:
 
-.. code-block:: console
+Now we need to clone the `irispy repository`_ from `GitHub`_ into a directory called ``irispy-git``.
+From the directory in which you want ``irispy-git`` to reside.
+If you want to develop ``irispy-lmsal``, you will want to fork the repository on GitHub and use that URL in the clone step above.
 
-    git clone https://gitlab.com/LMSAL_HUB/iris_hub/irispy-lmsal irispy-git
+.. code-block:: console
 
-If you want to develop ``irispy-lmsal``, we suggest forking the repository on GitLab and using that in the clone step above.
+    $ git clone <personal fork URL> irispy-git
+    $ cd irispy-git
+    $ git remote add upstream git@github.com:LM-SAL/irispy-lmsal.git
 
 Install ``irispy-lmsal``
 ^^^^^^^^^^^^^^^^^^^^^^^^
+
 Finally, we can install the development version.
 
 .. code-block:: console
 
-    cd irispy-git
-    pip install -e ".[dev]"
+    $ cd irispy-git
+    $ pip install -e ".[dev]"
 
-You should now be ready to use ``irispy-lmsal``.
-To check it's installed, open an Python/IPython/Jupyter Notebook session from any directory and try:
+You are now e ready to develop ``irispy-lmsal``.
 
-.. code-block:: python
+Notice we install no dependencies or use ``conda`` to install this.
+The reason for this is that it is simply easier to use ``pip`` to setup development packages.
 
-    import irispy
-
-To make sure you have the latest updates, regularly do
+At times you might need to get the updated changes, to do so:
 
 .. code-block:: console
 
-    git pull origin master
-
-Development dependencies
-------------------------
-We installed the stable versions of many packages.
-If you want to install development versions of any package you can do the following steps:
+    $ git remote update -p
 
-- Git clone the source code of the package into a directory called ``package-name-git``.
-  e.g., ``git clone https://github.com/sunpy/sunraster.git sunraster-git``
-- Change into the directory ``package-name-git``.
-  e.g., ``cd sunraster-git``
-- Install it using ``pip install -e .``.
+From here, you will need to decide if you need to merge changes or rebase changes when you need to contribute the changes back.
 
-.. _irispy repository: https://gitlab.com/LMSAL_HUB/iris_hub/irispy-lmsal/
-.. _GitLab: https://gitlab.com/
+.. _irispy repository: https://github.com/LM-SAL/irispy-lmsal
+.. _GitHub: https://github.com/
```

### Comparing `irispy-lmsal-0.2.0rc3/docs/known_issues.rst` & `irispy-lmsal-0.2.0rc4/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/docs/make.bat` & `irispy-lmsal-0.2.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/examples/mg_ii_dopplergrams.py` & `irispy-lmsal-0.2.0rc4/examples/mg_ii_dopplergrams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,149 @@
 """
 ==================
 Mg II Dopplergrams
 ==================
 
 In this example we are going to produce a Dopplergram for the Mg II k line from a IRIS 400-step raster.
-The Dopplergram is obtained by subtracting the intensities at symmetrical velocity shifts from the line core
-(e.g. ±50 km/s).
-For this kind of analysis we need a consistent wavelength calibration for each step of the raster.
+The Dopplergram is obtained by subtracting the intensities at symmetrical velocity shifts from the line core (e.g. ±50 km/s).
 
-This very large dense raster took more than three hours to complete the 400 scans (30 s exposures), which
-means that the spacecraft's orbital velocity changes during the observations.
+This very large dense raster took more than three hours to complete the 400 scans (30 s exposures), which means that the spacecraft's orbital velocity changes during the observations.
 This means that any precise wavelength calibration will need to correct for those shifts.
 """
-# sphinx_gallery_thumbnail_number = 5
+import tarfile
 
 import astropy.units as u
 import matplotlib.pyplot as plt
 import numpy as np
+import pooch
 from astropy.coordinates import SpectralCoord
 from astropy.io import fits
 from scipy.constants import c
 from scipy.interpolate import interp1d
 
 from irispy.io import read_files
 from irispy.utils import image_clipping
-from irispy.utils.utils import _download_data
 
 ###############################################################################
 # We start with getting the data. This is done by downloading the data from the IRIS archive.
 #
-# In this case, we will use requests as to keep this example self contained
+# In this case, we will use ``pooch`` as to keep this example self contained
 # but using your browser will also work.
 #
 # Using the url: http://www.lmsal.com/solarsoft/irisa/data/level2_compressed/2014/07/08/
 # we are after `iris_l2_20140708_114109_3824262996_raster.tar.gz` which is ~730 MB in size.
 
-
-urls = [
-    "http://www.lmsal.com/solarsoft/irisa/data/level2_compressed/2014/07/08/20140708_114109_3824262996/iris_l2_20140708_114109_3824262996_raster.tar.gz"
-]
-_download_data(urls)
-raster_filename = "iris_l2_20140708_114109_3824262996_raster_t000_r00000.fits"
+downloaded_tar_iris_file = pooch.retrieve(
+    "http://www.lmsal.com/solarsoft/irisa/data/level2_compressed/2014/07/08/20140708_114109_3824262996/iris_l2_20140708_114109_3824262996_raster.tar.gz",
+    known_hash=None,
+)
 
 ###############################################################################
-# We will open file using `irispy`.
+# Now to open the file using ``irispy-lmsal``.
 # Note that when ``memmap=True``, the data values are read from the FITS file
 # directly without the scaling to Float32, the data values are no longer in DN,
-# but in scaled integer units that start at −2$^{16}$/2.
+# but in scaled integer units that start at -2$^{16}$/2.
 
-raster = read_files(raster_filename, memmap=True, uncertainty=False)
-print(raster)
+raster = read_files(downloaded_tar_iris_file, memmap=True, uncertainty=False)
 
 ###############################################################################
-# We see that Mg II k 2796 is the last key.
-# We will plot the spatially averaged spectrum
+# We are after the Mg II k window, which we can select using a key.
 
 mg_ii = raster["Mg II k 2796"][0]
 (mg_wave,) = mg_ii.axis_world_coords("wl")
 
+# We will plot the spatially averaged spectrum
 plt.plot(mg_wave.to("nm"), mg_ii.data.mean((0, 1)))
+plt.ylabel("DN (Memory Mapped Value)")
+plt.xlabel("Wavelength (nm)")
 
 plt.show()
 
 ###############################################################################
 # To better understand the orbital velocity problem let us look at how the
 # line intensity varies for a strong Mn I line at around 280.2 nm, in
 # between the Mg II k and h lines. For this dataset, the line core of this
-# line falls around index 350. To plot a spectroheliogram in the correct
-# orientation we will transpose the data
+# line falls around index 350. To plot a spectrogram in the correct
+# orientation we will transpose the data.
 
 lower_corner = [SpectralCoord(280.2, unit=u.nm), None]
 upper_corner = [SpectralCoord(280.2, unit=u.nm), None]
 mg_crop = mg_ii.crop(lower_corner, upper_corner)
 
-plt.figure(figsize=(6, 10))
 vmin, vmax = image_clipping(mg_ii.data[..., 350])
-ax = mg_crop.plot(vmin=vmin, vmax=vmax + 1000)
+plt.figure(figsize=(6, 10))
+plt.imshow(
+    mg_ii.data[..., 350].T,
+    origin="lower",
+    aspect=0.5,
+    vmin=vmin,
+    vmax=vmax,
+)
+plt.xlabel("Solar X (arcsec)")
+plt.ylabel("Solar Y (arcsec)")
 
 plt.show()
 
 ###############################################################################
-# You can see a regular bright-dark pattern along the x axis, an
+# You can see a regular bright-dark pattern along the Y axis, an
 # indication that its intensities are not taken at the same position in
 # the line because of wavelength shifts. The shifts are caused by the
 # orbital velocity changes, and we can find these in the auxiliary
 # metadata which are to be found in the extension past the "last" window
-# in the data set
+# in the FITS file.
 
-aux = fits.getdata(raster_filename, 9)
-aux_hd = fits.getheader(raster_filename, 9)
-v_obs = aux[:, aux_hd["OBS_VRIX"]]
-v_obs /= 1000.0  # convert to km/s
+# astropy.io.fits does not support opening tar files, so we need to extract.
+tar_iris_file = tarfile.open(downloaded_tar_iris_file, "r:gz")
+tar_iris_file.extractall("./")
+tar_iris_file.close()
+raster_filename = "iris_l2_20140708_114109_3824262996_raster_t000_r00000.fits"
 
+# In this case, it is the 9th HDU, which we access directly
+aux_data = fits.getdata(raster_filename, 9)
+aux_header = fits.getheader(raster_filename, 9)
+v_obs = aux_data[:, aux_header["OBS_VRIX"]]
+# Convert to km/s
+v_obs /= 1000.0
+
+plt.figure()
 plt.plot(v_obs)
 plt.ylabel("Orbital velocity (km/s)")
 plt.xlabel("Scan number")
 
 plt.show()
 
 ###############################################################################
 # To look at intensities at any given scan we only need to subtract this
 # velocity shift from the wavelength scale, but to look at the whole image
 # at a given wavelength we must interpolate the original data to take this
 # shift into account. Here is a way to do it (note that array dimensions
-# apply to this specific set only!)
+# apply to this specific example).
 
 c_kms = c / 1000.0
 wave_shift = -v_obs * mg_wave[350] / (c_kms)
 # Linear interpolation in wavelength, for each scan
 for i in range(mg_ii.data.shape[0]):
-    tmp = interp1d(mg_wave - wave_shift[i], mg_ii.data[:, i, :], bounds_error=False)
-    mg_ii.data[:, i, :] = tmp(mg_wave)
+    method = interp1d(mg_wave - wave_shift[i], mg_ii.data[:, i, :], bounds_error=False)
+    mg_ii.data[:, i, :] = method(mg_wave)
 
 ###############################################################################
 # Now we can plot the shifted data to see that the large scale shifts
 # have disappeared
 
-plt.figure(figsize=(6, 10))
 vmin, vmax = image_clipping(mg_ii.data[..., 350])
+plt.figure(figsize=(6, 10))
 plt.imshow(
     mg_ii.data[..., 350].T,
     origin="lower",
     aspect=0.5,
     vmin=vmin,
     vmax=vmax,
 )
+plt.xlabel("Solar X (arcsec)")
+plt.ylabel("Solar Y (arcsec)")
 
 plt.show()
 
 ###############################################################################
 # Some residual shift remains, but we will not correct for it here. A more
 # elaborate correction can be obtained by the IDL routine
 # ``iris_prep_wavecorr_l2``, but this has not yet been ported to Python
@@ -151,19 +166,21 @@
 index_m = np.argmin(np.abs(velocity + pos))
 doppl = mg_ii.data[..., index_m] - mg_ii.data[..., index_p]
 
 ###############################################################################
 # And now we can plot this as before (intensity units are again arbitrary
 # because of the unscaled DNs):
 
-fig = plt.figure(figsize=(6, 10))
 vmin, vmax = image_clipping(doppl)
+plt.figure(figsize=(6, 10))
 plt.imshow(
     doppl.T,
     cmap="gist_gray",
     origin="lower",
     aspect=0.5,
     vmin=vmin,
     vmax=vmax,
 )
+plt.xlabel("Solar X (arcsec)")
+plt.ylabel("Solar Y (arcsec)")
 
 plt.show()
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sg_psfs.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sg_psfs.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_20130211.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_20130211.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_20130715.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_20130715.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20150331.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20150331.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20161022.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20161022.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20191101.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20191101.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/iris_sra_c_20200223.geny` & `irispy-lmsal-0.2.0rc4/irispy/data/iris_sra_c_20200223.geny`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/__init__.py` & `irispy-lmsal-0.2.0rc4/irispy/data/test/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 IRISPy test data files.
 """
-import os
 import glob
+from pathlib import Path
 
 from astropy.utils.data import get_pkg_data_filename
 
 import irispy
 
 __all__ = ["rootdir", "file_list", "get_test_filepath"]
 
-rootdir = os.path.join(os.path.dirname(irispy.__file__), "data", "test")
+rootdir = Path(irispy.__file__).parent / "data" / "test"
+file_list = glob.glob(str(Path(rootdir) / "*.[!p]*"))
 
 
 def get_test_filepath(filename, **kwargs):
     """
     Return the full path to a test file in the ``data/test`` directory.
 
     Parameters
@@ -35,10 +36,7 @@
     Notes
     -----
 
     This is a wrapper around `astropy.utils.data.get_pkg_data_filename` which
     sets the ``package`` kwarg to be 'irispy.data.test`.
     """
     return get_pkg_data_filename(filename, package="irispy.data.test", **kwargs)
-
-
-file_list = glob.glob(os.path.join(rootdir, "*.[!p]*"))
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version001.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version001.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version002.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version002.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version003.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version003.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version004.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version004.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version005.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version005.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/idl_iris_get_response_20130903_new_version006.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/idl_iris_get_response_20130903_new_version006.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/test/test_response.sav` & `irispy-lmsal-0.2.0rc4/irispy/data/test/test_response.sav`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v36-table10.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v34-table10.csv`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v36-table2000.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v34-table2000.csv`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Spaceholder,OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
-,0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
-,100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
-,200,C II   Si IV   Mg II w s   ,1,1,0.541666667
-,300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,500,C II   Mg II w s   ,1,1,0.291666667
-,600,Si IV   Mg II w s   ,1,1,0.291666667
-,700,Mg II h/k   Mg II w s   ,1,1,0.291666667
-,800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
-,900,C II   Mg II h/k   Mg II w   ,1,1,0.75
-,1000,C II   Si IV   Mg II w   ,1,1,0.75
-,1100,C II   Si IV   Mg II h/k   ,1,1,0.75
-,1200,C II   Si IV   ,1,1,0.5
-,1300,C II   Mg II h/k   ,1,1,0.5
-,1400,Si IV   Mg II h/k   ,1,1,0.5
-,1500,C II   ,1,1,0.25
-,1600,Si IV   ,1,1,0.25
-,1700,Mg II h/k   ,1,1,0.25
-,1800,Mg II w   ,1,1,0.25
-,1900,Mg II h/k   Mg II w   ,1,1,0.5
-,0,Exposure 1s,1,1,1
-,2000,Deep x 0.5,0.5,2,1
-,4000,Deep x 2,2,0.5,1
-,6000,Deep x 4,4,0.25,1
-,8000,Deep x 8,8,0.125,1
-,10000,Deep x 15,15,0.066666667,1
-,12000,Deep x 30,30,0.033333333,1
-,14000,Deep x 60,60,0.016666667,1
-,0,"Spatial x 1, Spectral x 1",1,1,1
-,20000,"Spatial x 1, Spectral x 2",1,0.5,1
-,40000,"Spatial x 1, Spectral x 4",1,0.25,1
-,60000,"Spatial x 1, Spectral x 8",1,0.125,1
-,80000,"Spatial x 2, Spectral x 1",1,0.5,1
-,100000,"Spatial x 2, Spectral x 2",1,0.25,1
-,120000,"Spatial x 2, Spectral x 4",1,0.125,1
-,140000,"Spatial x 2, Spectral x 8",1,0.0625,1
-,160000,"Spatial x 4, Spectral x 1",1,0.25,1
-,180000,"Spatial x 4, Spectral x 2",1,0.125,1
-,200000,"Spatial x 4, Spectral x 4",1,0.0625,1
-,220000,"Spatial x 4, Spectral x 8",1,0.03125,1
-,0,FUV binned same as NUV,1,1,1
-,250000,FUV spectrally rebinned x 2,1,0.5,1
-,500000,FUV spectrally rebinned x 4,1,0.25,1
-,0,SJI cadence default,1,1,1
-,1000000,SJI cadence 0.25x faster,1,1,0.25
-,2000000,SJI cadence 0.5x faster,1,1,0.5
-,3000000,SJI cadence 3x faster,1,1,2
-,4000000,SJI cadence 10x faster,1,1,10
-,0,Non-simultaneous readout,1,1,1
-,5000000,Simultaneous readout,1,1,1
-,0,Default compression,1,1,1
-,10000000,Lossless compression,1,1.5,1.5
-,0,Large linelist,1,1,1
-,20000000,Medium linelist,1,1,1
-,40000000,Small linelist,1,1,1
-,60000000,Flare linelist 1,1,1,1
-,80000000,Full readout,3,1.497619048,1
+OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
+0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
+100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
+200,C II   Si IV   Mg II w s   ,1,1,0.541666667
+300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
+400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
+500,C II   Mg II w s   ,1,1,0.291666667
+600,Si IV   Mg II w s   ,1,1,0.291666667
+700,Mg II h/k   Mg II w s   ,1,1,0.291666667
+800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
+900,C II   Mg II h/k   Mg II w   ,1,1,0.75
+1000,C II   Si IV   Mg II w   ,1,1,0.75
+1100,C II   Si IV   Mg II h/k   ,1,1,0.75
+1200,C II   Si IV   ,1,1,0.5
+1300,C II   Mg II h/k   ,1,1,0.5
+1400,Si IV   Mg II h/k   ,1,1,0.5
+1500,C II   ,1,1,0.25
+1600,Si IV   ,1,1,0.25
+1700,Mg II h/k   ,1,1,0.25
+1800,Mg II w   ,1,1,0.25
+1900,Mg II h/k   Mg II w   ,1,1,0.5
+0,Exposure 1s,1,1,1
+2000,Deep x 0.5,0.5,2,1
+4000,Deep x 2,2,0.5,1
+6000,Deep x 4,4,0.25,1
+8000,Deep x 8,8,0.125,1
+10000,Deep x 15,15,0.066666667,1
+12000,Deep x 30,30,0.033333333,1
+14000,Deep x 60,60,0.016666667,1
+0,"Spatial x 1, Spectral x 1",1,1,1
+20000,"Spatial x 1, Spectral x 2",1,0.5,1
+40000,"Spatial x 1, Spectral x 4",1,0.25,1
+60000,"Spatial x 1, Spectral x 8",1,0.125,1
+80000,"Spatial x 2, Spectral x 1",1,0.5,1
+100000,"Spatial x 2, Spectral x 2",1,0.25,1
+120000,"Spatial x 2, Spectral x 4",1,0.125,1
+140000,"Spatial x 2, Spectral x 8",1,0.0625,1
+160000,"Spatial x 4, Spectral x 1",1,0.25,1
+180000,"Spatial x 4, Spectral x 2",1,0.125,1
+200000,"Spatial x 4, Spectral x 4",1,0.0625,1
+220000,"Spatial x 4, Spectral x 8",1,0.03125,1
+0,FUV binned same as NUV,1,1,1
+250000,FUV spectrally rebinned x 2,1,0.5,1
+500000,FUV spectrally rebinned x 4,1,0.25,1
+0,SJI cadence default,1,1,1
+1000000,SJI cadence 0.25x faster,1,1,0.25
+2000000,SJI cadence 0.5x faster,1,1,0.5
+3000000,SJI cadence 3x faster,1,1,2
+4000000,SJI cadence 10x faster,1,1,10
+0,Non-simultaneous readout,1,1,1
+5000000,Simultaneous readout,1,1,1
+0,Default compression,1,1,1
+10000000,Lossless compression,1,1.5,1.5
+0,Large linelist,1,1,1
+20000000,Medium linelist,1,1,1
+40000000,Small linelist,1,1,1
+60000000,Flare linelist 1,1,1,1
+80000000,Full readout,3,1.497619048,1
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v38-table10.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v38-table10.csv`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v38-table2000.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v36-table2000.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-,OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
-,0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
-,100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
-,200,C II   Si IV   Mg II w s   ,1,1,0.541666667
-,300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,500,C II   Mg II w s   ,1,1,0.291666667
-,600,Si IV   Mg II w s   ,1,1,0.291666667
-,700,Mg II h/k   Mg II w s   ,1,1,0.291666667
-,800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
-,900,C II   Mg II h/k   Mg II w   ,1,1,0.75
-,1000,C II   Si IV   Mg II w   ,1,1,0.75
-,1100,C II   Si IV   Mg II h/k   ,1,1,0.75
-,1200,C II   Si IV   ,1,1,0.5
-,1300,C II   Mg II h/k   ,1,1,0.5
-,1400,Si IV   Mg II h/k   ,1,1,0.5
-,1500,C II   ,1,1,0.25
-,1600,Si IV   ,1,1,0.25
-,1700,Mg II h/k   ,1,1,0.25
-,1800,Mg II w   ,1,1,0.25
-,1900,Mg II h/k   Mg II w   ,1,1,0.5
-,0,Exposure 1s,1,1,1
-,2000,Deep x 0.5,0.5,2,1
-,4000,Deep x 2,2,0.5,1
-,6000,Deep x 4,4,0.25,1
-,8000,Deep x 8,8,0.125,1
-,10000,Deep x 15,15,0.066666667,1
-,12000,Deep x 30,30,0.033333333,1
-,0,"Spatial x 1, Spectral x 1",1,1,1
-,20000,"Spatial x 1, Spectral x 2",1,0.5,1
-,40000,"Spatial x 1, Spectral x 4",1,0.25,1
-,60000,"Spatial x 1, Spectral x 8",1,0.125,1
-,80000,"Spatial x 2, Spectral x 1",1,0.5,1
-,100000,"Spatial x 2, Spectral x 2",1,0.25,1
-,120000,"Spatial x 2, Spectral x 4",1,0.125,1
-,140000,"Spatial x 2, Spectral x 8",1,0.0625,1
-,160000,"Spatial x 4, Spectral x 1",1,0.25,1
-,180000,"Spatial x 4, Spectral x 2",1,0.125,1
-,200000,"Spatial x 4, Spectral x 4",1,0.0625,1
-,220000,"Spatial x 4, Spectral x 8",1,0.03125,1
-,0,FUV binned same as NUV,1,1,1
-,250000,FUV spectrally rebinned x 2,1,0.5,1
-,500000,FUV spectrally rebinned x 4,1,0.25,1
-,750000,FUV spectrally rebinned x 8,1,0.125,1
-,0,SJI cadence default,1,1,1
-,1000000,SJI cadence 0.25x faster,1,1,0.25
-,2000000,SJI cadence 0.5x faster,1,1,0.5
-,3000000,SJI cadence 3x faster,1,1,2
-,4000000,SJI cadence 10x faster,1,1,10
-,0,Default compression,1,1,1
-,10000000,Lossless compression,1,1.5,1.5
-,0,Large linelist,1,1,1
-,20000000,Medium linelist,1,1,1
-,40000000,Small linelist,1,1,1
-,60000000,Flare linelist 1,1,1,1
-,80000000,Full readout,3,1.497619048,1
+OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
+0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
+100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
+200,C II   Si IV   Mg II w s   ,1,1,0.541666667
+300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
+400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
+500,C II   Mg II w s   ,1,1,0.291666667
+600,Si IV   Mg II w s   ,1,1,0.291666667
+700,Mg II h/k   Mg II w s   ,1,1,0.291666667
+800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
+900,C II   Mg II h/k   Mg II w   ,1,1,0.75
+1000,C II   Si IV   Mg II w   ,1,1,0.75
+1100,C II   Si IV   Mg II h/k   ,1,1,0.75
+1200,C II   Si IV   ,1,1,0.5
+1300,C II   Mg II h/k   ,1,1,0.5
+1400,Si IV   Mg II h/k   ,1,1,0.5
+1500,C II   ,1,1,0.25
+1600,Si IV   ,1,1,0.25
+1700,Mg II h/k   ,1,1,0.25
+1800,Mg II w   ,1,1,0.25
+1900,Mg II h/k   Mg II w   ,1,1,0.5
+0,Exposure 1s,1,1,1
+2000,Deep x 0.5,0.5,2,1
+4000,Deep x 2,2,0.5,1
+6000,Deep x 4,4,0.25,1
+8000,Deep x 8,8,0.125,1
+10000,Deep x 15,15,0.066666667,1
+12000,Deep x 30,30,0.033333333,1
+14000,Deep x 60,60,0.016666667,1
+0,"Spatial x 1, Spectral x 1",1,1,1
+20000,"Spatial x 1, Spectral x 2",1,0.5,1
+40000,"Spatial x 1, Spectral x 4",1,0.25,1
+60000,"Spatial x 1, Spectral x 8",1,0.125,1
+80000,"Spatial x 2, Spectral x 1",1,0.5,1
+100000,"Spatial x 2, Spectral x 2",1,0.25,1
+120000,"Spatial x 2, Spectral x 4",1,0.125,1
+140000,"Spatial x 2, Spectral x 8",1,0.0625,1
+160000,"Spatial x 4, Spectral x 1",1,0.25,1
+180000,"Spatial x 4, Spectral x 2",1,0.125,1
+200000,"Spatial x 4, Spectral x 4",1,0.0625,1
+220000,"Spatial x 4, Spectral x 8",1,0.03125,1
+0,FUV binned same as NUV,1,1,1
+250000,FUV spectrally rebinned x 2,1,0.5,1
+500000,FUV spectrally rebinned x 4,1,0.25,1
+0,SJI cadence default,1,1,1
+1000000,SJI cadence 0.25x faster,1,1,0.25
+2000000,SJI cadence 0.5x faster,1,1,0.5
+3000000,SJI cadence 3x faster,1,1,2
+4000000,SJI cadence 10x faster,1,1,10
+0,Non-simultaneous readout,1,1,1
+5000000,Simultaneous readout,1,1,1
+0,Default compression,1,1,1
+10000000,Lossless compression,1,1.5,1.5
+0,Large linelist,1,1,1
+20000000,Medium linelist,1,1,1
+40000000,Small linelist,1,1,1
+60000000,Flare linelist 1,1,1,1
+80000000,Full readout,3,1.497619048,1
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v40-table10.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v40-table10.csv`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/data/v40-table2000.csv` & `irispy-lmsal-0.2.0rc4/irispy/data/v40-table2000.csv`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-,OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
-,0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
-,100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
-,200,C II   Si IV   Mg II w s   ,1,1,0.541666667
-,300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
-,500,C II   Mg II w s   ,1,1,0.291666667
-,600,Si IV   Mg II w s   ,1,1,0.291666667
-,700,Mg II h/k   Mg II w s   ,1,1,0.291666667
-,800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
-,900,C II   Mg II h/k   Mg II w   ,1,1,0.75
-,1000,C II   Si IV   Mg II w   ,1,1,0.75
-,1100,C II   Si IV   Mg II h/k   ,1,1,0.75
-,1200,C II   Si IV   ,1,1,0.5
-,1300,C II   Mg II h/k   ,1,1,0.5
-,1400,Si IV   Mg II h/k   ,1,1,0.5
-,1500,C II   ,1,1,0.25
-,1600,Si IV   ,1,1,0.25
-,1700,Mg II h/k   ,1,1,0.25
-,1800,Mg II w   ,1,1,0.25
-,1900,Mg II h/k   Mg II w   ,1,1,0.5
-,0,Exposure 1s,1,1,1
-,2000,Deep x 0.5,0.5,2,1
-,4000,Deep x 2,2,0.5,1
-,6000,Deep x 4,4,0.25,1
-,8000,Deep x 8,8,0.125,1
-,10000,Deep x 15,15,0.066666667,1
-,12000,Deep x 30,30,0.033333333,1
-,0,"Spatial x 1, Spectral x 1",1,1,1
-,20000,"Spatial x 1, Spectral x 2",1,0.5,1
-,40000,"Spatial x 1, Spectral x 4",1,0.25,1
-,60000,"Spatial x 1, Spectral x 8",1,0.125,1
-,80000,"Spatial x 2, Spectral x 1",1,0.5,1
-,100000,"Spatial x 2, Spectral x 2",1,0.25,1
-,120000,"Spatial x 2, Spectral x 4",1,0.125,1
-,140000,"Spatial x 2, Spectral x 8",1,0.0625,1
-,160000,"Spatial x 4, Spectral x 1",1,0.25,1
-,180000,"Spatial x 4, Spectral x 2",1,0.125,1
-,200000,"Spatial x 4, Spectral x 4",1,0.0625,1
-,220000,"Spatial x 4, Spectral x 8",1,0.03125,1
-,0,FUV binned same as NUV,1,1,1
-,250000,FUV spectrally rebinned x 2,1,0.5,1
-,500000,FUV spectrally rebinned x 4,1,0.25,1
-,750000,FUV spectrally rebinned x 8,1,0.125,1
-,0,SJI cadence 10s,1,1,1
-,1000000,SJI cadence 0.25x faster,1,1,0.25
-,2000000,SJI cadence 0.5x faster,1,1,0.5
-,3000000,SJI cadence 3x faster,1,1,2
-,4000000,SJI cadence 10x faster,1,1,10
-,8000000,AEC enabled,1,1.5,1.5
-,9000000,Flatfield and calibration,1,1,1
-,0,Lossy compression,1,1,1
-,10000000,Lossless compression,1,1.5,1.5
-,0,Large linelist,1,1,1
-,40000000,Small linelist,1,1,1
-,180000000,Full readout,1,1,1
+OBS ID,Size + description,Impact on cadence (>1 = slower),Impact on SG datarate,Impact on SJI datarate
+0,C II   Si IV   Mg II h/k   Mg II w   ,1,1,1
+100,C II   Si IV   Mg II h/k   Mg II w s   ,1,1,0.791666667
+200,C II   Si IV   Mg II w s   ,1,1,0.541666667
+300,C II   Mg II h/k   Mg II w s   ,1,1,0.541666667
+400,Si IV   Mg II h/k   Mg II w s   ,1,1,0.541666667
+500,C II   Mg II w s   ,1,1,0.291666667
+600,Si IV   Mg II w s   ,1,1,0.291666667
+700,Mg II h/k   Mg II w s   ,1,1,0.291666667
+800,Si IV   Mg II h/k   Mg II w   ,1,1,0.75
+900,C II   Mg II h/k   Mg II w   ,1,1,0.75
+1000,C II   Si IV   Mg II w   ,1,1,0.75
+1100,C II   Si IV   Mg II h/k   ,1,1,0.75
+1200,C II   Si IV   ,1,1,0.5
+1300,C II   Mg II h/k   ,1,1,0.5
+1400,Si IV   Mg II h/k   ,1,1,0.5
+1500,C II   ,1,1,0.25
+1600,Si IV   ,1,1,0.25
+1700,Mg II h/k   ,1,1,0.25
+1800,Mg II w   ,1,1,0.25
+1900,Mg II h/k   Mg II w   ,1,1,0.5
+0,Exposure 1s,1,1,1
+2000,Deep x 0.5,0.5,2,1
+4000,Deep x 2,2,0.5,1
+6000,Deep x 4,4,0.25,1
+8000,Deep x 8,8,0.125,1
+10000,Deep x 15,15,0.066666667,1
+12000,Deep x 30,30,0.033333333,1
+0,"Spatial x 1, Spectral x 1",1,1,1
+20000,"Spatial x 1, Spectral x 2",1,0.5,1
+40000,"Spatial x 1, Spectral x 4",1,0.25,1
+60000,"Spatial x 1, Spectral x 8",1,0.125,1
+80000,"Spatial x 2, Spectral x 1",1,0.5,1
+100000,"Spatial x 2, Spectral x 2",1,0.25,1
+120000,"Spatial x 2, Spectral x 4",1,0.125,1
+140000,"Spatial x 2, Spectral x 8",1,0.0625,1
+160000,"Spatial x 4, Spectral x 1",1,0.25,1
+180000,"Spatial x 4, Spectral x 2",1,0.125,1
+200000,"Spatial x 4, Spectral x 4",1,0.0625,1
+220000,"Spatial x 4, Spectral x 8",1,0.03125,1
+0,FUV binned same as NUV,1,1,1
+250000,FUV spectrally rebinned x 2,1,0.5,1
+500000,FUV spectrally rebinned x 4,1,0.25,1
+750000,FUV spectrally rebinned x 8,1,0.125,1
+0,SJI cadence 10s,1,1,1
+1000000,SJI cadence 0.25x faster,1,1,0.25
+2000000,SJI cadence 0.5x faster,1,1,0.5
+3000000,SJI cadence 3x faster,1,1,2
+4000000,SJI cadence 10x faster,1,1,10
+8000000,AEC enabled,1,1.5,1.5
+9000000,Flatfield and calibration,1,1,1
+0,Lossy compression,1,1,1
+10000000,Lossless compression,1,1.5,1.5
+0,Large linelist,1,1,1
+40000000,Small linelist,1,1,1
+180000000,Full readout,1,1,1
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/io/sji.py` & `irispy-lmsal-0.2.0rc4/irispy/io/sji.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,130 +1,179 @@
 from copy import copy
 
+import astropy.modeling.models as m
 import astropy.units as u
+import gwcs
+import gwcs.coordinate_frames as cf
 import numpy as np
 from astropy.io import fits
-from astropy.time import Time, TimeDelta
+from astropy.time import Time
 from astropy.wcs import WCS
+from dkist.wcs.models import CoupledCompoundModel, VaryingCelestialTransform
+from sunpy.coordinates.ephemeris import get_body_heliographic_stonyhurst
+from sunpy.coordinates.frames import Helioprojective
 
-from irispy.sji import IRISMapCube, IRISMapCubeSequence
+from irispy.sji import SJICube
 from irispy.utils import calculate_uncertainty
 from irispy.utils.constants import BAD_PIXEL_VALUE_SCALED, BAD_PIXEL_VALUE_UNSCALED, DN_UNIT, READOUT_NOISE
 
 __all__ = ["read_sji_lvl2"]
 
 
-def read_sji_lvl2(filename, uncertainty=False, memmap=False):
+def _create_gwcs(hdulist: fits.HDUList) -> gwcs.WCS:
     """
-    Read level 2 SJI FITS into an IRISMapCube instance.
+    Creates the GWCS object for the SJI file.
+
+    Parameters
+    ----------
+    hdulist : `astropy.io.fits.HDUList`
+        The HDU list of the SJI file.
+
+    Returns
+    -------
+    `gwcs.WCS`
+        GWCS object for the SJI file.
+    """
+    pc_table = hdulist[1].data[:, hdulist[1].header["PC1_1IX"] : hdulist[1].header["PC2_2IX"] + 1].reshape(-1, 2, 2)
+    crval_table = hdulist[1].data[:, hdulist[1].header["XCENIX"] : hdulist[1].header["YCENIX"] + 1]
+    crpix = [hdulist[0].header["CRPIX1"], hdulist[0].header["CRPIX2"]]
+    cdelt = [hdulist[0].header["CDELT1"], hdulist[0].header["CDELT2"]]
+    celestial = VaryingCelestialTransform(
+        crpix=crpix * u.pixel,
+        cdelt=cdelt * u.arcsec / u.pixel,
+        pc_table=pc_table * u.arcsec,
+        crval_table=crval_table * u.arcsec,
+    )
+    base_time = Time(hdulist[0].header["STARTOBS"], format="isot", scale="utc")
+    times = hdulist[1].data[:, hdulist[1].header["TIME"]] * u.s
+    # We need to account for a non-zero time delta.
+    base_time += times[0]
+    times -= times[0]
+    temporal = m.Tabular1D(
+        np.arange(hdulist[1].data.shape[0]) * u.pix,
+        lookup_table=times,
+        fill_value=np.nan,
+        bounds_error=False,
+        method="linear",
+    )
+    forward_transform = CoupledCompoundModel("&", left=celestial, right=temporal)
+    celestial_frame = cf.CelestialFrame(
+        axes_order=(0, 1),
+        unit=(u.arcsec, u.arcsec),
+        reference_frame=Helioprojective(observer="earth", obstime=base_time),
+        axis_physical_types=["custom:pos.helioprojective.lon", "custom:pos.helioprojective.lat"],
+        axes_names=("Longitude", "Latitude"),
+    )
+    temporal_frame = cf.TemporalFrame(Time(base_time), unit=(u.s,), axes_order=(2,), axes_names=("Time (UTC)",))
+    output_frame = cf.CompositeFrame([celestial_frame, temporal_frame])
+    input_frame = cf.CoordinateFrame(
+        axes_order=(0, 1, 2),
+        naxes=3,
+        axes_type=["PIXEL", "PIXEL", "PIXEL"],
+        unit=(u.pix, u.pix, u.pix),
+    )
+    return gwcs.WCS(forward_transform, input_frame=input_frame, output_frame=output_frame)
+
+
+def _create_wcs(hdulist):
+    """
+    This is required as occasionally we need a normal WCS instead of a gWCS due
+    to compatibility issues.
+
+    This has been set to have an Earth Observer at the time of the
+    observation.
+    """
+    wcses = []
+    base_time = Time(hdulist[0].header["STARTOBS"], format="isot", scale="utc")
+    times = hdulist[1].data[:, hdulist[1].header["TIME"]] * u.s
+    # We need to account for a non-zero time delta.
+    base_time += times[0]
+    times -= times[0]
+    for i in range(hdulist[0].header["NAXIS3"]):
+        header = copy(hdulist[0].header)
+        header.pop("NAXIS3")
+        header.pop("PC3_1")
+        header.pop("PC3_2")
+        header.pop("CTYPE3")
+        header.pop("CUNIT3")
+        header.pop("CRVAL3")
+        header.pop("CRPIX3")
+        header.pop("CDELT3")
+        header["NAXIS"] = 2
+        header["CRVAL1"] = hdulist[1].data[i, hdulist[1].header["XCENIX"]]
+        header["CRVAL2"] = hdulist[1].data[i, hdulist[1].header["YCENIX"]]
+        header["PC1_1"] = hdulist[1].data[0, hdulist[1].header["PC1_1IX"]]
+        header["PC1_2"] = hdulist[1].data[0, hdulist[1].header["PC1_2IX"]]
+        header["PC2_1"] = hdulist[1].data[0, hdulist[1].header["PC2_1IX"]]
+        header["PC2_2"] = hdulist[1].data[0, hdulist[1].header["PC2_2IX"]]
+        header["DATE_OBS"] = (base_time + times[i]).isot
+        location = get_body_heliographic_stonyhurst("Earth", header["DATE_OBS"])
+        header["HGLN_OBS"] = location.lon.value
+        header["HGLT_OBS"] = location.lat.value
+        wcses.append(WCS(header))
+    return wcses
+
+
+def read_sji_lvl2(filename, *, uncertainty=False, memmap=False):
+    """
+    Reads a level 2 SJI FITS.
 
     Parameters
     ----------
     filename: `str`
         Filename to read.
     uncertainty : `bool`, optional
         If `True` (not the default), will compute the uncertainty for the data (slower and
-        uses more memory). If `memmap=True`, the uncertainty is never computed.
+        uses more memory). If ``memmap=True``, the uncertainty is never computed.
     memmap : `bool`, optional
         If `True` (not the default), will not load arrays into memory, and will only read from
         the file into memory when needed. This option is faster and uses a
         lot less memory. However, because FITS scaling is not done on-the-fly,
         the data units will be unscaled, not the usual data numbers (DN).
 
     Returns
     -------
-    `irispy.sji.IRISMapCubeSequence`
+    `irispy.sji.SJICube`
+        The data cube, using a gWCS.
     """
-    list_of_cubes = []
     with fits.open(filename, memmap=memmap, do_not_scale_image_data=memmap) as hdulist:
         hdulist.verify("silentfix")
-        startobs = hdulist[0].header.get("STARTOBS")
-        startobs = Time(startobs) if startobs else None
-        endobs = hdulist[0].header.get("ENDOBS")
-        endobs = Time(endobs) if endobs else None
-        meta = {
-            "TWAVE1": hdulist[0].header.get("TWAVE1"),
-            "TELESCOP": hdulist[0].header.get("TELESCOP"),
-            "INSTRUME": hdulist[0].header.get("INSTRUME"),
-            "DATA_LEV": hdulist[0].header.get("DATA_LEV"),
-            "OBSID": hdulist[0].header.get("OBSID"),
-            "STARTOBS": startobs,
-            "ENDOBS": endobs,
-            "SAT_ROT": hdulist[0].header["SAT_ROT"] * u.deg,
-            "NBFRAMES": hdulist[0].data.shape[0],
-            "OBS_DESC": hdulist[0].header.get("OBS_DESC"),
-            "FOVX": hdulist[0].header["FOVX"] * u.arcsec,
-            "FOVY": hdulist[0].header["FOVY"] * u.arcsec,
-            "XCEN": hdulist[0].header["XCEN"] * u.arcsec,
-            "YCEN": hdulist[0].header["YCEN"] * u.arcsec,
-        }
-        times = Time(hdulist[0].header["STARTOBS"]) + TimeDelta(
-            hdulist[1].data[:, hdulist[1].header["TIME"]], format="sec"
+        extra_coords = [
+            ("exposure time", 0, hdulist[1].data[:, hdulist[1].header["EXPTIMES"]] * u.s),
+            ("obs_vrix", 0, hdulist[1].data[:, hdulist[1].header["OBS_VRIX"]] * u.m / u.s),
+            ("ophaseix", 0, hdulist[1].data[:, hdulist[1].header["OPHASEIX"]] * u.arcsec),
+            ("pztx", 0, hdulist[1].data[:, hdulist[1].header["PZTX"]] * u.arcsec),
+            ("pzty", 0, hdulist[1].data[:, hdulist[1].header["PZTY"]] * u.arcsec),
+            ("slit x position", 0, hdulist[1].data[:, hdulist[1].header["SLTPX1IX"]] * u.arcsec),
+            ("slit y position", 0, hdulist[1].data[:, hdulist[1].header["SLTPX2IX"]] * u.arcsec),
+            ("xcenix", 0, hdulist[1].data[:, hdulist[1].header["XCENIX"]] * u.arcsec),
+            ("ycenix", 0, hdulist[1].data[:, hdulist[1].header["YCENIX"]] * u.arcsec),
+        ]
+        data = hdulist[0].data
+        data_nan_masked = hdulist[0].data
+        out_uncertainty = None
+        if memmap:
+            data_nan_masked[data == BAD_PIXEL_VALUE_UNSCALED] = 0
+            mask = None
+            scaled = False
+            unit = DN_UNIT["SJI_UNSCALED"]
+        elif not memmap:
+            data_nan_masked[data == BAD_PIXEL_VALUE_SCALED] = np.nan
+            mask = data_nan_masked == BAD_PIXEL_VALUE_SCALED
+            scaled = True
+            unit = DN_UNIT["SJI"]
+            if uncertainty:
+                out_uncertainty = calculate_uncertainty(data, READOUT_NOISE["SJI"], DN_UNIT["SJI"])
+        else:
+            raise ValueError(f"memmap={memmap} is not supported.")
+        map_cube = SJICube(
+            data_nan_masked,
+            _create_gwcs(hdulist),
+            uncertainty=out_uncertainty,
+            unit=unit,
+            meta=hdulist[0].header,
+            mask=mask,
+            scaled=scaled,
+            _basic_wcs=_create_wcs(hdulist),
         )
-        # The IRIS FITS files contain the per-exposure WCS metadata
-        # (reference coordinate and PCij matrix) in an extension, while the primary
-        # header has only values averaged over the observation
-        for i in range(hdulist[0].header["NAXIS3"]):
-            data = hdulist[0].data[i]
-            data_nan_masked = hdulist[0].data[i]
-            out_uncertainty = None
-            if memmap:
-                data_nan_masked[data == BAD_PIXEL_VALUE_UNSCALED] = 0
-                mask = None
-                scaled = False
-                unit = DN_UNIT["SJI_UNSCALED"]
-                out_uncertainty = None
-            elif not memmap:
-                data_nan_masked[data == BAD_PIXEL_VALUE_SCALED] = np.nan
-                mask = data_nan_masked == BAD_PIXEL_VALUE_SCALED
-                scaled = True
-                unit = DN_UNIT["SJI"]
-                if uncertainty:
-                    out_uncertainty = calculate_uncertainty(data, READOUT_NOISE["SJI"], DN_UNIT["SJI"])
-            else:
-                raise ValueError(f"memmap={memmap} is not supported.")
-            pztx = hdulist[1].data[i, hdulist[1].header["PZTX"]] * u.arcsec
-            pzty = hdulist[1].data[i, hdulist[1].header["PZTY"]] * u.arcsec
-            exposure_time = hdulist[1].data[i, hdulist[1].header["EXPTIMES"]] * u.s
-            obs_vrix = hdulist[1].data[i, hdulist[1].header["OBS_VRIX"]] * u.m / u.s
-            ophaseix = hdulist[1].data[i, hdulist[1].header["OPHASEIX"]] * u.arcsec
-            slit_pos_x = hdulist[1].data[i, hdulist[1].header["SLTPX1IX"]] * u.arcsec
-            slit_pos_y = hdulist[1].data[i, hdulist[1].header["SLTPX2IX"]] * u.arcsec
-            global_coords = [
-                ("time", "time", times[i]),
-                ("pztx", "custom: PZTX", pztx),
-                ("pzty", "custom: PZTY", pzty),
-                ("obs_vrix", "custom: OBS_VRIX", obs_vrix),
-                ("ophaseix", "custom: OPHASEIX", ophaseix),
-                ("exposure time", "obs.exposure", exposure_time),
-                ("slit x position", "custom: SLTPX1IX", slit_pos_x * u.pix),
-                ("slit y position", "custom: SLTPX2IX", slit_pos_y * u.pix),
-            ]
-            header = copy(hdulist[0].header)
-            header.pop("NAXIS3")
-            header.pop("PC3_1")
-            header.pop("PC3_2")
-            header.pop("CTYPE3")
-            header.pop("CUNIT3")
-            header.pop("CRVAL3")
-            header.pop("CRPIX3")
-            header.pop("CDELT3")
-            header["NAXIS"] = 2
-            header["CRVAL1"] = hdulist[1].data[i, hdulist[1].header["XCENIX"]]
-            header["CRVAL2"] = hdulist[1].data[i, hdulist[1].header["YCENIX"]]
-            header["PC1_1"] = hdulist[1].data[0, hdulist[1].header["PC1_1IX"]]
-            header["PC1_2"] = hdulist[1].data[0, hdulist[1].header["PC1_2IX"]]
-            header["PC2_1"] = hdulist[1].data[0, hdulist[1].header["PC2_1IX"]]
-            header["PC2_2"] = hdulist[1].data[0, hdulist[1].header["PC2_2IX"]]
-            wcs = WCS(header)
-            map_cube = IRISMapCube(
-                data_nan_masked,
-                wcs,
-                uncertainty=out_uncertainty,
-                unit=unit,
-                meta=meta,
-                mask=mask,
-                scaled=scaled,
-            )
-            [map_cube.global_coords.add(*global_coord) for global_coord in global_coords]
-            list_of_cubes.append(map_cube)
-    return IRISMapCubeSequence(list_of_cubes, meta=meta, common_axis=None, times=times)
+        [map_cube.extra_coords.add(*extra_coord) for extra_coord in extra_coords]
+    return map_cube
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/io/spectrograph.py` & `irispy-lmsal-0.2.0rc4/irispy/spectrograph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,359 @@
 import logging
-import tarfile
 import textwrap
-from copy import copy
-from pathlib import Path
 
 import astropy.units as u
+import matplotlib.pyplot as plt
 import numpy as np
 from astropy.coordinates import SkyCoord
-from astropy.io import fits
-from astropy.time import Time, TimeDelta
-from astropy.wcs import WCS
+from astropy.time import Time
+from ndcube import NDCollection
 from sunpy.coordinates import Helioprojective
-
+from sunraster import SpectrogramCube as SpecCube
+from sunraster import SpectrogramSequence as SpecSeq
 from sunraster.meta import Meta, SlitSpectrographMetaABC
+from sunraster.spectrogram import APPLY_EXPOSURE_TIME_ERROR
 
-from irispy.spectrograph import IRISCollection, IRISSpectrogramCube, IRISSpectrogramCubeSequence
-from irispy.utils import calculate_uncertainty
-from irispy.utils.constants import DN_UNIT, READOUT_NOISE, SLIT_WIDTH, SPECTRAL_BAND
+from irispy import utils
+from irispy.utils.constants import SPECTRAL_BAND
+from irispy.visualization import Plotter, _set_axis_colors
 
-__all__ = ["read_spectrograph_lvl2"]
+__all__ = ["Collection", "SpectrogramCube", "SpectrogramCubeSequence", "SGMeta"]
 
 
-def _pc_matrix(lam, angle_1, angle_2):
-    return angle_1, -1 * lam * angle_2, 1 / lam * angle_2, angle_1
+class Collection(NDCollection):
+    def __str__(self):
+        return textwrap.dedent(
+            f"""
+            Collection
+            ----------
+            Cube keys: {tuple(self.keys())}
+            Number of Cubes: {len(self)}
+            Aligned dimensions: {self.aligned_dimensions}
+            Aligned physical types: {self.aligned_axis_physical_types}
+            """,
+        )
 
 
-def read_spectrograph_lvl2(filenames, spectral_windows=None, uncertainty=False, memmap=False):
+class SpectrogramCube(SpecCube):
     """
-    Reads IRIS level 2 spectrograph FITS from an OBS into an
-    `.IRISSpectrograph` instance.
+    Class representing SpectrogramCube data described by a single WCS.
 
     Parameters
     ----------
-    filenames: `list` of `str` or `str`
-        Filename of filenames to be read. They must all be associated with the same
-        OBS number.
-        If you provide a tar file, it will be extracted at the same location.
-    spectral_windows: iterable of `str` or `str`
-        Spectral windows to extract from files. Default=None, implies, extract all
-        spectral windows.
-    uncertainty : `bool`, optional
-        If `True` (not the default), will compute the uncertainty for the data (slower and
-        uses more memory). If `memmap=True`, the uncertainty is never computed.
-    memmap : `bool`, optional
-        If `True` (not the default), will not load arrays into memory, and will only read from
-        the file into memory when needed. This option is faster and uses a
-        lot less memory. However, because FITS scaling is not done on-the-fly,
-        the data units will be unscaled, not the usual data numbers (DN).
-
-    Returns
-    -------
-    `ndcube.NDCollection`
+    data: `numpy.ndarray`
+        The array holding the actual data in this object.
+    wcs: `ndcube.wcs.wcs.WCS`
+        The WCS object containing the axes' information
+    unit : `astropy.unit.Unit` or `str`
+        Unit for the dataset. Strings that can be converted to a Unit are allowed.
+    meta : dict-like object
+        Additional meta information about the dataset. Must contain at least the
+        following keys:
+        - detector type: str, (FUV1, FUV2 or NUV)
+        - OBSID: int
+        - spectral window: str
+    uncertainty : any type, optional
+        Uncertainty in the dataset. Should have an attribute uncertainty_type
+        that defines what kind of uncertainty is stored, for example "std"
+        for standard deviation or "var" for variance. A metaclass defining
+        such an interface is NDUncertainty - but isn't mandatory. If the uncertainty
+        has no such attribute the uncertainty is stored as UnknownUncertainty.
+        Defaults to None.
+    mask : any type, optional
+        Mask for the dataset. Masks should follow the numpy convention
+        that valid data points are marked by False and invalid ones with True.
+        Defaults to None.
+    copy : `bool`, optional
+        Indicates whether to save the arguments as copy. True copies every attribute
+        before saving it while False tries to save every parameter as reference.
+        Note however that it is not always possible to save the input as reference.
+        Default is False.
     """
-    if isinstance(filenames, str):
-        if tarfile.is_tarfile(filenames):
-            parent = Path(filenames.replace(".tar.gz", "")).mkdir(parents=True, exist_ok=True)
-            with tarfile.open(filenames, "r") as tar:
-                tar.extractall(parent)
-                filenames = [parent / file for file in tar.getnames()]
-        else:
-            filenames = [filenames]
 
-    # Collecting the window observations
-    with fits.open(filenames[0], memmap=memmap, do_not_scale_image_data=memmap) as hdulist:
-        hdulist.verify("silentfix")
-        windows_in_obs = np.array(
-            [hdulist[0].header["TDESC{0}".format(i)] for i in range(1, hdulist[0].header["NWIN"] + 1)]
+    def __init__(
+        self,
+        data,
+        wcs,
+        uncertainty,
+        unit,
+        meta,
+        *,
+        mask=None,
+        copy=False,
+    ):
+        super().__init__(
+            data,
+            wcs,
+            unit=unit,
+            uncertainty=uncertainty,
+            mask=mask,
+            meta=meta,
+            copy=copy,
         )
-        # If spectral_window is not set then get every window.
-        # Else take the appropriate windows
-        if not spectral_windows:
-            spectral_windows_req = windows_in_obs
-            window_fits_indices = range(1, len(hdulist) - 2)
-        else:
-            if isinstance(spectral_windows, str):
-                spectral_windows_req = [spectral_windows]
-            else:
-                spectral_windows_req = spectral_windows
-            spectral_windows_req = np.asarray(spectral_windows_req, dtype="U")
-            window_is_in_obs = np.asarray([window in windows_in_obs for window in spectral_windows_req])
-            if not all(window_is_in_obs):
-                missing_windows = window_is_in_obs == False
-                raise ValueError(
-                    f"Spectral windows {spectral_windows[missing_windows]} not in file {filenames[0]}"
-                )
-            window_fits_indices = np.nonzero(np.in1d(windows_in_obs, spectral_windows))[0] + 1
-        data_dict = dict([(window_name, list()) for window_name in spectral_windows_req])
 
-    for filename in filenames:
-        with fits.open(filename, memmap=memmap, do_not_scale_image_data=memmap) as hdulist:
-            hdulist.verify("silentfix")
-            # Extract axis-aligned metadata.
-            times = Time(hdulist[0].header["STARTOBS"]) + TimeDelta(
-                hdulist[-2].data[:, hdulist[-2].header["TIME"]], format="sec"
-            )
-            fov_center = SkyCoord(
-                Tx=hdulist[-2].data[:, hdulist[-2].header["XCENIX"]],
-                Ty=hdulist[-2].data[:, hdulist[-2].header["YCENIX"]],
-                unit=u.arcsec,
-                frame=Helioprojective,
+    def __getitem__(self, item):
+        result = super().__getitem__(item)
+        return SpectrogramCube(
+            result.data,
+            result.wcs,
+            result.uncertainty,
+            result.unit,
+            result.meta,
+            mask=result.mask,
+        )
+
+    def __repr__(self):
+        return f"{object.__repr__(self)}\n{str(self)}"
+
+    def __str__(self):
+        instance_start = None
+        instance_end = None
+        if self.global_coords and "time" in self.global_coords:
+            instance_start = self.global_coords["time"].min().isot
+            instance_end = self.global_coords["time"].max().isot
+        elif self.extra_coords and self.axis_world_coords("time", wcs=self.extra_coords):
+            instance_start = self.axis_world_coords("time", wcs=self.extra_coords)[0].min().isot
+            instance_end = self.axis_world_coords("time", wcs=self.extra_coords)[0].max().isot
+        return textwrap.dedent(
+            f"""
+            SpectrogramCube
+            ---------------
+            OBS ID:             {self.meta.get("OBSID")}
+            OBS Description:    {self.meta.get("OBS_DESC")}
+            OBS period:         {self.meta.get("STARTOBS")} -- {self.meta.get("ENDOBS")}
+            Spectrogram period: {instance_start} -- {instance_end}
+            Data shape:         {self.dimensions}
+            Axis Types:         {self.array_axis_physical_types}
+            Roll:               {self.meta.get("SAT_ROT")}
+            """,
+        )
+
+    def plot(self, *args, **kwargs):
+        cmap = kwargs.get("cmap")
+        if not cmap:
+            try:
+                cmap = plt.get_cmap(name=f"irissji{int(self.meta.detector[:3])}")
+            except Exception as e:  # NOQA: BLE001
+                logging.debug(e)
+                cmap = "viridis"
+        kwargs["cmap"] = cmap
+        if len(self.dimensions) == 1:
+            kwargs.pop("cmap")
+        ax = Plotter(ndcube=self).plot(*args, **kwargs)
+        _set_axis_colors(ax)
+        return ax
+
+    def convert_to(self, new_unit_type, time_obs=None, response_version=4):
+        """
+        Converts data, unit and uncertainty attributes to new unit type.
+
+        Takes into consideration also the observation time and response version.
+
+        The presence or absence of the exposure time correction is
+        preserved in the conversions.
+
+        Parameters
+        ----------
+        new_unit_type : `str`
+            Unit type to convert data to. Three values are accepted:
+            "DN": Relevant IRIS data number based on detector type.
+            "photons": photon counts
+            "radiance": Perorms radiometric calibration conversion.
+        time_obs : `astropy.time.Time`, optional
+            Observation times of the datapoints.
+            Must be in the format of, e.g.,
+            ``time_obs=Time('2013-09-03')``,
+            The argument time_obs is ignored for versions 1 and 2.
+        response_version : `int`, optional
+            Version number of effective area file to be used, by default = 6.
+
+        Returns
+        -------
+        `SpectrogramCube`
+            New SpectrogramCube in new units.
+        """
+        detector_type = utils.get_detector_type(self.meta)
+        if new_unit_type == "radiance" or self.unit.is_equivalent(utils.RADIANCE_UNIT):
+            # Get spectral dispersion per pixel.
+            spectral_wcs_index = np.where(np.array(self.wcs.wcs.ctype) == "WAVE")[0][0]
+            spectral_dispersion_per_pixel = (
+                self.wcs.wcs.cdelt[spectral_wcs_index] * self.wcs.wcs.cunit[spectral_wcs_index]
             )
-            obs_vrix = hdulist[-2].data[:, hdulist[-2].header["OBS_VRIX"]] * u.m / u.s
-            ophaseix = hdulist[-2].data[:, hdulist[-2].header["OPHASEIX"]]
-            exposure_times_fuv = hdulist[-2].data[:, hdulist[-2].header["EXPTIMEF"]] * u.s
-            exposure_times_nuv = hdulist[-2].data[:, hdulist[-2].header["EXPTIMEN"]] * u.s
-            for i, window_name in enumerate(spectral_windows_req):
-                meta = IRISSGMeta(
-                    hdulist[0].header,
-                    window_name,
-                    data_shape=hdulist[window_fits_indices[i]].data.shape,
+            # Get solid angle from slit width for a pixel.
+            lat_wcs_index = ["HPLT" in c for c in self.wcs.wcs.ctype]
+            lat_wcs_index = np.arange(len(self.wcs.wcs.ctype))[lat_wcs_index]
+            lat_wcs_index = lat_wcs_index[0]
+            solid_angle = self.wcs.wcs.cdelt[lat_wcs_index] * self.wcs.wcs.cunit[lat_wcs_index] * utils.SLIT_WIDTH
+            # Get wavelength for each pixel.
+            obs_wavelength = self.axis_world_coords(2)
+
+        if new_unit_type == "DN" or new_unit_type == "photons":
+            if self.unit.is_equivalent(utils.RADIANCE_UNIT):
+                # Convert from radiance to counts/s
+                new_data_quantities = utils.convert_or_undo_photons_per_sec_to_radiance(
+                    (self.data * self.unit, self.uncertainty.array * self.unit),
+                    time_obs,
+                    response_version,
+                    obs_wavelength,
+                    detector_type,
+                    spectral_dispersion_per_pixel,
+                    solid_angle,
+                    undo=True,
+                )
+                new_data = new_data_quantities[0].value
+                new_uncertainty = new_data_quantities[1].value
+                new_unit = new_data_quantities[0].unit
+                self = SpectrogramCube(
+                    new_data,
+                    self.wcs,
+                    new_uncertainty,
+                    new_unit,
+                    self.meta,
+                    mask=self.mask,
                 )
-                exposure_times = exposure_times_nuv
-                DN_unit = DN_UNIT["NUV"]
-                readout_noise = READOUT_NOISE["NUV"]
-                if "FUV" in meta.detector:
-                    exposure_times = exposure_times_fuv
-                    DN_unit = DN_UNIT["FUV"]
-                    readout_noise = READOUT_NOISE["FUV"]
-                meta.add("exposure time", exposure_times, None, 0)
-                meta.add("exposure FOV center", fov_center, None, 0)
-                meta.add("observer radial velocity", obs_vrix, None, 0)
-                meta.add("orbital phase", ophaseix, None, 0)
-                # Sit-and-stare have a CDELT of 0 which causes issues in WCS.
-                # In this case, set CDELT to a small number.
-                header = copy(hdulist[window_fits_indices[i]].header)
-                # Account for a slit offset (POFFYNUV (45) or POFFYFUV (34))
-                idx = 45
-                if meta.spectral_band == "FUV":
-                    idx = 34
-                header["CRVAL3"] -= hdulist[-2].data[:, idx].mean() * (SLIT_WIDTH.value / 2)
-                if header["CDELT3"] == 0:
-                    header["CDELT3"] = 1e-10
-                    ang1, ang2, ang3, ang4 = _pc_matrix(
-                        header["CDELT3"] / header["CDELT2"],
-                        hdulist[-2].data[:, 20].mean(),
-                        hdulist[-2].data[:, 22].mean(),
-                    )
-                    header["PC2_2"] = ang1
-                    header["PC2_3"] = ang2
-                    header["PC3_2"] = ang3
-                    header["PC3_3"] = ang4
+                self._extra_coords = self.extra_coords
+            if new_unit_type == "DN":
+                new_unit = utils.DN_UNIT[detector_type]
+            else:
+                new_unit = u.photon
+            new_data_arrays, new_unit = utils.convert_between_DN_and_photons(
+                (self.data, self.uncertainty.array),
+                self.unit,
+                new_unit,
+            )
+            new_data = new_data_arrays[0]
+            new_uncertainty = new_data_arrays[1]
+        elif new_unit_type == "radiance":
+            if self.unit.is_equivalent(utils.RADIANCE_UNIT):
+                new_data = self.data
+                new_uncertainty = self.uncertainty
+                new_unit = self.unit
+            else:
+                # Ensure spectrogram is in units of counts/s.
+                cube = self.convert_to("photons")
                 try:
-                    wcs = WCS(header)
-                except Exception as e:
-                    logging.warning(
-                        f"WCS failed to load while reading one step of the raster due to {e}"
-                        " The loading will continue but this will be missing in the final cube."
-                        f" Spectral window: {window_name}, step {i} in file: {filename}"
-                    )
-                    continue
-                out_uncertainty = None
-                data_mask = None
-                if not memmap:
-                    data_mask = hdulist[window_fits_indices[i]].data == -200.0
-                if uncertainty:
-                    out_uncertainty = calculate_uncertainty(
-                        hdulist[window_fits_indices[i]].data, readout_noise, DN_UNIT
-                    )
-                cube = IRISSpectrogramCube(
-                    hdulist[window_fits_indices[i]].data,
-                    wcs=wcs,
-                    uncertainty=out_uncertainty,
-                    unit=DN_unit,
-                    meta=meta,
-                    mask=data_mask,
+                    cube = cube.apply_exposure_time_correction()
+                except ValueError(APPLY_EXPOSURE_TIME_ERROR):
+                    pass
+                # Convert to radiance units.
+                new_data_quantities = utils.convert_or_undo_photons_per_sec_to_radiance(
+                    (cube.data * cube.unit, cube.uncertainty.array * cube.unit),
+                    time_obs,
+                    response_version,
+                    obs_wavelength,
+                    detector_type,
+                    spectral_dispersion_per_pixel,
+                    solid_angle,
                 )
-                cube.extra_coords.add("time", 0, times, physical_types="time")
-                data_dict[window_name].append(cube)
-    window_data_pairs = [
-        (window_name, IRISSpectrogramCubeSequence(data_dict[window_name], common_axis=0))
-        for window_name in spectral_windows_req
-    ]
-    return IRISCollection(window_data_pairs, aligned_axes=(0, 1, 2))
+                new_data = new_data_quantities[0].value
+                new_uncertainty = new_data_quantities[1].value
+                new_unit = new_data_quantities[0].unit
+        else:
+            raise ValueError("Input unit type not recognized.")
+        new_cube = SpectrogramCube(
+            new_data,
+            self.wcs,
+            new_uncertainty,
+            new_unit,
+            self.meta,
+            mask=self.mask,
+        )
+        new_cube._extra_coords = self.extra_coords
+        return new_cube
+
+
+class SpectrogramCubeSequence(SpecSeq):
+    """
+    Class for holding, slicing and plotting IRIS spectrogram data.
+
+    This class contains all the functionality of its super class with
+    some additional functionalities.
+
+    Parameters
+    ----------
+    data_list: `list`
+        List of `SpectrogramCube` objects from the same spectral window and OBS ID.
+    meta: `dict` or header object, optional
+        Metadata associated with the sequence.
+    common_axis: `int`, optional
+        The axis of the NDCubes corresponding to time.
+    """
+
+    def __init__(self, data_list, meta=None, common_axis=0):
+        # Check that all spectrograms are from same spectral window and OBS ID.
+        if len(np.unique([cube.meta["OBSID"] for cube in data_list])) != 1:
+            raise ValueError("Constituent SpectrogramCube objects must have same value of 'OBSID' in its meta.")
+        super().__init__(data_list, meta=meta, common_axis=common_axis)
+
+    def __str__(self):
+        # Overload it get the class name in the string
+        return super().__str__()
+
+    def convert_to(self, new_unit_type, *, copy=False):
+        """
+        Converts data, uncertainty and unit of each spectrogram in sequence to
+        new unit.
 
+        Parameters
+        ----------
+        new_unit_type: `str`
+           Unit type to convert data to.  Three values are accepted:
+           "DN": Relevant IRIS data number based on detector type.
+           "photons": photon counts
+           "radiance": Perorms radiometric calibration conversion.
+        copy: `bool`
+            If True a new instance with the converted data values is return.
+            If False, the current instance is overwritten.
+            Default=False
+        """
+        converted_data_list = []
+        for cube in self.data:
+            converted_data_list.append(cube.convert_to(new_unit_type))
+        if copy is True:
+            return SpectrogramCubeSequence(converted_data_list, meta=self.meta, common_axis=self._common_axis)
+        self.data = converted_data_list
+        return None
 
-class IRISSGMeta(Meta, metaclass=SlitSpectrographMetaABC):
+
+class SGMeta(Meta, metaclass=SlitSpectrographMetaABC):
     def __init__(self, header, spectral_window, **kwargs):
         super().__init__(header, **kwargs)
-        spectral_windows = np.array([self["TDESC{0}".format(i)] for i in range(1, self["NWIN"] + 1)])
+        spectral_windows = np.array([self[f"TDESC{i}"] for i in range(1, self["NWIN"] + 1)])
         window_mask = np.array([spectral_window in window for window in spectral_windows])
         if window_mask.sum() < 1:
             raise ValueError(
                 "Spectral window not found. "
                 f"Input spectral window: {spectral_window}; "
-                f"Spectral windows in header: {spectral_windows}"
+                f"Spectral windows in header: {spectral_windows}",
             )
-        elif window_mask.sum() > 1:
+        if window_mask.sum() > 1:
             raise ValueError(
                 "Spectral window must be unique. "
                 f"Input spectral window: {spectral_window}; "
-                f"Ambiguous spectral windows in header: {spectral_windows[window_mask]}"
+                f"Ambiguous spectral windows in header: {spectral_windows[window_mask]}",
             )
         self._iwin = np.arange(len(spectral_windows))[window_mask][0] + 1
 
     def __str__(self):
         return textwrap.dedent(
             f"""
-                IRISMeta
-                --------
+                SGMeta
+                ------
                 Observatory:     {self.observatory}
                 Instrument:      {self.instrument}
                 Detector:        {self.detector}
                 Spectral Window: {self.spectral_window}
                 Spectral Range:  {self.spectral_range}
                 Spectral Band:   {self.spectral_band}
                 Dimensions:      {self.dimensions}
                 Date:            {self.date_reference}
                 OBS ID:          {self.observing_mode_id}
                 OBS Description: {self.observing_mode_description}
-                """
+                """,
         )
 
     def __repr__(self):
         return f"{object.__repr__(self)}\n{str(self)}"
 
     def _construct_time(self, key):
         val = self.get(key)
@@ -386,9 +527,8 @@
     @property
     def spectral_summing_factor(self):
         """
         Number of pixels summed together in the spectral direction.
         """
         if "fuv" in self.detector.lower():
             return self.get("SUMSPTRF")
-        else:
-            return self.get("SUMSPTRN")
+        return self.get("SUMSPTRN")
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/io/tests/test_utils.py` & `irispy-lmsal-0.2.0rc4/irispy/io/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,12 @@
 import pytest
 
-from irispy.data.test import get_test_filepath
 from irispy.io.utils import fitsinfo, read_files
 
 
-@pytest.fixture
-def raster_file():
-    return get_test_filepath("iris_l2_20170502_052551_3893010094_raster_t000_r00000.fits")
-
-
-@pytest.fixture
-def sji_1330_file():
-    return get_test_filepath("iris_l2_20170502_052551_3893010094_SJI_1330_t000.fits")
-
-
-@pytest.fixture
-def sji_1400_file():
-    return get_test_filepath("iris_l2_20170502_052551_3893010094_SJI_1400_t000.fits")
-
-
-@pytest.fixture
-def sji_2796_file():
-    return get_test_filepath("iris_l2_20170502_052551_3893010094_SJI_2796_t000.fits")
-
-
-@pytest.fixture
-def sji_2832_file():
-    return get_test_filepath("iris_l2_20170502_052551_3893010094_SJI_2832_t000.fits")
-
-
 def test_fitsinfo(capsys, raster_file, sji_1330_file, sji_1400_file, sji_2796_file, sji_2832_file):
     fitsinfo(raster_file)
     captured = capsys.readouterr()
     assert raster_file in captured.out
 
     fitsinfo(sji_1330_file)
     captured = capsys.readouterr()
@@ -53,21 +27,21 @@
 
 def test_read_files_errors_with_mix(raster_file, sji_1330_file):
     with pytest.raises(ValueError, match="You cannot mix raster and SJI files."):
         read_files([raster_file, sji_1330_file])
 
 
 def test_read_files_raster(raster_file):
-    # Simple test to ensure it doesnt error
+    # Simple test to ensure it does not error
     read_files(raster_file)
     read_files([raster_file])
 
 
 def test_read_files_sji(sji_1330_file, sji_1400_file, sji_2796_file, sji_2832_file):
-    # Simple test to ensure it doesnt error
+    # Simple test to ensure it does not error
     read_files(sji_1330_file)
     read_files(sji_1400_file)
     read_files(sji_2796_file)
     read_files(sji_2832_file)
     read_files([sji_2832_file])
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/io/utils.py` & `irispy-lmsal-0.2.0rc4/irispy/io/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+import logging
 import tarfile
 from pathlib import Path
 
 from astropy.io import fits
 
 __all__ = ["fitsinfo", "read_files"]
 
 
 def fitsinfo(filename):
     """
-    Prints information about the extension of a raster or SJI IRIS Level 2 data
+    Prints information about the extension of a raster or SJI level 2 data
     file.
 
     Parameters
     ----------
     filename : str
         Filename to load.
     """
     with fits.open(filename) as hdulist:
         hdulist.info()
         hdr = hdulist[0].header
-        print("Observation description: ", hdr["OBS_DESC"], "\n")
+        logging.info(f"Observation description: {hdr['OBS_DESC']}")
         nwin = hdr["NWIN"]
-        modifer = ""
+        modifier = ""
         for i in range(nwin):
-            print(f"Extension No. {i+1} stores data and header of {hdr[f'TDESC{i+1}']}: ", end="")
-            if "SJI" not in hdr["TDET{}".format(i + 1)]:
-                modifer = f" ({hdr[f'TDET{i+1}'][0:3]})"
-            print(f"{hdr[f'TWMIN{i+1}']:.2f} - {hdr[f'TWMAX{i+1}']:.2f} AA" + modifer)
+            logging.info(f"Extension No. {i+1} stores data and header of {hdr[f'TDESC{i+1}']}: ")
+            if "SJI" not in hdr[f"TDET{i + 1}"]:
+                modifier = f" ({hdr[f'TDET{i+1}'][0:3]})"
+            logging.info(f"{hdr[f'TWMIN{i+1}']:.2f} - {hdr[f'TWMAX{i+1}']:.2f} AA" + modifier)
 
 
-def read_files(filename, spectral_windows=None, uncertainty=False, memmap=False):
+def read_files(filename, *, spectral_windows=None, uncertainty=False, memmap=False):
     """
-    A wrapper function to read a raster or SJI IRIS Level 2 data file.
+    A wrapper function to read a raster or SJI level 2 data file.
 
     You can provide one SJI image or a one raster image or a list of raster images.
 
     If you mix raster and SJI images, the function will raise an error.
 
     Parameters
     ----------
-    filename : `list of `str`, `str`
+    filename : `list of `str`, `str`, `pathlib.Path`
         Filename(s) to load.
         If given a string, will load that file.
         If given a list of strings, it will check they are all raster files and load them.
     spectral_windows: iterable of `str` or `str`
         Spectral windows to extract from files. Default=None, implies, extract all
         spectral windows.
     uncertainty : `bool`, optional
@@ -53,37 +54,39 @@
         If `True` (not the default), will not load arrays into memory, and will only read from
         the file into memory when needed. This option is faster and uses a
         lot less memory. However, because FITS scaling is not done on-the-fly,
         the data units will be unscaled, not the usual data numbers (DN).
 
     Returns
     -------
-    The corresponding `irispy.sji.IRISMapCube` or `irispy.spectrogram.IRISSpectrogramCube`.
+    The corresponding `irispy.sji.SJICube` or `irispy.spectrogram.SpectrogramCube`.
     """
     from irispy.io.sji import read_sji_lvl2
     from irispy.io.spectrograph import read_spectrograph_lvl2
 
-    if isinstance(filename, str):
+    if isinstance(filename, Path):
+        filename = str(filename)
+    if isinstance(filename, (str, Path)):
         if tarfile.is_tarfile(filename):
             path = Path(filename.replace(".tar.gz", ""))
             path.mkdir(parents=True, exist_ok=True)
             with tarfile.open(filename, "r") as tar:
                 tar.extractall(path)
                 filename = [path / file for file in tar.getnames()]
         else:
             filename = [filename]
-
     intrume = fits.getval(filename[0], "INSTRUME")
     all_instrume = [fits.getval(f, "INSTRUME") for f in filename]
-    if not all([intrume == i for i in all_instrume]):
+    if not all(intrume == i for i in all_instrume):
         raise ValueError("You cannot mix raster and SJI files.")
-
     if intrume == "SJI":
         if len(filename) > 1:
             raise ValueError("You cannot load more than one SJI file at a time.")
         return read_sji_lvl2(filename[0], memmap=memmap, uncertainty=uncertainty)
-    elif intrume == "SPEC":
+    if intrume == "SPEC":
         return read_spectrograph_lvl2(
-            filename, spectral_windows=spectral_windows, memmap=memmap, uncertainty=uncertainty
+            filename,
+            spectral_windows=spectral_windows,
+            memmap=memmap,
+            uncertainty=uncertainty,
         )
-    else:
-        raise ValueError(f"Unsupported instrument: {intrume}")
+    raise ValueError(f"Unsupported instrument: {intrume}")
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/obsid.py` & `irispy-lmsal-0.2.0rc4/irispy/obsid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import os
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from astropy import units as u
 from pkg_resources import resource_filename
 
-dir_path = os.path.dirname(os.path.realpath(__file__))
+dir_path = Path(__file__).parent
 
 __all__ = ["ObsID"]
 
 
 class ObsID(dict):
     """
     A class to convert the IRIS OBS ID to human-readable format.
@@ -31,15 +31,15 @@
     >>> from irispy import obsid
     >>> obsid.ObsID(3675508564)
     IRIS OBS ID 3675508564
     ----------------------
     Description:            Large dense 96-step raster 31.35x120 96s
     SJI filters:                                    C II   Mg II w s
     SJI field of view:                                       120x120
-    Exposure time:                                               8.0 s
+    Exposure time:                                             8.0 s
     Binning:                               Spatial x 1, Spectral x 1
     FUV binning:                         FUV spectrally rebinned x 4
     SJI cadence:                                 SJI cadence default
     Compression:                                Lossless compression
     Linelist:                                       Flare linelist 1
 
     The data can be accessed as in a dictionary:
@@ -80,16 +80,15 @@
     def _exptime_to_quant(exptime):
         """
         Converts an 'exptime' string (used in IRIS tables and OBS_DESC) to a
         Quantity instance in seconds.
         """
         if exptime == "Exposure 1s":
             return 1.0 * u.s
-        else:
-            return float(exptime.split(" x ")[1]) * u.s
+        return float(exptime.split(" x ")[1]) * u.s
 
     def _read_obsid(self, obsid):
         """
         Reads different fields from OBS ID number.
         """
         data = {}
         options = {}
@@ -102,15 +101,15 @@
             "SJI cadence default": "sji_cadence",
             "SJI cadence 10s": "sji_cadence",
             "FUV binned same as NUV": "fuv_binning",
             "Spatial x 1, Spectral x 1": "binning",
             "Exposure 1s": "exptime",
             "C II   Si IV   Mg II h/k   Mg II w   ": "sjis",
         }
-        versions = [36, 38, 40]
+        versions = [34, 36, 38, 40]
         if len(str(obsid)) != 10:
             raise ValueError("Invalid OBS ID: must have 10 digits.")
         # here choose between tables
         version = int(str(obsid)[:2])
         if version not in versions:
             raise ValueError("Invalid OBS ID: two first digits must one of" " {}".format(versions))
         obsid = int(str(obsid)[2:])  # version digits are no longer needed
@@ -118,16 +117,16 @@
         table2 = pd.read_csv(resource_filename("irispy", "data/v%i-table2000.csv" % version))
         id_raster = int(str(obsid)[-2:])
         try:
             meta = table1.where(table1["OBS-ID"] == id_raster).dropna().iloc[0]
         except IndexError:
             raise ValueError(
                 "Invalid OBS ID: last two numbers must be between"
-                " {} and {}".format(table1["OBS-ID"].min(), table1["OBS-ID"].max())
-            )
+                " {} and {}".format(table1["OBS-ID"].min(), table1["OBS-ID"].max()),
+            ) from None
 
         data["raster_step"] = meta["Raster step"]
         data["raster_fov"] = meta["Raster FOV"]
         data["spec_cadence"] = meta["Spectral cadence"]
         data["sji_fov"] = meta["SJI FOV"]
         data["raster_desc"] = meta["Description"]
         data["raster_fulldesc"] = "{} {} {}".format(
@@ -135,15 +134,15 @@
             data["raster_fov"],
             data["spec_cadence"],
         )
         field_ranges = np.concatenate(
             [  # find all dividers between fields
                 table2.where(table2["OBS ID"] == 0).dropna(how="all").index,
                 np.array([len(table2)]),
-            ]
+            ],
         )
         # field indices, start from largest and subtract
         for start, end in zip(field_ranges[-2::-1], field_ranges[:0:-1]):
             table = table2.iloc[start:end]
             for i in np.arange(start, end)[::-1]:
                 index = i
                 tmp = table["OBS ID"].loc[i]
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/tests/test_obsid.py` & `irispy-lmsal-0.2.0rc4/irispy/tests/test_obsid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,76 @@
 import astropy.units as u
 import pytest
 
 from irispy.obsid import ObsID
 
-OBSIDS = [3677508065, 3880903651, 4050607445]
-INVALID_OBSID = [4643502010, 4050607495, 3880903650, 3680903685, 335987081297, 40]
+OBSIDS = [
+    3400109162,
+    3677508065,
+    3880903651,
+    4050607445,
+]
+INVALID_OBSID = [
+    4643502010,
+    4050607495,
+    3880903650,
+    3680903685,
+    335987081297,
+    40,
+]
 TEST_DATA = {}
-TEST_DATA["exptime"] = [8 * u.s, 30 * u.s, 4 * u.s]
+TEST_DATA["exptime"] = [
+    8 * u.s,
+    8 * u.s,
+    30 * u.s,
+    4 * u.s,
+]
 TEST_DATA["raster_desc"] = [
+    "Very large coarse 64-step raster",
     "Very large dense 96-step raster",
     "Small sit-and-stare",
     "Very large dense raster (tight timing)",
 ]
-TEST_DATA["sjis"] = ["C II   Si IV   Mg II h/k   Mg II w", "Si IV", "Si IV   Mg II h/k"]
+TEST_DATA["sjis"] = [
+    "C II   Si IV   Mg II h/k",
+    "C II   Si IV   Mg II h/k   Mg II w",
+    "Si IV",
+    "Si IV   Mg II h/k",
+]
 TEST_DATA["binning"] = [
+    "Spatial x 2, Spectral x 2",
     "Spatial x 1, Spectral x 1",
     "Spatial x 2, Spectral x 8",
     "Spatial x 2, Spectral x 2",
 ]
 TEST_DATA["fuv_binning"] = [
+    "FUV binned same as NUV",
     "FUV spectrally rebinned x 4",
     "FUV spectrally rebinned x 8",
     "FUV spectrally rebinned x 4",
 ]
 TEST_DATA["sji_cadence"] = [
+    "SJI cadence default",
     "SJI cadence 0.5x faster",
     "SJI cadence default",
     "SJI cadence 10s",
 ]
-TEST_DATA["linelist"] = ["Flare linelist 1", "Full readout", "Small linelist"]
+TEST_DATA["linelist"] = [
+    "Large linelist",
+    "Flare linelist 1",
+    "Full readout",
+    "Small linelist",
+]
 
 
 @pytest.mark.parametrize(
-    "attr_name, test_input, expected_output",
+    ("attr_name", "test_input", "expected_output"),
     [(name, obs, output[i]) for (name, output) in TEST_DATA.items() for i, obs in enumerate(OBSIDS)],
 )
 def test_attribute(attr_name, test_input, expected_output):
     assert ObsID(test_input)[attr_name] == expected_output
 
 
 @pytest.mark.parametrize("test_input", [INVALID_OBSID])
 def test_invalid_obsid(test_input):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Invalid OBS ID: must have 10 digits."):
         ObsID(test_input)
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/tests/test_spectrograph.py` & `irispy-lmsal-0.2.0rc4/irispy/tests/test_spectrograph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import copy
-import os.path
 
 import astropy.units as u
 import numpy as np
-import pytest
 from astropy.io import fits
 from astropy.time import Time, TimeDelta
 from astropy.wcs import WCS
 
 import irispy.data.test
-from irispy import IRISSpectrogramCube, IRISSpectrogramCubeSequence, utils
-from irispy.data.test import get_test_filepath
+from irispy import SpectrogramCube, SpectrogramCubeSequence, utils
 from irispy.io.spectrograph import read_spectrograph_lvl2
 
 testpath = irispy.data.test.rootdir
 # Arrays of DN
 SOURCE_DATA_DN = np.array(
     [
         [[0.563, 1.132, -1.343], [-0.719, 1.441, 1.566]],
         [[0.563, 1.132, -1.343], [-0.719, 1.441, 1.566]],
-    ]
+    ],
 )
 SOURCE_UNCERTAINTY_DN = np.sqrt(SOURCE_DATA_DN)
 # Arrays relating SOURCE_DATA_DN to photons in NUV and FUV
 SOURCE_DATA_PHOTONS_NUV = np.array(
     [
         [[10.134, 20.376, -24.174], [-12.942, 25.938, 28.188]],
         [[10.134, 20.376, -24.174], [-12.942, 25.938, 28.188]],
-    ]
+    ],
 )
 SOURCE_DATA_PHOTONS_FUV = np.array(
     [
         [[2.252, 4.528, -5.372], [-2.876, 5.764, 6.264]],
         [[2.252, 4.528, -5.372], [-2.876, 5.764, 6.264]],
-    ]
+    ],
 )
 SOURCE_UNCERTAINTY_PHOTONS_NUV = np.sqrt(SOURCE_DATA_PHOTONS_NUV)
 SOURCE_UNCERTAINTY_PHOTONS_FUV = np.sqrt(SOURCE_DATA_PHOTONS_FUV)
 time_dim_len = SOURCE_DATA_DN.shape[0]
 single_exposure_time = 2.0
 EXPOSURE_TIME = u.Quantity(np.zeros(time_dim_len) + single_exposure_time, unit=u.s)
 # Define an sample wcs object
@@ -73,157 +70,149 @@
     (
         "time",
         0,
         (Time("2017-01-01") + TimeDelta(np.arange(time_dim_len, time_dim_len * 2), format="sec")),
     ),
     ("exposure time", 0, EXPOSURE_TIME),
 ]
-# Define IRISSpectrogramCubes in various units.
-spectrogram_DN0 = IRISSpectrogramCube(
+# Define SpectrogramCubes in various units.
+spectrogram_DN0 = SpectrogramCube(
     SOURCE_DATA_DN,
     wcs0,
     SOURCE_UNCERTAINTY_DN,
     utils.DN_UNIT["FUV"],
     meta0,
 )
 spectrogram_DN0.extra_coords.add(*extra_coords0[0])
 spectrogram_DN0.extra_coords.add(*extra_coords0[1])
-spectrogram_photon0 = IRISSpectrogramCube(
+spectrogram_photon0 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV,
     u.photon,
     meta0,
 )
 spectrogram_DN0.extra_coords.add(*extra_coords0[0])
 spectrogram_DN0.extra_coords.add(*extra_coords0[1])
-spectrogram_DN_per_s0 = IRISSpectrogramCube(
+spectrogram_DN_per_s0 = SpectrogramCube(
     SOURCE_DATA_DN / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_DN / single_exposure_time,
     utils.DN_UNIT["FUV"] / u.s,
     meta0,
 )
 spectrogram_DN_per_s0.extra_coords.add(*extra_coords0[0])
 spectrogram_DN_per_s0.extra_coords.add(*extra_coords0[1])
-spectrogram_photon_per_s0 = IRISSpectrogramCube(
+spectrogram_photon_per_s0 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV / single_exposure_time,
     u.photon / u.s,
     meta0,
 )
 spectrogram_photon_per_s0.extra_coords.add(*extra_coords0[0])
 spectrogram_photon_per_s0.extra_coords.add(*extra_coords0[1])
-spectrogram_DN1 = IRISSpectrogramCube(
+spectrogram_DN1 = SpectrogramCube(
     SOURCE_DATA_DN,
     wcs0,
     SOURCE_UNCERTAINTY_DN,
     utils.DN_UNIT["FUV"],
     meta0,
 )
 spectrogram_DN1.extra_coords.add(*extra_coords1[0])
 spectrogram_DN1.extra_coords.add(*extra_coords1[1])
-spectrogram_photon1 = IRISSpectrogramCube(
+spectrogram_photon1 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV,
     u.photon,
     meta0,
 )
 spectrogram_photon1.extra_coords.add(*extra_coords1[0])
 spectrogram_photon1.extra_coords.add(*extra_coords1[1])
-spectrogram_DN_per_s1 = IRISSpectrogramCube(
+spectrogram_DN_per_s1 = SpectrogramCube(
     SOURCE_DATA_DN / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_DN / single_exposure_time,
     utils.DN_UNIT["FUV"] / u.s,
     meta0,
 )
 spectrogram_DN_per_s1.extra_coords.add(*extra_coords1[0])
 spectrogram_DN_per_s1.extra_coords.add(*extra_coords1[1])
-spectrogram_photon_per_s1 = IRISSpectrogramCube(
+spectrogram_photon_per_s1 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV / single_exposure_time,
     u.photon / u.s,
     meta0,
-    extra_coords1,
 )
 spectrogram_DN0.extra_coords.add(*extra_coords0[0])
 spectrogram_DN0.extra_coords.add(*extra_coords0[1])
-spectrogram_photon_per_s_per_s0 = IRISSpectrogramCube(
+spectrogram_photon_per_s_per_s0 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV / single_exposure_time / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV / single_exposure_time / single_exposure_time,
     u.photon / u.s / u.s,
     meta0,
 )
 spectrogram_photon_per_s_per_s0.extra_coords.add(*extra_coords0[0])
 spectrogram_photon_per_s_per_s0.extra_coords.add(*extra_coords0[1])
-spectrogram_photon_s0 = IRISSpectrogramCube(
+spectrogram_photon_s0 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV * single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV * single_exposure_time,
     u.photon * u.s,
     meta0,
 )
 spectrogram_photon_s0.extra_coords.add(*extra_coords0[0])
 spectrogram_photon_s0.extra_coords.add(*extra_coords0[1])
-spectrogram_photon_per_s_per_s1 = IRISSpectrogramCube(
+spectrogram_photon_per_s_per_s1 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV / single_exposure_time / single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV / single_exposure_time / single_exposure_time,
     u.photon / u.s / u.s,
     meta0,
 )
 spectrogram_photon_per_s_per_s1.extra_coords.add(*extra_coords1[0])
 spectrogram_photon_per_s_per_s1.extra_coords.add(*extra_coords1[1])
-spectrogram_photon_s1 = IRISSpectrogramCube(
+spectrogram_photon_s1 = SpectrogramCube(
     SOURCE_DATA_PHOTONS_FUV * single_exposure_time,
     wcs0,
     SOURCE_UNCERTAINTY_PHOTONS_FUV * single_exposure_time,
     u.photon * u.s,
     meta0,
 )
 spectrogram_photon_s1.extra_coords.add(*extra_coords1[0])
 spectrogram_photon_s1.extra_coords.add(*extra_coords1[1])
-# Define meta dict for an IRISSpectrogramCubeSequence
+# Define meta dict for an SpectrogramCubeSequence
 meta_seq = {
     "detector type": "FUV",
     "spectral window": "C II 1336",
     "brightest wavelength": 100,
     "min wavelength": 90,
     "max wavelength": 110,
 }
-# Define IRISSpectrogramCubeSequences
-sequence_DN = IRISSpectrogramCubeSequence([spectrogram_DN0, spectrogram_DN1], meta_seq)
-sequence_photon = IRISSpectrogramCubeSequence([spectrogram_photon0, spectrogram_photon1], meta_seq)
-sequence_DN_per_s = IRISSpectrogramCubeSequence([spectrogram_DN_per_s0, spectrogram_DN_per_s1], meta_seq)
-sequence_photon_per_s = IRISSpectrogramCubeSequence(
-    [spectrogram_photon_per_s0, spectrogram_photon_per_s1], meta_seq
+# Define SpectrogramCubeSequences
+sequence_DN = SpectrogramCubeSequence([spectrogram_DN0, spectrogram_DN1], meta_seq)
+sequence_photon = SpectrogramCubeSequence([spectrogram_photon0, spectrogram_photon1], meta_seq)
+sequence_DN_per_s = SpectrogramCubeSequence([spectrogram_DN_per_s0, spectrogram_DN_per_s1], meta_seq)
+sequence_photon_per_s = SpectrogramCubeSequence([spectrogram_photon_per_s0, spectrogram_photon_per_s1], meta_seq)
+sequence_photon_per_s_per_s = SpectrogramCubeSequence(
+    [spectrogram_photon_per_s_per_s0, spectrogram_photon_per_s1],
+    meta_seq,
 )
-sequence_photon_per_s_per_s = IRISSpectrogramCubeSequence(
-    [spectrogram_photon_per_s_per_s0, spectrogram_photon_per_s1], meta_seq
-)
-sequence_photon_s = IRISSpectrogramCubeSequence([spectrogram_photon_s0, spectrogram_photon_s1], meta_seq)
-
-
-@pytest.fixture
-def iris_l2_test_raster():
-    return read_spectrograph_lvl2(get_test_filepath("iris_l2_20170502_052551_3893010094_raster_t000_r00000.fits"))
+sequence_photon_s = SpectrogramCubeSequence([spectrogram_photon_s0, spectrogram_photon_s1], meta_seq)
 
 
-def test_fits_data_comparison(iris_l2_test_raster):
+def test_fits_data_comparison(raster_file):
     """
     Make sure the data is the same in pyfits and irispy.
     """
-    with fits.open(
-        os.path.join(testpath, "iris_l2_20170502_052551_3893010094_raster_t000_r00000.fits")
-    ) as hdulist:
+    iris_l2_test_raster = read_spectrograph_lvl2(raster_file)
+    with fits.open(raster_file) as hdulist:
         spectral_window1 = hdulist[0].header["TDESC1"]
         spectral_window2 = hdulist[0].header["TDESC2"]
         spectral_window3 = hdulist[0].header["TDESC3"]
         data1 = copy.deepcopy(hdulist[1].data)
         data2 = copy.deepcopy(hdulist[2].data)
         data3 = copy.deepcopy(hdulist[3].data)
         np.testing.assert_array_almost_equal(iris_l2_test_raster[spectral_window1].data[0].data, data1)
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/constants.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/response.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 This module provides general utility functions for IRIS Responses.
 """
-import os
 import datetime
+from pathlib import Path
 
 import astropy.units as u
 import numpy as np
 import scipy
 import scipy.io
 from astropy.time import Time
 from astropy.units.quantity import Quantity
 from sunpy.time import parse_time
 
-from irispy.data import rootdir
+from irispy.data import ROOTDIR
 
 RESPONSE_VERSION_FILENAMES = {
     "1": "iris_sra_20130211.geny",
     "2": "iris_sra_20130715.geny",
     "3": "iris_sra_c_20150331.geny",
     "4": "iris_sra_c_20161022.geny",
     "5": "iris_sra_c_20191101.geny",
@@ -55,94 +55,71 @@
     effective areas.
 
     Returns
     -------
     `dict`
         Various parameters regarding IRIS response or effective area structure.
         Includes the following keys:
-        date_obs: `astropy.time.Time`
-        lambda: `astropy.units.Quantity`
-        area_sg: `astropy.units.Quantity`
-        name_sg: `str`
-        dn2phot_sg: `tuple` of length 2
-        area_sji: `astropy.units.Quantity`
-        name_sji: `str`
-        dn2phot_sji:  `tuple` of length 4
-        comment: `str`
-        version: `int`
-        version_date: `astropy.time.Time`
+        date_obs : `astropy.time.Time`
+        lambda : `astropy.units.Quantity`
+        area_sg : `astropy.units.Quantity`
+        name_sg : `str`
+        dn2phot_sg : `tuple` of length 2
+        area_sji : `astropy.units.Quantity`
+        name_sji : `str`
+        dn2phot_sji : `tuple` of length 4
+        comment : `str`
+        version : `int`
+        version_date : `astropy.time.Time`
     """
     response_filename = RESPONSE_VERSION_FILENAMES[str(response_version)]
-    path = os.path.join(rootdir, response_filename)
+    path = Path(ROOTDIR) / response_filename
     raw_response_data = scipy.io.readsav(path)
     iris_response = {name: raw_response_data["p0"][name][0] for name in raw_response_data["p0"].dtype.names}
     # Convert some properties to more convenient types.
     iris_response["LAMBDA"] = Quantity(iris_response["LAMBDA"], unit=u.nm)
     iris_response["AREA_SG"] = Quantity(iris_response["AREA_SG"], unit=u.cm**2)
     iris_response["AREA_SJI"] = Quantity(iris_response["AREA_SJI"], unit=u.cm**2)
     iris_response["GEOM_AREA"] = Quantity(iris_response["GEOM_AREA"], unit=u.cm**2)
-    iris_response["VERSION"] = iris_response["VERSION"]
+    iris_response["VERSION"] = int(iris_response["VERSION"])
     # Convert some properties not found in version below version 3 to
     # more convenient types.
-    if int(iris_response["VERSION"]) > 2:
+    if iris_response["VERSION"] > 2:
         # If DATE_OBS has a value, convert to `astropy.time.Time`, else set to None.
         try:
             iris_response["DATE_OBS"] = parse_time(iris_response["DATE_OBS"], format="utime")
-        except Exception:
+        except Exception:  # NOQA: BLE001
             iris_response["DATE_OBS"] = None
         time_obs = np.array([time_obs.value])
-        # Convert C_F_TIME to array of time objects while conserving shape.
-        c_f_time = np.empty(iris_response["C_F_TIME"].shape, dtype=object)
-        for i, row in enumerate(iris_response["C_F_TIME"]):
-            for j, t in enumerate(row):
-                c_f_time[i][j] = parse_time(t, format="utime")
-        iris_response["C_F_TIME"] = c_f_time
-        # Convert C_F_LAMBDA to Quantity.
+        iris_response["C_F_TIME"] = Time(iris_response["C_F_TIME"], format="utime")
         iris_response["C_F_LAMBDA"] = Quantity(iris_response["C_F_LAMBDA"], unit="nm")
-        # Convert C_N_TIME to array of time objects while
-        # conserving shape.
-        c_n_time = np.empty(iris_response["C_N_TIME"].shape, dtype=object)
-        for i, row in enumerate(iris_response["C_N_TIME"]):
-            for j, t in enumerate(row):
-                c_n_time[i][j] = parse_time(t, format="utime")
-        iris_response["C_N_TIME"] = c_n_time
-        # Convert C_N_LAMBDA to Quantity.
+        iris_response["C_N_TIME"] = Time(iris_response["C_N_TIME"], format="utime")
         iris_response["C_N_LAMBDA"] = Quantity(iris_response["C_N_LAMBDA"], unit="nm")
-        # Convert C_S_TIME to array of time objects while
-        # conserving shape.
-        c_s_time = np.empty(iris_response["C_S_TIME"].shape, dtype=object)
-        for i, row in enumerate(iris_response["C_S_TIME"]):
-            for j, column in enumerate(row):
-                for k, t in enumerate(column):
-                    c_s_time[i][j][k] = parse_time(t, format="utime")
-        iris_response["C_S_TIME"] = c_s_time
-        # Convert DATE in ELEMENTS array to array of time objects.
-        for i, t in enumerate(iris_response["ELEMENTS"]["DATE"]):
-            iris_response["ELEMENTS"]["DATE"][i] = parse_time(t, format="iso")
-            # Convert VERSION_DATE to time object.
-            iris_response["VERSION_DATE"] = parse_time(iris_response["VERSION_DATE"])
-    if int(iris_response["VERSION"]) < 2:
-        # Change DATE tag in data with version < 2 to VERSION_DATE to
+        iris_response["C_S_TIME"] = Time(iris_response["C_S_TIME"], format="utime")
+        iris_response["ELEMENTS"]["DATE"] = parse_time(iris_response["ELEMENTS"]["DATE"].astype(str).tolist())
+        iris_response["VERSION_DATE"] = parse_time(iris_response["VERSION_DATE"])
+    if iris_response["VERSION"] <= 2:
+        # Change DATE tag in data with version <= 2 to VERSION_DATE to
         # be consistent with more recent versions.
         iris_response["VERSION_DATE"] = Time(
             datetime.datetime(
                 int(iris_response["DATE"][0:4]),
                 int(iris_response["DATE"][4:6]),
                 int(iris_response["DATE"][6:8]),
-            )
+            ),
         )
         del iris_response["DATE"]
-    if int(iris_response["VERSION"]) > 2 and time_obs is not None:
+    if iris_response["VERSION"] > 2 and time_obs is not None:
         try:
             n_time_obs = len(time_obs)
-        except Exception:
+        except Exception:  # NOQA: BLE001
             n_time_obs = 1
         iris_response["AREA_SG"] = np.zeros(iris_response["AREA_SG"].shape)
         iris_response["AREA_SJI"] = np.zeros(iris_response["AREA_SJI"].shape)
-        # 1. FUV SG effective areas
+        # FUV SG effective areas
         lambran_fuv = np.array([[133.1, 135.9], [138.8, 140.8]])
         # Rough SG spectral ranges.  Setting effective area to 0 outside of these.
         shp_fuv = iris_response["COEFFS_FUV"].shape
         # Time-dependent response for shp_0[0] = 3 wavelengths
         iris_fit_fuv = np.zeros((n_time_obs, shp_fuv[0]))
         for j in range(shp_fuv[0]):
             iris_fit_fuv[:, j] = fit_iris_xput(
@@ -176,17 +153,17 @@
                 iris_response["COEFFS_NUV"][j, :, :],
             )
         # Interpolate onto lambda grid
         w_nuv = np.where(
             np.logical_and(
                 iris_response["LAMBDA"].value >= lambran_nuv[0],
                 iris_response["LAMBDA"].value <= lambran_nuv[1],
-            )
+            ),
         )
-        if int(iris_response["VERSION"]) <= 3:
+        if iris_response["VERSION"] <= 3:
             for k in range(n_time_obs):
                 interpol_nuv = scipy.interpolate.interp1d(
                     iris_response["C_N_LAMBDA"][:],
                     np.squeeze(iris_fit_nuv[k, :]),
                     fill_value="extrapolate",
                 )
                 iris_response["AREA_SG"][1, w_nuv] = interpol_nuv(iris_response["LAMBDA"][w_nuv])
@@ -196,33 +173,32 @@
                     iris_response["C_N_LAMBDA"][:],
                     np.squeeze(iris_fit_nuv[k, :]),
                     extrapolate=True,
                     bc_type="natural",
                     axis=0,
                 )
                 iris_response["AREA_SG"][1, w_nuv] = interpol_nuv(iris_response["LAMBDA"][w_nuv])
-        # 3. SJI effective areas
-        if int(iris_response["VERSION"]) <= 3:  # Meaning for version 3 only
-            shp_sji = iris_response["COEFFS_SJI"].shape
-            for j in range(shp_sji[0]):
+        # SJI effective areas
+        if 2 < iris_response["VERSION"] < 4:  # Version 3 only
+            for j in range(iris_response["COEFFS_SJI"].shape[0]):
                 # Calculate pre-launch area from the individual elements
                 prelaunch_area = iris_response["GEOM_AREA"]
                 for k in range(len(iris_response["INDEX_EL_SJI"][j, :])):
                     index_values0 = iris_response["INDEX_EL_SJI"][j, k]
                     prelaunch_area = prelaunch_area * iris_response["ELEMENTS"][index_values0].trans
                 # Time dependent response
                 iris_fit_sji = fit_iris_xput(
                     time_obs,
                     iris_response["C_S_TIME"][j, :, :],
                     iris_response["COEFFS_SJI"][j, :, :],
                 )
-                # Time dependetn profiles
+                # Time dependent profiles
                 for k in range(n_time_obs):
                     iris_response["AREA_SJI"][j, :] = prelaunch_area * iris_fit_sji[k]
-        else:  # For version 4 and above
+        else:  # Version 4 and above
             for nuv in range(2):
                 # Calculate baseline SJI area curves
                 area_sji = iris_response["GEOM_AREA"]
                 for m in range(len(iris_response["INDEX_EL_SJI"][nuv * 2, :])):
                     index_values1 = iris_response["INDEX_EL_SJI"][nuv * 2 : nuv * 2 + 2, m]
                     area_sji = area_sji * iris_response["ELEMENTS"][index_values1].trans
                 # Apply time dependent profile shape adjustment to FUV SJI
@@ -232,15 +208,15 @@
                     weight = np.array([2.4, 1.0])  # Typical solar ratio CII : SiIV
                     wavelength = iris_response["C_F_LAMBDA"]
                     n_wavelength = len(wavelength)
                     wavelength = np.array(
                         [
                             wavelength[0].value,
                             (wavelength[n_wavelength - 2].value * 2.0 + wavelength[n_wavelength - 1].value) / 3.0,
-                        ]
+                        ],
                     )  # 2 wavelengths in nm
                     # Calculate baseline SG area for scaling purposes
                     area_sg = iris_response["GEOM_AREA"]
                     for n in range(len(iris_response["INDEX_EL_SG"][nuv, :])):
                         index_values2 = iris_response["INDEX_EL_SG"][nuv, n]
                         area_sg = area_sg * iris_response["ELEMENTS"][index_values2].trans
                     # SG and SJI areas at wavelength
@@ -255,38 +231,38 @@
                         interpol_sji = scipy.interpolate.interp1d(
                             iris_response["LAMBDA"],
                             np.squeeze(area_sji[n]),
                             fill_value="extrapolate",
                         )
                         area_sj2[n, :] = interpol_sji(wavelength)
                     # Calculate the normalized slant function scal, apply to asji
-                    for n in range(n_time_obs):
+                    for _ in range(n_time_obs):
                         # Best-estimate slant, i.e., eff.area @ wavelength / baseline SG @ wavelength
                         interpol_sg2 = scipy.interpolate.interp1d(
                             iris_response["LAMBDA"],
                             np.squeeze(iris_response["AREA_SG"][0, :]),
                             fill_value="extrapolate",
                         )
                         sca2 = interpol_sg2(wavelength) / area_sg2
                         # Normalize slant so that total(wei*asj2*sca2)/total(wei*asj2)=1
                         for m in range(2):
                             sca2n = sca2 * np.sum(weight * area_sj2[m, :]) / np.sum(weight * area_sj2[m, :] * sca2)
                             interpol_sca = scipy.interpolate.interp1d(
-                                wavelength, np.squeeze(sca2n), fill_value="extrapolate"
+                                wavelength,
+                                np.squeeze(sca2n),
+                                fill_value="extrapolate",
                             )
                             sca1n = interpol_sca(iris_response["LAMBDA"])
                             sca1n = np.clip(sca1n, a_min=0, a_max=None)
                             iris_response["AREA_SJI"][m] = area_sji[m] * sca1n
                 else:
-                    # NUV: essentially same calculation as r.version=3
-                    for n in range(n_time_obs):
-                        iris_response["AREA_SJI"] = [
-                            Quantity(x, unit=u.cm**2) for x in iris_response["AREA_SJI"]
-                        ]
-                        area_sji = [x for x in area_sji]
+                    # NUV: essentially same calculation as version = 3
+                    for _ in range(n_time_obs):
+                        iris_response["AREA_SJI"] = [Quantity(x, unit=u.cm**2) for x in iris_response["AREA_SJI"]]
+                        area_sji = list(area_sji)
                         iris_response["AREA_SJI"][2:4] = area_sji[:]
             for j in range(4):
                 # SJI specific time dependency
                 iris_fit_sji = fit_iris_xput(
                     time_obs,
                     iris_response["C_S_TIME"][j, :, :],
                     iris_response["COEFFS_SJI"][j, :, :],
@@ -326,31 +302,28 @@
 
     Returns
     -------
     `numpy.array`
         Yields the fit used to compute the effective area using the input times ``time_obs``.
     """
     time_obs = Time(parse_time(time_obs).utime, format="utime")
-    size_time_cal_coeffs = time_cal_coeffs.shape
-    size_cal_coeffs = cal_coeffs.shape
-    if size_time_cal_coeffs[1] != 2 or size_cal_coeffs[1] < 2:
+    if time_cal_coeffs.shape[1] != 2 or cal_coeffs.shape[1] < 2:
         # Raise ValueError as time coefficient have the wrong format.
         raise ValueError("Incorrect number of elements either in time_cal_coeffs or in cal_coeffs.")
     # Some time transformations.
     # Convert the time_cal_coeffs given in the .geny file into a ``astropy.time.Time``
     # object called t_cal_coeffs, so that the time differences will be in days...
-    t_cal_coeffs_flat = time_cal_coeffs.flatten()
-    t_cal_coeffs = t_cal_coeffs_flat.reshape(size_time_cal_coeffs)
+    t_cal_coeffs = time_cal_coeffs.flatten().reshape(time_cal_coeffs.shape)
     # Exponent for transition between exp.decay intervals.
     transition_exp = 1.5
     # For loop for carrying out the least-squares fit and computation of fit output.
     fit_out = np.zeros(len(time_obs))
     for i, t in enumerate(time_obs):
-        aux_cal_coeffs = np.zeros(2 * size_time_cal_coeffs[0])
-        fit_out = np.zeros(len(list(time_obs)), dtype=np.float64)
+        aux_cal_coeffs = np.zeros(2 * time_cal_coeffs.shape[0])
+        fit_out = np.zeros(len(list(time_obs)))
         # Looking for the closest time in the calibration time intervals.
         # Differences are given in years before passing to the next stage.
         t_diff = Time(t, format="utime") - t_cal_coeffs
         t_diff = t_diff.flatten()
         # To convert to an array, quantities need to be dimensionless, hence dividing out the unit.
         t_diff = np.array([x.to(u.year).value for x in t_diff])
         idx = np.where(t_diff < 0)[0]
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/spectrograph.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/spectrograph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     -------
     `list` of `numpy.ndarray`
         Data arrays converted to new_unit.
     `astropy.unit.Unit`
         Unit of new data arrays with any inverse time component preserved.
     """
     if old_unit == new_unit or old_unit == new_unit / u.s:
-        new_data_arrays = [data for data in old_data_arrays]
+        new_data_arrays = list(old_data_arrays)
         new_unit_time_accounted = old_unit
     else:
         # During calculations, the time component due to exposure
         # time correction, if it has been applied, is ignored.
         # Check here whether the time correction is present in the
         # original unit so that is carried through to new unit.
         if u.s not in (old_unit * u.s).decompose().bases:
@@ -64,14 +64,15 @@
     data_quantities,
     time_obs,
     response_version,
     obs_wavelength,
     detector_type,
     spectral_dispersion_per_pixel,
     solid_angle,
+    *,
     undo=False,
 ):
     """
     Converts data quantities from counts/s to radiance (or vice versa).
 
     Parameters
     ----------
@@ -109,36 +110,37 @@
     # Check data quantities are in the right units.
     if undo is True:
         for i, data in enumerate(data_quantities):
             if not data.unit.is_equivalent(RADIANCE_UNIT):
                 raise ValueError(
                     "Invalid unit provided.  As kwarg undo=True, "
                     "unit must be equivalent to {}.  Error found for {}th element "
-                    "of data_quantities. Unit: {}".format(RADIANCE_UNIT, i, data.unit)
+                    "of data_quantities. Unit: {}".format(RADIANCE_UNIT, i, data.unit),
                 )
     else:
         for data in data_quantities:
             if data.unit != u.photon / u.s:
                 raise ValueError(
                     "Invalid unit provided.  As kwarg undo=False, "
                     "unit must be equivalent to {}.  Error found for {}th element "
-                    "of data_quantities. Unit: {}".format(u.photon / u.s, i, data.unit)
+                    "of data_quantities. Unit: {}".format(u.photon / u.s, i, data.unit),
                 )
     photons_per_sec_to_radiance_factor = calculate_photons_per_sec_to_radiance_factor(
         time_obs,
         response_version,
         obs_wavelength,
         detector_type,
         spectral_dispersion_per_pixel,
         solid_angle,
     )
     # Change shape of arrays so they are compatible for broadcasting
     # with data and uncertainty arrays.
     photons_per_sec_to_radiance_factor = reshape_1D_wavelength_dimensions_for_broadcast(
-        photons_per_sec_to_radiance_factor, data_quantities[0].ndim
+        photons_per_sec_to_radiance_factor,
+        data_quantities[0].ndim,
     )
     # Perform (or undo) radiometric conversion.
     if undo is True:
         new_data_quantities = [
             (data / photons_per_sec_to_radiance_factor).to(u.photon / u.s) for data in data_quantities
         ]
     else:
@@ -184,15 +186,18 @@
     -------
     `astropy.units.Quantity`
         Mutliplicative conversion factor from counts/s to radiance units
         for input wavelengths.
     """
     # Get effective area and interpolate to observed wavelength grid.
     eff_area_interp = get_interpolated_effective_area(
-        time_obs, response_version, detector_type, obs_wavelength=wavelength
+        time_obs,
+        response_version,
+        detector_type,
+        obs_wavelength=wavelength,
     )
     # Return radiometric conversed data assuming input data is in units of photons/s.
     return (
         constants.h
         * constants.c
         / wavelength
         / u.photon
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_response.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import os.path
+from pathlib import Path
 
 import numpy as np
 import numpy.testing as np_test
 import pytest
 import scipy.io
 from sunpy.time import parse_time
 
 from irispy import utils
 from irispy.data.test import rootdir
 
 # Arrays for the fit_iris_xput method
-r = os.path.join(rootdir, "..", "iris_sra_c_20161022.geny")
-raw_response_data = scipy.io.readsav(r, python_dict=True, verbose=False)
-iris_response = dict([(name, raw_response_data["p0"][name][0]) for name in raw_response_data["p0"].dtype.names])
+raw_response_data = scipy.io.readsav(Path(rootdir) / ".." / "iris_sra_c_20161022.geny", python_dict=True, verbose=False)
+iris_response = {name: raw_response_data["p0"][name][0] for name in raw_response_data["p0"].dtype.names}
 time_obs = [parse_time("2013-09-03")]
 time_cal_coeffs0 = parse_time(iris_response.get("C_F_TIME"), format="utime")
 time_cal_coeffs1 = parse_time(iris_response.get("C_N_TIME"), format="utime")
 cal_coeffs0 = iris_response.get("COEFFS_FUV")[0, :, :]
 cal_coeffs1 = iris_response.get("COEFFS_FUV")[1, :, :]
 cal_coeffs2 = iris_response.get("COEFFS_FUV")[2, :, :]
 cal_coeffs3 = iris_response.get("COEFFS_NUV")[0, :, :]
@@ -35,102 +34,72 @@
 def test_get_iris_response_greater_than_6():
     with pytest.raises(KeyError):
         utils.get_iris_response(time_obs, response_version=13)
 
 
 # Tests for get_iris_response function
 # Version 1
-sav_file_path1 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version001.sav")
+sav_file_path1 = Path(rootdir) / "idl_iris_get_response_20130903_new_version001.sav"
 test_iris_response1 = scipy.io.readsav(sav_file_path1, python_dict=True, verbose=False)
 iris_response_load1 = test_iris_response1["iris_response"][0]
 area_sg_load1 = iris_response_load1.area_sg
 area_sji_load1 = iris_response_load1.area_sji
 
 # Version 2
-sav_file_path2 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version002.sav")
+sav_file_path2 = Path(rootdir) / "idl_iris_get_response_20130903_new_version002.sav"
 test_iris_response2 = scipy.io.readsav(sav_file_path2, python_dict=True, verbose=False)
 iris_response_load2 = test_iris_response2["iris_response"][0]
 area_sg_load2 = iris_response_load2.area_sg
 area_sji_load2 = iris_response_load2.area_sji
 
 # Version 3
-sav_file_path3 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version003.sav")
+sav_file_path3 = Path(rootdir) / "idl_iris_get_response_20130903_new_version003.sav"
 
 test_iris_response3 = scipy.io.readsav(sav_file_path3, python_dict=True, verbose=False)
 iris_response_load3 = test_iris_response3["iris_response"][0]
 area_sg_load3 = iris_response_load3.area_sg
 area_sji_load3 = iris_response_load3.area_sji
 
 # Version 4
-sav_file_path4 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version004.sav")
+sav_file_path4 = Path(rootdir) / "idl_iris_get_response_20130903_new_version004.sav"
 test_iris_response4 = scipy.io.readsav(sav_file_path4, python_dict=True, verbose=False)
 iris_response_load4 = test_iris_response4["iris_response"][0]
 area_sg_load4 = iris_response_load4.area_sg
 area_sji_load4 = iris_response_load4.area_sji
 
 # Version 5
-sav_file_path5 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version005.sav")
+sav_file_path5 = Path(rootdir) / "idl_iris_get_response_20130903_new_version005.sav"
 test_iris_response5 = scipy.io.readsav(sav_file_path5, python_dict=True, verbose=False)
 iris_response_load5 = test_iris_response5["iris_response"][0]
 area_sg_load5 = iris_response_load5.area_sg
 area_sji_load5 = iris_response_load5.area_sji
 
 # Version 6
-sav_file_path6 = os.path.join(rootdir, "idl_iris_get_response_20130903_new_version006.sav")
+sav_file_path6 = Path(rootdir) / "idl_iris_get_response_20130903_new_version006.sav"
 test_iris_response6 = scipy.io.readsav(sav_file_path6, python_dict=True, verbose=False)
 iris_response_load6 = test_iris_response6["iris_response"][0]
 area_sg_load6 = iris_response_load6.area_sg
 area_sji_load6 = iris_response_load6.area_sji
 
 
-@pytest.fixture
-def iris_responsev1():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=1)
-
-
 def test_get_iris_response_version1(iris_responsev1):
     np_test.assert_almost_equal(iris_responsev1["AREA_SG"].value, area_sg_load1, decimal=6)
     np_test.assert_almost_equal(iris_responsev1["AREA_SJI"].value, area_sji_load1, decimal=6)
 
 
-@pytest.fixture
-def iris_responsev2():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=2)
-
-
 def test_get_iris_response_version2(iris_responsev2):
     np_test.assert_almost_equal(iris_responsev2["AREA_SG"].value, area_sg_load2, decimal=6)
     np_test.assert_almost_equal(iris_responsev2["AREA_SJI"].value, area_sji_load2, decimal=6)
 
 
-@pytest.fixture
-def iris_responsev3():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=3)
-
-
 def test_get_iris_response_version3(iris_responsev3):
     np_test.assert_almost_equal(iris_responsev3["AREA_SG"].value, area_sg_load3, decimal=6)
     np_test.assert_almost_equal(iris_responsev3["AREA_SJI"].value, area_sji_load3, decimal=6)
 
 
-@pytest.fixture
-def iris_responsev4():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=4)
-
-
-@pytest.fixture
-def iris_responsev5():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=5)
-
-
-@pytest.fixture
-def iris_responsev6():
-    return utils.get_iris_response(time_obs=parse_time("2013-09-03"), response_version=6)
-
-
 def test_get_iris_response_version4(iris_responsev4):
     np_test.assert_almost_equal(iris_responsev4["AREA_SG"].value, area_sg_load4, decimal=3)
     np_test.assert_almost_equal(iris_responsev4["AREA_SJI"].value, area_sji_load4, decimal=3)
 
 
 def test_get_iris_response_version5(iris_responsev5):
     np_test.assert_almost_equal(iris_responsev5["AREA_SG"].value, area_sg_load5, decimal=3)
@@ -139,15 +108,15 @@
 
 def test_get_iris_response_version6(iris_responsev6):
     np_test.assert_almost_equal(iris_responsev6["AREA_SG"].value, area_sg_load6, decimal=3)
     np_test.assert_almost_equal(iris_responsev6["AREA_SJI"].value, area_sji_load6, decimal=3)
 
 
 @pytest.mark.parametrize(
-    "input_arrays, expected_array",
+    ("input_arrays", "expected_array"),
     [
         ([time_obs, time_cal_coeffs0, cal_coeffs0], iris_fit_expected0),
         ([time_obs, time_cal_coeffs0, cal_coeffs1], iris_fit_expected1),
         ([time_obs, time_cal_coeffs0, cal_coeffs2], iris_fit_expected2),
         ([time_obs, time_cal_coeffs1, cal_coeffs3], iris_fit_expected3),
         ([time_obs, time_cal_coeffs1, cal_coeffs4], iris_fit_expected4),
         ([time_obs, time_cal_coeffs1, cal_coeffs5], iris_fit_expected5),
@@ -159,15 +128,15 @@
         utils.fit_iris_xput(input_arrays[0], input_arrays[1], input_arrays[2]),
         expected_array,
         decimal=6,
     )
 
 
 def test_fixed_time():
-    sav_file_path6 = os.path.join(rootdir, "test_response.sav")
+    sav_file_path6 = Path(rootdir) / "test_response.sav"
     response = scipy.io.readsav(sav_file_path6, python_dict=True, verbose=False)
     response = response["test"][0]
     area_sg = response.area_sg
     area_sji = response.area_sji
     python_response = utils.get_iris_response(parse_time("2013-08-31"), response_version=6)
     np_test.assert_almost_equal(python_response["AREA_SG"].value, area_sg, decimal=3)
     np_test.assert_almost_equal(python_response["AREA_SJI"].value, area_sji, decimal=3)
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_spectrograph.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_spectrograph.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 SOURCE_DATA_PHOTONS_SJI_1 = np.array([[18, 36, 54], [72, 90, 108]])
 
 single_exposure_time = 2.0
 EXPOSURE_TIME = np.zeros(3) + single_exposure_time
 
 
 @pytest.mark.parametrize(
-    "data_arrays, old_unit, new_unit, expected_data_arrays, expected_unit",
+    ("data_arrays", "old_unit", "new_unit", "expected_data_arrays", "expected_unit"),
     [
         (
             [SOURCE_DATA_DN, SOURCE_DATA_DN],
             DN_UNIT["FUV"],
             u.photon,
             [SOURCE_DATA_PHOTONS_FUV, SOURCE_DATA_PHOTONS_FUV],
             u.photon,
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/tests/test_utils.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,48 @@
 
 from irispy import utils
 
 data_dust = np.array(
     [
         [[-1, 2, -3, 4], [2, -200, 5, 3], [0, 1, 2, -300]],
         [[2, -200, 5, 1], [10, -5, 2, 2], [10, -3, 3, 0]],
-    ]
+    ],
 )
 dust_mask_expected = np.array(
     [
         [
             [True, True, True, True],
             [True, True, True, True],
             [True, True, False, False],
         ],
         [[True, True, True, False], [True, True, True, True], [True, True, True, True]],
-    ]
+    ],
 )
 
 
 @pytest.mark.parametrize(
-    "test_input, expected_output",
+    ("test_input", "expected_output"),
     [
         ({"detector type": "FUV1"}, "FUV"),
         ({"detector type": "NUV"}, "NUV"),
         ({"detector type": "SJI"}, "SJI"),
     ],
 )
 def test_get_detector_type(test_input, expected_output):
     assert utils.get_detector_type(test_input) == expected_output
 
 
-@pytest.mark.parametrize("input_array, expected_array", [(data_dust, dust_mask_expected)])
+@pytest.mark.parametrize(("input_array", "expected_array"), [(data_dust, dust_mask_expected)])
 def test_calculate_dust_mask(input_array, expected_array):
     np_test.assert_array_equal(utils.calculate_dust_mask(input_array), expected_array)
 
 
 def test_get_iris_response_version():
     # For now just checks the code runs
     start_obs = parse_time("2013-07-20T17:10:23")
     obs_wavelength = np.linspace(1400.5, 1404.9915000926703, num=692, endpoint=True)
     utils.get_interpolated_effective_area(
-        start_obs, response_version=6, detector_type="FUV", obs_wavelength=obs_wavelength * u.Angstrom
+        start_obs,
+        response_version=6,
+        detector_type="FUV",
+        obs_wavelength=obs_wavelength * u.Angstrom,
     )
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy/utils/utils.py` & `irispy-lmsal-0.2.0rc4/irispy/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 This module provides general utility functions.
 """
-import shutil
 import numbers
-import tarfile
-from pathlib import Path
 
 import astropy.units as u
 import numpy as np
-import requests
 from astropy.modeling.models import custom_model
 from scipy import interpolate, ndimage
 
 from irispy.utils.response import get_iris_response
 
 __all__ = [
     "get_detector_type",
@@ -20,31 +16,14 @@
     "calculate_dust_mask",
     "gaussian1d_on_linear_bg",
     "image_clipping",
     "calculate_uncertainty",
 ]
 
 
-def _download_data(urls: list):
-    """
-    This only should be called in the irispy-lmsal example gallery.
-
-    THIS IS NOT A USER FACING FUNCTION TO DOWNLOAD DATA.
-    """
-    for url in urls:
-        filename = url.split("/")[-1]
-        if not Path(filename).exists():
-            with requests.get(url, stream=True) as r:
-                with open(filename, "wb") as f:
-                    shutil.copyfileobj(r.raw, f)
-        if ".tar.gz" in filename:
-            with tarfile.open(filename, "r") as tar:
-                tar.extractall(Path(filename).parent)
-
-
 def image_clipping(image, cutoff=1.5e-3, gamma=1.0):
     """
     Computes and returns the min and max values of the input (image), clipping
     brightest and darkest pixels.
 
     Parameters
     ----------
@@ -69,15 +48,15 @@
         hist = np.histogram(image, bins=nbins)
         fak = 1
     else:
         nbins = 10000
         fak = nbins / (hmax - hmin)
         hist = np.histogram((image - hmin) * fak, range=(0.0, float(nbins)), bins=nbins)
     h = hist[0]
-    bin = hist[1]
+    bins = hist[1]
     nh = np.size(h)
     # Integrate the histogram so that h(i) holds the number of points
     # with equal or lower intensity.
     for i in range(1, nh - 1):
         h[i] = h[i] + h[i - 1]
     h = h / float(h[nh - 2])
     h[nh - 1] = 1
@@ -85,16 +64,16 @@
     # vmin/vmax are the indices of the point where the number of pixels
     # with lower/higher intensity reach the given limit. This has to be
     # converted to a real image value by dividing by the scalefactor
     # fak and adding the min value of the image
     # Note that the bottom value is taken off (addition of h[0] to cutoff),
     # there are often very many points in IRIS images that are set to zero, this
     # removes them from calculation... and seems to work.
-    vmin = (np.max(np.where(h <= (cutoff + h[0]), bin[1:] - bin[0], 0)) / fak + hmin) ** gamma
-    vmax = (np.min(np.where(h >= (1.0 - cutoff), bin[1:] - bin[0], nh - 2)) / fak + hmin) ** gamma
+    vmin = (np.max(np.where(h <= (cutoff + h[0]), bins[1:] - bins[0], 0)) / fak + hmin) ** gamma
+    vmax = (np.min(np.where(h >= (1.0 - cutoff), bins[1:] - bins[0], nh - 2)) / fak + hmin) ** gamma
     return vmin, vmax
 
 
 @custom_model
 def gaussian1d_on_linear_bg(
     x,
     amplitude=None,
@@ -166,37 +145,34 @@
     # at which the data is recorded:
     eff_area_interp_base_unit = u.Angstrom
     tck = interpolate.splrep(
         response_wavelength.to(eff_area_interp_base_unit).value,
         eff_area.to(eff_area_interp_base_unit**2).value,
         s=0,
     )
-    eff_area_interp = interpolate.splev(obs_wavelength.to(eff_area_interp_base_unit).value, tck) * (
-        eff_area_interp_base_unit**2
-    )
-    return eff_area_interp
+    return interpolate.splev(obs_wavelength.to(eff_area_interp_base_unit).value, tck) * eff_area_interp_base_unit**2
 
 
 def calculate_dust_mask(data_array):
     """
     Calculate a mask with the dust positions in a given array.
 
     Parameters
     ----------
     data_array : `numpy.ndarray`
-        This array contains some dust poisition that will be calculated. The array
+        This array contains some dust position that will be calculated. The array
         must have scaled values.
 
     Returns
     -------
     `numpy.ndarray` of `bool`
         This array has the same shape than data_array and contains the dust positions
         when the value is True.
     """
-    # Creating a mask with the same shape than the inputed data array.
+    # Creating a mask with the same shape than the inputted data array.
     mask = np.zeros_like(data_array, dtype=bool)
     # Set the pixel value to True is the pixel is recognized as a dust pixel.
     mask[(data_array < 0.5) & (data_array > -200)] = True
     # Extending the mask to avoid the neighbours pixel influenced by the dust pixels.
     struct = np.array([np.zeros((3, 3)), np.ones((3, 3)), np.zeros((3, 3))], dtype=bool)
     mask = ndimage.binary_dilation(mask, structure=struct).astype(mask.dtype)
     return mask
@@ -207,15 +183,15 @@
     Calculates the uncertainty of a given data array.
 
     Parameters
     ----------
     data : np.array
         The data array.
     readout_noise : u.Quantity
-        The readout noise, needs to be a unit that is convertable to photon.
+        The readout noise, needs to be a unit that is convertible to photon.
     unit : u.Quantity
         The final unit that the value should be converted to.
 
     Returns
     -------
     float
         The readout noise with no unit.
```

### Comparing `irispy-lmsal-0.2.0rc3/irispy_lmsal.egg-info/SOURCES.txt` & `irispy-lmsal-0.2.0rc4/irispy_lmsal.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 .codecov.yaml
+.gitattributes
 .gitignore
-.gitlab-ci.yml
 .pre-commit-config.yaml
 .readthedocs.yml
+.rtd-environment.yml
 CHANGELOG.rst
 LICENSE.rst
-MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
+.github/workflows/ci.yml
 changelog/README.rst
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/guide.rst
-docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/known_issues.rst
 docs/make.bat
 docs/rtd_requirements.txt
-docs/code_api/index.rst
-docs/code_api/sji.rst
-docs/code_api/spectrograph.rst
-docs/code_api/utils.rst
+docs/reference/index.rst
+docs/reference/irispy.rst
+docs/reference/sji.rst
+docs/reference/spectrograph.rst
+docs/reference/utils.rst
 examples/README.txt
+examples/align_iris_aia_rolled.py
 examples/mg_ii_dopplergrams.py
-examples/overview.py
-examples/timeseries_analysis.py
+examples/raster.py
+examples/skip_umbral_flashes.py
+examples/south_sji.py
 irispy/__init__.py
 irispy/_version.py
+irispy/conftest.py
 irispy/obsid.py
 irispy/sji.py
 irispy/spectrograph.py
 irispy/version.py
 irispy/visualization.py
+irispy/_dev/__init__.py
+irispy/_dev/scm_version.py
 irispy/data/README.rst
 irispy/data/__init__.py
 irispy/data/_sample.py
 irispy/data/iris_sg_psfs.geny
 irispy/data/iris_sra_20130211.geny
 irispy/data/iris_sra_20130715.geny
 irispy/data/iris_sra_c_20150331.geny
 irispy/data/iris_sra_c_20161022.geny
 irispy/data/iris_sra_c_20191101.geny
 irispy/data/iris_sra_c_20200223.geny
 irispy/data/sample.py
+irispy/data/v34-table10.csv
+irispy/data/v34-table2000.csv
 irispy/data/v36-table10.csv
 irispy/data/v36-table2000.csv
 irispy/data/v38-table10.csv
 irispy/data/v38-table2000.csv
 irispy/data/v40-table10.csv
 irispy/data/v40-table2000.csv
 irispy/data/test/__init__.py
 irispy/data/test/compress.py
 irispy/data/test/idl_iris_get_response_20130903_new_version001.sav
 irispy/data/test/idl_iris_get_response_20130903_new_version002.sav
 irispy/data/test/idl_iris_get_response_20130903_new_version003.sav
 irispy/data/test/idl_iris_get_response_20130903_new_version004.sav
 irispy/data/test/idl_iris_get_response_20130903_new_version005.sav
 irispy/data/test/idl_iris_get_response_20130903_new_version006.sav
-irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_1330_t000.fits
-irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_1400_t000.fits
-irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_2796_t000.fits
-irispy/data/test/iris_l2_20170502_052551_3893010094_SJI_2832_t000.fits
-irispy/data/test/iris_l2_20170502_052551_3893010094_raster_t000_r00000.fits
+irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_1330_t000_test.fits
+irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_1400_t000_test.fits
+irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_2796_t000_test.fits
+irispy/data/test/iris_l2_20210905_001833_3620258102_SJI_2832_t000_test.fits
+irispy/data/test/iris_l2_20210905_001833_3620258102_raster_t000_r00000_test.fits
 irispy/data/test/test_response.sav
 irispy/io/__init__.py
 irispy/io/sji.py
 irispy/io/spectrograph.py
 irispy/io/utils.py
 irispy/io/tests/__init__.py
 irispy/io/tests/test_utils.py
@@ -90,12 +96,9 @@
 irispy/utils/tests/test_response.py
 irispy/utils/tests/test_spectrograph.py
 irispy/utils/tests/test_utils.py
 irispy/utils/tests/test_wobble.py
 irispy_lmsal.egg-info/PKG-INFO
 irispy_lmsal.egg-info/SOURCES.txt
 irispy_lmsal.egg-info/dependency_links.txt
-irispy_lmsal.egg-info/not-zip-safe
 irispy_lmsal.egg-info/requires.txt
-irispy_lmsal.egg-info/top_level.txt
-licenses/README.rst
-licenses/TEMPLATE_LICENSE.rst
+irispy_lmsal.egg-info/top_level.txt
```

### Comparing `irispy-lmsal-0.2.0rc3/tox.ini` & `irispy-lmsal-0.2.0rc4/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,41 @@
 [tox]
 envlist =
-    py{38,39,310}{,-oldestdeps,-devdeps,-online}
+    py{39,310,311}{,-oldestdeps,-devdeps,-online}
     build_docs
     codestyle
 isolated_build = true
 
 [testenv]
-pypi_filter = file://.test_package_pins.txt
-# We use bash in some of our enviroments so we have to whitelist it.
 whitelist_externals=
     /bin/bash
     /usr/bin/bash
-# Run the tests in a temporary directory to make sure that we don't import
-# irispy from the source tree
 changedir = .tmp/{envname}
-# tox environments are constructued with so-called 'factors' (or terms)
-# separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
-# will only take effect if that factor is included in the environment name. To
-# see a list of example environments that can be run, along with a description,
-# run:
-#
-#     tox -l -v
-#
 description =
     run tests
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     online: that require remote data
 setenv =
     MPLBACKEND = agg
     COLUMNS = 180
-    PYTEST_COMMAND = pytest -vvv -s -raR --pyargs irispy --cov-report=xml --cov=irispy --cov-config={toxinidir}/setup.cfg {toxinidir}/docs
-    py37: PYTEST_COMMAND = pytest -vvv -s -raR --pyargs irispy -p no:warnings --cov-report=xml --cov=irispy --cov-config={toxinidir}/setup.cfg {toxinidir}/docs
+    PYTEST_COMMAND = pytest -vvv -s -raR --pyargs irispy --cov-report=xml --cov=irispy {toxinidir}/docs
 deps =
-    # We need this for some packages.
-    setuptools
     # All our tests run in parallel which this plugin allows us to.
     pytest-xdist
     # We check codecov in tox builds.
     pytest-cov
-    # The devdeps factor is intended to be used to install the latest developer version.
-    # of key dependencies.
+    # The devdeps factor is intended to be used to install the latest developer version of key dependencies.
     devdeps: git+https://github.com/sunpy/sunraster
+    devdeps: git+https://github.com/sunpy/ndcube
     # Oldest deps we pin against.
-    oldestdeps: sunraster<0.3
+    oldestdeps: sunraster<0.5
     # These are specific online extras we use to run the online tests.
     online: pytest-rerunfailures
     online: pytest-timeout
-# The following indicates which extras_require from setup.cfg will be installed
-# dev is special in that it installs everything
 extras =
     dev
 commands =
     !online: {env:PYTEST_COMMAND} {posargs}
     online: {env:PYTEST_COMMAND} --reruns 2 --timeout=180 --remote-data=any {posargs}
 
 [testenv:build_docs]
@@ -60,15 +43,14 @@
 description = Invoke sphinx-build to build the HTML docs
 extras = dev
 commands =
     sphinx-build --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
     python -c 'import pathlib; print("Documentation available under file://\{0\}".format(pathlib.Path(r"{toxinidir}") / "docs" / "_build" / "index.html"))'
 
 [testenv:codestyle]
-pypi_filter =
 skip_install = true
 description = Run all style and file checks with pre-commit
 deps =
     pre-commit
 commands =
     pre-commit install-hooks
-    pre-commit run --all-files
+    pre-commit run --color always --all-files --show-diff-on-failure
```

