# Comparing `tmp/control-0.9.3.post2.tar.gz` & `tmp/control-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-0.9.3.post2.tar", last modified: Sat Dec 31 21:38:16 2022, max compression
+gzip compressed data, was "control-0.9.4.tar", last modified: Sat Jun 10 05:20:15 2023, max compression
```

## Comparing `control-0.9.3.post2.tar` & `control-0.9.4.tar`

### file list

```diff
@@ -1,226 +1,241 @@
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.229843 control-0.9.3.post2/
--rw-r--r--   0 murray     (501) staff       (20)      310 2021-03-20 16:01:30.000000 control-0.9.3.post2/.coveragerc
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.157965 control-0.9.3.post2/.github/
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.162210 control-0.9.3.post2/.github/conda-env/
--rw-r--r--   0 murray     (501) staff       (20)       57 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/conda-env/build-env.yml
--rw-r--r--   0 murray     (501) staff       (20)      195 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/conda-env/test-env.yml
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.162702 control-0.9.3.post2/.github/scripts/
--rw-r--r--   0 murray     (501) staff       (20)      988 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/scripts/set-conda-test-matrix.py
--rw-r--r--   0 murray     (501) staff       (20)      865 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/scripts/set-pip-test-matrix.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.163333 control-0.9.3.post2/.github/workflows/
--rw-r--r--   0 murray     (501) staff       (20)     1139 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/workflows/control-slycot-src.yml
--rw-r--r--   0 murray     (501) staff       (20)      835 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/workflows/install_examples.yml
--rw-r--r--   0 murray     (501) staff       (20)    11114 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/workflows/os-blas-test-matrix.yml
--rw-r--r--   0 murray     (501) staff       (20)     2391 2022-12-31 16:37:24.000000 control-0.9.3.post2/.github/workflows/python-package-conda.yml
--rw-r--r--   0 murray     (501) staff       (20)      494 2022-05-28 16:49:31.000000 control-0.9.3.post2/.gitignore
--rw-r--r--   0 murray     (501) staff       (20)      495 2022-12-31 16:37:24.000000 control-0.9.3.post2/.readthedocs.yaml
--rw-r--r--   0 murray     (501) staff       (20)    40928 2017-01-05 06:40:35.000000 control-0.9.3.post2/ChangeLog
--rw-r--r--   0 murray     (501) staff       (20)     1536 2016-05-30 18:51:51.000000 control-0.9.3.post2/LICENSE
--rw-r--r--   0 murray     (501) staff       (20)       91 2022-12-31 16:37:24.000000 control-0.9.3.post2/MANIFEST.in
--rw-r--r--   0 murray     (501) staff       (20)     6957 2022-12-31 21:38:16.229549 control-0.9.3.post2/PKG-INFO
--rw-r--r--   0 murray     (501) staff       (20)     2725 2014-08-09 17:40:09.000000 control-0.9.3.post2/Pending
--rw-r--r--   0 murray     (501) staff       (20)     5788 2022-12-31 16:37:24.000000 control-0.9.3.post2/README.rst
--rw-r--r--   0 murray     (501) staff       (20)     6897 2021-03-20 16:01:30.000000 control-0.9.3.post2/asv.conf.json
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.164008 control-0.9.3.post2/benchmarks/
--rw-r--r--   0 murray     (501) staff       (20)     1420 2022-12-31 16:37:24.000000 control-0.9.3.post2/benchmarks/README
--rw-r--r--   0 murray     (501) staff       (20)        0 2021-03-20 16:01:30.000000 control-0.9.3.post2/benchmarks/__init__.py
--rw-r--r--   0 murray     (501) staff       (20)     5847 2022-12-31 16:37:24.000000 control-0.9.3.post2/benchmarks/flatsys_bench.py
--rw-r--r--   0 murray     (501) staff       (20)     8768 2022-12-31 16:37:24.000000 control-0.9.3.post2/benchmarks/optimal_bench.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.164405 control-0.9.3.post2/conda-recipe/
--rw-r--r--   0 murray     (501) staff       (20)      126 2015-10-18 15:36:15.000000 control-0.9.3.post2/conda-recipe/bld.bat
--rw-r--r--   0 murray     (501) staff       (20)      632 2018-01-13 06:22:26.000000 control-0.9.3.post2/conda-recipe/meta.yaml
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.173645 control-0.9.3.post2/control/
--rw-r--r--   0 murray     (501) staff       (20)     2888 2022-12-31 20:47:27.000000 control-0.9.3.post2/control/__init__.py
--rw-r--r--   0 murray     (501) staff       (20)      166 2022-12-31 21:38:15.000000 control-0.9.3.post2/control/_version.py
--rw-r--r--   0 murray     (501) staff       (20)    12276 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/bdalg.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.174548 control-0.9.3.post2/control/bench/
--rw-r--r--   0 murray     (501) staff       (20)      532 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/bench/time_freqresp.py
--rw-r--r--   0 murray     (501) staff       (20)    14023 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/canonical.py
--rw-r--r--   0 murray     (501) staff       (20)    11236 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/config.py
--rw-r--r--   0 murray     (501) staff       (20)     3634 2018-01-13 06:22:26.000000 control-0.9.3.post2/control/ctrlutil.py
--rw-r--r--   0 murray     (501) staff       (20)     3781 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/delay.py
--rw-r--r--   0 murray     (501) staff       (20)    18769 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/descfcn.py
--rw-r--r--   0 murray     (501) staff       (20)     5823 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/dtime.py
--rw-r--r--   0 murray     (501) staff       (20)     3336 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/exception.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.176411 control-0.9.3.post2/control/flatsys/
--rw-r--r--   0 murray     (501) staff       (20)     3001 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/__init__.py
--rw-r--r--   0 murray     (501) staff       (20)     4602 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/basis.py
--rw-r--r--   0 murray     (501) staff       (20)     3431 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/bezier.py
--rw-r--r--   0 murray     (501) staff       (20)     8452 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/bspline.py
--rw-r--r--   0 murray     (501) staff       (20)    36690 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/flatsys.py
--rw-r--r--   0 murray     (501) staff       (20)     6339 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/linflat.py
--rw-r--r--   0 murray     (501) staff       (20)     2789 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/poly.py
--rw-r--r--   0 murray     (501) staff       (20)     7985 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/flatsys/systraj.py
--rw-r--r--   0 murray     (501) staff       (20)    29516 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/frdata.py
--rw-r--r--   0 murray     (501) staff       (20)    71873 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/freqplot.py
--rw-r--r--   0 murray     (501) staff       (20)     7316 2020-12-28 19:51:09.000000 control-0.9.3.post2/control/grid.py
--rw-r--r--   0 murray     (501) staff       (20)   123770 2022-12-31 18:06:04.000000 control-0.9.3.post2/control/iosys.py
--rw-r--r--   0 murray     (501) staff       (20)    16853 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/lti.py
--rw-r--r--   0 murray     (501) staff       (20)    20213 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/margins.py
--rw-r--r--   0 murray     (501) staff       (20)    22814 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/mateqn.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.177012 control-0.9.3.post2/control/matlab/
--rw-r--r--   0 murray     (501) staff       (20)    18522 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/matlab/__init__.py
--rw-r--r--   0 murray     (501) staff       (20)     8864 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/matlab/timeresp.py
--rw-r--r--   0 murray     (501) staff       (20)     7003 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/matlab/wrappers.py
--rw-r--r--   0 murray     (501) staff       (20)    18210 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/modelsimp.py
--rw-r--r--   0 murray     (501) staff       (20)    20454 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/namedio.py
--rw-r--r--   0 murray     (501) staff       (20)    13196 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/nichols.py
--rw-r--r--   0 murray     (501) staff       (20)    60168 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/optimal.py
--rw-r--r--   0 murray     (501) staff       (20)     8928 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/passivity.py
--rw-r--r--   0 murray     (501) staff       (20)    12053 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/phaseplot.py
--rw-r--r--   0 murray     (501) staff       (20)     4711 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/pzmap.py
--rw-r--r--   0 murray     (501) staff       (20)    30443 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/rlocus.py
--rw-r--r--   0 murray     (501) staff       (20)    10483 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/robust.py
--rw-r--r--   0 murray     (501) staff       (20)    15207 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/sisotool.py
--rw-r--r--   0 murray     (501) staff       (20)    38464 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/statefbk.py
--rw-r--r--   0 murray     (501) staff       (20)    72995 2022-12-31 18:06:04.000000 control-0.9.3.post2/control/statesp.py
--rw-r--r--   0 murray     (501) staff       (20)    22087 2022-12-31 18:06:04.000000 control-0.9.3.post2/control/stochsys.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.190260 control-0.9.3.post2/control/tests/
--rw-r--r--   0 murray     (501) staff       (20)        0 2015-08-19 02:39:58.000000 control-0.9.3.post2/control/tests/__init__.py
--rw-r--r--   0 murray     (501) staff       (20)    14005 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/bdalg_test.py
--rw-r--r--   0 murray     (501) staff       (20)     8189 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/bspline_test.py
--rw-r--r--   0 murray     (501) staff       (20)    17346 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/tests/canonical_test.py
--rw-r--r--   0 murray     (501) staff       (20)    12756 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/config_test.py
--rw-r--r--   0 murray     (501) staff       (20)     4211 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/conftest.py
--rw-r--r--   0 murray     (501) staff       (20)     9718 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/convert_test.py
--rw-r--r--   0 murray     (501) staff       (20)     1945 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/ctrlutil_test.py
--rw-r--r--   0 murray     (501) staff       (20)     3517 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/delay_test.py
--rw-r--r--   0 murray     (501) staff       (20)     7175 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/tests/descfcn_test.py
--rw-r--r--   0 murray     (501) staff       (20)    21638 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/discrete_test.py
--rw-r--r--   0 murray     (501) staff       (20)    31942 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/flatsys_test.py
--rw-r--r--   0 murray     (501) staff       (20)    22574 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/frd_test.py
--rw-r--r--   0 murray     (501) staff       (20)    23097 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/freqresp_test.py
--rw-r--r--   0 murray     (501) staff       (20)     1819 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/input_element_int_test.py
--rw-r--r--   0 murray     (501) staff       (20)    10594 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/interconnect_test.py
--rw-r--r--   0 murray     (501) staff       (20)    84090 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/iosys_test.py
--rw-r--r--   0 murray     (501) staff       (20)    11271 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/kwargs_test.py
--rw-r--r--   0 murray     (501) staff       (20)    12868 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/lti_test.py
--rw-r--r--   0 murray     (501) staff       (20)    13964 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/tests/margin_test.py
--rw-r--r--   0 murray     (501) staff       (20)    14543 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/tests/mateqn_test.py
--rw-r--r--   0 murray     (501) staff       (20)    15409 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/matlab2_test.py
--rw-r--r--   0 murray     (501) staff       (20)    30247 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/matlab_test.py
--rw-r--r--   0 murray     (501) staff       (20)     4121 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/minreal_test.py
--rw-r--r--   0 murray     (501) staff       (20)    10145 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/modelsimp_test.py
--rw-r--r--   0 murray     (501) staff       (20)     9002 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/namedio_test.py
--rw-r--r--   0 murray     (501) staff       (20)     2613 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/nichols_test.py
--rw-r--r--   0 murray     (501) staff       (20)    15532 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/nyquist_test.py
--rw-r--r--   0 murray     (501) staff       (20)    28110 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/optimal_test.py
--rw-r--r--   0 murray     (501) staff       (20)     3502 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/passivity_test.py
--rw-r--r--   0 murray     (501) staff       (20)     2901 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/phaseplot_test.py
--rw-r--r--   0 murray     (501) staff       (20)     3131 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/pzmap_test.py
--rw-r--r--   0 murray     (501) staff       (20)     5898 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/rlocus_test.py
--rw-r--r--   0 murray     (501) staff       (20)    13527 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/robust_test.py
--rw-r--r--   0 murray     (501) staff       (20)     8094 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/sisotool_test.py
--rw-r--r--   0 murray     (501) staff       (20)     9124 2021-03-20 16:01:30.000000 control-0.9.3.post2/control/tests/slycot_convert_test.py
--rw-r--r--   0 murray     (501) staff       (20)    38479 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/statefbk_test.py
--rw-r--r--   0 murray     (501) staff       (20)    51350 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/statesp_test.py
--rw-r--r--   0 murray     (501) staff       (20)    11765 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/stochsys_test.py
--rw-r--r--   0 murray     (501) staff       (20)     2326 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/timebase_test.py
--rw-r--r--   0 murray     (501) staff       (20)    50899 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/timeresp_test.py
--rw-r--r--   0 murray     (501) staff       (20)    13348 2022-05-28 16:49:31.000000 control-0.9.3.post2/control/tests/trdata_test.py
--rw-r--r--   0 murray     (501) staff       (20)    11145 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/type_conversion_test.py
--rw-r--r--   0 murray     (501) staff       (20)     3009 2021-12-31 17:02:21.000000 control-0.9.3.post2/control/tests/xferfcn_input_test.py
--rw-r--r--   0 murray     (501) staff       (20)    46834 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/tests/xferfcn_test.py
--rw-r--r--   0 murray     (501) staff       (20)    80523 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/timeresp.py
--rw-r--r--   0 murray     (501) staff       (20)    67610 2022-12-31 16:37:24.000000 control-0.9.3.post2/control/xferfcn.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.174421 control-0.9.3.post2/control.egg-info/
--rw-r--r--   0 murray     (501) staff       (20)     6957 2022-12-31 21:38:16.000000 control-0.9.3.post2/control.egg-info/PKG-INFO
--rw-r--r--   0 murray     (501) staff       (20)     5047 2022-12-31 21:38:16.000000 control-0.9.3.post2/control.egg-info/SOURCES.txt
--rw-r--r--   0 murray     (501) staff       (20)        1 2022-12-31 21:38:16.000000 control-0.9.3.post2/control.egg-info/dependency_links.txt
--rw-r--r--   0 murray     (501) staff       (20)      106 2022-12-31 21:38:16.000000 control-0.9.3.post2/control.egg-info/requires.txt
--rw-r--r--   0 murray     (501) staff       (20)        8 2022-12-31 21:38:16.000000 control-0.9.3.post2/control.egg-info/top_level.txt
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.209457 control-0.9.3.post2/doc/
--rw-r--r--   0 murray     (501) staff       (20)       10 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/.gitignore
--rw-r--r--   0 murray     (501) staff       (20)      731 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/Makefile
--rw-r--r--   0 murray     (501) staff       (20)      893 2019-04-17 04:46:11.000000 control-0.9.3.post2/doc/README
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.209833 control-0.9.3.post2/doc/_templates/
--rw-r--r--   0 murray     (501) staff       (20)      466 2021-12-31 17:02:21.000000 control-0.9.3.post2/doc/_templates/custom-class-template.rst
--rw-r--r--   0 murray     (501) staff       (20)     5846 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/classes.fig
--rw-r--r--   0 murray     (501) staff       (20)    12798 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/classes.pdf
--rw-r--r--   0 murray     (501) staff       (20)     1487 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/classes.rst
--rw-r--r--   0 murray     (501) staff       (20)     8619 2022-12-31 21:36:59.000000 control-0.9.3.post2/doc/conf.py
--rw-r--r--   0 murray     (501) staff       (20)     3223 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/control.rst
--rw-r--r--   0 murray     (501) staff       (20)    11385 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/conventions.rst
--rw-r--r--   0 murray     (501) staff       (20)    17263 2021-12-31 17:02:21.000000 control-0.9.3.post2/doc/cruise-control.py
--rw-r--r--   0 murray     (501) staff       (20)      324 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/cruise-control.rst
--rw-r--r--   0 murray     (501) staff       (20)   262738 2021-12-31 17:02:21.000000 control-0.9.3.post2/doc/cruise.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     2966 2021-12-31 17:02:21.000000 control-0.9.3.post2/doc/descfcn.rst
--rw-r--r--   0 murray     (501) staff       (20)   200784 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/describing_functions.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     1136 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/examples.rst
--rw-r--r--   0 murray     (501) staff       (20)    11469 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/flatsys.rst
--rw-r--r--   0 murray     (501) staff       (20)     1951 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/index.rst
--rw-r--r--   0 murray     (501) staff       (20)     3330 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/intro.rst
--rw-r--r--   0 murray     (501) staff       (20)    13001 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/iosys.rst
--rw-r--r--   0 murray     (501) staff       (20)     6691 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/kincar-flatsys.py
--rw-r--r--   0 murray     (501) staff       (20)      461 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/kincar-flatsys.rst
--rw-r--r--   0 murray     (501) staff       (20)   152602 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/kincar-fusion.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     2051 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/matlab.rst
--rw-r--r--   0 murray     (501) staff       (20)   175846 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/mpc-overview.png
--rw-r--r--   0 murray     (501) staff       (20)    26512 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/mpc_aircraft.ipynb
--rw-r--r--   0 murray     (501) staff       (20)    13290 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/optimal.rst
--rw-r--r--   0 murray     (501) staff       (20)     4481 2019-06-09 03:53:49.000000 control-0.9.3.post2/doc/phaseplots.py
--rw-r--r--   0 murray     (501) staff       (20)      246 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/phaseplots.rst
--rw-r--r--   0 murray     (501) staff       (20)   144671 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/pvtol-lqr-nested.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     6697 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/pvtol-lqr.py
--rw-r--r--   0 murray     (501) staff       (20)      611 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/pvtol-lqr.rst
--rw-r--r--   0 murray     (501) staff       (20)     4609 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/pvtol-nested.py
--rw-r--r--   0 murray     (501) staff       (20)      630 2021-12-31 17:02:21.000000 control-0.9.3.post2/doc/pvtol-nested.rst
--rw-r--r--   0 murray     (501) staff       (20)   151215 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/pvtol-outputfbk.ipynb
--rw-r--r--   0 murray     (501) staff       (20)      157 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/requirements.txt
--rw-r--r--   0 murray     (501) staff       (20)     5219 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/robust_mimo.py
--rw-r--r--   0 murray     (501) staff       (20)      301 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/robust_mimo.rst
--rw-r--r--   0 murray     (501) staff       (20)     2748 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/robust_siso.py
--rw-r--r--   0 murray     (501) staff       (20)      301 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/robust_siso.rst
--rwxr--r--   0 murray     (501) staff       (20)     1322 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/rss-balred.py
--rw-r--r--   0 murray     (501) staff       (20)      273 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/rss-balred.rst
--rw-r--r--   0 murray     (501) staff       (20)      863 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/secord-matlab.py
--rw-r--r--   0 murray     (501) staff       (20)      413 2020-01-04 20:02:34.000000 control-0.9.3.post2/doc/secord-matlab.rst
--rw-r--r--   0 murray     (501) staff       (20)     9650 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/steering-gainsched.py
--rw-r--r--   0 murray     (501) staff       (20)      245 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/steering-gainsched.rst
--rw-r--r--   0 murray     (501) staff       (20)    28691 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/steering-optimal.png
--rw-r--r--   0 murray     (501) staff       (20)     9963 2022-12-31 16:37:24.000000 control-0.9.3.post2/doc/steering-optimal.py
--rw-r--r--   0 murray     (501) staff       (20)      226 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/steering-optimal.rst
--rw-r--r--   0 murray     (501) staff       (20)   488326 2021-03-20 16:01:31.000000 control-0.9.3.post2/doc/steering.ipynb
--rw-r--r--   0 murray     (501) staff       (20)    94408 2022-05-28 16:49:31.000000 control-0.9.3.post2/doc/stochresp.ipynb
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.226787 control-0.9.3.post2/examples/
--rw-r--r--   0 murray     (501) staff       (20)      220 2014-08-09 17:40:09.000000 control-0.9.3.post2/examples/README
--rw-r--r--   0 murray     (501) staff       (20)      381 2019-06-09 03:53:49.000000 control-0.9.3.post2/examples/bdalg-matlab.py
--rw-r--r--   0 murray     (501) staff       (20)  1229504 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/bode-and-nyquist-plots.ipynb
--rw-r--r--   0 murray     (501) staff       (20)      714 2021-12-31 17:02:21.000000 control-0.9.3.post2/examples/check-controllability-and-observability.py
--rw-r--r--   0 murray     (501) staff       (20)    17263 2021-12-31 17:02:21.000000 control-0.9.3.post2/examples/cruise-control.py
--rw-r--r--   0 murray     (501) staff       (20)   262738 2021-12-31 17:02:21.000000 control-0.9.3.post2/examples/cruise.ipynb
--rw-r--r--   0 murray     (501) staff       (20)   200784 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/describing_functions.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     2935 2019-06-09 03:53:49.000000 control-0.9.3.post2/examples/genswitch.py
--rw-r--r--   0 murray     (501) staff       (20)     6691 2022-12-31 16:37:24.000000 control-0.9.3.post2/examples/kincar-flatsys.py
--rw-r--r--   0 murray     (501) staff       (20)   152602 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/kincar-fusion.ipynb
--rw-r--r--   0 murray     (501) staff       (20)    26512 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/mpc_aircraft.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     4481 2019-06-09 03:53:49.000000 control-0.9.3.post2/examples/phaseplots.py
--rw-r--r--   0 murray     (501) staff       (20)   144671 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/pvtol-lqr-nested.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     6697 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/pvtol-lqr.py
--rw-r--r--   0 murray     (501) staff       (20)     4429 2020-01-04 20:02:34.000000 control-0.9.3.post2/examples/pvtol-nested-ss.py
--rw-r--r--   0 murray     (501) staff       (20)     4609 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/pvtol-nested.py
--rw-r--r--   0 murray     (501) staff       (20)   151215 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/pvtol-outputfbk.ipynb
--rw-r--r--   0 murray     (501) staff       (20)    11035 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/pvtol.py
--rw-r--r--   0 murray     (501) staff       (20)     5219 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/robust_mimo.py
--rw-r--r--   0 murray     (501) staff       (20)     2748 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/robust_siso.py
--rwxr--r--   0 murray     (501) staff       (20)     1322 2020-01-04 20:02:34.000000 control-0.9.3.post2/examples/rss-balred.py
--rwxr-xr-x   0 murray     (501) staff       (20)      847 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/run_examples.sh
--rwxr-xr-x   0 murray     (501) staff       (20)      709 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/run_notebooks.sh
--rw-r--r--   0 murray     (501) staff       (20)      863 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/secord-matlab.py
--rw-r--r--   0 murray     (501) staff       (20)   630614 2021-12-31 17:02:21.000000 control-0.9.3.post2/examples/singular-values-plot.ipynb
--rw-r--r--   0 murray     (501) staff       (20)      802 2020-12-28 19:51:09.000000 control-0.9.3.post2/examples/sisotool_example.py
--rw-r--r--   0 murray     (501) staff       (20)     1345 2021-12-31 17:02:21.000000 control-0.9.3.post2/examples/slycot-import-test.py
--rw-r--r--   0 murray     (501) staff       (20)     9650 2022-12-31 16:37:24.000000 control-0.9.3.post2/examples/steering-gainsched.py
--rw-r--r--   0 murray     (501) staff       (20)     9963 2022-12-31 16:37:24.000000 control-0.9.3.post2/examples/steering-optimal.py
--rw-r--r--   0 murray     (501) staff       (20)   488326 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/steering.ipynb
--rw-r--r--   0 murray     (501) staff       (20)    94408 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/stochresp.ipynb
--rw-r--r--   0 murray     (501) staff       (20)     1043 2021-03-20 16:01:31.000000 control-0.9.3.post2/examples/test-response.py
--rw-r--r--   0 murray     (501) staff       (20)    13308 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/tfvis.py
--rw-r--r--   0 murray     (501) staff       (20)     1677 2019-06-09 03:53:49.000000 control-0.9.3.post2/examples/type2_type3.py
--rw-r--r--   0 murray     (501) staff       (20)    13510 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/vehicle-steering.png
--rw-r--r--   0 murray     (501) staff       (20)     3257 2022-05-28 16:49:31.000000 control-0.9.3.post2/examples/vehicle.py
-drwxr-xr-x   0 murray     (501) staff       (20)        0 2022-12-31 21:38:16.229092 control-0.9.3.post2/external/
--rw-r--r--   0 murray     (501) staff       (20)    49520 2014-08-09 17:40:09.000000 control-0.9.3.post2/external/controls.py
--rw-r--r--   0 murray     (501) staff       (20)    15577 2014-10-14 20:33:02.000000 control-0.9.3.post2/external/yottalab.py
--rw-r--r--   0 murray     (501) staff       (20)     1572 2022-12-31 21:36:59.000000 control-0.9.3.post2/pyproject.toml
--rw-r--r--   0 murray     (501) staff       (20)       38 2022-12-31 21:38:16.229909 control-0.9.3.post2/setup.cfg
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.438088 control-0.9.4/
+-rw-r--r--   0 murray     (501) staff       (20)      310 2021-03-20 16:01:30.000000 control-0.9.4/.coveragerc
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.345590 control-0.9.4/.github/
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.350153 control-0.9.4/.github/conda-env/
+-rw-r--r--   0 murray     (501) staff       (20)       57 2022-12-31 16:37:24.000000 control-0.9.4/.github/conda-env/build-env.yml
+-rw-r--r--   0 murray     (501) staff       (20)      280 2023-06-10 05:17:48.000000 control-0.9.4/.github/conda-env/doctest-env.yml
+-rw-r--r--   0 murray     (501) staff       (20)      195 2022-12-31 16:37:24.000000 control-0.9.4/.github/conda-env/test-env.yml
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.350575 control-0.9.4/.github/scripts/
+-rw-r--r--   0 murray     (501) staff       (20)      988 2022-12-31 16:37:24.000000 control-0.9.4/.github/scripts/set-conda-test-matrix.py
+-rw-r--r--   0 murray     (501) staff       (20)      865 2022-12-31 16:37:24.000000 control-0.9.4/.github/scripts/set-pip-test-matrix.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.351631 control-0.9.4/.github/workflows/
+-rw-r--r--   0 murray     (501) staff       (20)     1139 2022-12-31 16:37:24.000000 control-0.9.4/.github/workflows/control-slycot-src.yml
+-rw-r--r--   0 murray     (501) staff       (20)     1207 2023-06-10 05:17:48.000000 control-0.9.4/.github/workflows/doctest.yml
+-rw-r--r--   0 murray     (501) staff       (20)      937 2023-06-10 05:17:48.000000 control-0.9.4/.github/workflows/install_examples.yml
+-rw-r--r--   0 murray     (501) staff       (20)    11114 2022-12-31 16:37:24.000000 control-0.9.4/.github/workflows/os-blas-test-matrix.yml
+-rw-r--r--   0 murray     (501) staff       (20)     2391 2022-12-31 16:37:24.000000 control-0.9.4/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 murray     (501) staff       (20)      507 2023-06-10 05:17:48.000000 control-0.9.4/.gitignore
+-rw-r--r--   0 murray     (501) staff       (20)      495 2022-12-31 16:37:24.000000 control-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 murray     (501) staff       (20)    40928 2017-01-05 06:40:35.000000 control-0.9.4/ChangeLog
+-rw-r--r--   0 murray     (501) staff       (20)     1536 2016-05-30 18:51:51.000000 control-0.9.4/LICENSE
+-rw-r--r--   0 murray     (501) staff       (20)       91 2022-12-31 16:37:24.000000 control-0.9.4/MANIFEST.in
+-rw-r--r--   0 murray     (501) staff       (20)     7351 2023-06-10 05:20:15.437767 control-0.9.4/PKG-INFO
+-rw-r--r--   0 murray     (501) staff       (20)     2725 2014-08-09 17:40:09.000000 control-0.9.4/Pending
+-rw-r--r--   0 murray     (501) staff       (20)     6188 2023-06-10 05:17:48.000000 control-0.9.4/README.rst
+-rw-r--r--   0 murray     (501) staff       (20)     6897 2021-03-20 16:01:30.000000 control-0.9.4/asv.conf.json
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.352483 control-0.9.4/benchmarks/
+-rw-r--r--   0 murray     (501) staff       (20)     1420 2022-12-31 16:37:24.000000 control-0.9.4/benchmarks/README
+-rw-r--r--   0 murray     (501) staff       (20)        0 2021-03-20 16:01:30.000000 control-0.9.4/benchmarks/__init__.py
+-rw-r--r--   0 murray     (501) staff       (20)     5847 2022-12-31 16:37:24.000000 control-0.9.4/benchmarks/flatsys_bench.py
+-rw-r--r--   0 murray     (501) staff       (20)     3117 2023-06-10 05:17:48.000000 control-0.9.4/benchmarks/optestim_bench.py
+-rw-r--r--   0 murray     (501) staff       (20)     8768 2022-12-31 16:37:24.000000 control-0.9.4/benchmarks/optimal_bench.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.352962 control-0.9.4/conda-recipe/
+-rw-r--r--   0 murray     (501) staff       (20)      126 2015-10-18 15:36:15.000000 control-0.9.4/conda-recipe/bld.bat
+-rw-r--r--   0 murray     (501) staff       (20)      632 2018-01-13 06:22:26.000000 control-0.9.4/conda-recipe/meta.yaml
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.367105 control-0.9.4/control/
+-rw-r--r--   0 murray     (501) staff       (20)     3635 2023-06-10 05:17:48.000000 control-0.9.4/control/__init__.py
+-rw-r--r--   0 murray     (501) staff       (20)      160 2023-06-10 05:20:15.000000 control-0.9.4/control/_version.py
+-rw-r--r--   0 murray     (501) staff       (20)    13127 2023-06-10 05:17:48.000000 control-0.9.4/control/bdalg.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.368524 control-0.9.4/control/bench/
+-rw-r--r--   0 murray     (501) staff       (20)      596 2023-06-10 05:17:48.000000 control-0.9.4/control/bench/time_freqresp.py
+-rw-r--r--   0 murray     (501) staff       (20)    15599 2023-06-10 05:17:48.000000 control-0.9.4/control/canonical.py
+-rw-r--r--   0 murray     (501) staff       (20)    12976 2023-06-10 05:17:48.000000 control-0.9.4/control/config.py
+-rw-r--r--   0 murray     (501) staff       (20)     4690 2023-06-10 05:17:48.000000 control-0.9.4/control/ctrlutil.py
+-rw-r--r--   0 murray     (501) staff       (20)     4042 2023-06-10 05:17:48.000000 control-0.9.4/control/delay.py
+-rw-r--r--   0 murray     (501) staff       (20)    19696 2023-06-10 05:17:48.000000 control-0.9.4/control/descfcn.py
+-rw-r--r--   0 murray     (501) staff       (20)     4852 2023-06-10 05:17:48.000000 control-0.9.4/control/dtime.py
+-rw-r--r--   0 murray     (501) staff       (20)     3525 2023-06-10 05:17:48.000000 control-0.9.4/control/exception.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.370817 control-0.9.4/control/flatsys/
+-rw-r--r--   0 murray     (501) staff       (20)     3157 2023-06-10 05:17:48.000000 control-0.9.4/control/flatsys/__init__.py
+-rw-r--r--   0 murray     (501) staff       (20)     4602 2022-12-31 16:37:24.000000 control-0.9.4/control/flatsys/basis.py
+-rw-r--r--   0 murray     (501) staff       (20)     3431 2022-12-31 16:37:24.000000 control-0.9.4/control/flatsys/bezier.py
+-rw-r--r--   0 murray     (501) staff       (20)     8452 2022-12-31 16:37:24.000000 control-0.9.4/control/flatsys/bspline.py
+-rw-r--r--   0 murray     (501) staff       (20)    36945 2023-06-10 05:17:48.000000 control-0.9.4/control/flatsys/flatsys.py
+-rw-r--r--   0 murray     (501) staff       (20)     6339 2022-12-31 16:37:24.000000 control-0.9.4/control/flatsys/linflat.py
+-rw-r--r--   0 murray     (501) staff       (20)     2789 2022-12-31 16:37:24.000000 control-0.9.4/control/flatsys/poly.py
+-rw-r--r--   0 murray     (501) staff       (20)     7996 2023-06-10 05:17:48.000000 control-0.9.4/control/flatsys/systraj.py
+-rw-r--r--   0 murray     (501) staff       (20)    29993 2023-06-10 05:17:48.000000 control-0.9.4/control/frdata.py
+-rw-r--r--   0 murray     (501) staff       (20)    72817 2023-06-10 05:17:48.000000 control-0.9.4/control/freqplot.py
+-rw-r--r--   0 murray     (501) staff       (20)     7316 2023-06-10 05:17:48.000000 control-0.9.4/control/grid.py
+-rw-r--r--   0 murray     (501) staff       (20)   126373 2023-06-10 05:17:48.000000 control-0.9.4/control/iosys.py
+-rw-r--r--   0 murray     (501) staff       (20)    20415 2023-06-10 05:17:48.000000 control-0.9.4/control/lti.py
+-rw-r--r--   0 murray     (501) staff       (20)    20161 2023-06-10 05:17:48.000000 control-0.9.4/control/margins.py
+-rw-r--r--   0 murray     (501) staff       (20)    22814 2022-12-31 16:37:24.000000 control-0.9.4/control/mateqn.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.371532 control-0.9.4/control/matlab/
+-rw-r--r--   0 murray     (501) staff       (20)    18522 2023-06-10 05:17:48.000000 control-0.9.4/control/matlab/__init__.py
+-rw-r--r--   0 murray     (501) staff       (20)     9197 2023-06-10 05:17:48.000000 control-0.9.4/control/matlab/timeresp.py
+-rw-r--r--   0 murray     (501) staff       (20)     7338 2023-06-10 05:17:48.000000 control-0.9.4/control/matlab/wrappers.py
+-rw-r--r--   0 murray     (501) staff       (20)    18400 2023-06-10 05:17:48.000000 control-0.9.4/control/modelsimp.py
+-rw-r--r--   0 murray     (501) staff       (20)    24833 2023-06-10 05:17:48.000000 control-0.9.4/control/namedio.py
+-rw-r--r--   0 murray     (501) staff       (20)    13196 2022-05-28 16:49:31.000000 control-0.9.4/control/nichols.py
+-rw-r--r--   0 murray     (501) staff       (20)    99586 2023-06-10 05:17:48.000000 control-0.9.4/control/optimal.py
+-rw-r--r--   0 murray     (501) staff       (20)     8928 2022-12-31 16:37:24.000000 control-0.9.4/control/passivity.py
+-rw-r--r--   0 murray     (501) staff       (20)    12026 2023-06-10 05:17:48.000000 control-0.9.4/control/phaseplot.py
+-rw-r--r--   0 murray     (501) staff       (20)     4711 2022-05-28 16:49:31.000000 control-0.9.4/control/pzmap.py
+-rw-r--r--   0 murray     (501) staff       (20)    30307 2023-06-10 05:17:48.000000 control-0.9.4/control/rlocus.py
+-rw-r--r--   0 murray     (501) staff       (20)    11811 2023-06-10 05:17:48.000000 control-0.9.4/control/robust.py
+-rw-r--r--   0 murray     (501) staff       (20)    16549 2023-06-10 05:17:48.000000 control-0.9.4/control/sisotool.py
+-rw-r--r--   0 murray     (501) staff       (20)    41124 2023-06-10 05:17:48.000000 control-0.9.4/control/statefbk.py
+-rw-r--r--   0 murray     (501) staff       (20)    73088 2023-06-10 05:17:48.000000 control-0.9.4/control/statesp.py
+-rw-r--r--   0 murray     (501) staff       (20)    25918 2023-06-10 05:17:48.000000 control-0.9.4/control/stochsys.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.384320 control-0.9.4/control/tests/
+-rw-r--r--   0 murray     (501) staff       (20)        0 2015-08-19 02:39:58.000000 control-0.9.4/control/tests/__init__.py
+-rw-r--r--   0 murray     (501) staff       (20)    14005 2022-05-28 16:49:31.000000 control-0.9.4/control/tests/bdalg_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     8189 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/bspline_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    17447 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/canonical_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    12756 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/config_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     4428 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/conftest.py
+-rw-r--r--   0 murray     (501) staff       (20)     9718 2022-05-28 16:49:31.000000 control-0.9.4/control/tests/convert_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     2140 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/ctrlutil_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     3517 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/delay_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     7175 2021-12-31 17:02:21.000000 control-0.9.4/control/tests/descfcn_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    23017 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/discrete_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    31943 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/flatsys_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    22574 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/frd_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    23475 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/freqresp_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     1819 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/input_element_int_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    11992 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/interconnect_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    86585 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/iosys_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    12185 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/kwargs_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    14226 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/lti_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    13964 2021-12-31 17:02:21.000000 control-0.9.4/control/tests/margin_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    14543 2021-12-31 17:02:21.000000 control-0.9.4/control/tests/mateqn_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    15409 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/matlab2_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    30247 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/matlab_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     4121 2022-05-28 16:49:31.000000 control-0.9.4/control/tests/minreal_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    10145 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/modelsimp_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    10728 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/namedio_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     2613 2022-05-28 16:49:31.000000 control-0.9.4/control/tests/nichols_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    15951 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/nyquist_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    30745 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/optimal_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     3502 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/passivity_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     2901 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/phaseplot_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     3131 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/pzmap_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     5920 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/rlocus_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    13527 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/robust_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     8683 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/sisotool_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     9124 2021-03-20 16:01:30.000000 control-0.9.4/control/tests/slycot_convert_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    42462 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/statefbk_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    51350 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/statesp_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    19173 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/stochsys_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     2326 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/timebase_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    50899 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/timeresp_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    14241 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/trdata_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    11145 2022-12-31 16:37:24.000000 control-0.9.4/control/tests/type_conversion_test.py
+-rw-r--r--   0 murray     (501) staff       (20)     3009 2021-12-31 17:02:21.000000 control-0.9.4/control/tests/xferfcn_input_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    50740 2023-06-10 05:17:48.000000 control-0.9.4/control/tests/xferfcn_test.py
+-rw-r--r--   0 murray     (501) staff       (20)    81653 2023-06-10 05:17:48.000000 control-0.9.4/control/timeresp.py
+-rw-r--r--   0 murray     (501) staff       (20)    72036 2023-06-10 05:17:48.000000 control-0.9.4/control/xferfcn.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.368375 control-0.9.4/control.egg-info/
+-rw-r--r--   0 murray     (501) staff       (20)     7351 2023-06-10 05:20:15.000000 control-0.9.4/control.egg-info/PKG-INFO
+-rw-r--r--   0 murray     (501) staff       (20)     5518 2023-06-10 05:20:15.000000 control-0.9.4/control.egg-info/SOURCES.txt
+-rw-r--r--   0 murray     (501) staff       (20)        1 2023-06-10 05:20:15.000000 control-0.9.4/control.egg-info/dependency_links.txt
+-rw-r--r--   0 murray     (501) staff       (20)      106 2023-06-10 05:20:15.000000 control-0.9.4/control.egg-info/requires.txt
+-rw-r--r--   0 murray     (501) staff       (20)        8 2023-06-10 05:20:15.000000 control-0.9.4/control.egg-info/top_level.txt
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.403869 control-0.9.4/doc/
+-rw-r--r--   0 murray     (501) staff       (20)       19 2023-06-10 05:17:48.000000 control-0.9.4/doc/.gitignore
+-rw-r--r--   0 murray     (501) staff       (20)      739 2023-06-10 05:17:48.000000 control-0.9.4/doc/Makefile
+-rw-r--r--   0 murray     (501) staff       (20)      893 2019-04-17 04:46:11.000000 control-0.9.4/doc/README
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.405076 control-0.9.4/doc/_templates/
+-rw-r--r--   0 murray     (501) staff       (20)      466 2021-12-31 17:02:21.000000 control-0.9.4/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 murray     (501) staff       (20)     5846 2022-05-28 16:49:31.000000 control-0.9.4/doc/classes.fig
+-rw-r--r--   0 murray     (501) staff       (20)    12798 2022-05-28 16:49:31.000000 control-0.9.4/doc/classes.pdf
+-rw-r--r--   0 murray     (501) staff       (20)     9026 2023-06-10 05:17:48.000000 control-0.9.4/doc/classes.png
+-rw-r--r--   0 murray     (501) staff       (20)     1685 2023-06-10 05:17:48.000000 control-0.9.4/doc/classes.rst
+-rw-r--r--   0 murray     (501) staff       (20)     9042 2023-06-10 05:17:48.000000 control-0.9.4/doc/conf.py
+-rw-r--r--   0 murray     (501) staff       (20)     3279 2023-06-10 05:17:48.000000 control-0.9.4/doc/control.rst
+-rw-r--r--   0 murray     (501) staff       (20)    12515 2023-06-10 05:17:48.000000 control-0.9.4/doc/conventions.rst
+-rw-r--r--   0 murray     (501) staff       (20)    17263 2021-12-31 17:02:21.000000 control-0.9.4/doc/cruise-control.py
+-rw-r--r--   0 murray     (501) staff       (20)      324 2020-01-04 20:02:34.000000 control-0.9.4/doc/cruise-control.rst
+-rw-r--r--   0 murray     (501) staff       (20)   262738 2021-12-31 17:02:21.000000 control-0.9.4/doc/cruise.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     2966 2021-12-31 17:02:21.000000 control-0.9.4/doc/descfcn.rst
+-rw-r--r--   0 murray     (501) staff       (20)   200784 2021-03-20 16:01:31.000000 control-0.9.4/doc/describing_functions.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     1411 2023-06-10 05:17:48.000000 control-0.9.4/doc/examples.rst
+-rw-r--r--   0 murray     (501) staff       (20)    11469 2022-12-31 16:37:24.000000 control-0.9.4/doc/flatsys.rst
+-rw-r--r--   0 murray     (501) staff       (20)     1951 2021-03-20 16:01:31.000000 control-0.9.4/doc/index.rst
+-rw-r--r--   0 murray     (501) staff       (20)     3718 2023-06-10 05:17:48.000000 control-0.9.4/doc/intro.rst
+-rw-r--r--   0 murray     (501) staff       (20)    13017 2023-06-10 05:17:48.000000 control-0.9.4/doc/iosys.rst
+-rw-r--r--   0 murray     (501) staff       (20)     6691 2023-06-10 05:17:48.000000 control-0.9.4/doc/kincar-flatsys.py
+-rw-r--r--   0 murray     (501) staff       (20)      461 2020-01-04 20:02:34.000000 control-0.9.4/doc/kincar-flatsys.rst
+-rw-r--r--   0 murray     (501) staff       (20)   152602 2022-05-28 16:49:31.000000 control-0.9.4/doc/kincar-fusion.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     2051 2022-12-31 16:37:24.000000 control-0.9.4/doc/matlab.rst
+-rw-r--r--   0 murray     (501) staff       (20)  1052666 2023-06-10 05:17:48.000000 control-0.9.4/doc/mhe-pvtol.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)   175846 2021-03-20 16:01:31.000000 control-0.9.4/doc/mpc-overview.png
+-rw-r--r--   0 murray     (501) staff       (20)    26512 2023-06-10 05:17:48.000000 control-0.9.4/doc/mpc_aircraft.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    19125 2023-06-10 05:17:48.000000 control-0.9.4/doc/optimal.rst
+-rw-r--r--   0 murray     (501) staff       (20)     4481 2019-06-09 03:53:49.000000 control-0.9.4/doc/phaseplots.py
+-rw-r--r--   0 murray     (501) staff       (20)      246 2020-01-04 20:02:34.000000 control-0.9.4/doc/phaseplots.rst
+-rw-r--r--   0 murray     (501) staff       (20)   144671 2022-05-28 16:49:31.000000 control-0.9.4/doc/pvtol-lqr-nested.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     6697 2022-05-28 16:49:31.000000 control-0.9.4/doc/pvtol-lqr.py
+-rw-r--r--   0 murray     (501) staff       (20)      611 2020-01-04 20:02:34.000000 control-0.9.4/doc/pvtol-lqr.rst
+-rw-r--r--   0 murray     (501) staff       (20)     4609 2022-05-28 16:49:31.000000 control-0.9.4/doc/pvtol-nested.py
+-rw-r--r--   0 murray     (501) staff       (20)      630 2021-12-31 17:02:21.000000 control-0.9.4/doc/pvtol-nested.rst
+-rw-r--r--   0 murray     (501) staff       (20)   151215 2023-06-10 05:17:48.000000 control-0.9.4/doc/pvtol-outputfbk.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    10910 2023-06-10 05:17:48.000000 control-0.9.4/doc/pvtol.py
+-rw-r--r--   0 murray     (501) staff       (20)      157 2022-12-31 16:37:24.000000 control-0.9.4/doc/requirements.txt
+-rw-r--r--   0 murray     (501) staff       (20)     5219 2021-03-20 16:01:31.000000 control-0.9.4/doc/robust_mimo.py
+-rw-r--r--   0 murray     (501) staff       (20)      301 2020-01-04 20:02:34.000000 control-0.9.4/doc/robust_mimo.rst
+-rw-r--r--   0 murray     (501) staff       (20)     2748 2021-03-20 16:01:31.000000 control-0.9.4/doc/robust_siso.py
+-rw-r--r--   0 murray     (501) staff       (20)      301 2020-01-04 20:02:34.000000 control-0.9.4/doc/robust_siso.rst
+-rwxr--r--   0 murray     (501) staff       (20)     1322 2020-01-04 20:02:34.000000 control-0.9.4/doc/rss-balred.py
+-rw-r--r--   0 murray     (501) staff       (20)      273 2020-01-04 20:02:34.000000 control-0.9.4/doc/rss-balred.rst
+-rw-r--r--   0 murray     (501) staff       (20)     2049 2023-06-10 05:17:48.000000 control-0.9.4/doc/scherer_etal_ex7_H2_h2syn.py
+-rw-r--r--   0 murray     (501) staff       (20)      326 2023-06-10 05:17:48.000000 control-0.9.4/doc/scherer_etal_ex7_H2_h2syn.rst
+-rw-r--r--   0 murray     (501) staff       (20)     1274 2023-06-10 05:17:48.000000 control-0.9.4/doc/scherer_etal_ex7_Hinf_hinfsyn.py
+-rw-r--r--   0 murray     (501) staff       (20)      334 2023-06-10 05:17:48.000000 control-0.9.4/doc/scherer_etal_ex7_Hinf_hinfsyn.rst
+-rw-r--r--   0 murray     (501) staff       (20)      863 2021-03-20 16:01:31.000000 control-0.9.4/doc/secord-matlab.py
+-rw-r--r--   0 murray     (501) staff       (20)      413 2020-01-04 20:02:34.000000 control-0.9.4/doc/secord-matlab.rst
+-rw-r--r--   0 murray     (501) staff       (20)     9650 2022-12-31 16:37:24.000000 control-0.9.4/doc/steering-gainsched.py
+-rw-r--r--   0 murray     (501) staff       (20)      245 2022-12-31 16:37:24.000000 control-0.9.4/doc/steering-gainsched.rst
+-rw-r--r--   0 murray     (501) staff       (20)    28691 2022-12-31 16:37:24.000000 control-0.9.4/doc/steering-optimal.png
+-rw-r--r--   0 murray     (501) staff       (20)     9963 2023-06-10 05:17:48.000000 control-0.9.4/doc/steering-optimal.py
+-rw-r--r--   0 murray     (501) staff       (20)      226 2022-05-28 16:49:31.000000 control-0.9.4/doc/steering-optimal.rst
+-rw-r--r--   0 murray     (501) staff       (20)   488326 2021-03-20 16:01:31.000000 control-0.9.4/doc/steering.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    94408 2022-05-28 16:49:31.000000 control-0.9.4/doc/stochresp.ipynb
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.436436 control-0.9.4/examples/
+-rw-r--r--   0 murray     (501) staff       (20)      220 2014-08-09 17:40:09.000000 control-0.9.4/examples/README
+-rw-r--r--   0 murray     (501) staff       (20)      381 2019-06-09 03:53:49.000000 control-0.9.4/examples/bdalg-matlab.py
+-rw-r--r--   0 murray     (501) staff       (20)  1229504 2021-03-20 16:01:31.000000 control-0.9.4/examples/bode-and-nyquist-plots.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)      714 2021-12-31 17:02:21.000000 control-0.9.4/examples/check-controllability-and-observability.py
+-rw-r--r--   0 murray     (501) staff       (20)    17263 2021-12-31 17:02:21.000000 control-0.9.4/examples/cruise-control.py
+-rw-r--r--   0 murray     (501) staff       (20)   262738 2021-12-31 17:02:21.000000 control-0.9.4/examples/cruise.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)   200784 2021-03-20 16:01:31.000000 control-0.9.4/examples/describing_functions.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     2935 2019-06-09 03:53:49.000000 control-0.9.4/examples/genswitch.py
+-rw-r--r--   0 murray     (501) staff       (20)   143511 2023-06-10 05:17:48.000000 control-0.9.4/examples/interconnect_tutorial.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     6691 2023-06-10 05:17:48.000000 control-0.9.4/examples/kincar-flatsys.py
+-rw-r--r--   0 murray     (501) staff       (20)   152602 2022-05-28 16:49:31.000000 control-0.9.4/examples/kincar-fusion.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)  1052666 2023-06-10 05:17:48.000000 control-0.9.4/examples/mhe-pvtol.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    26512 2023-06-10 05:17:48.000000 control-0.9.4/examples/mpc_aircraft.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     4481 2019-06-09 03:53:49.000000 control-0.9.4/examples/phaseplots.py
+-rw-r--r--   0 murray     (501) staff       (20)   144671 2022-05-28 16:49:31.000000 control-0.9.4/examples/pvtol-lqr-nested.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     6697 2022-05-28 16:49:31.000000 control-0.9.4/examples/pvtol-lqr.py
+-rw-r--r--   0 murray     (501) staff       (20)     4429 2020-01-04 20:02:34.000000 control-0.9.4/examples/pvtol-nested-ss.py
+-rw-r--r--   0 murray     (501) staff       (20)     4609 2022-05-28 16:49:31.000000 control-0.9.4/examples/pvtol-nested.py
+-rw-r--r--   0 murray     (501) staff       (20)   151215 2023-06-10 05:17:48.000000 control-0.9.4/examples/pvtol-outputfbk.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    10910 2023-06-10 05:17:48.000000 control-0.9.4/examples/pvtol.py
+-rw-r--r--   0 murray     (501) staff       (20)     5219 2021-03-20 16:01:31.000000 control-0.9.4/examples/robust_mimo.py
+-rw-r--r--   0 murray     (501) staff       (20)     2748 2021-03-20 16:01:31.000000 control-0.9.4/examples/robust_siso.py
+-rwxr--r--   0 murray     (501) staff       (20)     1322 2020-01-04 20:02:34.000000 control-0.9.4/examples/rss-balred.py
+-rwxr-xr-x   0 murray     (501) staff       (20)      847 2021-03-20 16:01:31.000000 control-0.9.4/examples/run_examples.sh
+-rwxr-xr-x   0 murray     (501) staff       (20)      709 2021-03-20 16:01:31.000000 control-0.9.4/examples/run_notebooks.sh
+-rw-r--r--   0 murray     (501) staff       (20)     2049 2023-06-10 05:17:48.000000 control-0.9.4/examples/scherer_etal_ex7_H2_h2syn.py
+-rw-r--r--   0 murray     (501) staff       (20)     1274 2023-06-10 05:17:48.000000 control-0.9.4/examples/scherer_etal_ex7_Hinf_hinfsyn.py
+-rw-r--r--   0 murray     (501) staff       (20)      863 2021-03-20 16:01:31.000000 control-0.9.4/examples/secord-matlab.py
+-rw-r--r--   0 murray     (501) staff       (20)   534294 2023-06-10 05:17:48.000000 control-0.9.4/examples/simulating_discrete_nonlinear.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)   630614 2021-12-31 17:02:21.000000 control-0.9.4/examples/singular-values-plot.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)      802 2020-12-28 19:51:09.000000 control-0.9.4/examples/sisotool_example.py
+-rw-r--r--   0 murray     (501) staff       (20)     1345 2021-12-31 17:02:21.000000 control-0.9.4/examples/slycot-import-test.py
+-rw-r--r--   0 murray     (501) staff       (20)     9650 2022-12-31 16:37:24.000000 control-0.9.4/examples/steering-gainsched.py
+-rw-r--r--   0 murray     (501) staff       (20)     9963 2023-06-10 05:17:48.000000 control-0.9.4/examples/steering-optimal.py
+-rw-r--r--   0 murray     (501) staff       (20)   488326 2021-03-20 16:01:31.000000 control-0.9.4/examples/steering.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)    94408 2022-05-28 16:49:31.000000 control-0.9.4/examples/stochresp.ipynb
+-rw-r--r--   0 murray     (501) staff       (20)     1043 2021-03-20 16:01:31.000000 control-0.9.4/examples/test-response.py
+-rw-r--r--   0 murray     (501) staff       (20)    13308 2022-05-28 16:49:31.000000 control-0.9.4/examples/tfvis.py
+-rw-r--r--   0 murray     (501) staff       (20)     1677 2019-06-09 03:53:49.000000 control-0.9.4/examples/type2_type3.py
+-rw-r--r--   0 murray     (501) staff       (20)    13510 2022-05-28 16:49:31.000000 control-0.9.4/examples/vehicle-steering.png
+-rw-r--r--   0 murray     (501) staff       (20)     3257 2022-05-28 16:49:31.000000 control-0.9.4/examples/vehicle.py
+drwxr-xr-x   0 murray     (501) staff       (20)        0 2023-06-10 05:20:15.437323 control-0.9.4/external/
+-rw-r--r--   0 murray     (501) staff       (20)    49520 2014-08-09 17:40:09.000000 control-0.9.4/external/controls.py
+-rw-r--r--   0 murray     (501) staff       (20)    15577 2014-10-14 20:33:02.000000 control-0.9.4/external/yottalab.py
+-rw-r--r--   0 murray     (501) staff       (20)     1572 2022-12-31 21:36:59.000000 control-0.9.4/pyproject.toml
+-rw-r--r--   0 murray     (501) staff       (20)       38 2023-06-10 05:20:15.438140 control-0.9.4/setup.cfg
```

### Comparing `control-0.9.3.post2/.github/scripts/set-conda-test-matrix.py` & `control-0.9.4/.github/scripts/set-conda-test-matrix.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/.github/scripts/set-pip-test-matrix.py` & `control-0.9.4/.github/scripts/set-pip-test-matrix.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/.github/workflows/control-slycot-src.yml` & `control-0.9.4/.github/workflows/control-slycot-src.yml`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/.github/workflows/os-blas-test-matrix.yml` & `control-0.9.4/.github/workflows/os-blas-test-matrix.yml`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/.github/workflows/python-package-conda.yml` & `control-0.9.4/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/ChangeLog` & `control-0.9.4/ChangeLog`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/LICENSE` & `control-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/PKG-INFO` & `control-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control
-Version: 0.9.3.post2
+Version: 0.9.4
 Summary: Python Control Systems Library
 Author-email: Python Control Developers <python-control-developers@lists.sourceforge.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://python-control.org
 Project-URL: source, https://github.com/python-control/python-control
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -48,103 +48,113 @@
 
 Python Control Systems Library
 ==============================
 
 The Python Control Systems Library is a Python module that implements basic
 operations for analysis and design of feedback control systems.
 
-
 Have a go now!
-==============
+--------------
 Try out the examples in the examples folder using the binder service.
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/python-control/python-control/HEAD
 
+The package can also be installed on Google Colab using the commands::
+
+  !pip install control
+  import control as ct
 
 Features
 --------
 
 - Linear input/output systems in state-space and frequency domain
 - Block diagram algebra: serial, parallel, feedback, and other interconnections
 - Time response: initial, step, impulse
 - Frequency response: Bode, Nyquist, and Nichols plots
 - Control analysis: stability, reachability, observability, stability margins, root locus
 - Control design: eigenvalue placement, linear quadratic regulator, sisotool, hinfsyn, rootlocus_pid_designer
 - Estimator design: linear quadratic estimator (Kalman filter)
 - Nonlinear systems: optimization-based control, describing functions, differential flatness
 
 Links
-=====
+-----
 
 - Project home page: http://python-control.org
 - Source code repository: https://github.com/python-control/python-control
 - Documentation: http://python-control.readthedocs.org/
 - Issue tracker: https://github.com/python-control/python-control/issues
 - Mailing list: http://sourceforge.net/p/python-control/mailman/
 
-
 Dependencies
-============
+------------
 
 The package requires numpy, scipy, and matplotlib.  In addition, some routines
 use a module called slycot, that is a Python wrapper around some FORTRAN
 routines.  Many parts of python-control will work without slycot, but some
 functionality is limited or absent, and installation of slycot is recommended
 (see below). The Slycot wrapper can be found at:
 
 https://github.com/python-control/Slycot
 
+
 Installation
 ============
 
 Conda and conda-forge
 ---------------------
 
 The easiest way to get started with the Control Systems library is
 using `Conda <https://conda.io>`_.
 
-The Control Systems library has been packages for the `conda-forge
+The Control Systems library has packages available using the `conda-forge
 <https://conda-forge.org>`_ Conda channel, and as of Slycot version
 0.3.4, binaries for that package are available for 64-bit Windows,
 OSX, and Linux.
 
 To install both the Control Systems library and Slycot in an existing
 conda environment, run::
 
   conda install -c conda-forge control slycot
 
+Mixing packages from conda-forge and the default conda channel can
+sometimes cause problems with dependencies, so it is usually best to
+instally NumPy, SciPy, and Matplotlib from conda-forge as well.
+
 Pip
 ---
 
 To install using pip::
 
   pip install slycot   # optional; see below
   pip install control
 
 If you install Slycot using pip you'll need a development environment
-(e.g., Python development files, C and Fortran compilers).
+(e.g., Python development files, C and Fortran compilers).  Pip
+installation can be particularly complicated for Windows.
 
 Installing from source
 ----------------------
 
 To install from source, get the source code of the desired branch or release
 from the github repository or archive, unpack, and run from within the
 toplevel `python-control` directory::
 
   pip install .
   
 Article and Citation Information
 ================================
 
-An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
+An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about
+the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
 
   @inproceedings{python-control2021,
     title={The Python Control Systems Library (python-control)},
-    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
+    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and
+            Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
     booktitle={60th IEEE Conference on Decision and Control (CDC)},
     pages={4875--4881},
     year={2021},
     organization={IEEE}
   }
 
 or the GitHub site: https://github.com/python-control/python-control
```

### Comparing `control-0.9.3.post2/Pending` & `control-0.9.4/Pending`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/README.rst` & `control-0.9.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -18,103 +18,113 @@
 
 Python Control Systems Library
 ==============================
 
 The Python Control Systems Library is a Python module that implements basic
 operations for analysis and design of feedback control systems.
 
-
 Have a go now!
-==============
+--------------
 Try out the examples in the examples folder using the binder service.
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/python-control/python-control/HEAD
 
+The package can also be installed on Google Colab using the commands::
+
+  !pip install control
+  import control as ct
 
 Features
 --------
 
 - Linear input/output systems in state-space and frequency domain
 - Block diagram algebra: serial, parallel, feedback, and other interconnections
 - Time response: initial, step, impulse
 - Frequency response: Bode, Nyquist, and Nichols plots
 - Control analysis: stability, reachability, observability, stability margins, root locus
 - Control design: eigenvalue placement, linear quadratic regulator, sisotool, hinfsyn, rootlocus_pid_designer
 - Estimator design: linear quadratic estimator (Kalman filter)
 - Nonlinear systems: optimization-based control, describing functions, differential flatness
 
 Links
-=====
+-----
 
 - Project home page: http://python-control.org
 - Source code repository: https://github.com/python-control/python-control
 - Documentation: http://python-control.readthedocs.org/
 - Issue tracker: https://github.com/python-control/python-control/issues
 - Mailing list: http://sourceforge.net/p/python-control/mailman/
 
-
 Dependencies
-============
+------------
 
 The package requires numpy, scipy, and matplotlib.  In addition, some routines
 use a module called slycot, that is a Python wrapper around some FORTRAN
 routines.  Many parts of python-control will work without slycot, but some
 functionality is limited or absent, and installation of slycot is recommended
 (see below). The Slycot wrapper can be found at:
 
 https://github.com/python-control/Slycot
 
+
 Installation
 ============
 
 Conda and conda-forge
 ---------------------
 
 The easiest way to get started with the Control Systems library is
 using `Conda <https://conda.io>`_.
 
-The Control Systems library has been packages for the `conda-forge
+The Control Systems library has packages available using the `conda-forge
 <https://conda-forge.org>`_ Conda channel, and as of Slycot version
 0.3.4, binaries for that package are available for 64-bit Windows,
 OSX, and Linux.
 
 To install both the Control Systems library and Slycot in an existing
 conda environment, run::
 
   conda install -c conda-forge control slycot
 
+Mixing packages from conda-forge and the default conda channel can
+sometimes cause problems with dependencies, so it is usually best to
+instally NumPy, SciPy, and Matplotlib from conda-forge as well.
+
 Pip
 ---
 
 To install using pip::
 
   pip install slycot   # optional; see below
   pip install control
 
 If you install Slycot using pip you'll need a development environment
-(e.g., Python development files, C and Fortran compilers).
+(e.g., Python development files, C and Fortran compilers).  Pip
+installation can be particularly complicated for Windows.
 
 Installing from source
 ----------------------
 
 To install from source, get the source code of the desired branch or release
 from the github repository or archive, unpack, and run from within the
 toplevel `python-control` directory::
 
   pip install .
   
 Article and Citation Information
 ================================
 
-An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
+An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about
+the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
 
   @inproceedings{python-control2021,
     title={The Python Control Systems Library (python-control)},
-    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
+    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and
+            Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
     booktitle={60th IEEE Conference on Decision and Control (CDC)},
     pages={4875--4881},
     year={2021},
     organization={IEEE}
   }
 
 or the GitHub site: https://github.com/python-control/python-control
```

### Comparing `control-0.9.3.post2/asv.conf.json` & `control-0.9.4/asv.conf.json`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/benchmarks/README` & `control-0.9.4/benchmarks/README`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/benchmarks/flatsys_bench.py` & `control-0.9.4/benchmarks/flatsys_bench.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/benchmarks/optimal_bench.py` & `control-0.9.4/benchmarks/optimal_bench.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/conda-recipe/meta.yaml` & `control-0.9.4/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/__init__.py` & `control-0.9.4/control/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,14 +38,36 @@
 # SUCH DAMAGE.
 #
 # $Id$
 
 """
 The Python Control Systems Library :mod:`control` provides common functions
 for analyzing and designing feedback control systems.
+
+Documentation is available in two forms: docstrings provided with the code,
+and the python-control users guide, available from `the python-control
+homepage <https://www.python-control.org>`_.
+
+The docstring examples assume that the following import commands::
+
+  >>> import numpy as np
+  >>> import control as ct
+
+Available subpackages
+---------------------
+
+The main control package includes the most commpon functions used in
+analysis, design, and simulation of feedback control systems.  Several
+additional subpackages are available that provide more specialized
+functionality:
+
+* :mod:`~control.flatsys`: Differentially flat systems
+* :mod:`~control.matlab`: MATLAB compatibility module
+* :mod:`~control.optimal`: Optimization-based control
+
 """
 
 # Import functions from within the control system library
 # Note: the functions we use are specified as __all__ variables in the modules
 from .bdalg import *
 from .delay import *
 from .descfcn import *
```

### Comparing `control-0.9.3.post2/control/bdalg.py` & `control-0.9.4/control/bdalg.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,17 +95,25 @@
     If both systems have a defined timebase (dt = 0 for continuous time,
     dt > 0 for discrete time), then the timebase for both systems must
     match.  If only one of the system has a timebase, the return
     timebase will be set to match it.
 
     Examples
     --------
-    >>> sys3 = series(sys1, sys2) # Same as sys3 = sys2 * sys1
-
-    >>> sys5 = series(sys1, sys2, sys3, sys4) # More systems
+    >>> G1 = ct.rss(3)
+    >>> G2 = ct.rss(4)
+    >>> G = ct.series(G1, G2) # Same as sys3 = sys2 * sys1
+    >>> G.ninputs, G.noutputs, G.nstates
+    (1, 1, 7)
+
+    >>> G1 = ct.rss(2, inputs=2, outputs=3)
+    >>> G2 = ct.rss(3, inputs=3, outputs=1)
+    >>> G = ct.series(G1, G2) # Same as sys3 = sys2 * sys1
+    >>> G.ninputs, G.noutputs, G.nstates
+    (2, 1, 5)
 
     """
     from functools import reduce
     return reduce(lambda x, y:y*x, sysn, sys1)
 
 
 def parallel(sys1, *sysn):
@@ -142,17 +150,25 @@
     If both systems have a defined timebase (dt = 0 for continuous time,
     dt > 0 for discrete time), then the timebase for both systems must
     match.  If only one of the system has a timebase, the return
     timebase will be set to match it.
 
     Examples
     --------
-    >>> sys3 = parallel(sys1, sys2) # Same as sys3 = sys1 + sys2
-
-    >>> sys5 = parallel(sys1, sys2, sys3, sys4) # More systems
+    >>> G1 = ct.rss(3)
+    >>> G2 = ct.rss(4)
+    >>> G = ct.parallel(G1, G2) # Same as sys3 = sys1 + sys2
+    >>> G.ninputs, G.noutputs, G.nstates
+    (1, 1, 7)
+
+    >>> G1 = ct.rss(3, inputs=3, outputs=4)
+    >>> G2 = ct.rss(4, inputs=3, outputs=4)
+    >>> G = ct.parallel(G1, G2)  # Add another system
+    >>> G.ninputs, G.noutputs, G.nstates
+    (3, 4, 7)
 
     """
     from functools import reduce
     return reduce(lambda x, y:x+y, sysn, sys1)
 
 
 def negate(sys):
@@ -170,15 +186,21 @@
     Notes
     -----
     This function is a wrapper for the __neg__ function in the StateSpace and
     TransferFunction classes.  The output type is the same as the input type.
 
     Examples
     --------
-    >>> sys2 = negate(sys1) # Same as sys2 = -sys1.
+    >>> G = ct.tf([2], [1, 1])
+    >>> G.dcgain()
+    2.0
+
+    >>> Gn = ct.negate(G) # Same as sys2 = -sys1.
+    >>> Gn.dcgain()
+    -2.0
 
     """
     return -sys
 
 #! TODO: expand to allow sys2 default to work in MIMO case?
 def feedback(sys1, sys2=1, sign=-1):
     """
@@ -218,14 +240,22 @@
     This function is a wrapper for the feedback function in the StateSpace and
     TransferFunction classes.  It calls TransferFunction.feedback if `sys1` is a
     TransferFunction object, and StateSpace.feedback if `sys1` is a StateSpace
     object.  If `sys1` is a scalar, then it is converted to `sys2`'s type, and
     the corresponding feedback function is used.  If `sys1` and `sys2` are both
     scalars, then TransferFunction.feedback is used.
 
+    Examples
+    --------
+    >>> G = ct.rss(3, inputs=2, outputs=5)
+    >>> C = ct.rss(4, inputs=5, outputs=2)
+    >>> T = ct.feedback(G, C, sign=1)
+    >>> T.ninputs, T.noutputs, T.nstates
+    (2, 5, 7)
+
     """
     # Allow anything with a feedback function to call that function
     try:
         return sys1.feedback(sys2, sign)
     except AttributeError:
         pass
 
@@ -274,17 +304,25 @@
     -------
     sys: LTI system
         Combined LTI system, with input/output vectors consisting of all
         input/output vectors appended
 
     Examples
     --------
-    >>> sys1 = ss([[1., -2], [3., -4]], [[5.], [7]], [[6., 8]], [[9.]])
-    >>> sys2 = ss([[-1.]], [[1.]], [[1.]], [[0.]])
-    >>> sys = append(sys1, sys2)
+    >>> G1 = ct.rss(3)
+    >>> G2 = ct.rss(4)
+    >>> G = ct.append(G1, G2)
+    >>> G.ninputs, G.noutputs, G.nstates
+    (2, 2, 7)
+
+    >>> G1 = ct.rss(3, inputs=2, outputs=4)
+    >>> G2 = ct.rss(4, inputs=1, outputs=4)
+    >>> G = ct.append(G1, G2)
+    >>> G.ninputs, G.noutputs, G.nstates
+    (3, 8, 7)
 
     """
     s1 = ss._convert_to_statespace(sys[0])
     for s in sys[1:]:
         s1 = s1.append(s)
     return s1
 
@@ -319,19 +357,19 @@
     Returns
     -------
     sys: LTI system
         Connected and trimmed LTI system
 
     Examples
     --------
-    >>> sys1 = ss([[1., -2], [3., -4]], [[5.], [7]], [[6, 8]], [[9.]])
-    >>> sys2 = ss([[-1.]], [[1.]], [[1.]], [[0.]])
-    >>> sys = append(sys1, sys2)
-    >>> Q = [[1, 2], [2, -1]]  # negative feedback interconnection
-    >>> sysc = connect(sys, Q, [2], [1, 2])
+    >>> G = ct.rss(7, inputs=2, outputs=2)
+    >>> K = [[1, 2], [2, -1]]  # negative feedback interconnection
+    >>> T = ct.connect(G, K, [2], [1, 2])
+    >>> T.ninputs, T.noutputs, T.nstates
+    (1, 2, 7)
 
     Notes
     -----
     The :func:`~control.interconnect` function in the
     :ref:`input/output systems <iosys-module>` module allows the use
     of named signals and provides an alternative method for
     interconnecting multiple systems.
```

### Comparing `control-0.9.3.post2/control/canonical.py` & `control-0.9.4/control/canonical.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from numpy.linalg import solve, matrix_rank, eig
 
 from scipy.linalg import schur
 
 __all__ = ['canonical_form', 'reachable_form', 'observable_form', 'modal_form',
            'similarity_transform', 'bdschur']
 
+
 def canonical_form(xsys, form='reachable'):
     """Convert a system into canonical form
 
     Parameters
     ----------
     xsys : StateSpace object
         System to be transformed, with state 'x'
@@ -32,14 +33,32 @@
 
     Returns
     -------
     zsys : StateSpace object
         System in desired canonical form, with state 'z'
     T : (M, M) real ndarray
         Coordinate transformation matrix, z = T * x
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> Gc, T = ct.canonical_form(Gs)  # default reachable
+    >>> Gc.B
+    array([[1.],
+           [0.]])
+
+    >>> Gc, T = ct.canonical_form(Gs, 'observable')
+    >>> Gc.C
+    array([[1., 0.]])
+
+    >>> Gc, T = ct.canonical_form(Gs, 'modal')
+    >>> Gc.A                                                    # doctest: +SKIP
+    array([[-2.,  0.],
+           [ 0., -1.]])
+
     """
 
     # Call the appropriate tranformation function
     if form == 'reachable':
         return reachable_form(xsys)
     elif form == 'observable':
         return observable_form(xsys)
@@ -61,14 +80,23 @@
 
     Returns
     -------
     zsys : StateSpace object
         System in reachable canonical form, with state `z`
     T : (M, M) real ndarray
         Coordinate transformation: z = T * x
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> Gc, T = ct.reachable_form(Gs)  # default reachable
+    >>> Gc.B
+    array([[1.],
+           [0.]])
+
     """
     # Check to make sure we have a SISO system
     if not issiso(xsys):
         raise ControlNotImplemented(
             "Canonical forms for MIMO systems not yet supported")
 
     # Create a new system, starting with a copy of the old one
@@ -115,14 +143,22 @@
 
     Returns
     -------
     zsys : StateSpace object
         System in observable canonical form, with state `z`
     T : (M, M) real ndarray
         Coordinate transformation: z = T * x
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> Gc, T = ct.observable_form(Gs)
+    >>> Gc.C
+    array([[1., 0.]])
+
     """
     # Check to make sure we have a SISO system
     if not issiso(xsys):
         raise ControlNotImplemented(
             "Canonical forms for MIMO systems not yet supported")
 
     # Create a new system, starting with a copy of the old one
@@ -173,14 +209,28 @@
         so x = T z.
 
     Returns
     -------
     zsys : StateSpace object
         System in transformed coordinates, with state 'z'
 
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> Gs.A
+    array([[-3., -2.],
+           [ 1.,  0.]])
+
+    >>> T = np.array([[0, 1], [1, 0]])
+    >>> Gt = ct.similarity_transform(Gs, T)
+    >>> Gt.A
+    array([[ 0.,  1.],
+           [-2., -3.]])
+
     """
     # Create a new system, starting with a copy of the old one
     zsys = StateSpace(xsys)
 
     T = np.atleast_2d(T)
 
     # Define a function to compute the right inverse (solve x M = y)
@@ -240,15 +290,16 @@
 
 
 def _bdschur_condmax_search(aschur, tschur, condmax):
     """Block-diagonal Schur decomposition search up to condmax
 
     Iterates mb03rd with different pmax values until:
       - result is non-defective;
-      - or condition number of similarity transform is unchanging despite large pmax;
+      - or condition number of similarity transform is unchanging
+        despite large pmax;
       - or condition number of similarity transform is close to condmax.
 
     Parameters
     ----------
     aschur: (N, N) real ndarray
       Real Schur-form matrix
     tschur: (N, N) real ndarray
@@ -279,30 +330,33 @@
         raise ControlSlycot("can't find slycot module 'mb03rd'")
 
     # see notes on RuntimeError below
     pmaxlower = None
 
     # get lower bound; try condmax ** 0.5 first
     pmaxlower = condmax ** 0.5
-    amodal, tmodal, blksizes, eigvals = mb03rd(aschur.shape[0], aschur, tschur, pmax=pmaxlower)
+    amodal, tmodal, blksizes, eigvals = mb03rd(
+        aschur.shape[0], aschur, tschur, pmax=pmaxlower)
     if np.linalg.cond(tmodal) <= condmax:
         reslower = amodal, tmodal, blksizes, eigvals
     else:
         pmaxlower = 1.0
-        amodal, tmodal, blksizes, eigvals = mb03rd(aschur.shape[0], aschur, tschur, pmax=pmaxlower)
+        amodal, tmodal, blksizes, eigvals = mb03rd(
+            aschur.shape[0], aschur, tschur, pmax=pmaxlower)
         cond = np.linalg.cond(tmodal)
         if cond > condmax:
-            msg = 'minimum cond={} > condmax={}; try increasing condmax'.format(cond, condmax)
+            msg = f"minimum {cond=} > {condmax=}; try increasing condmax"
             raise RuntimeError(msg)
 
     pmax = pmaxlower
 
     # phase 1: search for upper bound on pmax
     for i in range(50):
-        amodal, tmodal, blksizes, eigvals = mb03rd(aschur.shape[0], aschur, tschur, pmax=pmax)
+        amodal, tmodal, blksizes, eigvals = mb03rd(
+            aschur.shape[0], aschur, tschur, pmax=pmax)
         cond = np.linalg.cond(tmodal)
         if cond < condmax:
             pmaxlower = pmax
             reslower = amodal, tmodal, blksizes, eigvals
         else:
             # upper bound found; go to phase 2
             pmaxupper = pmax
@@ -315,15 +369,16 @@
     else:
         # no upper bound found; return current result
         return reslower
 
     # phase 2: bisection search
     for i in range(50):
         pmax = (pmaxlower * pmaxupper) ** 0.5
-        amodal, tmodal, blksizes, eigvals = mb03rd(aschur.shape[0], aschur, tschur, pmax=pmax)
+        amodal, tmodal, blksizes, eigvals = mb03rd(
+            aschur.shape[0], aschur, tschur, pmax=pmax)
         cond = np.linalg.cond(tmodal)
 
         if cond < condmax:
             if not _bdschur_defective(blksizes, eigvals):
                 return amodal, tmodal, blksizes, eigvals
             pmaxlower = pmax
             reslower = amodal, tmodal, blksizes, eigvals
@@ -366,32 +421,40 @@
     associated eigenvalues.  The ordering is first by real part of
     eigenvalue, in descending order, then by absolute value of
     imaginary part of eigenvalue, also in decreasing order.
 
     If `sort` is 'discrete', the blocks are sorted as for
     'continuous', but applied to log of eigenvalues
     (i.e., continuous-equivalent eigenvalues).
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> amodal, tmodal, blksizes = ct.bdschur(Gs.A)
+    >>> amodal                                                   #doctest: +SKIP
+    array([[-2.,  0.],
+           [ 0., -1.]])
+
     """
     if condmax is None:
         condmax = np.finfo(np.float64).eps ** -0.5
 
     if not (np.isscalar(condmax) and condmax >= 1.0):
         raise ValueError('condmax="{}" must be a scalar >= 1.0'.format(condmax))
 
     a = np.atleast_2d(a)
     if a.shape[0] == 0 or a.shape[1] == 0:
         return a.copy(), np.eye(a.shape[1], a.shape[0]), np.array([])
 
     aschur, tschur = schur(a)
-    amodal, tmodal, blksizes, eigvals = _bdschur_condmax_search(aschur, tschur, condmax)
+    amodal, tmodal, blksizes, eigvals = _bdschur_condmax_search(
+        aschur, tschur, condmax)
 
     if sort in ('continuous', 'discrete'):
-
         idxs = np.cumsum(np.hstack([0, blksizes[:-1]]))
-
         ev_per_blk = [complex(eigvals[i].real, abs(eigvals[i].imag))
                       for i in idxs]
 
         if sort == 'discrete':
             ev_per_blk = np.log(ev_per_blk)
 
         # put most unstable first
@@ -401,15 +464,15 @@
         blkidxs = [np.arange(i0, i0+ilen)
                    for i0, ilen in zip(idxs, blksizes)]
 
         # reordered
         permidx = np.hstack([blkidxs[i] for i in sortidx])
         rperm = np.eye(amodal.shape[0])[permidx]
 
-        tmodal = tmodal @ rperm
+        tmodal = tmodal @ rperm.T
         amodal = rperm @ amodal @ rperm.T
         blksizes = blksizes[sortidx]
 
     elif sort is None:
         pass
 
     else:
@@ -422,24 +485,35 @@
     """Convert a system into modal canonical form
 
     Parameters
     ----------
     xsys : StateSpace object
         System to be transformed, with state `x`
     condmax : None or float, optional
-        An upper bound on individual transformations.  If None, use `bdschur` default.
+        An upper bound on individual transformations.  If None, use
+        `bdschur` default.
     sort : bool, optional
-        If False (default), Schur blocks will not be sorted.  See `bdschur` for sort order.
+        If False (default), Schur blocks will not be sorted.  See `bdschur`
+        for sort order.
 
     Returns
     -------
     zsys : StateSpace object
         System in modal canonical form, with state `z`
     T : (M, M) ndarray
         Coordinate transformation: z = T * x
+
+    Examples
+    --------
+    >>> Gs = ct.tf2ss([1], [1, 3, 2])
+    >>> Gc, T = ct.modal_form(Gs)  # default reachable
+    >>> Gc.A                                                    # doctest: +SKIP
+    array([[-2.,  0.],
+           [ 0., -1.]])
+
     """
 
     if sort:
         discrete = xsys.dt is not None and xsys.dt > 0
         bd_sort = 'discrete' if discrete else 'continuous'
     else:
         bd_sort = None
```

### Comparing `control-0.9.3.post2/control/config.py` & `control-0.9.4/control/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Eventually it will be possible to read and write configuration
 # files.  For now, you can just choose between MATLAB and FBS default
 # values + tweak a few other things.
 
 
 import collections
 import warnings
+from .exception import ControlArgument
 
 __all__ = ['defaults', 'set_defaults', 'reset_defaults',
            'use_matlab_defaults', 'use_fbs_defaults',
            'use_legacy_defaults', 'use_numpy_matrix']
 
 # Package level default values
 _control_defaults = {
@@ -61,30 +62,52 @@
 defaults = DefaultDict(_control_defaults)
 
 
 def set_defaults(module, **keywords):
     """Set default values of parameters for a module.
 
     The set_defaults() function can be used to modify multiple parameter
-    values for a module at the same time, using keyword arguments:
+    values for a module at the same time, using keyword arguments.
 
-        control.set_defaults('module', param1=val, param2=val)
+    Examples
+    --------
+    >>> ct.defaults['freqplot.number_of_samples']
+    1000
+    >>> ct.set_defaults('freqplot', number_of_samples=100)
+    >>> ct.defaults['freqplot.number_of_samples']
+    100
+    >>> # do some customized freqplotting
 
     """
     if not isinstance(module, str):
         raise ValueError("module must be a string")
     for key, val in keywords.items():
         keyname = module + '.' + key
         if keyname not in defaults and f"deprecated.{keyname}" not in defaults:
             raise TypeError(f"unrecognized keyword: {key}")
         defaults[module + '.' + key] = val
 
 
 def reset_defaults():
-    """Reset configuration values to their default (initial) values."""
+    """Reset configuration values to their default (initial) values.
+
+    Examples
+    --------
+    >>> ct.defaults['freqplot.number_of_samples']
+    1000
+    >>> ct.set_defaults('freqplot', number_of_samples=100)
+    >>> ct.defaults['freqplot.number_of_samples']
+    100
+
+    >>> # do some customized freqplotting
+    >>> ct.reset_defaults()
+    >>> ct.defaults['freqplot.number_of_samples']
+    1000
+
+    """
     # System level defaults
     defaults.update(_control_defaults)
 
     from .freqplot import _freqplot_defaults, _nyquist_defaults
     defaults.update(_freqplot_defaults)
     defaults.update(_nyquist_defaults)
 
@@ -177,28 +200,38 @@
     """Use MATLAB compatible configuration settings.
 
     The following conventions are used:
         * Bode plots plot gain in dB, phase in degrees, frequency in
           rad/sec, with grids
         * State space class and functions use Numpy matrix objects
 
+    Examples
+    --------
+    >>> ct.use_matlab_defaults()
+    >>> # do some matlab style plotting
+
     """
     set_defaults('freqplot', dB=True, deg=True, Hz=False, grid=True)
     set_defaults('statesp', use_numpy_matrix=True)
 
 
 # Set defaults to match FBS (Astrom and Murray)
 def use_fbs_defaults():
     """Use `Feedback Systems <http://fbsbook.org>`_ (FBS) compatible settings.
 
     The following conventions are used:
         * Bode plots plot gain in powers of ten, phase in degrees,
           frequency in rad/sec, no grid
         * Nyquist plots use dashed lines for mirror image of Nyquist curve
 
+    Examples
+    --------
+    >>> ct.use_fbs_defaults()
+    >>> # do some FBS style plotting
+
     """
     set_defaults('freqplot', dB=False, deg=True, Hz=False, grid=False)
     set_defaults('nyquist', mirror_style='--')
 
 
 # Decide whether to use numpy.matrix for state space operations
 def use_numpy_matrix(flag=True, warn=True):
@@ -218,28 +251,41 @@
         the warning message.
 
     Notes
     -----
     Prior to release 0.9.x, the default type for 2D arrays is the Numpy
     `matrix` class.  Starting in release 0.9.0, the default type for state
     space operations is a 2D array.
+
+    Examples
+    --------
+    >>> ct.use_numpy_matrix(True, False)
+    >>> # do some legacy calculations using np.matrix
+
     """
     if flag and warn:
         warnings.warn("Return type numpy.matrix is deprecated.",
                       stacklevel=2, category=DeprecationWarning)
     set_defaults('statesp', use_numpy_matrix=flag)
 
 
 def use_legacy_defaults(version):
     """ Sets the defaults to whatever they were in a given release.
 
     Parameters
     ----------
     version : string
         Version number of the defaults desired. Ranges from '0.1' to '0.8.4'.
+
+    Examples
+    --------
+    >>> ct.use_legacy_defaults("0.9.0")
+    (0, 9, 0)
+    >>> # do some legacy style plotting
+
     """
     import re
     (major, minor, patch) = (None, None, None)  # default values
 
     # Early release tag format: REL-0.N
     match = re.match("REL-0.([12])", version)
     if match: (major, minor, patch) = (0, int(match.group(1)), 0)
@@ -306,7 +352,29 @@
         # time responses are only squeezed if SISO
         set_defaults('control', squeeze_time_response=True)
 
         # switched mirror_style of nyquist from '-' to '--'
         set_defaults('nyquist', mirror_style='-')
 
     return (major, minor, patch)
+
+
+#
+# Utility function for processing legacy keywords
+#
+# Use this function to handle a legacy keyword that has been renamed.  This
+# function pops the old keyword off of the kwargs dictionary and issues a
+# warning.  if both the old and new keyword are present, a ControlArgument
+# exception is raised.
+#
+def _process_legacy_keyword(kwargs, oldkey, newkey, newval):
+    if kwargs.get(oldkey) is not None:
+        warnings.warn(
+            f"keyworld '{oldkey}' is deprecated; use '{newkey}'",
+            DeprecationWarning)
+        if newval is not None:
+            raise ControlArgument(
+                f"duplicate keywords '{oldkey}' and '{newkey}'")
+        else:
+            return kwargs.pop(oldkey)
+    else:
+        return newval
```

### Comparing `control-0.9.3.post2/control/ctrlutil.py` & `control-0.9.4/control/delay.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# ctrlutil.py - control system utility functions
+# -*-coding: utf-8-*-
+#! TODO: add module docstring
+# delay.py - functions involving time delays
 #
-# Author: Richard M. Murray
-# Date: 24 May 09
+# Author: Sawyer Fuller
+# Date: 26 Aug 2010
 #
-# These are some basic utility functions that are used in the control
-# systems library and that didn't naturally fit anyplace else.
+# This file contains functions for implementing time delays (currently
+# only the pade() function).
 #
-# Copyright (c) 2009 by California Institute of Technology
+# Copyright (c) 2010 by California Institute of Technology
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 # 1. Redistributions of source code must retain the above copyright
@@ -36,87 +38,88 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
 # OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 # SUCH DAMAGE.
 #
 # $Id$
 
-# Packages that we need access to
-from . import lti
-import numpy as np
-import math
-
-__all__ = ['unwrap', 'issys', 'db2mag', 'mag2db']
-
-# Utility function to unwrap an angle measurement
-def unwrap(angle, period=2*math.pi):
-    """Unwrap a phase angle to give a continuous curve
 
-    Parameters
-    ----------
-    angle : array_like
-        Array of angles to be unwrapped
-    period : float, optional
-        Period (defaults to `2*pi`)
-
-    Returns
-    -------
-    angle_out : array_like
-        Output array, with jumps of period/2 eliminated
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> theta = [5.74, 5.97, 6.19, 0.13, 0.35, 0.57]
-    >>> unwrap(theta, period=2 * np.pi)
-    [5.74, 5.97, 6.19, 6.413185307179586, 6.633185307179586, 6.8531853071795865]
+__all__ = ['pade']
 
+def pade(T, n=1, numdeg=None):
     """
-    dangle = np.diff(angle)
-    dangle_desired = (dangle + period/2.) % period - period/2.
-    correction = np.cumsum(dangle_desired - dangle)
-    angle[1:] += correction
-    return angle
-
-def issys(obj):
-    """Return True if an object is a system, otherwise False"""
-    return isinstance(obj, lti.LTI)
-
-def db2mag(db):
-    """Convert a gain in decibels (dB) to a magnitude
+    Create a linear system that approximates a delay.
 
-    If A is magnitude,
-
-        db = 20 * log10(A)
+    Return the numerator and denominator coefficients of the Pade approximation.
 
     Parameters
     ----------
-    db : float or ndarray
-        input value or array of values, given in decibels
+    T : number
+        time delay
+    n : positive integer
+        degree of denominator of approximation
+    numdeg: integer, or None (the default)
+            If None, numerator degree equals denominator degree
+            If >= 0, specifies degree of numerator
+            If < 0, numerator degree is n+numdeg
 
     Returns
     -------
-    mag : float or ndarray
-        corresponding magnitudes
+    num, den : array
+        Polynomial coefficients of the delay model, in descending powers of s.
 
-    """
-    return 10. ** (db / 20.)
+    Notes
+    -----
+    Based on:
+      1. Algorithm 11.3.1 in Golub and van Loan, "Matrix Computation" 3rd.
+         Ed. pp. 572-574
+      2. M. Vajta, "Some remarks on Padé-approximations",
+         3rd TEMPUS-INTCOM Symposium
 
-def mag2db(mag):
-    """Convert a magnitude to decibels (dB)
-
-    If A is magnitude,
-
-        db = 20 * log10(A)
-
-    Parameters
-    ----------
-    mag : float or ndarray
-        input magnitude or array of magnitudes
-
-    Returns
-    -------
-    db : float or ndarray
-        corresponding values in decibels
+    Examples
+    --------
+    >>> delay = 1
+    >>> num, den = ct.pade(delay, 3)
+    >>> num, den
+    ([-1.0, 12.0, -60.0, 120.0], [1.0, 12.0, 60.0, 120.0])
+
+    >>> num, den = ct.pade(delay, 3, -2)
+    >>> num, den
+    ([-6.0, 24.0], [1.0, 6.0, 18.0, 24.0])
 
     """
-    return 20. * np.log10(mag)
+    if numdeg is None:
+        numdeg = n
+    elif numdeg < 0:
+        numdeg += n
+
+    if not T >= 0:
+        raise ValueError("require T >= 0")
+    if not n >= 0:
+        raise ValueError("require n >= 0")
+    if not (0 <= numdeg <= n):
+        raise ValueError("require 0 <= numdeg <= n")
+
+    if T == 0:
+        num = [1,]
+        den = [1,]
+    else:
+        num = [0. for i in range(numdeg+1)]
+        num[-1] = 1.
+        cn = 1.
+        for k in range(1, numdeg+1):
+            # derived from Gloub and van Loan eq. for Dpq(z) on p. 572
+            # this accumulative style follows Alg 11.3.1
+            cn *= -T * (numdeg - k + 1)/(numdeg + n - k + 1)/k
+            num[numdeg-k] = cn
+
+        den = [0. for i in range(n+1)]
+        den[-1] = 1.
+        cd = 1.
+        for k in range(1, n+1):
+            # see cn above
+            cd *= T * (n - k + 1)/(numdeg + n - k + 1)/k
+            den[n-k] = cd
+
+        num = [coeff/den[0] for coeff in num]
+        den = [coeff/den[0] for coeff in den]
+    return num, den
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `control-0.9.3.post2/control/descfcn.py` & `control-0.9.4/control/descfcn.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,14 +116,22 @@
         The (complex) value of the describing function at the given amplitudes.
 
     Raises
     ------
     TypeError
         If A[i] < 0 or if A[i] = 0 and the function F(0) is non-zero.
 
+    Examples
+    --------
+    >>> F = lambda x: np.exp(-x)      # Basic diode description
+    >>> A = np.logspace(-1, 1, 20)    # Amplitudes from 0.1 to 10.0
+    >>> df_values = ct.describing_function(F, A)
+    >>> len(df_values)
+    20
+
     """
     # If there is an analytical solution, trying using that first
     if try_method and hasattr(F, 'describing_function'):
         try:
             return np.vectorize(F.describing_function, otypes=[complex])(A)
         except NotImplementedError:
             # Drop through and do the numerical computation
@@ -235,18 +243,18 @@
         a potential limit cycle for the closed loop system with amplitude
         given by the first value of the tuple and frequency given by the
         second value.
 
     Examples
     --------
     >>> H_simple = ct.tf([8], [1, 2, 2, 1])
-    >>> F_saturation = ct.descfcn.saturation_nonlinearity(1)
+    >>> F_saturation = ct.saturation_nonlinearity(1)
     >>> amp = np.linspace(1, 4, 10)
-    >>> ct.describing_function_plot(H_simple, F_saturation, amp)
-    [(3.344008947853124, 1.414213099755523)]
+    >>> ct.describing_function_plot(H_simple, F_saturation, amp)  # doctest: +SKIP
+    [(3.343844998258643, 1.4142293090899216)]
 
     """
     # Decide whether to turn on warnings or not
     if warn is None:
         # Turn warnings on unless omega was specified
         warn = omega is None
 
@@ -350,14 +358,24 @@
         F = saturation_nonlinearity(ub[, lb])
 
     By default, the lower bound is set to the negative of the upper bound.
     Asymmetric saturation functions can be created, but note that these
     functions will not have zero bias and hence care must be taken in using
     the nonlinearity for analysis.
 
+    Examples
+    --------
+    >>> nl = ct.saturation_nonlinearity(5)
+    >>> nl(1)
+    1
+    >>> nl(10)
+    5
+    >>> nl(-10)
+    -5
+
     """
     def __init__(self, ub=1, lb=None):
         # Create the describing function nonlinearity object
         super(saturation_nonlinearity, self).__init__()
 
         # Process arguments
         if lb == None:
@@ -403,14 +421,28 @@
 
         F = relay_hysteresis_nonlinearity(b, c)
 
     The output of this function is `b` if `x > c` and `-b` if `x < -c`.  For
     `-c <= x <= c`, the value depends on the branch of the hysteresis loop (as
     illustrated in Figure 10.20 of FBS2e).
 
+    Examples
+    --------
+    >>> nl = ct.relay_hysteresis_nonlinearity(1, 2)
+    >>> nl(0)
+    -1
+    >>> nl(1)  # not enough for switching on
+    -1
+    >>> nl(5)
+    1
+    >>> nl(-1)  # not enough for switching off
+    1
+    >>> nl(-5)
+    -1
+
     """
     def __init__(self, b, c):
         # Create the describing function nonlinearity object
         super(relay_hysteresis_nonlinearity, self).__init__()
 
         # Initialize the state to bottom branch
         self.branch = -1        # lower branch
@@ -458,14 +490,30 @@
         F = friction_backlash_nonlinearity(b)
 
     This function maintains an internal state representing the 'center' of a
     mechanism with backlash.  If the new input is within `b/2` of the current
     center, the output is unchanged.  Otherwise, the output is given by the
     input shifted by `b/2`.
 
+    Examples
+    --------
+    >>> nl = ct.friction_backlash_nonlinearity(2)  # backlash of +/- 1
+    >>> nl(0)
+    0
+    >>> nl(1)  # not enough to overcome backlash
+    0
+    >>> nl(2)
+    1.0
+    >>> nl(1)
+    1.0
+    >>> nl(0)  # not enough to overcome backlash
+    1.0
+    >>> nl(-1)
+    0.0
+
     """
 
     def __init__(self, b):
         # Create the describing function nonlinearity object
         super(friction_backlash_nonlinearity, self).__init__()
 
         self.b = b              # backlash distance
```

### Comparing `control-0.9.3.post2/control/dtime.py` & `control-0.9.4/control/flatsys/linflat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,152 @@
-"""dtime.py
+# linflat.py - FlatSystem subclass for linear systems
+# RMM, 10 November 2012
+#
+# This file defines a FlatSystem class for a linear system.
+#
+# Copyright (c) 2012 by California Institute of Technology
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions
+# are met:
+#
+# 1. Redistributions of source code must retain the above copyright
+#    notice, this list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright
+#    notice, this list of conditions and the following disclaimer in the
+#    documentation and/or other materials provided with the distribution.
+#
+# 3. Neither the name of the California Institute of Technology nor
+#    the names of its contributors may be used to endorse or promote
+#    products derived from this software without specific prior
+#    written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL CALTECH
+# OR THE CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+# LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF
+# USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+# ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+# OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
+# SUCH DAMAGE.
+
+import numpy as np
+import control
+from .flatsys import FlatSystem
+from ..iosys import LinearIOSystem
 
-Functions for manipulating discrete time systems.
 
-Routines in this module:
+class LinearFlatSystem(FlatSystem, LinearIOSystem):
+    """Base class for a linear, differentially flat system.
 
-sample_system()
-c2d()
-"""
-
-"""Copyright (c) 2012 by California Institute of Technology
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions
-are met:
-
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-
-3. Neither the name of the California Institute of Technology nor
-   the names of its contributors may be used to endorse or promote
-   products derived from this software without specific prior
-   written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-FOR A PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL CALTECH
-OR THE CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF
-USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGE.
-
-Author: Richard M. Murray
-Date: 6 October 2012
-
-$Id: dtime.py 185 2012-08-30 05:44:32Z murrayrm $
-
-"""
-
-from .namedio import isctime
-from .statesp import StateSpace
-
-__all__ = ['sample_system', 'c2d']
-
-# Sample a continuous time system
-def sample_system(sysc, Ts, method='zoh', alpha=None, prewarp_frequency=None,
-        name=None, copy_names=True, **kwargs):
-    """
-    Convert a continuous time system to discrete time by sampling
+    This class is used to create a differentially flat system representation
+    from a linear system.
 
     Parameters
     ----------
-    sysc : LTI (:class:`StateSpace` or :class:`TransferFunction`)
-        Continuous time system to be converted
-    Ts : float > 0
-        Sampling period
-    method : string
-        Method to use for conversion, e.g. 'bilinear', 'zoh' (default)
-    alpha : float within [0, 1]
-            The generalized bilinear transformation weighting parameter, which
-            should only be specified with method="gbt", and is ignored
-            otherwise. See :func:`scipy.signal.cont2discrete`.
-    prewarp_frequency : float within [0, infinity)
-        The frequency [rad/s] at which to match with the input continuous-
-        time system's magnitude and phase (only valid for method='bilinear')
-    name : string, optional
-        Set the name of the sampled system.  If not specified and
-        if `copy_names` is `False`, a generic name <sys[id]> is generated
-        with a unique integer id.  If `copy_names` is `True`, the new system
-        name is determined by adding the prefix and suffix strings in
-        config.defaults['namedio.sampled_system_name_prefix'] and
-        config.defaults['namedio.sampled_system_name_suffix'], with the
-        default being to add the suffix '$sampled'.
-    copy_names : bool, Optional
-        If True, copy the names of the input signals, output
-        signals, and states to the sampled system.
-
-    Returns
-    -------
-    sysd : linsys
-        Discrete time system, with sampling rate Ts
-
-    Other Parameters
-    ----------------
+    linsys : StateSpace
+        LTI StateSpace system to be converted
     inputs : int, list of str or None, optional
-        Description of the system inputs.  If not specified, the origional
-        system inputs are used.  See :class:`InputOutputSystem` for more
-        information.
+        Description of the system inputs.  This can be given as an integer
+        count or as a list of strings that name the individual signals.
+        If an integer count is specified, the names of the signal will be
+        of the form `s[i]` (where `s` is one of `u`, `y`, or `x`).  If
+        this parameter is not given or given as `None`, the relevant
+        quantity will be determined when possible based on other
+        information provided to functions using the system.
     outputs : int, list of str or None, optional
         Description of the system outputs.  Same format as `inputs`.
     states : int, list of str, or None, optional
-        Description of the system states.  Same format as `inputs`. Only
-        available if the system is :class:`StateSpace`.
-
-    Notes
-    -----
-    See :meth:`StateSpace.sample` or :meth:`TransferFunction.sample` for
-    further details.
-
-    Examples
-    --------
-    >>> sysc = TransferFunction([1], [1, 2, 1])
-    >>> sysd = sample_system(sysc, 1, method='bilinear')
-    """
-
-    # Make sure we have a continuous time system
-    if not isctime(sysc):
-        raise ValueError("First argument must be continuous time system")
-
-    return sysc.sample(Ts,
-        method=method, alpha=alpha, prewarp_frequency=prewarp_frequency,
-        name=name, copy_names=copy_names, **kwargs)
-
-
-def c2d(sysc, Ts, method='zoh', prewarp_frequency=None):
-    """
-    Convert a continuous time system to discrete time by sampling
+        Description of the system states.  Same format as `inputs`.
+    dt : None, True or float, optional
+        System timebase.  None (default) indicates continuous
+        time, True indicates discrete time with undefined sampling
+        time, positive number is discrete time with specified
+        sampling time.
+    params : dict, optional
+        Parameter values for the systems.  Passed to the evaluation
+        functions for the system as default values, overriding internal
+        defaults.
+    name : string, optional
+        System name (used for specifying signals)
 
-    Parameters
-    ----------
-    sysc : LTI (:class:`StateSpace` or :class:`TransferFunction`)
-        Continuous time system to be converted
-    Ts : float > 0
-        Sampling period
-    method : string
-        Method to use for conversion, e.g. 'bilinear', 'zoh' (default)
-    prewarp_frequency : real within [0, infinity)
-        The frequency [rad/s] at which to match with the input continuous-
-        time system's magnitude and phase (only valid for method='bilinear')
-
-    Returns
-    -------
-    sysd : LTI of the same class
-        Discrete time system, with sampling rate Ts
-
-    Notes
-    -----
-    See :meth:`StateSpace.sample` or :meth:`TransferFunction.sample`` for
-    further details.
-
-    Examples
-    --------
-    >>> sysc = TransferFunction([1], [1, 2, 1])
-    >>> sysd = sample_system(sysc, 1, method='bilinear')
     """
 
-    #  Call the sample_system() function to do the work
-    sysd = sample_system(sysc, Ts,
-        method=method, prewarp_frequency=prewarp_frequency)
-
-    return sysd
+    def __init__(self, linsys, inputs=None, outputs=None, states=None,
+                 name=None):
+        """Define a flat system from a SISO LTI system.
+
+        Given a reachable, single-input/single-output, linear time-invariant
+        system, create a differentially flat system representation.
+
+        """
+        # Make sure we can handle the system
+        if (not control.isctime(linsys)):
+            raise control.ControlNotImplemented(
+                "requires continuous time, linear control system")
+        elif (not control.issiso(linsys)):
+            raise control.ControlNotImplemented(
+                "only single input, single output systems are supported")
+
+        # Initialize the object as a LinearIO system
+        LinearIOSystem.__init__(
+            self, linsys, inputs=inputs, outputs=outputs, states=states,
+            name=name)
+
+        # Find the transformation to chain of integrators form
+        # Note: store all array as ndarray, not matrix
+        zsys, Tr = control.reachable_form(linsys)
+        Tr = np.array(Tr[::-1, ::])     # flip rows
+
+        # Extract the information that we need
+        self.F = np.array(zsys.A[0, ::-1])      # input function coeffs
+        self.T = Tr                             # state space transformation
+        self.Tinv = np.linalg.inv(Tr)           # compute inverse once
+
+        # Compute the flat output variable z = C x
+        Cfz = np.zeros(np.shape(linsys.C)); Cfz[0, 0] = 1
+        self.Cf = Cfz @ Tr
+
+    # Compute the flat flag from the state (and input)
+    def forward(self, x, u, params):
+        """Compute the flat flag given the states and input.
+
+        See :func:`control.flatsys.FlatSystem.forward` for more info.
+
+        """
+        x = np.reshape(x, (-1, 1))
+        u = np.reshape(u, (1, -1))
+        zflag = [np.zeros(self.nstates + 1)]
+        zflag[0][0] = self.Cf @ x
+        H = self.Cf                     # initial state transformation
+        for i in range(1, self.nstates + 1):
+            zflag[0][i] = H @ (self.A @ x + self.B @ u)
+            H = H @ self.A       # derivative for next iteration
+        return zflag
+
+    # Compute state and input from flat flag
+    def reverse(self, zflag, params):
+        """Compute the states and input given the flat flag.
+
+        See :func:`control.flatsys.FlatSystem.reverse` for more info.
+
+        """
+        z = zflag[0][0:-1]
+        x = self.Tinv @ z
+        u = zflag[0][-1] - self.F @ z
+        return np.reshape(x, self.nstates), np.reshape(u, self.ninputs)
+
+    # Update function
+    def _rhs(self, t, x, u):
+        # Use LinearIOSystem._rhs instead of default (MRO) NonlinearIOSystem
+        return LinearIOSystem._rhs(self, t, x, u)
+
+    # output function
+    def _out(self, t, x, u):
+        # Use LinearIOSystem._out instead of default (MRO) NonlinearIOSystem
+        return LinearIOSystem._out(self, t, x, u)
```

### Comparing `control-0.9.3.post2/control/exception.py` & `control-0.9.4/control/exception.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,39 +59,42 @@
 class ControlNotImplemented(NotImplementedError):
     """Functionality is not yet implemented"""
     pass
 
 # Utility function to see if slycot is installed
 slycot_installed = None
 def slycot_check():
+    """Return True if slycot is installed, otherwise False."""
     global slycot_installed
     if slycot_installed is None:
         try:
             import slycot
             slycot_installed = True
         except:
             slycot_installed = False
     return slycot_installed
 
 
 # Utility function to see if pandas is installed
 pandas_installed = None
 def pandas_check():
+    """Return True if pandas is installed, otherwise False."""
     global pandas_installed
     if pandas_installed is None:
         try:
             import pandas
             pandas_installed = True
         except:
             pandas_installed = False
     return pandas_installed
 
 # Utility function to see if cvxopt is installed
 cvxopt_installed = None
 def cvxopt_check():
+    """Return True if cvxopt is installed, otherwise False."""
     global cvxopt_installed
     if cvxopt_installed is None:
         try:
             import cvxopt
             cvxopt_installed = True
         except:
             cvxopt_installed = False
```

### Comparing `control-0.9.3.post2/control/flatsys/__init__.py` & `control-0.9.4/control/flatsys/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 defined using the :class:`~control.flatsys.BasisFamily` class.  The resulting
 trajectory is return as a :class:`~control.flatsys.SystemTrajectory` object
 and can be evaluated using the :func:`~control.flatsys.SystemTrajectory.eval`
 member function.  Alternatively, the :func:`~control.flatsys.solve_flat_ocp`
 function can be used to solve an optimal control problem with trajectory and
 final costs or constraints.
 
+The docstring examples assume that the following import commands::
+
+  >>> import numpy as np
+  >>> import control as ct
+  >>> import control.flatsys as fs
+
 """
 
 # Basis function families
 from .basis import BasisFamily
 from .poly import PolyFamily
 from .bezier import BezierFamily
 from .bspline import BSplineFamily
```

### Comparing `control-0.9.3.post2/control/flatsys/basis.py` & `control-0.9.4/control/flatsys/basis.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/flatsys/bezier.py` & `control-0.9.4/control/flatsys/bezier.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/flatsys/bspline.py` & `control-0.9.4/control/flatsys/bspline.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/flatsys/flatsys.py` & `control-0.9.4/control/flatsys/flatsys.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,20 @@
     # Start by solving the least squares problem
     # TODO: add warning if rank is too small
     alpha, residuals, rank, s = np.linalg.lstsq(M, Z, rcond=None)
     if rank < Z.size:
         warnings.warn("basis too small; solution may not exist")
 
     if cost is not None or trajectory_constraints is not None:
+        # Make sure that we have enough timepoints to evaluate
+        if timepts.size < 3:
+            raise ControlArgument(
+                "There must be at least three time points if trajectory"
+                " cost or constraints are specified")
+
         # Search over the null space to minimize cost/satisfy constraints
         N = sp.linalg.null_space(M)
 
         # Precompute the collocation matrix the defines the flag at timepts
         Mt_list = []
         for t in timepts[1:-1]:
             Mt_list.append(_basis_flag_matrix(sys, basis, zflag_T0, t))
```

### Comparing `control-0.9.3.post2/control/flatsys/poly.py` & `control-0.9.4/control/flatsys/poly.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/flatsys/systraj.py` & `control-0.9.4/control/flatsys/systraj.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 # SUCH DAMAGE.
 
 import numpy as np
 from ..timeresp import TimeResponseData
 
 class SystemTrajectory:
-    """Class representing a system trajectory.
+    """Class representing a trajectory for a flat system.
 
     The `SystemTrajectory` class is used to represent the
     trajectory of a (differentially flat) system.  Used by the
     :func:`~control.trajsys.point_to_point` function to return a trajectory.
 
     Parameters
     ----------
```

### Comparing `control-0.9.3.post2/control/frdata.py` & `control-0.9.4/control/frdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     -----
     The main data members are 'omega' and 'fresp', where 'omega' is a 1D array
     of frequency points and and 'fresp' is a 3D array of frequency responses,
     with the first dimension corresponding to the output index of the FRD, the
     second dimension corresponding to the input index, and the 3rd dimension
     corresponding to the frequency points in omega.  For example,
 
-    >>> frdata[2,5,:] = numpy.array([1., 0.8-0.2j, 0.2-0.8j])
+    >>> frdata[2,5,:] = numpy.array([1., 0.8-0.2j, 0.2-0.8j])   # doctest: +SKIP
 
     means that the frequency response from the 6th input to the 3rd output at
     the frequencies defined in omega is set to the array above, i.e. the rows
     represent the outputs and the columns represent the inputs.
 
     A frequency response data object is callable and returns the value of the
     transfer function evaluated at a point in the complex plane (must be on
@@ -669,16 +669,25 @@
     If sys is already an frd, and its frequency range matches or
     overlaps the range given in omega then it is returned.  If sys is
     another LTI object or a transfer function, then it is converted to
     a frequency response data at the specified omega. If sys is a
     scalar, then the number of inputs and outputs can be specified
     manually, as in:
 
+    >>> import numpy as np
+    >>> from control.frdata import _convert_to_FRD
+
+    >>> omega = np.logspace(-1, 1)
     >>> frd = _convert_to_FRD(3., omega) # Assumes inputs = outputs = 1
-    >>> frd = _convert_to_FRD(1., omegs, inputs=3, outputs=2)
+    >>> frd.ninputs, frd.noutputs
+    (1, 1)
+
+    >>> frd = _convert_to_FRD(1., omega, inputs=3, outputs=2)
+    >>> frd.ninputs, frd.noutputs
+    (3, 2)
 
     In the latter example, sys's matrix transfer function is [[1., 1., 1.]
                                                               [1., 1., 1.]].
 
     """
 
     if isinstance(sys, FRD):
@@ -751,9 +760,21 @@
     -------
     sys: FRD
         New frequency response system
 
     See Also
     --------
     FRD, ss, tf
+
+    Examples
+    --------
+    >>> # Create from measurements
+    >>> response = [1.0, 1.0, 0.5]
+    >>> freqs = [1, 10, 100]
+    >>> F = ct.frd(response, freqs)
+
+    >>> G = ct.tf([1], [1, 1])
+    >>> freqs = [1, 10, 100]
+    >>> F = ct.frd(G, freqs)
+
     """
     return FRD(*args)
```

### Comparing `control-0.9.3.post2/control/freqplot.py` & `control-0.9.4/control/freqplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,16 +170,16 @@
        along the upper branch of the unit circle, using the mapping ``z =
        exp(1j * omega * dt)`` where `omega` ranges from 0 to `pi/dt` and `dt`
        is the discrete timebase.  If timebase not specified (``dt=True``),
        `dt` is set to 1.
 
     Examples
     --------
-    >>> sys = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
-    >>> mag, phase, omega = bode(sys)
+    >>> G = ct.ss([[-1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
+    >>> Gmag, Gphase, Gomega = ct.bode_plot(G)
 
     """
     # Make a copy of the kwargs dictionary since we will modify it
     kwargs = dict(kwargs)
 
     # Check to see if legacy 'Plot' keyword was used
     if 'Plot' in kwargs:
@@ -272,26 +272,29 @@
             #
             # Post-process the phase to handle initial value and wrapping
             #
 
             if initial_phase is None:
                 # Start phase in the range 0 to -360 w/ initial phase = -180
                 # If wrap_phase is true, use 0 instead (phase \in (-pi, pi])
-                initial_phase = -math.pi if wrap_phase is not True else 0
+                initial_phase_value = -math.pi if wrap_phase is not True else 0
             elif isinstance(initial_phase, (int, float)):
                 # Allow the user to override the default calculation
                 if deg:
-                    initial_phase = initial_phase/180. * math.pi
+                    initial_phase_value = initial_phase/180. * math.pi
+                else:
+                    initial_phase_value = initial_phase
+
             else:
                 raise ValueError("initial_phase must be a number.")
 
             # Shift the phase if needed
-            if abs(phase[0] - initial_phase) > math.pi:
+            if abs(phase[0] - initial_phase_value) > math.pi:
                 phase -= 2*math.pi * \
-                    round((phase[0] - initial_phase) / (2*math.pi))
+                    round((phase[0] - initial_phase_value) / (2*math.pi))
 
             # Phase wrapping
             if wrap_phase is False:
                 phase = unwrap(phase)   # unwrap the phase
             elif wrap_phase is True:
                 pass                    # default calculation OK
             elif isinstance(wrap_phase, (int, float)):
@@ -551,29 +554,29 @@
 
     Parameters
     ----------
     syslist : list of LTI
         List of linear input/output systems (single system is OK). Nyquist
         curves for each system are plotted on the same graph.
 
-    plot : boolean
-        If True, plot magnitude
-
-    omega : array_like
+    omega : array_like, optional
         Set of frequencies to be evaluated, in rad/sec.
 
-    omega_limits : array_like of two values
+    omega_limits : array_like of two values, optional
         Limits to the range of frequencies. Ignored if omega is provided, and
         auto-generated if omitted.
 
-    omega_num : int
+    omega_num : int, optional
         Number of frequency samples to plot.  Defaults to
         config.defaults['freqplot.number_of_samples'].
 
-    color : string
+    plot : boolean, optional
+        If True (default), plot the Nyquist plot.
+
+    color : string, optional
         Used to specify the color of the line and arrowhead.
 
     return_contour : bool, optional
         If 'True', return the contour used to evaluate the Nyquist plot.
 
     **kwargs : :func:`matplotlib.pyplot.plot` keyword properties, optional
         Additional keywords (passed to `matplotlib`)
@@ -683,18 +686,26 @@
        of the indentation is given by `indent_radius` and it is taken to the
        right of stable poles and the left of unstable poles.  If a pole is
        exactly on the imaginary axis, the `indent_direction` parameter can be
        used to set the direction of indentation.  Setting `indent_direction`
        to `none` will turn off indentation.  If `return_contour` is True, the
        exact contour used for evaluation is returned.
 
+    3. For those portions of the Nyquist plot in which the contour is
+       indented to avoid poles, resuling in a scaling of the Nyquist plot,
+       the line styles are according to the settings of the `primary_style`
+       and `mirror_style` keywords.  By default the scaled portions of the
+       primary curve use a dotted line style and the scaled portion of the
+       mirror image use a dashdot line style.
+
     Examples
     --------
-    >>> sys = ss([[1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
-    >>> count = nyquist_plot(sys)
+    >>> G = ct.zpk([], [-1, -2, -3], gain=100)
+    >>> ct.nyquist_plot(G)
+    2
 
     """
     # Check to see if legacy 'Plot' keyword was used
     if 'Plot' in kwargs:
         warnings.warn("'Plot' keyword is deprecated in nyquist_plot; "
                       "use 'plot'", FutureWarning)
         # Map 'Plot' keyword to 'plot' keyword
@@ -804,55 +815,56 @@
             if np.any(omega_sys * sys.dt > np.pi) and warn_nyquist:
                 warnings.warn("evaluation above Nyquist frequency")
 
         # do indentations in s-plane where it is more convenient
         splane_contour = 1j * omega_sys
 
         # Bend the contour around any poles on/near the imaginary axis
-        # TODO: smarter indent radius that depends on dcgain of system
-        # and timebase of discrete system.
         if isinstance(sys, (StateSpace, TransferFunction)) \
                 and indent_direction != 'none':
             if sys.isctime():
                 splane_poles = sys.poles()
                 splane_cl_poles = sys.feedback().poles()
             else:
-                # map z-plane poles to s-plane, ignoring any at the origin
-                # because we don't need to indent for them
+                # map z-plane poles to s-plane. We ignore any at the origin
+                # to avoid numerical warnings because we know we
+                # don't need to indent for them
                 zplane_poles = sys.poles()
                 zplane_poles = zplane_poles[~np.isclose(abs(zplane_poles), 0.)]
                 splane_poles = np.log(zplane_poles) / sys.dt
 
                 zplane_cl_poles = sys.feedback().poles()
+                # eliminate z-plane poles at the origin to avoid warnings
                 zplane_cl_poles = zplane_cl_poles[
-                    ~np.isclose(abs(zplane_poles), 0.)]
+                    ~np.isclose(abs(zplane_cl_poles), 0.)]
                 splane_cl_poles = np.log(zplane_cl_poles) / sys.dt
 
             #
             # Check to make sure indent radius is small enough
             #
-            # If there is a closed loop pole that is near the imaginary access
+            # If there is a closed loop pole that is near the imaginary axis
             # at a point that is near an open loop pole, it is possible that
             # indentation might skip or create an extraneous encirclement.
             # We check for that situation here and generate a warning if that
             # could happen.
             #
             for p_cl in splane_cl_poles:
                 # See if any closed loop poles are near the imaginary axis
                 if abs(p_cl.real) <= indent_radius:
                     # See if any open loop poles are close to closed loop poles
-                    p_ol = splane_poles[
-                        (np.abs(splane_poles - p_cl)).argmin()]
-
-                    if abs(p_ol - p_cl) <= indent_radius and \
-                       warn_encirclements:
-                        warnings.warn(
-                            "indented contour may miss closed loop pole; "
-                            "consider reducing indent_radius to be less than "
-                            f"{abs(p_ol - p_cl):5.2g}", stacklevel=2)
+                    if len(splane_poles) > 0:
+                        p_ol = splane_poles[
+                            (np.abs(splane_poles - p_cl)).argmin()]
+
+                        if abs(p_ol - p_cl) <= indent_radius and \
+                                warn_encirclements:
+                            warnings.warn(
+                                "indented contour may miss closed loop pole; "
+                                "consider reducing indent_radius to below "
+                                f"{abs(p_ol - p_cl):5.2g}", stacklevel=2)
 
             #
             # See if we should add some frequency points near imaginary poles
             #
             for p in splane_poles:
                 # See if we need to process this pole (skip if on the negative
                 # imaginary axis or not near imaginary axis + user override)
@@ -882,37 +894,38 @@
                 splane_contour = np.concatenate((
                     splane_contour[0:first_point+1],
                     (1j * np.linspace(
                         start_freq, p.imag + indent_radius, indent_points)),
                     splane_contour[last_point:]))
 
             # Indent points that are too close to a pole
-            for i, s in enumerate(splane_contour):
-                # Find the nearest pole
-                p = splane_poles[(np.abs(splane_poles - s)).argmin()]
-
-                # See if we need to indent around it
-                if abs(s - p) < indent_radius:
-                    # Figure out how much to offset (simple trigonometry)
-                    offset = np.sqrt(indent_radius ** 2 - (s - p).imag ** 2) \
-                        - (s - p).real
-
-                    # Figure out which way to offset the contour point
-                    if p.real < 0 or (p.real == 0 and
-                                      indent_direction == 'right'):
-                        # Indent to the right
-                        splane_contour[i] += offset
-
-                    elif p.real > 0 or (p.real == 0 and
-                                         indent_direction == 'left'):
-                        # Indent to the left
-                        splane_contour[i] -= offset
+            if len(splane_poles) > 0: # accomodate no splane poles if dtime sys
+                for i, s in enumerate(splane_contour):
+                    # Find the nearest pole
+                    p = splane_poles[(np.abs(splane_poles - s)).argmin()]
+
+                    # See if we need to indent around it
+                    if abs(s - p) < indent_radius:
+                        # Figure out how much to offset (simple trigonometry)
+                        offset = np.sqrt(indent_radius ** 2 - (s - p).imag ** 2) \
+                            - (s - p).real
+
+                        # Figure out which way to offset the contour point
+                        if p.real < 0 or (p.real == 0 and
+                                        indent_direction == 'right'):
+                            # Indent to the right
+                            splane_contour[i] += offset
+
+                        elif p.real > 0 or (p.real == 0 and
+                                            indent_direction == 'left'):
+                            # Indent to the left
+                            splane_contour[i] -= offset
 
-                    else:
-                        raise ValueError("unknown value for indent_direction")
+                        else:
+                            raise ValueError("unknown value for indent_direction")
 
         # change contour to z-plane if necessary
         if sys.isctime():
             contour = splane_contour
         else:
             contour = np.exp(splane_contour * sys.dt)
 
@@ -1017,17 +1030,19 @@
             # we move along the curve
             curve_offset = _compute_curve_offset(
                 resp, scale_mask, max_curve_offset)
 
             # Plot the scaled sections of the curve (changing linestyle)
             x_scl = np.ma.masked_where(scale_mask, resp.real)
             y_scl = np.ma.masked_where(scale_mask, resp.imag)
-            plt.plot(
-                x_scl * (1 + curve_offset), y_scl * (1 + curve_offset),
-                primary_style[1], color=c, **kwargs)
+            if x_scl.count() >= 1 and y_scl.count() >= 1:
+                plt.plot(
+                    x_scl * (1 + curve_offset),
+                    y_scl * (1 + curve_offset),
+                    primary_style[1], color=c, **kwargs)
 
             # Plot the primary curve (invisible) for setting arrows
             x, y = resp.real.copy(), resp.imag.copy()
             x[reg_mask] *= (1 + curve_offset[reg_mask])
             y[reg_mask] *= (1 + curve_offset[reg_mask])
             p = plt.plot(x, y, linestyle='None', color=c, **kwargs)
 
@@ -1037,18 +1052,19 @@
                 ax, p[0], arrow_pos, arrowstyle=arrow_style, dir=1)
 
             # Plot the mirror image
             if mirror_style is not False:
                 # Plot the regular and scaled segments
                 plt.plot(
                     x_reg, -y_reg, mirror_style[0], color=c, **kwargs)
-                plt.plot(
-                    x_scl * (1 - curve_offset),
-                    -y_scl * (1 - curve_offset),
-                    mirror_style[1], color=c, **kwargs)
+                if x_scl.count() >= 1 and y_scl.count() >= 1:
+                    plt.plot(
+                        x_scl * (1 - curve_offset),
+                        -y_scl * (1 - curve_offset),
+                        mirror_style[1], color=c, **kwargs)
 
                 # Add the arrows (on top of an invisible contour)
                 x, y = resp.real.copy(), resp.imag.copy()
                 x[reg_mask] *= (1 - curve_offset[reg_mask])
                 y[reg_mask] *= (1 - curve_offset[reg_mask])
                 p = plt.plot(x, -y, linestyle='None', color=c, **kwargs)
                 _add_arrows_to_line2D(
@@ -1248,14 +1264,21 @@
         Range of frequencies (list or bounds) in rad/sec
     **kwargs : :func:`matplotlib.pyplot.plot` keyword properties, optional
         Additional keywords (passed to `matplotlib`)
 
     Returns
     -------
     None
+
+    Examples
+    --------
+    >>> P = ct.tf([1], [1, 1])
+    >>> C = ct.tf([2], [1])
+    >>> ct.gangof4_plot(P, C)
+
     """
     if not P.issiso() or not C.issiso():
         # TODO: Add MIMO go4 plots.
         raise ControlMIMONotImplemented(
             "Gang of four is currently only implemented for SISO systems.")
 
     # Get the default parameter values
@@ -1391,23 +1414,21 @@
     ----------------
     grid : bool
         If True, plot grid lines on gain and phase plots.  Default is set by
         `config.defaults['freqplot.grid']`.
 
     Examples
     --------
-    >>> import numpy as np
+    >>> omegas = np.logspace(-4, 1, 1000)
     >>> den = [75, 1]
-    >>> sys = TransferFunction(
-        [[[87.8], [-86.4]], [[108.2], [-109.6]]], [[den, den], [den, den]])
-    >>> omega = np.logspace(-4, 1, 1000)
-    >>> sigma, omega = singular_values_plot(sys, plot=True)
-    >>> singular_values_plot(sys, 0.0, plot=False)
-    (array([[197.20868123],
-           [  1.39141948]]), array([0.]))
+    >>> G = ct.tf([[[87.8], [-86.4]], [[108.2], [-109.6]]],
+    ...           [[den, den], [den, den]])
+    >>> sigmas, omegas = ct.singular_values_plot(G, omega=omegas, plot=False)
+
+    >>> sigmas, omegas = ct.singular_values_plot(G, 0.0, plot=False)
 
     """
 
     # Make a copy of the kwargs dictionary since we will modify it
     kwargs = dict(kwargs)
 
     # Get values for params (and pop from list to allow keyword use in plot)
@@ -1615,17 +1636,18 @@
     Returns
     -------
     omega : array
         Range of frequencies in rad/sec
 
     Examples
     --------
-    >>> from matlab import ss
-    >>> sys = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
-    >>> omega = _default_frequency_range(sys)
+    >>> G = ct.ss([[-1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
+    >>> omega = ct._default_frequency_range(G)
+    >>> omega.min(), omega.max()
+    (0.1, 100.0)
 
     """
     # Set default values for options
     number_of_samples = config._get_param(
         'freqplot', 'number_of_samples', number_of_samples)
     feature_periphery_decades = config._get_param(
         'freqplot', 'feature_periphery_decades', feature_periphery_decades, 1)
@@ -1745,16 +1767,11 @@
             'p',  # pico (10^-12)
             'f',  # femto (10^-15)
             'a',  # atto (10^-18)
             'z',  # zepto (10^-21)
             'y'][8 - pow1000]  # yocto (10^-24)
 
 
-def find_nearest_omega(omega_list, omega):
-    omega_list = np.asarray(omega_list)
-    return omega_list[(np.abs(omega_list - omega)).argmin()]
-
-
 # Function aliases
 bode = bode_plot
 nyquist = nyquist_plot
 gangof4 = gangof4_plot
```

### Comparing `control-0.9.3.post2/control/grid.py` & `control-0.9.4/control/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     ax = plt.axes()
 
     _final_setup(ax)
     return ax, f
 
 
 def zgrid(zetas=None, wns=None, ax=None):
-    '''Draws discrete damping and frequency grid'''
+    """Draws discrete damping and frequency grid"""
 
     fig = plt.gcf()
     if ax is None:
         ax = fig.gca()
 
     # Constant damping lines
     if zetas is None:
```

### Comparing `control-0.9.3.post2/control/iosys.py` & `control-0.9.4/control/iosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         indicates discrete time with unspecified sampling time, positive
         number is discrete time with specified sampling time, None indicates
         unspecified timebase (either continuous or discrete time).
     name : string, optional
         System name (used for specifying signals). If unspecified, a generic
         name <sys[id]> is generated with a unique integer id.
     params : dict, optional
-        Parameter values for the systems.  Passed to the evaluation functions
+        Parameter values for the system.  Passed to the evaluation functions
         for the system as default values, overriding internal defaults.
 
     Attributes
     ----------
     ninputs, noutputs, nstates : int
         Number of input, output and state variables
     input_index, output_index, state_index : dict
@@ -587,21 +587,16 @@
         # Set the system name, inputs, outputs, and states
         if 'copy' in kwargs:
             copy_names = kwargs.pop('copy')
             warn("keyword 'copy' is deprecated. please use 'copy_names'",
                 DeprecationWarning)
 
         if copy_names:
-            linsys._copy_names(self)
-            if name is None:
-                linsys.name = \
-                    config.defaults['namedio.linearized_system_name_prefix']+\
-                    linsys.name+\
-                    config.defaults['namedio.linearized_system_name_suffix']
-            else:
+            linsys._copy_names(self, prefix_suffix_name='linearized')
+            if name is not None:
                 linsys.name = name
 
         # re-init to include desired signal names if names were provided
         return LinearIOSystem(linsys, **kwargs)
 
 class LinearIOSystem(InputOutputSystem, StateSpace):
     """Input/output representation of a linear (state space) system.
@@ -672,14 +667,20 @@
             self, inputs=inputs, outputs=outputs, states=states,
             params=None, dt=dt, name=name)
 
         # Initalize additional state space variables
         StateSpace.__init__(
             self, linsys, remove_useless_states=False, init_namedio=False)
 
+    # When sampling a LinearIO system, return a LinearIOSystem
+    def sample(self, *args, **kwargs):
+        return LinearIOSystem(StateSpace.sample(self, *args, **kwargs))
+
+    sample.__doc__ = StateSpace.sample.__doc__
+
     # The following text needs to be replicated from StateSpace in order for
     # this entry to show up properly in sphinx doccumentation (not sure why,
     # but it was the only way to get it to work).
     #
     #: Deprecated attribute; use :attr:`nstates` instead.
     #:
     #: The ``state`` attribute was used to store the number of states for : a
@@ -1369,21 +1370,19 @@
     def unused_signals(self):
         """Find unused subsystem inputs and outputs
 
         Returns
         -------
 
         unused_inputs : dict
-
           A mapping from tuple of indices (isys, isig) to string
           '{sys}.{sig}', for all unused subsystem inputs.
 
         unused_outputs : dict
-
-          A mapping from tuple of indices (isys, isig) to string
+          A mapping from tuple of indices (osys, osig) to string
           '{sys}.{sig}', for all unused subsystem outputs.
 
         """
         used_sysinp_via_inp = np.nonzero(self.input_map)[0]
         used_sysout_via_out = np.nonzero(self.output_map)[1]
         used_sysinp_via_con, used_sysout_via_con = np.nonzero(self.connect_map)
 
@@ -1429,18 +1428,21 @@
 
         """
         return {(isys, isig): f'{sys.name}.{basename}'
                 for isys, sys in enumerate(self.syslist)
                 for sig, isig in sys.output_index.items()
                 if sig == (basename)}
 
-    def check_unused_signals(self, ignore_inputs=None, ignore_outputs=None):
+    def check_unused_signals(
+            self, ignore_inputs=None, ignore_outputs=None, warning=True):
         """Check for unused subsystem inputs and outputs
 
-        If any unused inputs or outputs are found, emit a warning.
+        Check to see if there are any unused signals and return a list of
+        unused input and output signal descriptions.  If `warning` is True
+        and any unused inputs or outputs are found, emit a warning.
 
         Parameters
         ----------
         ignore_inputs : list of input-spec
           Subsystem inputs known to be unused.  input-spec can be any of:
             'sig', 'sys.sig', (isys, isig), ('sys', isig)
 
@@ -1450,14 +1452,24 @@
         ignore_outputs : list of output-spec
           Subsystem outputs known to be unused.  output-spec can be any of:
             'sig', 'sys.sig', (isys, isig), ('sys', isig)
 
           If the 'sig' form is used, all subsystem outputs with that
           name are considered ignored.
 
+        Returns
+        -------
+        dropped_inputs: list of tuples
+            A list of the dropped input signals, with each element of the
+            list in the form of (isys, isig).
+
+        dropped_outputs: list of tuples
+            A list of the dropped output signals, with each element of the
+            list in the form of (osys, osig).
+
         """
 
         if ignore_inputs is None:
             ignore_inputs = []
 
         if ignore_outputs is None:
             ignore_outputs = []
@@ -1473,15 +1485,15 @@
                     raise ValueError("Couldn't find ignored input "
                                      f"{ignore_input} in subsystems")
                 ignore_input_map.update(ignore_idxs)
             else:
                 ignore_input_map[self._parse_signal(
                     ignore_input, 'input')[:2]] = ignore_input
 
-        # (isys, isig) -> signal-spec
+        # (osys, osig) -> signal-spec
         ignore_output_map = {}
         for ignore_output in ignore_outputs:
             if isinstance(ignore_output, str) and '.' not in ignore_output:
                 ignore_found = self._find_outputs_by_basename(ignore_output)
                 if not ignore_found:
                     raise ValueError("Couldn't find ignored output "
                                      f"{ignore_output} in subsystems")
@@ -1492,38 +1504,40 @@
 
         dropped_inputs = set(unused_inputs) - set(ignore_input_map)
         dropped_outputs = set(unused_outputs) - set(ignore_output_map)
 
         used_ignored_inputs = set(ignore_input_map) - set(unused_inputs)
         used_ignored_outputs = set(ignore_output_map) - set(unused_outputs)
 
-        if dropped_inputs:
+        if warning and dropped_inputs:
             msg = ('Unused input(s) in InterconnectedSystem: '
                    + '; '.join(f'{inp}={unused_inputs[inp]}'
                                for inp in dropped_inputs))
             warn(msg)
 
-        if dropped_outputs:
+        if warning and dropped_outputs:
             msg = ('Unused output(s) in InterconnectedSystem: '
                    + '; '.join(f'{out} : {unused_outputs[out]}'
                                for out in dropped_outputs))
             warn(msg)
 
-        if used_ignored_inputs:
+        if warning and used_ignored_inputs:
             msg = ('Input(s) specified as ignored is (are) used: '
                    + '; '.join(f'{inp} : {ignore_input_map[inp]}'
                                for inp in used_ignored_inputs))
             warn(msg)
 
-        if used_ignored_outputs:
+        if warning and used_ignored_outputs:
             msg = ('Output(s) specified as ignored is (are) used: '
                    + '; '.join(f'{out}={ignore_output_map[out]}'
                                for out in used_ignored_outputs))
             warn(msg)
 
+        return dropped_inputs, dropped_outputs
+
 
 class LinearICSystem(InterconnectedSystem, LinearIOSystem):
 
     """Interconnection of a set of linear input/output systems.
 
     This class is used to implement a system that is an interconnection of
     linear input/output systems.  It has all of the structure of an
@@ -1681,14 +1695,23 @@
     1. If a smaller number of initial conditions are given than the number of
        states in the system, the initial conditions will be padded with
        zeros.  This is often useful for interconnected control systems where
        the process dynamics are the first system and all other components
        start with zero initial condition since this can be specified as
        [xsys_0, 0].  A warning is issued if the initial conditions are padded
        and and the final listed initial state is not zero.
+    
+    2. If discontinuous inputs are given, the underlying SciPy numerical
+       integration algorithms can sometimes produce erroneous results due
+       to the default tolerances that are used.  The `ivp_method` and
+       `ivp_keywords` parameters can be used to tune the ODE solver and
+       produce better results.  In particular, using 'LSODA' as the
+       `ivp_method` or setting the `rtol` parameter to a smaller value
+       (e.g. using `ivp_kwargs={'rtol': 1e-4}`) can provide more accurate
+       results.
 
     """
     #
     # Process keyword arguments
     #
 
     # Figure out the method to be used
@@ -1839,15 +1862,15 @@
         # Compute the input and output at each point in time
         for i, t in enumerate(t_eval):
             u[:, i] = ufun(t)
             y[:, i] = sys._out(t, [], u[:, i])
 
         return TimeResponseData(
             t_eval, y, None, u, issiso=sys.issiso(),
-            output_labels=sys.output_index, input_labels=sys.input_index,
+            output_labels=sys.output_labels, input_labels=sys.input_labels,
             transpose=transpose, return_x=return_x, squeeze=squeeze)
 
     # Create a lambda function for the right hand side
     def ivp_rhs(t, x):
         return sys._rhs(t, x, ufun(t))
 
     # Perform the simulation
@@ -1918,16 +1941,16 @@
         soln.success = True     # No way to fail
 
     else:                       # Neither ctime or dtime??
         raise TypeError("Can't determine system type")
 
     return TimeResponseData(
         soln.t, y, soln.y, u, issiso=sys.issiso(),
-        output_labels=sys.output_index, input_labels=sys.input_index,
-        state_labels=sys.state_index,
+        output_labels=sys.output_labels, input_labels=sys.input_labels,
+        state_labels=sys.state_labels,
         transpose=transpose, return_x=return_x, squeeze=squeeze)
 
 
 def find_eqpt(sys, x0, u0=None, y0=None, t=0, params=None,
               iu=None, iy=None, ix=None, idx=None, dx0=None,
               return_y=False, return_result=False):
     """Find the equilibrium point for an input/output system.
@@ -2348,20 +2371,22 @@
     --------
     tf
     ss2tf
     tf2ss
 
     Examples
     --------
-    >>> # Create a Linear I/O system object from from for matrices
-    >>> sys1 = ss([[1, -2], [3 -4]], [[5], [7]], [[6, 8]], [[9]])
+    Create a Linear I/O system object from matrices.
+
+    >>> G = ct.ss([[-1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
+
+    Convert a TransferFunction to a StateSpace object.
 
-    >>> # Convert a TransferFunction to a StateSpace object.
-    >>> sys_tf = tf([2.], [1., 3])
-    >>> sys2 = ss(sys_tf)
+    >>> sys_tf = ct.tf([2.], [1., 3])
+    >>> sys2 = ct.ss(sys_tf)
 
     """
     # See if this is a nonlinear I/O system
     if len(args) > 0 and (hasattr(args[0], '__call__') or args[0] is None) \
        and not isinstance(args[0], (InputOutputSystem, LTI)):
         # Function as first (or second) argument => assume nonlinear IO system
         return NonlinearIOSystem(*args, **kwargs)
@@ -2375,15 +2400,20 @@
         if isinstance(sys, LTI):
             # Check for system with no states and specified state names
             if sys.nstates is None and 'states' in kwargs:
                 warn("state labels specified for "
                      "non-unique state space realization")
 
             # Create a state space system from an LTI system
-            sys = LinearIOSystem(_convert_to_statespace(sys), **kwargs)
+            sys = LinearIOSystem(
+                _convert_to_statespace(
+                    sys,
+                    use_prefix_suffix=not sys._generic_name_check()),
+                **kwargs)
+
         else:
             raise TypeError("ss(sys): sys must be a StateSpace or "
                             "TransferFunction object.  It is %s." % type(sys))
     else:
         raise TypeError(
             "Needs 1, 4, or 5 arguments; received %i." % len(args))
 
@@ -2472,14 +2502,23 @@
 
     Create a stable, discrete-time, random state space system
 
     Create a stable *discrete time* random state space object.  This
     function calls :func:`rss` using either the `dt` keyword provided by
     the user or `dt=True` if not specified.
 
+    Examples
+    --------
+    >>> G = ct.drss(states=4, outputs=2, inputs=1)
+    >>> G.ninputs, G.noutputs, G.nstates
+    (1, 2, 4)
+    >>> G.isdtime()
+    True
+
+
     """
     # Make sure the timebase makes sense
     if 'dt' in kwargs:
         dt = kwargs['dt']
 
         if dt == 0:
             raise ValueError("drss called with continuous timebase")
@@ -2562,31 +2601,34 @@
     ss2io
     tf2ss
 
     Examples
     --------
     >>> num = [[[1., 2.], [3., 4.]], [[5., 6.], [7., 8.]]]
     >>> den = [[[9., 8., 7.], [6., 5., 4.]], [[3., 2., 1.], [-1., -2., -3.]]]
-    >>> sys1 = tf2ss(num, den)
+    >>> sys1 = ct.tf2ss(num, den)
 
-    >>> sys_tf = tf(num, den)
-    >>> sys2 = tf2ss(sys_tf)
+    >>> sys_tf = ct.tf(num, den)
+    >>> G = ct.tf2ss(sys_tf)
+    >>> G.ninputs, G.noutputs, G.nstates
+    (2, 2, 8)
 
     """
     # Convert the system to a state space system
     linsys = tf2ss(*args)
 
     # Now convert the state space system to an I/O system
     return LinearIOSystem(linsys, **kwargs)
 
 
 # Function to create an interconnected system
-def interconnect(syslist, connections=None, inplist=None, outlist=None,
-                 params=None, check_unused=True, ignore_inputs=None,
-                 ignore_outputs=None, warn_duplicate=None, **kwargs):
+def interconnect(
+        syslist, connections=None, inplist=None, outlist=None, params=None,
+        check_unused=True, add_unused=False, ignore_inputs=None,
+        ignore_outputs=None, warn_duplicate=None, **kwargs):
     """Interconnect a set of input/output systems.
 
     This function creates a new system that is an interconnection of a set of
     input/output systems.  If all of the input systems are linear I/O systems
     (type :class:`~control.LinearIOSystem`) then the resulting system will be
     a linear interconnected I/O system (type :class:`~control.LinearICSystem`)
     with the appropriate inputs, outputs, and states.  Otherwise, an
@@ -2649,16 +2691,16 @@
 
             [input-spec1, input-spec2, ...]
 
         Each system input is added to the input for the listed subsystem.  If
         the system input connects to only one subsystem input, a single input
         specification can be given (without the inner list).
 
-        If omitted, the input map can be specified using the
-        :func:`~control.InterconnectedSystem.set_input_map` method.
+        If omitted the `input` parameter will be used to identify the list
+        of input signals to the overall system.
 
     outlist : list of output connections, optional
         List of connections for how the outputs from the subsystems are mapped
         to overall system outputs.  The output connection description is the
         same as the form defined in the inplist specification (including the
         optional gain term).  Numbered outputs must be chosen from the list of
         subsystem outputs, but named outputs can also be contained in the list
@@ -2703,68 +2745,71 @@
         * dt = True: discrete time with unspecified sampling period
         * dt = None: no timebase specified
 
     name : string, optional
         System name (used for specifying signals). If unspecified, a generic
         name <sys[id]> is generated with a unique integer id.
 
-    check_unused : bool
+    check_unused : bool, optional
         If True, check for unused sub-system signals.  This check is
         not done if connections is False, and neither input nor output
         mappings are specified.
 
-    ignore_inputs : list of input-spec
+    add_unused : bool, optional
+        If True, subsystem signals that are not connected to other components
+        are added as inputs and outputs of the interconnected system.
+
+    ignore_inputs : list of input-spec, optional
         A list of sub-system inputs known not to be connected.  This is
         *only* used in checking for unused signals, and does not
         disable use of the input.
 
         Besides the usual input-spec forms (see `connections`), an
         input-spec can be just the signal base name, in which case all
         signals from all sub-systems with that base name are
         considered ignored.
 
-    ignore_outputs : list of output-spec
+    ignore_outputs : list of output-spec, optional
         A list of sub-system outputs known not to be connected.  This
         is *only* used in checking for unused signals, and does not
         disable use of the output.
 
         Besides the usual output-spec forms (see `connections`), an
         output-spec can be just the signal base name, in which all
         outputs from all sub-systems with that base name are
         considered ignored.
 
-    warn_duplicate : None, True, or False
+    warn_duplicate : None, True, or False, optional
         Control how warnings are generated if duplicate objects or names are
         detected.  In `None` (default), then warnings are generated for
         systems that have non-generic names.  If `False`, warnings are not
         generated and if `True` then warnings are always generated.
 
 
     Examples
     --------
-    >>> P = control.LinearIOSystem(
-    >>>        control.rss(2, 2, 2, strictly_proper=True), name='P')
-    >>> C = control.LinearIOSystem(control.rss(2, 2, 2), name='C')
-    >>> T = control.interconnect(
-    >>>     [P, C],
-    >>>     connections = [
-    >>>       ['P.u[0]', 'C.y[0]'], ['P.u[1]', 'C.y[1]'],
-    >>>       ['C.u[0]', '-P.y[0]'], ['C.u[1]', '-P.y[1]']],
-    >>>     inplist = ['C.u[0]', 'C.u[1]'],
-    >>>     outlist = ['P.y[0]', 'P.y[1]'],
-    >>> )
+    >>> P = ct.rss(2, 2, 2, strictly_proper=True, name='P')
+    >>> C = ct.rss(2, 2, 2, name='C')
+    >>> T = ct.interconnect(
+    ...     [P, C],
+    ...     connections = [
+    ...         ['P.u[0]', 'C.y[0]'], ['P.u[1]', 'C.y[1]'],
+    ...         ['C.u[0]', '-P.y[0]'], ['C.u[1]', '-P.y[1]']],
+    ...     inplist = ['C.u[0]', 'C.u[1]'],
+    ...     outlist = ['P.y[0]', 'P.y[1]'],
+    ... )
 
     For a SISO system, this example can be simplified by using the
     :func:`~control.summing_block` function and the ability to automatically
     interconnect signals with the same names:
 
-    >>> P = control.tf(1, [1, 0], inputs='u', outputs='y')
-    >>> C = control.tf(10, [1, 1], inputs='e', outputs='u')
-    >>> sumblk = control.summing_junction(inputs=['r', '-y'], output='e')
-    >>> T = control.interconnect([P, C, sumblk], inputs='r', outputs='y')
+    >>> P = ct.tf(1, [1, 0], inputs='u', outputs='y')
+    >>> C = ct.tf(10, [1, 1], inputs='e', outputs='u')
+    >>> sumblk = ct.summing_junction(inputs=['r', '-y'], output='e')
+    >>> T = ct.interconnect([P, C, sumblk], inputs='r', outputs='y')
 
     Notes
     -----
     If a system is duplicated in the list of systems to be connected,
     a warning is generated and a copy of the system is created with the
     name of the new system determined by adding the prefix and suffix
     strings in config.defaults['namedio.linearized_system_name_prefix']
@@ -2836,25 +2881,25 @@
     for signal in inplist:
         # Create an empty connection and append to inplist
         connection = []
 
         # Check for signal names without a system name
         if isinstance(signal, str) and len(signal.split('.')) == 1:
             # Get the signal name
-            name = signal[1:] if signal[0] == '-' else signal
+            signal_name = signal[1:] if signal[0] == '-' else signal
             sign = '-' if signal[0] == '-' else ""
 
             # Look for the signal name as a system input
             for sys in syslist:
-                if name in sys.input_index.keys():
-                    connection.append(sign + sys.name + "." + name)
+                if signal_name in sys.input_labels:
+                    connection.append(sign + sys.name + "." + signal_name)
 
             # Make sure we found the name
             if len(connection) == 0:
-                raise ValueError("could not find signal %s" % name)
+                raise ValueError("could not find signal %s" % signal_name)
             else:
                 new_inplist.append(connection)
         else:
             new_inplist.append(signal)
     inplist = new_inplist
 
     # Process output list
@@ -2864,36 +2909,56 @@
     for signal in outlist:
         # Create an empty connection and append to inplist
         connection = []
 
         # Check for signal names without a system name
         if isinstance(signal, str) and len(signal.split('.')) == 1:
             # Get the signal name
-            name = signal[1:] if signal[0] == '-' else signal
+            signal_name = signal[1:] if signal[0] == '-' else signal
             sign = '-' if signal[0] == '-' else ""
 
             # Look for the signal name as a system output
             for sys in syslist:
-                if name in sys.output_index.keys():
-                    connection.append(sign + sys.name + "." + name)
+                if signal_name in sys.output_index.keys():
+                    connection.append(sign + sys.name + "." + signal_name)
 
             # Make sure we found the name
             if len(connection) == 0:
-                raise ValueError("could not find signal %s" % name)
+                raise ValueError("could not find signal %s" % signal_name)
             else:
                 new_outlist.append(connection)
         else:
             new_outlist.append(signal)
     outlist = new_outlist
 
     newsys = InterconnectedSystem(
-        syslist, connections=connections, inplist=inplist, outlist=outlist,
-        inputs=inputs, outputs=outputs, states=states,
+        syslist, connections=connections, inplist=inplist,
+        outlist=outlist, inputs=inputs, outputs=outputs, states=states,
         params=params, dt=dt, name=name, warn_duplicate=warn_duplicate)
 
+    # See if we should add any signals
+    if add_unused:
+        # Get all unused signals
+        dropped_inputs, dropped_outputs = newsys.check_unused_signals(
+            ignore_inputs, ignore_outputs, warning=False)
+
+        # Add on any unused signals that we aren't ignoring
+        for isys, isig in dropped_inputs:
+            inplist.append((isys, isig))
+            inputs.append(newsys.syslist[isys].input_labels[isig])
+        for osys, osig in dropped_outputs:
+            outlist.append((osys, osig))
+            outputs.append(newsys.syslist[osys].output_labels[osig])
+
+        # Rebuild the system with new inputs/outputs
+        newsys = InterconnectedSystem(
+            syslist, connections=connections, inplist=inplist,
+            outlist=outlist, inputs=inputs, outputs=outputs, states=states,
+            params=params, dt=dt, name=name, warn_duplicate=warn_duplicate)
+
     # check for implicitly dropped signals
     if check_unused:
         newsys.check_unused_signals(ignore_inputs, ignore_outputs)
 
     # If all subsystems are linear systems, maintain linear structure
     if all([isinstance(sys, LinearIOSystem) for sys in newsys.syslist]):
         return LinearICSystem(newsys, None)
@@ -2938,18 +3003,20 @@
     -------
     sys : static LinearIOSystem
         Linear input/output system object with no states and only a direct
         term that implements the summing junction.
 
     Examples
     --------
-    >>> P = control.tf2io(ct.tf(1, [1, 0]), inputs='u', outputs='y')
-    >>> C = control.tf2io(ct.tf(10, [1, 1]), inputs='e', outputs='u')
-    >>> sumblk = control.summing_junction(inputs=['r', '-y'], output='e')
-    >>> T = control.interconnect((P, C, sumblk), inputs='r', outputs='y')
+    >>> P = ct.tf2io(1, [1, 0], inputs='u', outputs='y')
+    >>> C = ct.tf2io(10, [1, 1], inputs='e', outputs='u')
+    >>> sumblk = ct.summing_junction(inputs=['r', '-y'], output='e')
+    >>> T = ct.interconnect([P, C, sumblk], inputs='r', outputs='y')
+    >>> T.ninputs, T.noutputs, T.nstates
+    (1, 1, 2)
 
     """
     # Utility function to parse input and output signal lists
     def _parse_list(signals, signame='input', prefix='u'):
         # Parse signals, including gains
         if isinstance(signals, int):
             nsignals = signals
```

### Comparing `control-0.9.3.post2/control/lti.py` & `control-0.9.4/control/lti.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """lti.py
 
 The lti module contains the LTI parent class to the child classes StateSpace
 and TransferFunction.  It is designed for use in the python-control library.
-
-Routines in this module:
-
-LTI.__init__
-isdtime()
-isctime()
-timebase()
-common_timebase()
 """
 
 import numpy as np
 
-from numpy import absolute, real, angle, abs
+from numpy import real, angle, abs
 from warnings import warn
 from . import config
-from .namedio import NamedIOSystem, isdtime
+from .namedio import NamedIOSystem
 
 __all__ = ['poles', 'zeros', 'damp', 'evalfr', 'frequency_response',
-           'freqresp', 'dcgain', 'pole', 'zero']
+           'freqresp', 'dcgain', 'bandwidth', 'pole', 'zero']
 
 
 class LTI(NamedIOSystem):
     """LTI is a parent class to linear time-invariant (LTI) system objects.
 
     LTI is the parent to the StateSpace and TransferFunction child classes. It
     contains the number of inputs and outputs, and the timebase (dt) for the
@@ -106,29 +98,29 @@
 
     def damp(self):
         '''Natural frequency, damping ratio of system poles
 
         Returns
         -------
         wn : array
-            Natural frequencies for each system pole
+            Natural frequency for each system pole
         zeta : array
             Damping ratio for each system pole
         poles : array
-            Array of system poles
+            System pole locations
         '''
         poles = self.poles()
 
         if self.isdtime(strict=True):
             splane_poles = np.log(poles.astype(complex))/self.dt
         else:
             splane_poles = poles
-        wn = absolute(splane_poles)
-        Z = -real(splane_poles)/wn
-        return wn, Z, poles
+        wn = abs(splane_poles)
+        zeta = -real(splane_poles)/wn
+        return wn, zeta, poles
 
     def frequency_response(self, omega, squeeze=None):
         """Evaluate the linear time-invariant system at an array of angular
         frequencies.
 
         Reports the frequency response of the system,
 
@@ -198,14 +190,76 @@
         zeroresp = self(0 if self.isctime() else 1,
                         warn_infinite=warn_infinite)
         if np.all(np.logical_or(np.isreal(zeroresp), np.isnan(zeroresp.imag))):
             return zeroresp.real
         else:
             return zeroresp
 
+    def bandwidth(self, dbdrop=-3):
+        """Evaluate the bandwidth of the LTI system for a given dB drop.
+
+        Evaluate the first frequency that the response magnitude is lower than
+        DC gain by dbdrop dB.
+
+        Parameters
+        ----------
+        dpdrop : float, optional
+            A strictly negative scalar in dB (default = -3) defines the
+            amount of gain drop for deciding bandwidth.
+
+        Returns
+        -------
+        bandwidth : ndarray
+            The first frequency (rad/time-unit) where the gain drops below
+            dbdrop of the dc gain of the system, or nan if the system has
+            infinite dc gain, inf if the gain does not drop for all frequency
+
+        Raises
+        ------
+        TypeError
+            if 'sys' is not an SISO LTI instance
+        ValueError
+            if 'dbdrop' is not a negative scalar
+        """
+        # check if system is SISO and dbdrop is a negative scalar
+        if not self.issiso():
+            raise TypeError("system should be a SISO system")
+
+        if (not np.isscalar(dbdrop)) or dbdrop >= 0:
+            raise ValueError("expecting dbdrop be a negative scalar in dB")
+
+        dcgain = self.dcgain()
+        if np.isinf(dcgain):
+            # infinite dcgain, return np.nan
+            return np.nan
+
+        # use frequency range to identify the 0-crossing (dbdrop) bracket
+        from control.freqplot import _default_frequency_range
+        omega = _default_frequency_range(self)
+        mag, phase, omega = self.frequency_response(omega)
+        idx_dropped = np.nonzero(mag - dcgain*10**(dbdrop/20) < 0)[0]
+
+        if idx_dropped.shape[0] == 0:
+            # no frequency response is dbdrop below the dc gain, return np.inf
+            return np.inf
+        else:
+            # solve for the bandwidth, use scipy.optimize.root_scalar() to
+            # solve using bisection
+            import scipy
+            result = scipy.optimize.root_scalar(
+                lambda w: np.abs(self(w*1j)) - np.abs(dcgain)*10**(dbdrop/20),
+                bracket=[omega[idx_dropped[0] - 1], omega[idx_dropped[0]]],
+                method='bisect')
+
+            # check solution
+            if result.converged:
+                return np.abs(result.root)
+            else:
+                raise Exception(result.message)
+
     def ispassive(self):
         # importing here prevents circular dependancy
         from control.passivity import ispassive
         return ispassive(self)
 
     #
     # Deprecated functions
@@ -280,66 +334,71 @@
 def zero(sys):
     warn("zero() will be deprecated; use zeros()", PendingDeprecationWarning)
     return zeros(sys)
 
 
 def damp(sys, doprint=True):
     """
-    Compute natural frequency, damping ratio, and poles of a system
-
-    The function takes 1 or 2 parameters
+    Compute natural frequencies, damping ratios, and poles of a system
 
     Parameters
     ----------
-    sys: LTI (StateSpace or TransferFunction)
+    sys : LTI (StateSpace or TransferFunction)
         A linear system object
-    doprint:
-        if true, print table with values
+    doprint : bool (optional)
+        if True, print table with values
 
     Returns
     -------
-    wn: array
-        Natural frequencies of the poles
-    damping: array
-        Damping values
-    poles: array
-        Pole locations
+    wn : array
+        Natural frequency for each system pole
+    zeta : array
+        Damping ratio for each system pole
+    poles : array
+        System pole locations
 
     See Also
     --------
     pole
 
     Notes
     -----
     If the system is continuous,
         wn = abs(poles)
-        Z  = -real(poles)/poles.
+        zeta  = -real(poles)/poles
 
     If the system is discrete, the discrete poles are mapped to their
     equivalent location in the s-plane via
 
-        s = log10(poles)/dt
+        s = log(poles)/dt
 
     and
 
         wn = abs(s)
-        Z = -real(s)/wn.
+        zeta = -real(s)/wn.
+
+    Examples
+    --------
+    >>> G = ct.tf([1], [1, 4])
+    >>> wn, zeta, poles = ct.damp(G)
+        Eigenvalue (pole)       Damping     Frequency
+                       -4             1             4
 
     """
-    wn, damping, poles = sys.damp()
+    wn, zeta, poles = sys.damp()
     if doprint:
-        print('_____Eigenvalue______ Damping___ Frequency_')
-        for p, d, w in zip(poles, damping, wn):
+        print('    Eigenvalue (pole)       Damping     Frequency')
+        for p, z, w in zip(poles, zeta, wn):
             if abs(p.imag) < 1e-12:
-                print("%10.4g            %10.4g %10.4g" %
-                      (p.real, 1.0, -p.real))
+                print("           %10.4g    %10.4g    %10.4g" %
+                      (p.real, 1.0, w))
             else:
-                print("%10.4g%+10.4gj %10.4g %10.4g" %
-                      (p.real, p.imag, d, w))
-    return wn, damping, poles
+                print("%10.4g%+10.4gj    %10.4g    %10.4g" %
+                      (p.real, p.imag, z, w))
+    return wn, zeta, poles
 
 
 def evalfr(sys, x, squeeze=None):
     """Evaluate the transfer function of an LTI system for complex frequency x.
 
     Returns the complex frequency response `sys(x)` where `x` is `s` for
     continuous-time systems and `z` for discrete-time systems, with
@@ -382,18 +441,16 @@
     Notes
     -----
     This function is a wrapper for :meth:`StateSpace.__call__` and
     :meth:`TransferFunction.__call__`.
 
     Examples
     --------
-    >>> sys = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
-    >>> evalfr(sys, 1j)
-    array([[ 44.8-21.4j]])
-    >>> # This is the transfer function matrix evaluated at s = i.
+    >>> G = ct.ss([[-1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
+    >>> fresp = ct.evalfr(G, 1j)  # evaluate at s = 1j
 
     .. todo:: Add example with MIMO system
 
     """
     return sys.__call__(x, squeeze=squeeze)
 
 
@@ -445,20 +502,16 @@
     Notes
     -----
     This function is a wrapper for :meth:`StateSpace.frequency_response` and
     :meth:`TransferFunction.frequency_response`.
 
     Examples
     --------
-    >>> sys = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
-    >>> mag, phase, omega = freqresp(sys, [0.1, 1., 10.])
-    >>> mag
-    array([[[ 58.8576682 ,  49.64876635,  13.40825927]]])
-    >>> phase
-    array([[[-0.05408304, -0.44563154, -0.66837155]]])
+    >>> G = ct.ss([[-1, -2], [3, -4]], [[5], [7]], [[6, 8]], [[9]])
+    >>> mag, phase, omega = ct.freqresp(G, [0.1, 1., 10.])
 
     .. todo::
         Add example with MIMO system
 
         #>>> sys = rss(3, 2, 2)
         #>>> mag, phase, omega = freqresp(sys, [0.1, 1., 10.])
         #>>> mag[0, 1, :]
@@ -484,18 +537,69 @@
     Returns
     -------
     gain : ndarray
         The zero-frequency gain, or (inf + nanj) if the system has a pole at
         the origin, (nan + nanj) if there is a pole/zero cancellation at the
         origin.
 
+    Examples
+    --------
+    >>> G = ct.tf([1], [1, 2])
+    >>> ct.dcgain(G)                                            # doctest: +SKIP
+    0.5
+
     """
     return sys.dcgain()
 
 
+def bandwidth(sys, dbdrop=-3):
+    """Return the first freqency where the gain drop by dbdrop of the system.
+
+    Parameters
+    ----------
+    sys: StateSpace or TransferFunction
+        Linear system
+    dbdrop : float, optional
+        By how much the gain drop in dB (default = -3) that defines the
+        bandwidth. Should be a negative scalar
+
+    Returns
+    -------
+    bandwidth : ndarray
+        The first frequency (rad/time-unit) where the gain drops below dbdrop
+        of the dc gain of the system, or nan if the system has infinite dc
+        gain, inf if the gain does not drop for all frequency
+
+    Raises
+    ------
+    TypeError
+        if 'sys' is not an SISO LTI instance
+    ValueError
+        if 'dbdrop' is not a negative scalar
+
+    Example
+    -------
+    >>> G = ct.tf([1], [1, 1])
+    >>> ct.bandwidth(G)
+    0.9976
+
+    >>> G1 = ct.tf(0.1, [1, 0.1])
+    >>> wn2 = 1
+    >>> zeta2 = 0.001
+    >>> G2 = ct.tf(wn2**2, [1, 2*zeta2*wn2, wn2**2])
+    >>> ct.bandwidth(G1*G2)
+    0.1018
+
+    """
+    if not isinstance(sys, LTI):
+        raise TypeError("sys must be a LTI instance.")
+
+    return sys.bandwidth(dbdrop)
+
+
 # Process frequency responses in a uniform way
 def _process_frequency_response(sys, omega, out, squeeze=None):
     # Set value of squeeze argument if not set
     if squeeze is None:
         squeeze = config.defaults['control.squeeze_frequency_response']
 
     if np.asarray(omega).ndim < 1:
```

### Comparing `control-0.9.3.post2/control/margins.py` & `control-0.9.4/control/margins.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,17 +472,17 @@
         1d array of (non-negative) frequencies where Nyquist plot
         intersects the real axis
     gain : ndarray
         1d array of corresponding gains
 
     Examples
     --------
-    >>> tf = TransferFunction([1], [1, 2, 3, 4])
-    >>> phase_crossover_frequencies(tf)
-    (array([ 1.73205081,  0.        ]), array([-0.5 ,  0.25]))
+    >>> G = ct.tf([1], [1, 2, 3, 4])
+    >>> x_omega, x_gain = ct.phase_crossover_frequencies(G)
+
     """
     # Convert to a transfer function
     tf = xferfcn._convert_to_transfer_function(sys)
 
     if not issiso(tf):
         raise ControlMIMONotImplemented(
             "Can only calculate crossovers for SISO system")
@@ -533,16 +533,16 @@
 
     If there is more than one gain crossover, the one at the smallest margin
     (deviation from gain = 1), in absolute sense, is returned. Likewise the
     smallest phase margin (in absolute sense) is returned.
 
     Examples
     --------
-    >>> sys = tf(1, [1, 2, 1, 0])
-    >>> gm, pm, wcg, wcp = margin(sys)
+    >>> G = ct.tf(1, [1, 2, 1, 0])
+    >>> gm, pm, wcg, wcp = ct.margin(G)
 
     """
     if len(args) == 1:
         sys = args[0]
         margin = stability_margins(sys)
     elif len(args) == 3:
         margin = stability_margins(args)
```

### Comparing `control-0.9.3.post2/control/mateqn.py` & `control-0.9.4/control/mateqn.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/matlab/__init__.py` & `control-0.9.4/control/matlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
 
 System gain and dynamics
 ----------------------------------------------------------------------------
 
 ==  ==========================  ============================================
 \*  :func:`dcgain`              steady-state (D.C.) gain
-\   lti/bandwidth               system bandwidth
+\*  :func:`bandwidth`           system bandwidth
 \   lti/norm                    h2 and Hinfinity norms of LTI models
 \*  :func:`pole`                system poles
 \*  :func:`zero`                system (transmission) zeros
 \   lti/order                   model order (number of states)
 \*  :func:`~control.pzmap`      pole-zero map (TF only)
 \   lti/iopzmap                 input/output pole-zero map
 \*  :func:`damp`                natural frequency, damping of system poles
```

### Comparing `control-0.9.3.post2/control/matlab/timeresp.py` & `control-0.9.4/control/matlab/timeresp.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 
     See Also
     --------
     lsim, initial, impulse
 
     Examples
     --------
-    >>> yout, T = step(sys, T, X0)
+    >>> from control.matlab import step, rss
+
+    >>> G = rss(4)
+    >>> yout, T = step(G)
+
     '''
     from ..timeresp import step_response
 
     # Switch output argument order and transpose outputs
     out = step_response(sys, T, X0, input, output,
                         transpose=True, return_x=return_x)
     return (out[1], out[0], out[2]) if return_x else (out[1], out[0])
@@ -111,15 +115,19 @@
 
     See Also
     --------
     step, lsim, initial, impulse
 
     Examples
     --------
-    >>> S = stepinfo(sys, T)
+    >>> from control.matlab import stepinfo, rss
+
+    >>> G = rss(4)
+    >>> S = stepinfo(G)
+
     """
     from ..timeresp import step_info
 
     # Call step_info with MATLAB defaults
     S = step_info(sysdata, T=T, T_num=None, yfinal=yfinal,
                   SettlingTimeThreshold=SettlingTimeThreshold,
                   RiseTimeLimits=RiseTimeLimits)
@@ -162,15 +170,19 @@
 
     See Also
     --------
     lsim, step, initial
 
     Examples
     --------
-    >>> yout, T = impulse(sys, T)
+    >>> from control.matlab import rss, impulse
+
+    >>> G = rss()
+    >>> yout, T = impulse(G)
+
     '''
     from ..timeresp import impulse_response
 
     # Switch output argument order and transpose outputs
     out = impulse_response(sys, T, X0, input, output,
                            transpose = True, return_x=return_x)
     return (out[1], out[0], out[2]) if return_x else (out[1], out[0])
@@ -210,15 +222,18 @@
 
     See Also
     --------
     lsim, step, impulse
 
     Examples
     --------
-    >>> yout, T = initial(sys, T, X0)
+    >>> from control.matlab import initial, rss
+
+    >>> G = rss(4)
+    >>> yout, T = initial(G)
 
     '''
     from ..timeresp import initial_response
 
     # Switch output argument order and transpose outputs
     T, yout, xout = initial_response(sys, T, X0, output=output,
                                      transpose=True, return_x=True)
@@ -257,14 +272,19 @@
 
     See Also
     --------
     step, initial, impulse
 
     Examples
     --------
-    >>> yout, T, xout = lsim(sys, U, T, X0)
+    >>> from control.matlab import rss, lsim
+
+    >>> G = rss(4)
+    >>> T = np.linspace(0,10)
+    >>> yout, T, xout = lsim(G, T=T)
+
     '''
     from ..timeresp import forced_response
 
     # Switch output argument order and transpose outputs (and always return x)
     out = forced_response(sys, T, U, X0, return_x=True, transpose=True)
     return out[1], out[0], out[2]
```

### Comparing `control-0.9.3.post2/control/matlab/wrappers.py` & `control-0.9.4/control/matlab/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Wrappers for the MATLAB compatibility module
 """
 
 import numpy as np
 from ..iosys import ss
 from ..xferfcn import tf
-from ..ctrlutil import issys
+from ..lti import LTI
 from ..exception import ControlArgument
 from scipy.signal import zpk2tf
 from warnings import warn
 
 __all__ = ['bode', 'nyquist', 'ngrid', 'dcgain']
 
 def bode(*args, **kwargs):
@@ -22,43 +22,47 @@
     Parameters
     ----------
     sys : LTI, or list of LTI
         System for which the Bode response is plotted and give. Optionally
         a list of systems can be entered, or several systems can be
         specified (i.e. several parameters). The sys arguments may also be
         interspersed with format strings. A frequency argument (array_like)
-        may also be added, some examples:
-        * >>> bode(sys, w)                    # one system, freq vector
-        * >>> bode(sys1, sys2, ..., sysN)     # several systems
-        * >>> bode(sys1, sys2, ..., sysN, w)
-        * >>> bode(sys1, 'plotstyle1', ..., sysN, 'plotstyleN') # + plot formats
+        may also be added, some examples::
+
+        >>> bode(sys, w)                    # one system, freq vector              # doctest: +SKIP
+        >>> bode(sys1, sys2, ..., sysN)     # several systems                      # doctest: +SKIP
+        >>> bode(sys1, sys2, ..., sysN, w)                                         # doctest: +SKIP
+        >>> bode(sys1, 'plotstyle1', ..., sysN, 'plotstyleN') # + plot formats     # doctest: +SKIP
+
     omega: freq_range
         Range of frequencies in rad/s
     dB : boolean
         If True, plot result in dB
     Hz : boolean
         If True, plot frequency in Hz (omega must be provided in rad/sec)
     deg : boolean
         If True, return phase in degrees (else radians)
     plot : boolean
         If True, plot magnitude and phase
 
     Examples
     --------
+    >>> from control.matlab import ss, bode
+
     >>> sys = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
     >>> mag, phase, omega = bode(sys)
 
     .. todo::
 
         Document these use cases
 
-        * >>> bode(sys, w)
-        * >>> bode(sys1, sys2, ..., sysN)
-        * >>> bode(sys1, sys2, ..., sysN, w)
-        * >>> bode(sys1, 'plotstyle1', ..., sysN, 'plotstyleN')
+        * >>> bode(sys, w)                                      # doctest: +SKIP
+        * >>> bode(sys1, sys2, ..., sysN)                       # doctest: +SKIP
+        * >>> bode(sys1, sys2, ..., sysN, w)                    # doctest: +SKIP
+        * >>> bode(sys1, 'plotstyle1', ..., sysN, 'plotstyleN') # doctest: +SKIP
     """
     from ..freqplot import bode_plot
 
     # If first argument is a list, assume python-control calling format
     if hasattr(args[0], '__iter__'):
         return bode_plot(*args, **kwargs)
 
@@ -116,15 +120,15 @@
 
 def _parse_freqplot_args(*args):
     """Parse arguments to frequency plot routines (bode, nyquist)"""
     syslist, plotstyle, omega, other = [], [], None, {}
     i = 0
     while i < len(args):
         # Check to see if this is a system of some sort
-        if issys(args[i]):
+        if isinstance(args[i], LTI):
             # Append the system to our list of systems
             syslist.append(args[i])
             i += 1
 
             # See if the next object is a plotsytle (string)
             if (i < len(args) and isinstance(args[i], str)):
                 plotstyle.append(args[i])
```

### Comparing `control-0.9.3.post2/control/modelsimp.py` & `control-0.9.4/control/modelsimp.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,18 @@
     In practice, we compute the square root of the eigenvalues of the matrix
     formed by taking the product of the observability and controllability
     gramians.  There are other (more efficient) methods based on solving the
     Lyapunov equation in a particular way (more details soon).
 
     Examples
     --------
-    >>> H = hsvd(sys)
+    >>> G = ct.tf2ss([1], [1, 2])
+    >>> H = ct.hsvd(G)
+    >>> H[0]
+    0.25
 
     """
     # TODO: implement for discrete time systems
     if (isdtime(sys, strict=True)):
         raise NotImplementedError("Function not implemented in discrete time")
 
     Wc = gram(sys, 'c')
@@ -131,15 +134,19 @@
             * if `method` is not either ``'matchdc'`` or ``'truncate'``
 
             * if eigenvalues of `sys.A` are not all in left half plane
               (`sys` must be stable)
 
     Examples
     --------
-    >>> rsys = modred(sys, ELIM, method='truncate')
+    >>> G = ct.rss(4)
+    >>> Gr = ct.modred(G, [0, 2], method='matchdc')
+    >>> Gr.nstates
+    2
+
     """
 
     # Check for ss system object, need a utility for this?
 
     # TODO: Check for continous or discrete, only continuous supported for now
     #   if isCont():
     #       dico = 'C'
@@ -251,15 +258,18 @@
         if slycot routine ab09ad, ab09md, or ab09nd is not found
 
     ValueError
         if there are more unstable modes than any value in orders
 
     Examples
     --------
-    >>> rsys = balred(sys, orders, method='truncate')
+    >>> G = ct.rss(4)
+    >>> Gr = ct.balred(G, orders=2, method='matchdc')
+    >>> Gr.nstates
+    2
 
     """
     if method != 'truncate' and method != 'matchdc':
         raise ValueError("supported methods are 'truncate' or 'matchdc'")
     elif method == 'truncate':
         try:
             from slycot import ab09md, ab09ad
@@ -382,15 +392,15 @@
     Returns
     -------
     sys: StateSpace
         A reduced order model sys=ss(Ar,Br,Cr,Dr)
 
     Examples
     --------
-    >>> rsys = era(YY, m, n, nin, nout, r)
+    >>> rsys = era(YY, m, n, nin, nout, r)                      # doctest: +SKIP
 
     """
     raise NotImplementedError('This function is not implemented yet.')
 
 
 def markov(Y, U, m=None, transpose=False):
     """Calculate the first `m` Markov parameters [D CB CAB ...]
@@ -442,18 +452,18 @@
     This function does not currently comply with the Python Control Library
     :ref:`time-series-convention` for representation of time series data.
     Use `transpose=False` to make use of the standard convention (this
     will be updated in a future release).
 
     Examples
     --------
-    >>> T = numpy.linspace(0, 10, 100)
-    >>> U = numpy.ones((1, 100))
-    >>> T, Y, _ = forced_response(tf([1], [1, 0.5], True), T, U)
-    >>> H = markov(Y, U, 3, transpose=False)
+    >>> T = np.linspace(0, 10, 100)
+    >>> U = np.ones((1, 100))
+    >>> T, Y = ct.forced_response(ct.tf([1], [1, 0.5], True), T, U)
+    >>> H = ct.markov(Y, U, 3, transpose=False)
 
     """
     # Convert input parameters to 2D arrays (if they aren't already)
     Umat = np.array(U, ndmin=2)
     Ymat = np.array(Y, ndmin=2)
 
     # If data is in transposed format, switch it around
```

### Comparing `control-0.9.3.post2/control/namedio.py` & `control-0.9.4/control/namedio.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 import numpy as np
 from copy import deepcopy
 from warnings import warn
 from . import config
 
 __all__ = ['issiso', 'timebase', 'common_timebase', 'timebaseEqual',
            'isdtime', 'isctime']
+
 # Define module default parameter values
 _namedio_defaults = {
     'namedio.state_name_delim': '_',
     'namedio.duplicate_system_name_prefix': '',
     'namedio.duplicate_system_name_suffix': '$copy',
     'namedio.linearized_system_name_prefix': '',
     'namedio.linearized_system_name_suffix': '$linearized',
     'namedio.sampled_system_name_prefix': '',
-    'namedio.sampled_system_name_suffix': '$sampled'
+    'namedio.sampled_system_name_suffix': '$sampled',
+    'namedio.converted_system_name_prefix': '',
+    'namedio.converted_system_name_suffix': '$converted',
 }
-    
-    
+
+
 class NamedIOSystem(object):
     def __init__(
             self, name=None, inputs=None, outputs=None, states=None, **kwargs):
 
         # system name
         self.name = self._name_or_default(name)
 
@@ -45,19 +48,23 @@
 
     #
     # Functions to manipulate the system name
     #
     _idCounter = 0              # Counter for creating generic system name
 
     # Return system name
-    def _name_or_default(self, name=None):
+    def _name_or_default(self, name=None, prefix_suffix_name=None):
         if name is None:
             name = "sys[{}]".format(NamedIOSystem._idCounter)
             NamedIOSystem._idCounter += 1
-        return name
+        prefix = "" if prefix_suffix_name is None else config.defaults[
+            'namedio.' + prefix_suffix_name + '_system_name_prefix']
+        suffix = "" if prefix_suffix_name is None else config.defaults[
+            'namedio.' + prefix_suffix_name + '_system_name_suffix']
+        return prefix + name + suffix
 
     # Check if system name is generic
     def _generic_name_check(self):
         import re
         return re.match(r'^sys\[\d*\]$', self.name) is not None
 
     #
@@ -95,24 +102,32 @@
             str += f"States ({self.nstates}): {self.state_labels}"
         return str
 
     # Find a signal by name
     def _find_signal(self, name, sigdict):
         return sigdict.get(name, None)
 
-    def _copy_names(self, sys):
+    def _copy_names(self, sys, prefix="", suffix="", prefix_suffix_name=None):
         """copy the signal and system name of sys. Name is given as a keyword
         in case a specific name (e.g. append 'linearized') is desired. """
-        self.name = sys.name
-        self.ninputs, self.input_index = \
-            sys.ninputs, sys.input_index.copy()
-        self.noutputs, self.output_index = \
-            sys.noutputs, sys.output_index.copy()
-        self.nstates, self.state_index = \
-            sys.nstates, sys.state_index.copy()
+        # Figure out the system name and assign it
+        if prefix == "" and prefix_suffix_name is not None:
+            prefix = config.defaults[
+                'namedio.' + prefix_suffix_name + '_system_name_prefix']
+        if suffix == "" and prefix_suffix_name is not None:
+            suffix = config.defaults[
+                'namedio.' + prefix_suffix_name + '_system_name_suffix']
+        self.name = prefix + sys.name + suffix
+
+        # Name the inputs, outputs, and states
+        self.input_index = sys.input_index.copy()
+        self.output_index = sys.output_index.copy()
+        if self.nstates and sys.nstates:
+            # only copy state names for state space systems
+            self.state_index = sys.state_index.copy()
 
     def copy(self, name=None, use_prefix_suffix=True):
         """Make a copy of an input/output system
 
         A copy of the system is made, with a new name.  The `name` keyword
         can be used to specify a specific name for the system.  If no name
         is given and `use_prefix_suffix` is True, the name is constructed
@@ -124,18 +139,16 @@
         """
         # Create a copy of the system
         newsys = deepcopy(self)
 
         # Update the system name
         if name is None and use_prefix_suffix:
             # Get the default prefix and suffix to use
-            dup_prefix = config.defaults['namedio.duplicate_system_name_prefix']
-            dup_suffix = config.defaults['namedio.duplicate_system_name_suffix']
             newsys.name = self._name_or_default(
-                dup_prefix + self.name + dup_suffix)
+                self.name, prefix_suffix_name='duplicate')
         else:
             newsys.name = self._name_or_default(name)
 
         return newsys
 
     def set_inputs(self, inputs, prefix='u'):
 
@@ -580,7 +593,107 @@
 
     elif all(isinstance(s, str) for s in signals):
         # Use the list of strings as the signal names
         return len(signals), {signals[i]: i for i in range(len(signals))}
 
     else:
         raise TypeError("Can't parse signal list %s" % str(signals))
+
+
+#
+# Utility functions to process signal indices
+#
+# Signal indices can be specified in one of four ways:
+#
+# 1. As a positive integer 'm', in which case we return a list
+#    corresponding to the first 'm' elements of a range of a given length
+#
+# 2. As a negative integer '-m', in which case we return a list
+#    corresponding to the last 'm' elements of a range of a given length
+#
+# 3. As a slice, in which case we return the a list corresponding to the
+#    indices specified by the slice of a range of a given length
+#
+# 4. As a list of ints or strings specifying specific indices.  Strings are
+#    compared to a list of labels to determine the index.
+#
+def _process_indices(arg, name, labels, length):
+    # Default is to return indices up to a certain length
+    arg = length if arg is None else arg
+
+    if isinstance(arg, int):
+        # Return the start or end of the list of possible indices
+        return list(range(arg)) if arg > 0 else list(range(length))[arg:]
+
+    elif isinstance(arg, slice):
+        # Return the indices referenced by the slice
+        return list(range(length))[arg]
+
+    elif isinstance(arg, list):
+        # Make sure the length is OK
+        if len(arg) > length:
+            raise ValueError(
+                f"{name}_indices list is too long; max length = {length}")
+
+        # Return the list, replacing strings with corresponding indices
+        arg=arg.copy()
+        for i, idx in enumerate(arg):
+            if isinstance(idx, str):
+                arg[i] = labels.index(arg[i])
+        return arg
+
+    raise ValueError(f"invalid argument for {name}_indices")
+
+#
+# Process control and disturbance indices
+#
+# For systems with inputs and disturbances, the control_indices and
+# disturbance_indices keywords are used to specify which is which.  If only
+# one is given, the other is assumed to be the remaining indices in the
+# system input.  If neither is given, the disturbance inputs are assumed to
+# be the same as the control inputs.
+#
+def _process_control_disturbance_indices(
+        sys, control_indices, disturbance_indices):
+
+    if control_indices is None and disturbance_indices is None:
+        # Disturbances enter in the same place as the controls
+        dist_idx = ctrl_idx = list(range(sys.ninputs))
+
+    elif control_indices is not None:
+        # Process the control indices
+        ctrl_idx = _process_indices(
+            control_indices, 'control', sys.input_labels, sys.ninputs)
+
+        # Disturbance indices are the complement of control indices
+        dist_idx = [i for i in range(sys.ninputs) if i not in ctrl_idx]
+
+    else:  # disturbance_indices is not None
+        # If passed an integer, count from the end of the input vector
+        arg = -disturbance_indices if isinstance(disturbance_indices, int) \
+            else disturbance_indices
+
+        dist_idx = _process_indices(
+            arg, 'disturbance', sys.input_labels, sys.ninputs)
+
+        # Set control indices to complement disturbance indices
+        ctrl_idx = [i for i in range(sys.ninputs) if i not in dist_idx]
+
+    return ctrl_idx, dist_idx
+
+
+# Process labels
+def _process_labels(labels, name, default):
+    if isinstance(labels, str):
+        labels = [labels.format(i=i) for i in range(len(default))]
+
+    if labels is None:
+        labels = default
+    elif isinstance(labels, list):
+        if len(labels) != len(default):
+            raise ValueError(
+                f"incorrect length of {name}_labels: {len(labels)}"
+                f" instead of {len(default)}")
+    else:
+        raise ValueError(f"{name}_labels should be a string or a list")
+
+    return labels
```

### Comparing `control-0.9.3.post2/control/nichols.py` & `control-0.9.4/control/nichols.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/optimal.py` & `control-0.9.4/control/optimal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # optimal.py - optimization based control module
 #
 # RMM, 11 Feb 2021
 #
 
-"""The :mod:`~control.optimal` module provides support for optimization-based
+"""The :mod:`control.optimal` module provides support for optimization-based
 controllers for nonlinear systems with state and input constraints.
 
+The docstring examples assume that the following import commands::
+
+  >>> import numpy as np
+  >>> import control as ct
+  >>> import control.optimal as obc
+
 """
 
 import numpy as np
 import scipy as sp
 import scipy.optimize as opt
 import control as ct
 import warnings
 import logging
 import time
 
 from . import config
 from .exception import ControlNotImplemented
-from .timeresp import TimeResponseData
+from .namedio import _process_indices, _process_labels, \
+    _process_control_disturbance_indices
+
 
 # Define module default parameter values
 _optimal_trajectory_methods = {'shooting', 'collocation'}
 _optimal_defaults = {
     'optimal.minimize_method': None,
     'optimal.minimize_options': {},
     'optimal.minimize_kwargs': {},
@@ -101,22 +109,22 @@
     minimize_options : str, optional
         Set the options keyword used by :func:`scipy.optimize.minimize`.
     minimize_kwargs : str, optional
         Pass additional keywords to :func:`scipy.optimize.minimize`.
 
     Notes
     -----
-    To describe an optimal control problem we need an input/output system, a
-    time horizon, a cost function, and (optionally) a set of constraints on
-    the state and/or input, either along the trajectory and at the terminal
-    time.  This class sets up an optimization over the inputs at each point in
-    time, using the integral and terminal costs as well as the trajectory and
-    terminal constraints.  The `compute_trajectory` method sets up an
-    optimization problem that can be solved using
-    :func:`scipy.optimize.minimize`.
+    To describe an optimal control problem we need an input/output system,
+    a set of time points over a a fixed horizon, a cost function, and
+    (optionally) a set of constraints on the state and/or input, either
+    along the trajectory and at the terminal time.  This class sets up an
+    optimization over the inputs at each point in time, using the integral
+    and terminal costs as well as the trajectory and terminal constraints.
+    The `compute_trajectory` method sets up an optimization problem that
+    can be solved using :func:`scipy.optimize.minimize`.
 
     The `_cost_function` method takes the information computes the cost of the
     trajectory generated by the proposed input.  It does this by calling a
     user-defined function for the integral_cost given the current states and
     inputs at each point along the trajectory and then adding the value of a
     user-defined terminal cost at the final point in the trajectory.
 
@@ -134,17 +142,18 @@
 
     The default values for ``minimize_method``, ``minimize_options``,
     ``minimize_kwargs``, ``solve_ivp_method``, and ``solve_ivp_options`` can
     be set using config.defaults['optimal.<keyword>'].
 
     """
     def __init__(
-            self, sys, timepts, integral_cost, trajectory_constraints=[],
-            terminal_cost=None, terminal_constraints=[], initial_guess=None,
-            trajectory_method=None, basis=None, log=False, **kwargs):
+            self, sys, timepts, integral_cost, trajectory_constraints=None,
+            terminal_cost=None, terminal_constraints=None, initial_guess=None,
+            trajectory_method=None, basis=None, log=False, kwargs_check=True,
+            **kwargs):
         """Set up an optimal control problem."""
         # Save the basic information for use later
         self.system = sys
         self.timepts = timepts
         self.integral_cost = integral_cost
         self.terminal_cost = terminal_cost
         self.terminal_constraints = terminal_constraints
@@ -179,15 +188,15 @@
             if self.solve_ivp_kwargs['method'] is not None or \
                  len(self.solve_ivp_kwargs) > 1:
                 raise TypeError(
                     "solve_ivp method, kwargs not allowed for"
                     " discrete time systems")
 
         # Make sure there were no extraneous keywords
-        if kwargs:
+        if kwargs_check and kwargs:
             raise TypeError("unrecognized keyword(s): ", str(kwargs))
 
         self.trajectory_constraints = _process_constraints(
             trajectory_constraints, "trajectory")
         self.terminal_constraints = _process_constraints(
             terminal_constraints, "terminal")
 
@@ -825,15 +834,15 @@
             if the optimization failed.
 
         """
         res = self.compute_trajectory(x, squeeze=squeeze)
         return res.inputs[:, 0]
 
     # Create an input/output system implementing an MPC controller
-    def create_mpc_iosystem(self):
+    def create_mpc_iosystem(self, **kwargs):
         """Create an I/O system implementing an MPC controller"""
         # Check to make sure we are in discrete time
         if self.system.dt == 0:
             raise ct.ControlNotImplemented(
                 "MPC for continuous time systems not implemented")
 
         def _update(t, x, u, params={}):
@@ -853,19 +862,25 @@
 
         def _output(t, x, u, params={}):
             # Start with initial guess and recompute based on input state (u)
             self.initial_guess = x
             res = self.compute_trajectory(u, print_summary=False)
             return res.inputs[:, 0]
 
+        # Define signal names, if they are not already given
+        if kwargs.get('inputs') is None:
+            kwargs['inputs'] = self.system.state_labels
+        if kwargs.get('outputs') is None:
+            kwargs['outputs'] = self.system.input_labels
+        if kwargs.get('states') is None:
+            kwargs['states'] = self.system.ninputs * \
+                (self.timepts.size if self.basis is None else self.basis.N)
+
         return ct.NonlinearIOSystem(
-            _update, _output, dt=self.system.dt,
-            inputs=self.system.nstates, outputs=self.system.ninputs,
-            states=self.system.ninputs * \
-                (self.timepts.size if self.basis is None else self.basis.N))
+            _update, _output, dt=self.system.dt, **kwargs)
 
 
 # Optimal control result
 class OptimalControlResult(sp.optimize.OptimizeResult):
     """Result from solving an optimal control problem.
 
     This class is a subclass of :class:`scipy.optimize.OptimizeResult` with
@@ -919,38 +934,38 @@
 
         # Optionally print summary information
         if print_summary:
             ocp._print_statistics()
             print("* Final cost:", self.cost)
 
         # Process data as a time response (with "outputs" = inputs)
-        response = TimeResponseData(
+        response = ct.TimeResponseData(
             ocp.timepts, inputs, states, issiso=ocp.system.issiso(),
             transpose=transpose, return_x=return_states, squeeze=squeeze)
 
         self.time = response.time
         self.inputs = response.outputs
         self.states = response.states
 
 
 # Compute the input for a nonlinear, (constrained) optimal control problem
 def solve_ocp(
-        sys, horizon, X0, cost, trajectory_constraints=None, terminal_cost=None,
-        terminal_constraints=[], initial_guess=None, basis=None, squeeze=None,
+        sys, timepts, X0, cost, trajectory_constraints=None, terminal_cost=None,
+        terminal_constraints=None, initial_guess=None, basis=None, squeeze=None,
         transpose=None, return_states=True, print_summary=True, log=False,
         **kwargs):
 
     """Compute the solution to an optimal control problem
 
     Parameters
     ----------
     sys : InputOutputSystem
         I/O system for which the optimal input will be computed.
 
-    horizon : 1D array_like
+    timepts : 1D array_like
         List of times at which the optimal input should be computed.
 
     X0: array-like or number, optional
         Initial condition (default = 0).
 
     cost : callable
         Function that returns the integral cost given the current state
@@ -980,17 +995,17 @@
 
     terminal_constraints : list of tuples, optional
         List of constraints that should hold at the end of the trajectory.
         Same format as `constraints`.
 
     initial_guess : 1D or 2D array_like
         Initial inputs to use as a guess for the optimal input.  The inputs
-        should either be a 2D vector of shape (ninputs, horizon) or a 1D
-        input of shape (ninputs,) that will be broadcast by extension of the
-        time axis.
+        should either be a 2D vector of shape (ninputs, len(timepts)) or a
+        1D input of shape (ninputs,) that will be broadcast by extension of
+        the time axis.
 
     log : bool, optional
         If `True`, turn on logging messages (using Python logging module).
 
     print_summary : bool, optional
         If `True` (default), print a short summary of the computation.
 
@@ -1025,15 +1040,15 @@
         number and time).
 
     res.states : array
         Time evolution of the state vector (if return_states=True).
 
     Notes
     -----
-    Additional keyword parameters can be used to fine tune the behavior of
+    Additional keyword parameters can be used to fine-tune the behavior of
     the underlying optimization and integration functions.  See
     :func:`OptimalControlProblem` for more information.
 
     """
     # Process keyword arguments
     if trajectory_constraints is None:
         # Backwards compatibility
@@ -1059,41 +1074,41 @@
             warnings.warn(
                 "'method' parameter is deprecated; assuming trajectory_method",
                 DeprecationWarning)
             kwargs['trajectory_method'] = method
 
     # Set up the optimal control problem
     ocp = OptimalControlProblem(
-        sys, horizon, cost, trajectory_constraints=trajectory_constraints,
+        sys, timepts, cost, trajectory_constraints=trajectory_constraints,
         terminal_cost=terminal_cost, terminal_constraints=terminal_constraints,
         initial_guess=initial_guess, basis=basis, log=log, **kwargs)
 
     # Solve for the optimal input from the current state
     return ocp.compute_trajectory(
         X0, squeeze=squeeze, transpose=transpose, print_summary=print_summary,
         return_states=return_states)
 
 
 # Create a model predictive controller for an optimal control problem
 def create_mpc_iosystem(
-        sys, horizon, cost, constraints=[], terminal_cost=None,
-        terminal_constraints=[], log=False, **kwargs):
+        sys, timepts, cost, constraints=None, terminal_cost=None,
+        terminal_constraints=None, log=False, **kwargs):
     """Create a model predictive I/O control system
 
     This function creates an input/output system that implements a model
-    predictive control for a system given the time horizon, cost function and
+    predictive control for a system given the time points, cost function and
     constraints that define the finite-horizon optimization that should be
     carried out at each state.
 
     Parameters
     ----------
     sys : InputOutputSystem
         I/O system for which the optimal input will be computed.
 
-    horizon : 1D array_like
+    timepts : 1D array_like
         List of times at which the optimal input should be computed.
 
     cost : callable
         Function that returns the integral cost given the current state
         and input.  Called as cost(x, u).
 
     constraints : list of tuples, optional
@@ -1114,29 +1129,844 @@
     Returns
     -------
     ctrl : InputOutputSystem
         An I/O system taking the current state of the model system and
         returning the current input to be applied that minimizes the cost
         function while satisfying the constraints.
 
+    Other Parameters
+    ----------------
+    inputs, outputs, states : int or list of str, optional
+        Set the names of the inputs, outputs, and states, as described in
+        :func:`~control.InputOutputSystem`.
+    name : string, optional
+        System name (used for specifying signals). If unspecified, a generic
+        name <sys[id]> is generated with a unique integer id.
+
     Notes
     -----
-    Additional keyword parameters can be used to fine tune the behavior of
+    Additional keyword parameters can be used to fine-tune the behavior of
     the underlying optimization and integrations functions.  See
     :func:`OptimalControlProblem` for more information.
 
     """
     # Set up the optimal control problem
     ocp = OptimalControlProblem(
-        sys, horizon, cost, trajectory_constraints=constraints,
+        sys, timepts, cost, trajectory_constraints=constraints,
         terminal_cost=terminal_cost, terminal_constraints=terminal_constraints,
-        log=log, **kwargs)
+        log=log, kwargs_check=False, **kwargs)
 
     # Return an I/O system implementing the model predictive controller
-    return ocp.create_mpc_iosystem()
+    return ocp.create_mpc_iosystem(**kwargs)
+
+
+#
+# Optimal (moving horizon) estimation problem
+#
+
+class OptimalEstimationProblem():
+    """Description of a finite horizon, optimal estimation problem.
+
+    The `OptimalEstimationProblem` class holds all of the information
+    required to specify an optimal estimation problem: the system dynamics,
+    cost function (negative of the log likelihood), and constraints.
+
+    Parameters
+    ----------
+    sys : InputOutputSystem
+        I/O system for which the optimal input will be computed.
+    timepts: 1D array
+            Set up time points at which the inputs and outputs are given.
+    integral_cost : callable
+        Function that returns the integral cost given the estimated state,
+        system inputs, and output error.  Called as integral_cost(xhat, u,
+        v, w) where xhat is the estimated state, u is the appplied input to
+        the system, v is the estimated disturbance input, and w is the
+        difference between the measured and the estimated output.
+    trajectory_constraints : list of constraints, optional
+       List of constraints that should hold at each point in the time
+       vector.  Each element of the list should be an object of type
+       :class:`~scipy.optimize.LinearConstraint` with arguments `(A, lb,
+       ub)` or :class:`~scipy.optimize.NonlinearConstraint` with arguments
+       `(fun, lb, ub)`.  The constraints will be applied at each time point
+       along the trajectory.
+    terminal_cost : callable, optional
+        Function that returns the terminal cost given the initial estimated
+        state and expected value.  Called as terminal_cost(xhat, x0).
+    control_indices : int, slice, or list of int or string, optional
+        Specify the indices in the system input vector that correspond to
+        the control inputs.  These inputs will be used as known control
+        inputs for the estimator.  If value is an integer `m`, the first
+        `m` system inputs are used.  Otherwise, the value should be a slice
+        or a list of indices.  The list of indices can be specified as
+        either integer offsets or as system input signal names.  If not
+        specified, defaults to the complement of the disturbance indices
+        (see also notes below).
+    disturbance_indices : int, list of int, or slice, optional
+        Specify the indices in the system input vector that correspond to
+        the process disturbances.  If value is an integer `m`, the last `m`
+        system inputs are used.  Otherwise, the value should be a slice or
+        a list of indices, as describedf for `control_indices`.  If not
+        specified, defaults to the complement of the control indicies (see
+        also notes below).
+
+    Returns
+    -------
+    oep : OptimalEstimationProblem
+        Optimal estimation problem object, to be used in computing optimal
+        estimates.
+
+    Other Parameters
+    ----------------
+    terminal_constraints : list of constraints, optional
+        List of constraints that should hold at the terminal point in time,
+        in the same form as `trajectory_constraints`.
+    solve_ivp_method : str, optional
+        Set the method used by :func:`scipy.integrate.solve_ivp`.
+    solve_ivp_kwargs : str, optional
+        Pass additional keywords to :func:`scipy.integrate.solve_ivp`.
+    minimize_method : str, optional
+        Set the method used by :func:`scipy.optimize.minimize`.
+    minimize_options : str, optional
+        Set the options keyword used by :func:`scipy.optimize.minimize`.
+    minimize_kwargs : str, optional
+        Pass additional keywords to :func:`scipy.optimize.minimize`.
+
+    Notes
+    -----
+    To describe an optimal estimation problem we need an input/output system,
+    a set of time points, applied inputs and measured outputs, a cost
+    function, and (optionally) a set of constraints on the state and/or inputs
+    along the trajectory (and at the terminal time).  This class sets up an
+    optimization over the state and disturbances at each point in time, using
+    the integral and terminal costs as well as the trajectory constraints.
+    The :func:`~control.optimal.OptimalEstimationProblem.compute_estimate`
+    method solves the underling optimization problem using
+    :func:`scipy.optimize.minimize`.
+
+    The control input and disturbance indices can be specified using the
+    `control_indices` and `disturbance_indices` keywords.  If only one is
+    given, the other is assumed to be the remaining indices in the system
+    input.  If neither is given, the disturbance inputs are assumed to be
+    the same as the control inputs.
+
+    The "cost" (e.g. negative of the log likelihood) of the estimated
+    trajectory is computed using the estimated state, the disturbances and
+    noise, and the measured output.  This is done by calling a user-defined
+    function for the integral_cost along the trajectory and then adding the
+    value of a user-defined terminal cost at the initial point in the
+    trajectory.
+
+    The constraint functions are evaluated at each point on the trajectory
+    generated by the proposed estimate and disturbances.  As in the case of
+    the cost function, the constraints are evaluated at the estimated
+    state, inputs, and measured outputs along each point on the trajectory.
+    This information is compared against the constraint upper and lower
+    bounds.  The constraint function is processed in the class initializer,
+    so that it only needs to be computed once.
+
+    The default values for ``minimize_method``, ``minimize_options``,
+    ``minimize_kwargs``, ``solve_ivp_method``, and ``solve_ivp_options``
+    can be set using config.defaults['optimal.<keyword>'].
+
+    """
+    def __init__(
+            self, sys, timepts, integral_cost, terminal_cost=None,
+            trajectory_constraints=None, control_indices=None,
+            disturbance_indices=None, **kwargs):
+        """Set up an optimal control problem."""
+        # Save the basic information for use later
+        self.system = sys
+        self.timepts = timepts
+        self.integral_cost = integral_cost
+        self.terminal_cost = terminal_cost
+
+        # Process keyword arguments
+        self.minimize_kwargs = {}
+        self.minimize_kwargs['method'] = kwargs.pop(
+            'minimize_method', config.defaults['optimal.minimize_method'])
+        self.minimize_kwargs['options'] = kwargs.pop(
+            'minimize_options', config.defaults['optimal.minimize_options'])
+        self.minimize_kwargs.update(kwargs.pop(
+            'minimize_kwargs', config.defaults['optimal.minimize_kwargs']))
+
+        # Save input and disturbance indices (and create input array)
+        self.control_indices = control_indices
+        self.disturbance_indices = disturbance_indices
+        self.ctrl_idx, self.dist_idx = None, None
+        self.inputs = np.zeros((sys.ninputs, len(timepts)))
+
+        # Make sure there were no extraneous keywords
+        if kwargs:
+            raise TypeError("unrecognized keyword(s): ", str(kwargs))
+
+        self.trajectory_constraints = _process_constraints(
+            trajectory_constraints, "trajectory")
+
+        #
+        # Compute and store constraints
+        #
+        # While the constraints are evaluated during the execution of the
+        # SciPy optimization method itself, we go ahead and pre-compute the
+        # `scipy.optimize.NonlinearConstraint` function that will be passed to
+        # the optimizer on initialization, since it doesn't change.  This is
+        # mainly a matter of computing the lower and upper bound vectors,
+        # which we need to "stack" to account for the evaluation at each
+        # trajectory time point plus any terminal constraints (in a way that
+        # is consistent with the `_constraint_function` that is used at
+        # evaluation time.
+        #
+        # TODO: when using the collocation method, linear constraints on the
+        # states and inputs can potentially maintain their linear structure
+        # rather than being converted to nonlinear constraints.
+        #
+        constraint_lb, constraint_ub, eqconst_value = [], [], []
+
+        # Go through each time point and stack the bounds
+        for t in self.timepts:
+            for type, fun, lb, ub in self.trajectory_constraints:
+                if np.all(lb == ub):
+                    # Equality constraint
+                    eqconst_value.append(lb)
+                else:
+                    # Inequality constraint
+                    constraint_lb.append(lb)
+                    constraint_ub.append(ub)
+
+        # Turn constraint vectors into 1D arrays
+        self.constraint_lb = np.hstack(constraint_lb) if constraint_lb else []
+        self.constraint_ub = np.hstack(constraint_ub) if constraint_ub else []
+        self.eqconst_value = np.hstack(eqconst_value) if eqconst_value else []
+
+        # Create the constraints (inequality and equality)
+        # TODO: keep track of linear vs nonlinear
+        self.constraints = []
+
+        if len(self.constraint_lb) != 0:
+            self.constraints.append(sp.optimize.NonlinearConstraint(
+                self._constraint_function, self.constraint_lb,
+                self.constraint_ub))
+
+        if len(self.eqconst_value) != 0:
+            self.constraints.append(sp.optimize.NonlinearConstraint(
+                self._eqconst_function, self.eqconst_value,
+                self.eqconst_value))
+
+        # Add the collocation constraints
+        colloc_zeros = np.zeros(sys.nstates * (self.timepts.size - 1))
+        self.colloc_vals = np.zeros((sys.nstates, self.timepts.size - 1))
+        self.constraints.append(sp.optimize.NonlinearConstraint(
+            self._collocation_constraint, colloc_zeros, colloc_zeros))
+
+        # Initialize run-time statistics
+        self._reset_statistics()
+
+    #
+    # Cost function
+    #
+    # We are given the estimated states, applied inputs, and measured
+    # outputs at each time point and we use a zero-order hold approximation
+    # to compute the integral cost plus the terminal (initial) cost:
+    #
+    #   cost = sum_{k=1}^{N-1} integral_cost(xhat[k], u[k], v[k], w[k]) * dt
+    #          + terminal_cost(xhat[0], x0)
+    #
+    def _cost_function(self, xvec):
+        # Compute the estimated states and disturbance inputs
+        xhat, u, v, w = self._compute_states_inputs(xvec)
+
+        # Trajectory cost
+        if ct.isctime(self.system):
+            # Evaluate the costs
+            costs = np.array([self.integral_cost(
+                xhat[:, i], u[:, i], v[:, i], w[:, i]) for
+                     i in range(self.timepts.size)])
+
+            # Compute the time intervals and integrate the cost (trapezoidal)
+            cost = 0.5 * (costs[:-1] + costs[1:]) @ np.diff(self.timepts)
+
+        else:
+            # Sum the integral cost over the time (second) indices
+            # cost += self.integral_cost(xhat[:, i], u[:, i], v[:, i], w[:, i])
+            cost = sum(map(self.integral_cost, xhat.T, u.T, v.T, w.T))
+
+        # Terminal cost
+        if self.terminal_cost is not None and self.x0 is not None:
+            cost += self.terminal_cost(xhat[:, 0], self.x0)
+
+        # Update statistics
+        self.cost_evaluations += 1
+
+        # Return the total cost for this input sequence
+        return cost
+
+    #
+    # Constraints
+    #
+    # We are given the constraints along the trajectory and the terminal
+    # constraints, which each take inputs [xhat, u, v, w] and evaluate the
+    # constraint.  How we handle these depends on the type of constraint:
+    #
+    # * For linear constraints (LinearConstraint), a combined (hstack'd)
+    #   vector of the estimate state and inputs is multiplied by the
+    #   polytope A matrix for comparison against the upper and lower
+    #   bounds.
+    #
+    # * For nonlinear constraints (NonlinearConstraint), a user-specific
+    #   constraint function having the form
+    #
+    #      constraint_fun(xhat, u, v, w)
+    #
+    #   is called at each point along the trajectory and compared against the
+    #   upper and lower bounds.
+    #
+    # * If the upper and lower bound for the constraint are identical, then
+    #   we separate out the evaluation into two different constraints, which
+    #   allows the SciPy optimizers to be more efficient (and stops them
+    #   from generating a warning about mixed constraints).  This is handled
+    #   through the use of the `_eqconst_function` and `eqconst_value`
+    #   members.
+    #
+    # In both cases, the constraint is specified at a single point, but we
+    # extend this to apply to each point in the trajectory.  This means
+    # that for N time points with m trajectory constraints and p terminal
+    # constraints we need to compute N*m + p constraints, each of which
+    # holds at a specific point in time, and implements the original
+    # constraint.
+    #
+    def _constraint_function(self, xvec):
+        # Compute the estimated states and disturbance inputs
+        xhat, u, v, w = self._compute_states_inputs(xvec)
+
+        #
+        # Evaluate the constraint function along the trajectory
+        #
+        # TODO: vectorize
+        value = []
+        for i, t in enumerate(self.timepts):
+            for ctype, fun, lb, ub in self.trajectory_constraints:
+                if np.all(lb == ub):
+                    # Skip equality constraints
+                    continue
+                elif ctype == opt.LinearConstraint:
+                    # `fun` is the A matrix associated with the polytope...
+                    value.append(fun @ np.hstack(
+                        [xhat[:, i], u[:, i], v[:, i], w[:, i]]))
+                elif ctype == opt.NonlinearConstraint:
+                    value.append(fun(xhat[:, i], u[:, i], v[:, i], w[:, i]))
+                else:      # pragma: no cover
+                    # Checked above => we should never get here
+                    raise TypeError(f"unknown constraint type {ctype}")
+
+        # Update statistics
+        self.constraint_evaluations += 1
+
+        # Return the value of the constraint function
+        return np.hstack(value)
+
+    def _eqconst_function(self, xvec):
+        # Compute the estimated states and disturbance inputs
+        xhat, u, v, w = self._compute_states_inputs(xvec)
+
+        # Evaluate the constraint function along the trajectory
+        # TODO: vectorize
+        value = []
+        for i, t in enumerate(self.timepts):
+            for ctype, fun, lb, ub in self.trajectory_constraints:
+                if np.any(lb != ub):
+                    # Skip inequality constraints
+                    continue
+                elif ctype == opt.LinearConstraint:
+                    # `fun` is the A matrix associated with the polytope...
+                    value.append(fun @ np.hstack(
+                        [xhat[:, i], u[:, i], v[:, i], w[:, i]]))
+                elif ctype == opt.NonlinearConstraint:
+                    value.append(fun(xhat[:, i], u[:, i], v[:, i], w[:, i]))
+                else:      # pragma: no cover
+                    # Checked above => we should never get here
+                    raise TypeError(f"unknown constraint type {ctype}")
+
+        # Update statistics
+        self.eqconst_evaluations += 1
+
+        # Return the value of the constraint function
+        return np.hstack(value)
+
+    def _collocation_constraint(self, xvec):
+        # Compute the estimated states and disturbance inputs
+        xhat, u, v, w = self._compute_states_inputs(xvec)
+
+        # Create the input vector for the system
+        self.inputs.fill(0.)
+        self.inputs[self.ctrl_idx, :] = u
+        self.inputs[self.dist_idx, :] += v
+
+        if self.system.isctime():
+            # Compute the collocation constraints
+            # TODO: vectorize
+            fk = self.system._rhs(
+                self.timepts[0], xhat[:, 0], self.inputs[:, 0])
+            for i, t in enumerate(self.timepts[:-1]):
+                # From M. Kelly, SIAM Review (2017), equation (3.2), i = k+1
+                # x[k+1] - x[k] = 0.5 hk (f(x[k+1], u[k+1] + f(x[k], u[k]))
+                fkp1 = self.system._rhs(t, xhat[:, i+1], self.inputs[:, i+1])
+                self.colloc_vals[:, i] = xhat[:, i+1] - xhat[:, i] - \
+                    0.5 * (self.timepts[i+1] - self.timepts[i]) * (fkp1 + fk)
+                fk = fkp1
+        else:
+            # TODO: vectorize
+            for i, t in enumerate(self.timepts[:-1]):
+                # x[k+1] = f(x[k], u[k], v[k])
+                self.colloc_vals[:, i] = xhat[:, i+1] - \
+                    self.system._rhs(t, xhat[:, i], self.inputs[:, i])
+
+        # Return the value of the constraint function
+        return self.colloc_vals.reshape(-1)
+
+    #
+    # Initial guess processing
+    #
+    def _process_initial_guess(self, initial_guess):
+        if initial_guess is None:
+            return np.zeros(
+                (self.system.nstates + self.ndisturbances) * self.timepts.size)
+        else:
+            if initial_guess[0].shape != \
+               (self.system.nstates, self.timepts.size):
+                raise ValueError(
+                    "initial guess for state estimate must have shape "
+                    f"{self.system.nstates} x {self.timepts.size}")
+
+            elif initial_guess[1].shape != \
+                 (self.ndisturbances, self.timepts.size):
+                raise ValueError(
+                    "initial guess for disturbances must have shape "
+                    f"{self.ndisturbances} x {self.timepts.size}")
+
+            return np.hstack([
+                initial_guess[0].reshape(-1),           # estimated states
+                initial_guess[1].reshape(-1)])          # disturbances
+
+    #
+    # Compute the states and inputs from the optimization parameter vector
+    # and the internally stored inputs and measured outputs.
+    #
+    # The optimization parameter vector has elements (xhat[0], ...,
+    # xhat[N-1], v[0], ..., v[N-2]) where N is the number of time
+    # points.  The system inputs u and measured outputs y are locally
+    # stored in self.u and self.y when compute_estimate() is called.
+    #
+    def _compute_states_inputs(self, xvec):
+        # Extract the state estimate and disturbances
+        xhat = xvec[:self.system.nstates * self.timepts.size].reshape(
+            self.system.nstates, -1)
+        v = xvec[self.system.nstates * self.timepts.size:].reshape(
+            self.ndisturbances, -1)
+
+        # Create the input vector for the system
+        self.inputs[self.ctrl_idx, :] = self.u
+        self.inputs[self.dist_idx, :] = v
+
+        # Compute the estimated output
+        yhat = np.vstack([
+            self.system._out(self.timepts[i], xhat[:, i], self.inputs[:, i])
+            for i in range(self.timepts.size)]).T
+
+        return xhat, self.u, v, self.y - yhat
+
+    #
+    # Optimization statistics
+    #
+    # To allow some insight into where time is being spent, we keep track
+    # of the number of times that various functions are called and (TODO)
+    # how long we spent inside each function.
+    #
+    def _reset_statistics(self):
+        """Reset counters for keeping track of statistics"""
+        self.cost_evaluations, self.cost_process_time = 0, 0
+        self.constraint_evaluations, self.constraint_process_time = 0, 0
+        self.eqconst_evaluations, self.eqconst_process_time = 0, 0
+
+    def _print_statistics(self, reset=True):
+        """Print out summary statistics from last run"""
+        print("Summary statistics:")
+        print("* Cost function calls:", self.cost_evaluations)
+        if self.constraint_evaluations:
+            print("* Constraint calls:", self.constraint_evaluations)
+        if self.eqconst_evaluations:
+            print("* Eqconst calls:", self.eqconst_evaluations)
+        if reset:
+            self._reset_statistics()
+
+    #
+    # Optimal estimate computations
+    #
+    def compute_estimate(
+            self, Y, U, X0=None, initial_guess=None,
+            squeeze=None, print_summary=True):
+        """Compute the optimal input at state x
+
+        Parameters
+        ----------
+        Y : 2D array
+            Measured outputs at each time point.
+        U : 2D array
+            Applied inputs at each time point.
+        X0 : 1D array
+            Expected initial value of the state.
+        initial_guess : 2-tuple of 2D arrays
+            A 2-tuple consisting of the estimated states and disturbance
+            values to use as a guess for the optimal estimated trajectory.
+        squeeze : bool, optional
+            If True and if the system has a single disturbance input and
+            single measured output, return the system input and output as a
+            1D array rather than a 2D array.  If False, return the system
+            output as a 2D array even if the system is SISO.  Default value
+            set by config.defaults['control.squeeze_time_response'].
+        print_summary : bool, optional
+            If `True` (default), print a short summary of the computation.
+
+        Returns
+        -------
+        res : OptimalEstimationResult
+            Bundle object with the results of the optimal estimation problem.
+        res.success : bool
+            Boolean flag indicating whether the optimization was successful.
+        res.time : array
+            Time values of the input (same as self.timepts).
+        res.inputs : array
+            Estimated disturbance inputs for the system trajectory.
+        res.states : array
+            Time evolution of the estimated state vector.
+        res.outputs: array
+            Estimated measurement noise for the system trajectory.
+
+        """
+        # Store the inputs and outputs (for use in _constraint_function)
+        self.u = np.atleast_1d(U).reshape(-1, self.timepts.size)
+        self.y = np.atleast_1d(Y).reshape(-1, self.timepts.size)
+        self.x0 = X0
+
+        # Figure out the number of disturbances
+        if self.disturbance_indices is None and self.control_indices is None:
+            self.ctrl_idx, self.dist_idx = \
+                _process_control_disturbance_indices(
+                    self.system, None, self.system.ninputs - self.u.shape[0])
+        elif self.ctrl_idx is None or self.dist_idx is None:
+            self.ctrl_idx, self.dist_idx = \
+                _process_control_disturbance_indices(
+                    self.system, self.control_indices,
+                    self.disturbance_indices)
+        self.ndisturbances = len(self.dist_idx)
+
+        # Make sure the dimensions of the inputs are OK
+        if self.u.shape[0] != len(self.ctrl_idx):
+            raise ValueError(
+                "input vector is incorrect shape; "
+                f"should be {len(self.ctrl_idx)} x {self.timepts.size}")
+        if self.y.shape[0] != self.system.noutputs:
+            raise ValueError(
+                "measurements vector is incorrect shape; "
+                f"should be {self.system.noutputs} x {self.timepts.size}")
+
+        # Process the initial guess
+        initial_guess = self._process_initial_guess(initial_guess)
+
+        # Call ScipPy optimizer
+        res = sp.optimize.minimize(
+            self._cost_function, initial_guess,
+            constraints=self.constraints, **self.minimize_kwargs)
+
+        # Process and return the results
+        return OptimalEstimationResult(
+            self, res, squeeze=squeeze, print_summary=print_summary)
+
+
+    #
+    # Create an input/output system implementing an moving horizon estimator
+    #
+    # This function creates an input/output system that has internal state
+    # xhat, u, v, y for all previous time points.  When the system update
+    # function is called,
+    #
+    def create_mhe_iosystem(
+            self, estimate_labels=None, measurement_labels=None,
+            control_labels=None, inputs=None, outputs=None, **kwargs):
+        """Create an I/O system implementing an MPC controller
+
+        This function creates an input/output system that implements a
+        moving horizon estimator for a an optimal estimation problem.  The
+        I/O system takes the system measurements and applied inputs as as
+        inputs and outputs the estimated state.
+
+        Parameters
+        ----------
+        estimate_labels : str or list of str, optional
+            Set the name of the signals to use for the estimated state
+            (estimator outputs).  If a single string is specified, it
+            should be a format string using the variable ``i`` as an index.
+            Otherwise, a list of strings matching the size of the estimated
+            state should be used.  Default is "xhat[{i}]".  These settings
+            can also be overriden using the `outputs` keyword.
+        measurement_labels, control_labels : str or list of str, optional
+            Set the name of the measurement and control signal names
+            (estimator inputs).  If a single string is specified, it should
+            be a format string using the variable ``i`` as an index.
+            Otherwise, a list of strings matching the size of the system
+            inputs and outputs should be used.  Default is the signal names
+            for the system outputs and control inputs. These settings can
+            also be overriden using the `inputs` keyword.
+        **kwargs, optional
+            Additional keyword arguments to set system, input, and output
+            signal names; see :func:`~control.InputOutputSystem`.
+
+        Returns
+        -------
+        estim : InputOutputSystem
+            An I/O system taking the measured output and applied input for
+            the model system and returning the estimated state of the
+            system, as determined by solving the optimal estimation problem.
+
+        Notes
+        -----
+        The labels for the input signals for the system are determined
+        based on the signal names for the system model used in the optimal
+        estimation problem.  The system name and signal names can be
+        overridden using the `name`, `input`, and `output` keywords, as
+        described in :func:`~control.InputOutputSystem`.
+
+        """
+        # Check to make sure we are in discrete time
+        if self.system.dt == 0:
+            raise ct.ControlNotImplemented(
+                "MHE for continuous time systems not implemented")
+
+        # Figure out the location of the disturbances
+        self.ctrl_idx, self.dist_idx = \
+            _process_control_disturbance_indices(
+                self.system, self.control_indices, self.disturbance_indices)
+
+        # Figure out the signal labels to use
+        estimate_labels = _process_labels(
+            estimate_labels, 'estimate',
+            [f'xhat[{i}]' for i in range(self.system.nstates)])
+        outputs = estimate_labels if outputs is None else outputs
+
+        measurement_labels = _process_labels(
+            measurement_labels, 'measurement', self.system.output_labels)
+        control_labels = _process_labels(
+            control_labels, 'control',
+            [self.system.input_labels[i] for i in self.ctrl_idx])
+        inputs = measurement_labels + control_labels if inputs is None \
+            else inputs
+
+        nstates = (self.system.nstates + self.system.ninputs
+                   + self.system.noutputs) * self.timepts.size
+        if kwargs.get('states'):
+            raise ValueError("user-specified state signal names not allowed")
+
+        # Utility function to extract elements from MHE state vector
+        def _xvec_next(xvec, off, size):
+            len_ = size * self.timepts.size
+            return (off + len_,
+                    xvec[off:off + len_].reshape(-1, self.timepts.size))
+
+        # Update function for the estimator
+        def _mhe_update(t, xvec, uvec, params={}):
+            # Inputs are the measurements and inputs
+            y = uvec[:self.system.noutputs].reshape(-1, 1)
+            u = uvec[self.system.noutputs:].reshape(-1, 1)
+
+            # Estimator state = [xhat, v, Y, U]
+            off, xhat = _xvec_next(xvec, 0, self.system.nstates)
+            off, U = _xvec_next(xvec, off, len(self.ctrl_idx))
+            off, V = _xvec_next(xvec, off, len(self.dist_idx))
+            off, Y = _xvec_next(xvec, off, self.system.noutputs)
+
+            # Shift the states and add the new measurements and inputs
+            # TODO: look for Numpy shift() operator
+            xhat = np.hstack([xhat[:, 1:], xhat[:, -1:]])
+            U = np.hstack([U[:, 1:], u])
+            V = np.hstack([V[:, 1:], V[:, -1:]])
+            Y = np.hstack([Y[:, 1:], y])
+
+            # Compute the new states and disturbances
+            est = self.compute_estimate(
+                Y, U, X0=xhat[:, 0], initial_guess=(xhat, V),
+                print_summary=False)
+
+            # Restack the new state
+            return np.hstack([
+                est.states.reshape(-1), U.reshape(-1),
+                est.inputs.reshape(-1), Y.reshape(-1)])
+
+        # Output function
+        def _mhe_output(t, xvec, uvec, params={}):
+            # Get the states and inputs
+            off, xhat = _xvec_next(xvec, 0, self.system.nstates)
+            off, u_v = _xvec_next(xvec, off, self.system.ninputs)
+
+            # Compute the estimate at the next time point
+            return self.system._rhs(t, xhat[:, -1], u_v[:, -1])
+
+        return ct.NonlinearIOSystem(
+            _mhe_update, _mhe_output, dt=self.system.dt,
+            states=nstates, inputs=inputs, outputs=outputs, **kwargs)
+
+
+# Optimal estimation result
+class OptimalEstimationResult(sp.optimize.OptimizeResult):
+    """Result from solving an optimal estimationproblem.
+
+    This class is a subclass of :class:`scipy.optimize.OptimizeResult` with
+    additional attributes associated with solving optimal estimation
+    problems.
+
+    Attributes
+    ----------
+    states : ndarray
+        Estimated state trajectory.
+    inputs : ndarray
+        The disturbances associated with the estimated state trajectory.
+    outputs :
+        The error between measured outputs and estiamted outputs.
+    success : bool
+        Whether or not the optimizer exited successful.
+    problem : OptimalControlProblem
+        Optimal control problem that generated this solution.
+    cost : float
+        Final cost of the return solution.
+    system_simulations, {cost, constraint, eqconst}_evaluations : int
+        Number of system simulations and evaluations of the cost function,
+        (inequality) constraint function, and equality constraint function
+        performed during the optimzation.
+    {cost, constraint, eqconst}_process_time : float
+        If logging was enabled, the amount of time spent evaluating the cost
+        and constraint functions.
+
+    """
+    def __init__(
+            self, oep, res, return_states=True, print_summary=False,
+            transpose=None, squeeze=None):
+        """Create a OptimalControlResult object"""
+
+        # Copy all of the fields we were sent by sp.optimize.minimize()
+        for key, val in res.items():
+            setattr(self, key, val)
+
+        # Remember the optimal control problem that we solved
+        self.problem = oep
+
+        # Parse the optimization variables into states and inputs
+        xhat, u, v, w = oep._compute_states_inputs(res.x)
+
+        # See if we got an answer
+        if not res.success:
+            warnings.warn(
+                "unable to solve optimal control problem\n"
+                "scipy.optimize.minimize returned " + res.message, UserWarning)
+
+        # Save the final cost
+        self.cost = res.fun
+
+        # Optionally print summary information
+        if print_summary:
+            oep._print_statistics()
+            print("* Final cost:", self.cost)
+
+        # Process data as a time response (with "outputs" = inputs)
+        response = ct.TimeResponseData(
+            oep.timepts, w, xhat, v, issiso=oep.system.issiso(),
+            squeeze=squeeze)
+
+        self.time = response.time
+        self.inputs = response.inputs
+        self.states = response.states
+        self.outputs = response.outputs
+
+
+# Compute the moving horizon estimate for a nonlinear system
+def solve_oep(
+        sys, timepts, Y, U, trajectory_cost, X0=None,
+        trajectory_constraints=None, initial_guess=None,
+        squeeze=None, print_summary=True, **kwargs):
+
+    """Compute the solution to a moving horizon estimation problem
+
+    Parameters
+    ----------
+    sys : InputOutputSystem
+        I/O system for which the optimal input will be computed.
+    timepts : 1D array_like
+        List of times at which the optimal input should be computed.
+    Y, U: 2D array_like
+        Values of the outputs and inputs at each time point.
+    trajectory_cost : callable
+        Function that returns the cost given the current state
+        and input.  Called as `cost(y, u, x0)`.
+    X0: 1D array_like, optional
+        Mean value of the initial condition (defaults to 0).
+    trajectory_constraints : list of tuples, optional
+        List of constraints that should hold at each point in the time vector.
+        See :func:`solve_ocp` for more information.
+    control_indices : int, slice, or list of int or string, optional
+        Specify the indices in the system input vector that correspond to
+        the control inputs.  For more information on possible values, see
+        :func:`~control.optimal.OptimalEstimationProblem`
+    disturbance_indices : int, list of int, or slice, optional
+        Specify the indices in the system input vector that correspond to
+        the input disturbances.  For more information on possible values, see
+        :func:`~control.optimal.OptimalEstimationProblem`
+    initial_guess : 2D array_like, optional
+        Initial guess for the state estimate at each time point.
+    print_summary : bool, optional
+        If `True` (default), print a short summary of the computation.
+    squeeze : bool, optional
+        If True and if the system has a single output, return the system
+        output as a 1D array rather than a 2D array.  If False, return the
+        system output as a 2D array even if the system is SISO.  Default value
+        set by config.defaults['control.squeeze_time_response'].
+
+    Returns
+    -------
+    res : TimeResponseData
+        Bundle object with the estimated state and noise values.
+    res.success : bool
+        Boolean flag indicating whether the optimization was successful.
+    res.time : array
+        Time values of the input.
+    res.inputs : array
+        Disturbance values corresponding to the estimated state.  If the
+        system is SISO and squeeze is not True, the array is 1D (indexed by
+        time).  If the system is not SISO or squeeze is False, the array is
+        2D (indexed by the output number and time).
+    res.states : array
+        Estimated state vector over the given time points.
+    res.outputs : array
+        Noise values corresponding to the estimated state.  If the system
+        is SISO and squeeze is not True, the array is 1D (indexed by time).
+        If the system is not SISO or squeeze is False, the array is 2D
+        (indexed by the output number and time).
+
+    Notes
+    -----
+    Additional keyword parameters can be used to fine-tune the behavior of
+    the underlying optimization and integration functions.  See
+    :func:`~control.optimal.OptimalControlProblem` for more information.
+
+    """
+    # Set up the optimal control problem
+    oep = OptimalEstimationProblem(
+        sys, timepts, trajectory_cost,
+        trajectory_constraints=trajectory_constraints, **kwargs)
+
+    # Solve for the optimal input from the current state
+    return oep.compute_estimate(
+        Y, U, X0=X0, initial_guess=initial_guess,
+        squeeze=squeeze, print_summary=print_summary)
 
 
 #
 # Functions to create cost functions (quadratic cost function)
 #
 # Since a quadratic function is common as a cost function, we provide a
 # function that will take a Q and R matrix and return a callable that
@@ -1192,14 +2022,61 @@
     if R is None:
         return lambda x, u: ((x-x0) @ Q @ (x-x0)).item()
 
     # Received both Q and R matrices
     return lambda x, u: ((x-x0) @ Q @ (x-x0) + (u-u0) @ R @ (u-u0)).item()
 
 
+def gaussian_likelihood_cost(sys, Rv, Rw=None):
+    """Create cost function for Gaussian likelihoods
+
+    Returns a quadratic cost function that can be used for an optimal
+    estimation problem.  The cost function is of the form
+
+      cost = v^T R_v^{-1} v + w^T R_w^{-1} w
+
+    Parameters
+    ----------
+    sys : InputOutputSystem
+        I/O system for which the cost function is being defined.
+    Rv : 2D array_like
+        Covariance matrix for input (or state) disturbances.
+    Rw : 2D array_like
+        Covariance matrix for sensor noise.
+
+    Returns
+    -------
+    cost_fun : callable
+        Function that can be used to evaluate the cost for a given
+        disturbance and sensor noise.  The call signature of the function
+        is cost_fun(v, w).
+
+    """
+    # Process the input arguments
+    if Rv is not None:
+        Rv = np.atleast_2d(Rv)
+
+    if Rw is not None:
+        Rw = np.atleast_2d(Rw)
+        if Rw.size == 1:         # allow scalar weights
+            Rw = np.eye(sys.noutputs) * Rw.item()
+        elif Rw.shape != (sys.noutputs, sys.noutputs):
+            raise ValueError("Rw matrix is the wrong shape")
+
+    if Rv is None:
+        return lambda xhat, u, v, w: (w @ np.linalg.inv(Rw) @ w).item()
+
+    if Rw is None:
+        return lambda xhat, u, v, w: (v @ np.linalg.inv(Rv) @ v).item()
+
+    # Received both Rv and Rw matrices
+    return lambda xhat, u, v, w: \
+        (v @ np.linalg.inv(Rv) @ v + w @ np.linalg.inv(Rw) @ w).item()
+
+
 #
 # Functions to create constraints: either polytopes (A x <= b) or ranges
 # (lb # <= x <= ub).
 #
 # As in the cost function evaluation, the main "trick" in creating a constrain
 # on the state or input is to properly evaluate the constraint on the stacked
 # state and input vector at the current time point.  The constraint itself
@@ -1243,15 +2120,15 @@
     # Return a linear constraint object based on the polynomial
     return (opt.LinearConstraint,
             np.hstack([A, np.zeros((A.shape[0], sys.ninputs))]),
             np.full(A.shape[0], -np.inf), b)
 
 
 def state_range_constraint(sys, lb, ub):
-    """Create state constraint from polytope
+    """Create state constraint from range
 
     Creates a linear constraint on the system state that bounds the range of
     the individual states to be between `lb` and `ub`.  The upper and lower
     bounds can be set of `inf` and `-inf` to indicate there is no constraint
     or to the same value to describe an equality constraint.
 
     Parameters
@@ -1441,14 +2318,54 @@
         # Separate the constraint into states and inputs
         return sys._out(0, x, u)
 
     # Return a nonlinear constraint object based on the polynomial
     return (opt.NonlinearConstraint, _evaluate_output_range_constraint, lb, ub)
 
 #
+# Create a constraint on the disturbance input
+#
+
+def disturbance_range_constraint(sys, lb, ub):
+    """Create constraint for bounded disturbances
+
+    This function computes a constraint that puts a bound on the size of
+    input disturbances.  The output of this function can be passed as a
+    trajectory constraint for optimal estimation problems.
+
+    Parameters
+    ----------
+    sys : InputOutputSystem
+        I/O system for which the constraint is being defined.
+    lb : 1D array
+        Lower bound for each of the disturbancs.
+    ub : 1D array
+        Upper bound for each of the disturbances.
+
+    Returns
+    -------
+    constraint : tuple
+        A tuple consisting of the constraint type and parameter values.
+
+    """
+    # Convert bounds to lists and make sure they are the right dimension
+    lb = np.atleast_1d(lb).reshape(-1)
+    ub = np.atleast_1d(ub).reshape(-1)
+    if lb.shape != ub.shape:
+        raise ValueError("upper and lower bound shapes must match")
+    ndisturbances = lb.size
+
+    # Generate a linear constraint on the input disturbances
+    xvec_len = sys.nstates + sys.ninputs + sys.noutputs
+    A = np.zeros((ndisturbances, xvec_len))
+    A[:, sys.nstates + sys.ninputs - ndisturbances:-sys.noutputs] = \
+        np.eye(ndisturbances)
+    return opt.LinearConstraint(A, lb, ub)
+
+#
 # Utility functions
 #
 
 #
 # Process trajectory constraints
 #
 # Constraints were originally specified as a tuple with the type of
@@ -1456,15 +2373,17 @@
 # directly as SciPy constraint objects.
 #
 # The _process_constraints() function will covert everything to a consistent
 # internal representation (currently a tuple with the constraint type as the
 # first element.
 #
 def _process_constraints(clist, name):
-    if isinstance(
+    if clist is None:
+        clist = []
+    elif isinstance(
             clist, (tuple, opt.LinearConstraint, opt.NonlinearConstraint)):
         clist = [clist]
     elif not isinstance(clist, list):
         raise TypeError(f"{name} constraints must be a list")
 
     # Process individual list elements
     constraint_list = []
```

### Comparing `control-0.9.3.post2/control/passivity.py` & `control-0.9.4/control/passivity.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/phaseplot.py` & `control-0.9.4/control/phaseplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,14 @@
     parms: tuple, optional
         List of parameters to pass to vector field: `func(x, t, *parms)`
 
     See also
     --------
     box_grid : construct box-shaped grid of initial conditions
 
-    Examples
-    --------
-
     """
 
     #
     # Figure out ranges for phase plot (argument processing)
     #
     #! TODO: need to add error checking to arguments
     #! TODO: think through proper action if multiple options are given
```

### Comparing `control-0.9.3.post2/control/pzmap.py` & `control-0.9.4/control/pzmap.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/rlocus.py` & `control-0.9.4/control/rlocus.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             ax.set_ylim(ylim)
 
         # Draw the grid
         if grid:
             if isdtime(sys, strict=True):
                 zgrid(ax=ax)
             else:
-                _sgrid_func(fig=fig if sisotool else None)
+                _sgrid_func(ax)
         else:
             ax.axhline(0., linestyle=':', color='k', linewidth=.75, zorder=-20)
             ax.axvline(0., linestyle=':', color='k', linewidth=.75, zorder=-20)
             if isdtime(sys, strict=True):
                 ax.add_patch(plt.Circle(
                     (0, 0), radius=1.0, linestyle=':', edgecolor='k',
                     linewidth=0.75, fill=False, zorder=-20))
@@ -656,21 +656,15 @@
     """Remove a line from the ax when a label is specified"""
     for line in reversed(ax.lines):
         if line.get_label() == label:
             line.remove()
             del line
 
 
-def _sgrid_func(fig=None, zeta=None, wn=None):
-    if fig is None:
-        fig = plt.gcf()
-        ax = fig.gca()
-    else:
-        ax = fig.axes[1]
-
+def _sgrid_func(ax, zeta=None, wn=None):
     # Get locator function for x-axis, y-axis tick marks
     xlocator = ax.get_xaxis().get_major_locator()
     ylocator = ax.get_yaxis().get_major_locator()
 
     # Decide on the location for the labels (?)
     ylim = ax.get_ylim()
     ytext_pos_lim = ylim[1] - (ylim[1] - ylim[0]) * 0.03
```

### Comparing `control-0.9.3.post2/control/robust.py` & `control-0.9.4/control/robust.py`

 * *Files 24% similar despite different names*

```diff
@@ -66,15 +66,32 @@
 
     See Also
     --------
     StateSpace
 
     Examples
     --------
-    >>> K = h2syn(P,nmeas,ncon)
+    >>> # Unstable first order SISI system
+    >>> G = ct.tf([1], [1, -1], inputs=['u'], outputs=['y'])
+    >>> max(G.poles()) < 0  # Is G stable?
+    False
+
+    >>> # Create partitioned system with trivial unity systems
+    >>> P11 = ct.tf([0], [1], inputs=['w'], outputs=['z'])
+    >>> P12 = ct.tf([1], [1], inputs=['u'], outputs=['z'])
+    >>> P21 = ct.tf([1], [1], inputs=['w'], outputs=['y'])
+    >>> P22 = G
+    >>> P = ct.interconnect([P11, P12, P21, P22],
+    ...                     inplist=['w', 'u'], outlist=['z', 'y'])
+
+    >>> # Synthesize H2 optimal stabilizing controller
+    >>> K = ct.h2syn(P, nmeas=1, ncon=1)
+    >>> T = ct.feedback(G, K, sign=1)
+    >>> max(T.poles()) < 0  # Is T stable?
+    True
 
     """
     # Check for ss system object, need a utility for this?
 
     # TODO: Check for continous or discrete, only continuous supported right now
     # if isCont():
     #    dico = 'C'
@@ -130,15 +147,31 @@
 
     See Also
     --------
     StateSpace
 
     Examples
     --------
-    >>> K, CL, gam, rcond = hinfsyn(P,nmeas,ncon)
+    >>> # Unstable first order SISI system
+    >>> G = ct.tf([1], [1,-1], inputs=['u'], outputs=['y'])
+    >>> max(G.poles()) < 0
+    False
+
+    >>> # Create partitioned system with trivial unity systems
+    >>> P11 = ct.tf([0], [1], inputs=['w'], outputs=['z'])
+    >>> P12 = ct.tf([1], [1], inputs=['u'], outputs=['z'])
+    >>> P21 = ct.tf([1], [1], inputs=['w'], outputs=['y'])
+    >>> P22 = G
+    >>> P = ct.interconnect([P11, P12, P21, P22], inplist=['w', 'u'], outlist=['z', 'y'])
+
+    >>> # Synthesize Hinf optimal stabilizing controller
+    >>> K, CL, gam, rcond = ct.hinfsyn(P, nmeas=1, ncon=1)
+    >>> T = ct.feedback(G, K, sign=1)
+    >>> max(T.poles()) < 0
+    True
 
     """
 
     # Check for ss system object, need a utility for this?
 
     # TODO: Check for continous or discrete, only continuous supported right now
     # if isCont():
@@ -217,36 +250,41 @@
         w = ss([], [], [], [])
     return w
 
 
 def augw(g, w1=None, w2=None, w3=None):
     """Augment plant for mixed sensitivity problem.
 
-    Parameters
-    ----------
-    g: LTI object, ny-by-nu
-    w1: weighting on S; None, scalar, or k1-by-ny LTI object
-    w2: weighting on KS; None, scalar, or k2-by-nu LTI object
-    w3: weighting on T; None, scalar, or k3-by-ny LTI object
-    p: augmented plant; StateSpace object
-
     If a weighting is None, no augmentation is done for it.  At least
     one weighting must not be None.
 
     If a weighting w is scalar, it will be replaced by I*w, where I is
     ny-by-ny for w1 and w3, and nu-by-nu for w2.
 
+    Parameters
+    ----------
+    g: LTI object, ny-by-nu
+        Plant
+    w1: None, scalar, or k1-by-ny LTI object
+        Weighting on S
+    w2: None, scalar, or k2-by-nu LTI object
+        Weighting on KS
+    w3: None, scalar, or k3-by-ny LTI object
+        Weighting on T
+
     Returns
     -------
-    p: plant augmented with weightings, suitable for submission to hinfsyn or h2syn.
+    p: StateSpace
+        Plant augmented with weightings, suitable for submission to hinfsyn or
+        h2syn.
 
     Raises
     ------
     ValueError
-        - if all weightings are None
+        If all weightings are None
 
     See Also
     --------
     h2syn, hinfsyn, mixsyn
     """
 
     from . import append, ss, connect
@@ -327,33 +365,43 @@
 def mixsyn(g, w1=None, w2=None, w3=None):
     """Mixed-sensitivity H-infinity synthesis.
 
     mixsyn(g,w1,w2,w3) -> k,cl,info
 
     Parameters
     ----------
-    g: LTI; the plant for which controller must be synthesized
-    w1: weighting on s = (1+g*k)**-1; None, or scalar or k1-by-ny LTI
-    w2: weighting on k*s; None, or scalar or k2-by-nu LTI
-    w3: weighting on t = g*k*(1+g*k)**-1; None, or scalar or k3-by-ny LTI
-    At least one of w1, w2, and w3 must not be None.
+    g: LTI
+        The plant for which controller must be synthesized
+    w1: None, or scalar or k1-by-ny LTI
+        Weighting on S = (1+G*K)**-1
+    w2: None, or scalar or k2-by-nu LTI
+        Weighting on K*S
+    w3: None, or scalar or k3-by-ny LTI
+        Weighting on T = G*K*(1+G*K)**-1;
 
     Returns
     -------
-    k: synthesized controller; StateSpace object
-    cl: closed system mapping evaluation inputs to evaluation outputs; if 
-    p is the augmented plant, with
-        [z] = [p11 p12] [w], 
-        [y]   [p21   g] [u]
-    then cl is the system from w->z with u=-k*y.  StateSpace object.
-
-    info: tuple with entries, in order,
-        - gamma: scalar; H-infinity norm of cl
-        - rcond: array; estimates of reciprocal condition numbers
-          computed during synthesis.  See hinfsyn for details
+    k: StateSpace
+        Synthesized controller;
+    cl: StateSpace
+        Closed system mapping evaluation inputs to evaluation outputs.
+
+        Let p be the augmented plant, with::
+
+            [z] = [p11 p12] [w]
+            [y]   [p21   g] [u]
+
+        then cl is the system from w->z with `u = -k*y`.
+
+    info: tuple
+        gamma: scalar
+            H-infinity norm of cl
+        rcond: array
+            Estimates of reciprocal condition numbers
+            computed during synthesis.  See hinfsyn for details
 
     If a weighting w is scalar, it will be replaced by I*w, where I is
     ny-by-ny for w1 and w3, and nu-by-nu for w2.
 
     See Also
     --------
     hinfsyn, augw
```

### Comparing `control-0.9.3.post2/control/sisotool.py` & `control-0.9.4/control/sisotool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 __all__ = ['sisotool', 'rootlocus_pid_designer']
 
 from control.exception import ControlMIMONotImplemented
 from .freqplot import bode_plot
 from .timeresp import step_response
-from .namedio import issiso, common_timebase, isctime, isdtime
+from .namedio import common_timebase, isctime, isdtime
 from .xferfcn import tf
 from .iosys import ss
 from .bdalg import append, connect
-from .iosys import tf2io, ss2io, summing_junction, interconnect
-from control.statesp import _convert_to_statespace, StateSpace
+from .iosys import ss, tf2io, summing_junction, interconnect
+from control.statesp import _convert_to_statespace
 from . import config
 import numpy as np
 import matplotlib.pyplot as plt
 import warnings
 
 _sisotool_defaults = {
     'sisotool.initial_gain': 1
 }
 
 def sisotool(sys, initial_gain=None, xlim_rlocus=None, ylim_rlocus=None,
              plotstr_rlocus='C0', rlocus_grid=False, omega=None, dB=None,
              Hz=None, deg=None, omega_limits=None, omega_num=None,
              margins_bode=True, tvect=None, kvect=None):
-    """
-    Sisotool style collection of plots inspired by MATLAB's sisotool.
+    """Sisotool style collection of plots inspired by MATLAB's sisotool.
+
     The left two plots contain the bode magnitude and phase diagrams.
     The top right plot is a clickable root locus plot, clicking on the
     root locus will change the gain of the system. The bottom left plot
     shows a closed loop time response.
 
     Parameters
     ----------
     sys : LTI object
-        Linear input/output systems. If sys is SISO, use the same
-        system for the root locus and step response. If it is desired to
-        see a different step response than feedback(K*sys,1), such as a
-        disturbance response, sys can be provided as a two-input, two-output
-        system (e.g. by using :func:`bdgalg.connect' or
-        :func:`iosys.interconnect`). For two-input, two-output
-        system, sisotool inserts the negative of the selected gain K between
-        the first output and first input and uses the second input and output
-        for computing the step response. To see the disturbance response,
-        configure your plant to have as its second input the disturbance input.
-        To view the step response with a feedforward controller, give your
-        plant two identical inputs, and sum your feedback controller and your
-        feedforward controller and multiply them into your plant's second
-        input. It is also possible to accomodate a system with a gain in the
-        feedback.
+        Linear input/output systems. If sys is SISO, use the same system for
+        the root locus and step response. If it is desired to see a different
+        step response than feedback(K*sys,1), such as a disturbance response,
+        sys can be provided as a two-input, two-output system (e.g. by using
+        :func:`bdgalg.connect' or :func:`iosys.interconnect`). For two-input,
+        two-output system, sisotool inserts the negative of the selected gain
+        K between the first output and first input and uses the second input
+        and output for computing the step response. To see the disturbance
+        response, configure your plant to have as its second input the
+        disturbance input.  To view the step response with a feedforward
+        controller, give your plant two identical inputs, and sum your
+        feedback controller and your feedforward controller and multiply them
+        into your plant's second input. It is also possible to accomodate a
+        system with a gain in the feedback.
     initial_gain : float, optional
         Initial gain to use for plotting root locus. Defaults to 1
         (config.defaults['sisotool.initial_gain']).
     xlim_rlocus : tuple or list, optional
-        control of x-axis range, normally with tuple
+        Control of x-axis range, normally with tuple
         (see :doc:`matplotlib:api/axes_api`).
     ylim_rlocus : tuple or list, optional
         control of y-axis range
     plotstr_rlocus : :func:`matplotlib.pyplot.plot` format string, optional
-        plotting style for the root locus plot(color, linestyle, etc)
+        Plotting style for the root locus plot(color, linestyle, etc).
     rlocus_grid : boolean (default = False)
         If True plot s- or z-plane grid.
     omega : array_like
-        List of frequencies in rad/sec to be used for bode plot
+        List of frequencies in rad/sec to be used for bode plot.
     dB : boolean
-        If True, plot result in dB for the bode plot
+        If True, plot result in dB for the bode plot.
     Hz : boolean
-        If True, plot frequency in Hz for the bode plot (omega must be provided in rad/sec)
+        If True, plot frequency in Hz for the bode plot (omega must be
+        provided in rad/sec).
     deg : boolean
-        If True, plot phase in degrees for the bode plot (else radians)
+        If True, plot phase in degrees for the bode plot (else radians).
     omega_limits : array_like of two values
-        Limits of the to generate frequency vector.
-        If Hz=True the limits are in Hz otherwise in rad/s. Ignored if omega
-        is provided, and auto-generated if omitted.
+        Limits of the to generate frequency vector.  If Hz=True the limits
+        are in Hz otherwise in rad/s. Ignored if omega is provided, and
+        auto-generated if omitted.
     omega_num : int
         Number of samples to plot.  Defaults to
         config.defaults['freqplot.number_of_samples'].
     margins_bode : boolean
-        If True, plot gain and phase margin in the bode plot
+        If True, plot gain and phase margin in the bode plot.
     tvect : list or ndarray, optional
-        List of timesteps to use for closed loop step response
+        List of timesteps to use for closed loop step response.
 
     Examples
     --------
-    >>> sys = tf([1000], [1,25,100,0])
-    >>> sisotool(sys)
+    >>> G = ct.tf([1000], [1, 25, 100, 0])
+    >>> ct.sisotool(G)                                          # doctest: +SKIP
 
     """
     from .rlocus import root_locus
 
     # sys as loop transfer function if SISO
     if not sys.issiso():
         if not (sys.ninputs == 2 and sys.noutputs == 2):
@@ -154,17 +154,19 @@
     ax_mag.set_ylabel(ax_mag.get_ylabel(), fontsize=label_font_size)
     ax_mag.tick_params(axis='both', which='major', labelsize=label_font_size)
 
     ax_phase.set_title('Bode phase',fontsize=title_font_size)
     ax_phase.set_xlabel(ax_phase.get_xlabel(),fontsize=label_font_size)
     ax_phase.set_ylabel(ax_phase.get_ylabel(),fontsize=label_font_size)
     ax_phase.get_xaxis().set_label_coords(0.5, -0.15)
-    ax_phase.get_shared_x_axes().join(ax_phase, ax_mag)
     ax_phase.tick_params(axis='both', which='major', labelsize=label_font_size)
 
+    if not ax_phase.get_shared_x_axes().joined(ax_phase, ax_mag):
+        ax_phase.sharex(ax_mag)
+
     ax_step.set_title('Step response',fontsize = title_font_size)
     ax_step.set_xlabel('Time (seconds)',fontsize=label_font_size)
     ax_step.set_ylabel('Output',fontsize=label_font_size)
     ax_step.get_xaxis().set_label_coords(0.5, -0.15)
     ax_step.get_yaxis().set_label_coords(-0.15, 0.5)
     ax_step.tick_params(axis='both', which='major', labelsize=label_font_size)
 
@@ -196,36 +198,55 @@
     # Manually adjust the spacing and draw the canvas
     fig.subplots_adjust(top=0.9,wspace = 0.3,hspace=0.35)
     fig.canvas.draw()
 
 # contributed by Sawyer Fuller, minster@uw.edu 2021.11.02, based on
 # an implementation in Matlab by Martin Berg.
 def rootlocus_pid_designer(plant, gain='P', sign=+1, input_signal='r',
-                           Kp0=0, Ki0=0, Kd0=0, tau=0.01,
+                           Kp0=0, Ki0=0, Kd0=0, deltaK=0.001, tau=0.01,
                            C_ff=0, derivative_in_feedback_path=False,
                            plot=True):
     """Manual PID controller design based on root locus using Sisotool
 
-    Uses `Sisotool` to investigate the effect of adding or subtracting an
+    Uses `sisotool` to investigate the effect of adding or subtracting an
     amount `deltaK` to the proportional, integral, or derivative (PID) gains of
     a controller. One of the PID gains, `Kp`, `Ki`, or `Kd`, respectively, can
     be modified at a time. `Sisotool` plots the step response, frequency
-    response, and root locus.
-
-    When first run, `deltaK` is set to 0; click on a branch of the root locus
-    plot to try a different value. Each click updates plots and prints
-    the corresponding `deltaK`. To tune all three PID gains, repeatedly call
-    `rootlocus_pid_designer`, and select a different `gain` each time (`'P'`,
-    `'I'`, or `'D'`). Make sure to add the resulting `deltaK` to your chosen
-    initial gain on the next iteration.
+    response, and root locus of the closed-loop system controlling the
+    dynamical system specified by `plant`. Can be used with either non-
+    interactive plots (e.g. in a Jupyter Notebook), or interactive plots.
+
+    To use non-interactively, choose starting-point PID gains `Kp0`, `Ki0`,
+    and `Kd0` (you might want to start with all zeros to begin with), select
+    which gain you would like to vary (e.g. gain=`'P'`, `'I'`, or `'D'`), and
+    choose a value of `deltaK` (default 0.001) to specify by how much you
+    would like to change that gain. Repeatedly run `rootlocus_pid_designer`
+    with different values of `deltaK` until you are satisfied with the
+    performance for that gain. Then, to tune a different gain, e.g. `'I'`,
+    make sure to add your chosen `deltaK` to the previous gain you you were
+    tuning.
 
     Example: to examine the effect of varying `Kp` starting from an intial
-    value of 10, use the arguments `gain='P', Kp0=10`. Suppose a `deltaK`
-    value of 5 gives satisfactory performance. Then on the next iteration,
-    to tune the derivative gain, use the arguments `gain='D', Kp0=15`.
+    value of 10, use the arguments `gain='P', Kp0=10` and try varying values
+    of `deltaK`. Suppose a `deltaK` of 5 gives satisfactory performance. Then,
+    to tune the derivative gain, add your selected `deltaK` to `Kp0` in the
+    next call using the arguments `gain='D', Kp0=15`, to see how adding
+    different values of `deltaK` to your derivative gain affects performance.
+
+    To use with interactive plots, you will need to enable interactive mode
+    if you are in a Jupyter Notebook, e.g. using `%matplotlib`. See
+    `Interactive Plots <https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.ion.html>`_
+    for more information. Click on a branch of the root locus plot to try
+    different values of `deltaK`. Each click updates plots and prints the
+    corresponding `deltaK`. It may be helpful to zoom in using the magnifying
+    glass on the plot to get more locations to click. Just make sure to
+    deactivate magnification mode when you are done by clicking the magnifying
+    glass. Otherwise you will not be able to be able to choose a gain on the
+    root locus plot. When you are done, `%matplotlib inline` returns to inline,
+    non-interactive ploting.
 
     By default, all three PID terms are in the forward path C_f in the diagram
     shown below, that is,
 
     C_f = Kp + Ki/s + Kd*s/(tau*s + 1).
 
     ::
@@ -247,34 +268,31 @@
     `C_b` using `derivative_in_feedback_path=True`. This may be desired to
     avoid that the plant is subject to an impulse function when the reference
     `r` is a step input. `C_b` is otherwise set to zero.
 
     If `plant` is a 2-input system, the disturbance `d` is fed directly into
     its second input rather than being added to `u`.
 
-    Remark: It may be helpful to zoom in using the magnifying glass on the
-    plot. Just ake sure to deactivate magnification mode when you are done by
-    clicking the magnifying glass. Otherwise you will not be able to be able
-    to choose a gain on the root locus plot.
-
     Parameters
     ----------
     plant : :class:`LTI` (:class:`TransferFunction` or :class:`StateSpace` system)
-        The dynamical system to be controlled
+        The dynamical system to be controlled.
     gain : string (optional)
         Which gain to vary by `deltaK`. Must be one of `'P'`, `'I'`, or `'D'`
-        (proportional, integral, or derative)
+        (proportional, integral, or derative).
     sign : int (optional)
-        The sign of deltaK gain perturbation
+        The sign of deltaK gain perturbation.
     input : string (optional)
         The input used for the step response; must be `'r'` (reference) or
-        `'d'` (disturbance) (see figure above)
+        `'d'` (disturbance) (see figure above).
     Kp0, Ki0, Kd0 : float (optional)
         Initial values for proportional, integral, and derivative gains,
-        respectively
+        respectively.
+    deltaK : float (optional)
+        Perturbation value for gain specified by the `gain` keywoard.
     tau : float (optional)
         The time constant associated with the pole in the continuous-time
         derivative term. This is required to make the derivative transfer
         function proper.
     C_ff : float or :class:`LTI` system (optional)
         Feedforward controller. If :class:`LTI`, must have timebase that is
         compatible with plant.
@@ -285,24 +303,28 @@
         Whether to create Sisotool interactive plot.
 
     Returns
     -------
     closedloop : class:`StateSpace` system
         The closed-loop system using initial gains.
 
+    Notes
+    -----
+    When running using iPython or Jupyter, use `%matplotlib` to configure
+    the session for interactive support.
+
     """
 
-    plant = _convert_to_statespace(plant)
     if plant.ninputs == 1:
-        plant = ss2io(plant, inputs='u', outputs='y')
+        plant = ss(plant, inputs='u', outputs='y')
     elif plant.ninputs == 2:
-        plant = ss2io(plant, inputs=['u', 'd'], outputs='y')
+        plant = ss(plant, inputs=['u', 'd'], outputs='y')
     else:
         raise ValueError("plant must have one or two inputs")
-    C_ff = ss2io(_convert_to_statespace(C_ff),   inputs='r', outputs='uff')
+    C_ff = ss(_convert_to_statespace(C_ff),   inputs='r', outputs='uff')
     dt = common_timebase(plant, C_ff)
 
     # create systems used for interconnections
     e_summer = summing_junction(['r', '-y'], 'e')
     if plant.ninputs == 2:
         u_summer = summing_junction(['ufb', 'uff'], 'u')
     else:
@@ -329,27 +351,27 @@
     Kpgain = tf2io(tf(Kp0, 1),            inputs='prop_e',  outputs='ufb')
     Kigain = tf2io(tf(Ki0, 1),            inputs='int_e',   outputs='ufb')
     Kdgain = tf2io(tf(Kd0, 1),            inputs='deriv',  outputs='ufb')
 
     # for the gain that is varied, replace gain block with a special block
     # that has an 'input' and an 'output' that creates loop transfer function
     if gain in ('P', 'p'):
-        Kpgain = ss2io(ss([],[],[],[[0, 1], [-sign, Kp0]]),
+        Kpgain = ss([],[],[],[[0, 1], [-sign, Kp0]],
             inputs=['input', 'prop_e'], outputs=['output', 'ufb'])
     elif gain in ('I', 'i'):
-        Kigain = ss2io(ss([],[],[],[[0, 1], [-sign, Ki0]]),
+        Kigain = ss([],[],[],[[0, 1], [-sign, Ki0]],
             inputs=['input', 'int_e'],  outputs=['output', 'ufb'])
     elif gain in ('D', 'd'):
-        Kdgain = ss2io(ss([],[],[],[[0, 1], [-sign, Kd0]]),
+        Kdgain = ss([],[],[],[[0, 1], [-sign, Kd0]],
             inputs=['input', 'deriv'], outputs=['output', 'ufb'])
     else:
         raise ValueError(gain + ' gain not recognized.')
 
     # the second input and output are used by sisotool to plot step response
     loop = interconnect((plant, Kpgain, Kigain, Kdgain, prop, integ, deriv,
                             C_ff, e_summer, u_summer),
                             inplist=['input', input_signal],
                             outlist=['output', 'y'], check_unused=False)
     if plot:
-        sisotool(loop, kvect=(0.,))
+        sisotool(loop, initial_gain=deltaK)
     cl = loop[1, 1] # closed loop transfer function with initial gains
-    return StateSpace(cl.A, cl.B, cl.C, cl.D, cl.dt)
+    return ss(cl.A, cl.B, cl.C, cl.D, cl.dt)
```

### Comparing `control-0.9.3.post2/control/statefbk.py` & `control-0.9.4/control/statefbk.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,24 +38,26 @@
 # SUCH DAMAGE.
 #
 # $Id$
 
 # External packages and modules
 import numpy as np
 import scipy as sp
+import warnings
 
 from . import statesp
 from .mateqn import care, dare, _check_shape
 from .statesp import StateSpace, _ssmatrix, _convert_to_statespace
 from .lti import LTI
-from .namedio import isdtime, isctime
+from .namedio import isdtime, isctime, _process_indices, _process_labels
 from .iosys import InputOutputSystem, NonlinearIOSystem, LinearIOSystem, \
     interconnect, ss
 from .exception import ControlSlycot, ControlArgument, ControlDimension, \
     ControlNotImplemented
+from .config import _process_legacy_keyword
 
 # Make sure we have access to the right slycot routines
 try:
     from slycot import sb03md57
     # wrap without the deprecation warning
     def sb03md(n, C, A, U, dico, job='X',fact='N',trana='N',ldwork=None):
         ret = sb03md57(A, U, C, dico, job, fact, trana, ldwork)
@@ -117,15 +119,15 @@
        pole assignment by state feedback, IEEE Transactions on Automatic
        Control, Vol. 41, pp. 1432-1452, 1996.
 
     Examples
     --------
     >>> A = [[-1, -1], [0, 1]]
     >>> B = [[0], [1]]
-    >>> K = place(A, B, [-2, -5])
+    >>> K = ct.place(A, B, [-2, -5])
 
     See Also
     --------
     place_varga, acker
 
     """
     from scipy.signal import place_poles
@@ -333,20 +335,21 @@
     sys : LTI StateSpace system
         Linear system
     Q, R : 2D array
         State and input weight matrices
     N : 2D array, optional
         Cross weight matrix
     integral_action : ndarray, optional
-        If this keyword is specified, the controller includes integral action
-        in addition to state feedback.  The value of the `integral_action``
-        keyword should be an ndarray that will be multiplied by the current to
-        generate the error for the internal integrator states of the control
-        law.  The number of outputs that are to be integrated must match the
-        number of additional rows and columns in the ``Q`` matrix.
+        If this keyword is specified, the controller includes integral
+        action in addition to state feedback.  The value of the
+        `integral_action` keyword should be an ndarray that will be
+        multiplied by the current state to generate the error for the
+        internal integrator states of the control law.  The number of
+        outputs that are to be integrated must match the number of
+        additional rows and columns in the `Q` matrix.
     method : str, optional
         Set the method used for computing the result.  Current methods are
         'slycot' and 'scipy'.  If set to None (default), try 'slycot' first
         and then 'scipy'.
 
     Returns
     -------
@@ -369,16 +372,16 @@
        will be called.
 
     2. The return type for 2D arrays depends on the default class set for
        state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> K, S, E = lqr(sys, Q, R, [N])
-    >>> K, S, E = lqr(A, B, Q, R, [N])
+    >>> K, S, E = lqr(sys, Q, R, [N])                           # doctest: +SKIP
+    >>> K, S, E = lqr(A, B, Q, R, [N])                          # doctest: +SKIP
 
     """
     #
     # Process the arguments and figure out what inputs we received
     #
 
     # If we were passed a discrete time system as the first arg, use dlqr()
@@ -482,20 +485,21 @@
     dsys : LTI :class:`StateSpace`
         Discrete-time linear system
     Q, R : 2D array
         State and input weight matrices
     N : 2D array, optional
         Cross weight matrix
     integral_action : ndarray, optional
-        If this keyword is specified, the controller includes integral action
-        in addition to state feedback.  The value of the `integral_action``
-        keyword should be an ndarray that will be multiplied by the current to
-        generate the error for the internal integrator states of the control
-        law.  The number of outputs that are to be integrated must match the
-        number of additional rows and columns in the ``Q`` matrix.
+        If this keyword is specified, the controller includes integral
+        action in addition to state feedback.  The value of the
+        `integral_action` keyword should be an ndarray that will be
+        multiplied by the current state to generate the error for the
+        internal integrator states of the control law.  The number of
+        outputs that are to be integrated must match the number of
+        additional rows and columns in the `Q` matrix.
     method : str, optional
         Set the method used for computing the result.  Current methods are
         'slycot' and 'scipy'.  If set to None (default), try 'slycot' first
         and then 'scipy'.
 
     Returns
     -------
@@ -513,16 +517,16 @@
     Notes
     -----
     The return type for 2D arrays depends on the default class set for
     state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> K, S, E = dlqr(dsys, Q, R, [N])
-    >>> K, S, E = dlqr(A, B, Q, R, [N])
+    >>> K, S, E = dlqr(dsys, Q, R, [N])                         # doctest: +SKIP
+    >>> K, S, E = dlqr(A, B, Q, R, [N])                         # doctest: +SKIP
     """
 
     #
     # Process the arguments and figure out what inputs we received
     #
 
     # Get the system description
@@ -593,32 +597,32 @@
     # Compute the result (dimension and symmetry checking done in dare())
     S, E, K = dare(A, B, Q, R, N, method=method, S_s="N")
     return _ssmatrix(K), _ssmatrix(S), E
 
 
 # Function to create an I/O sytems representing a state feedback controller
 def create_statefbk_iosystem(
-        sys, gain, integral_action=None, estimator=None, type=None,
-        xd_labels='xd[{i}]', ud_labels='ud[{i}]', gainsched_indices=None,
-        gainsched_method='linear', name=None, inputs=None, outputs=None,
-        states=None):
+        sys, gain, integral_action=None, estimator=None, controller_type=None,
+        xd_labels=None, ud_labels=None, gainsched_indices=None,
+        gainsched_method='linear', control_indices=None, state_indices=None,
+        name=None, inputs=None, outputs=None, states=None, **kwargs):
     """Create an I/O system using a (full) state feedback controller
 
     This function creates an input/output system that implements a
     state feedback controller of the form
 
         u = ud - K_p (x - xd) - K_i integral(C x - C x_d)
 
     It can be called in the form
 
         ctrl, clsys = ct.create_statefbk_iosystem(sys, K)
 
-    where ``sys`` is the process dynamics and ``K`` is the state (+ integral)
+    where `sys` is the process dynamics and `K` is the state (+ integral)
     feedback gain (eg, from LQR).  The function returns the controller
-    ``ctrl`` and the closed loop systems ``clsys``, both as I/O systems.
+    `ctrl` and the closed loop systems `clsys`, both as I/O systems.
 
     A gain scheduled controller can also be created, by passing a list of
     gains and a corresponding list of values of a set of scheduling
     variables.  In this case, the controller has the form
 
         u = ud - K_p(mu) (x - xd) - K_i(mu) integral(C x - C x_d)
 
@@ -627,146 +631,183 @@
     Parameters
     ----------
     sys : InputOutputSystem
         The I/O system that represents the process dynamics.  If no estimator
         is given, the output of this system should represent the full state.
 
     gain : ndarray or tuple
-        If a array is give, it represents the state feedback gain (K).
+        If an array is given, it represents the state feedback gain (K).
         This matrix defines the gains to be applied to the system.  If
-        ``integral_action`` is None, then the dimensions of this array
+        `integral_action` is None, then the dimensions of this array
         should be (sys.ninputs, sys.nstates).  If `integral action` is
         set to a matrix or a function, then additional columns
         represent the gains of the integral states of the controller.
 
         If a tuple is given, then it specifies a gain schedule.  The tuple
-        should be of the form ``(gains, points)`` where gains is a list of
+        should be of the form `(gains, points)` where gains is a list of
         gains :math:`K_j` and points is a list of values :math:`\\mu_j` at
         which the gains are computed.  The `gainsched_indices` parameter
         should be used to specify the scheduling variables.
 
     xd_labels, ud_labels : str or list of str, optional
-        Set the name of the signals to use for the desired state and inputs.
-        If a single string is specified, it should be a format string using
-        the variable ``i`` as an index.  Otherwise, a list of strings
-        matching the size of xd and ud, respectively, should be used.
-        Default is ``'xd[{i}]'`` for xd_labels and ``'ud[{i}]'`` for
-        ud_labels.  These settings can also be overriden using the `inputs`
-        keyword.
+        Set the name of the signals to use for the desired state and
+        inputs.  If a single string is specified, it should be a
+        format string using the variable `i` as an index.  Otherwise,
+        a list of strings matching the size of xd and ud,
+        respectively, should be used.  Default is "xd[{i}]" for
+        xd_labels and "ud[{i}]" for ud_labels.  These settings can
+        also be overriden using the `inputs` keyword.
 
-    integral_action : None, ndarray, or func, optional
+    integral_action : ndarray, optional
         If this keyword is specified, the controller can include integral
-        action in addition to state feedback.  If ``integral_action`` is a
-        matrix, it will be multiplied by the current and desired state to
-        generate the error for the internal integrator states of the control
-        law.  If ``integral_action`` is a function ``h``, that function will
-        be called with the signature h(t, x, u, params) to obtain the
-        outputs that should be integrated.  The number of outputs that are
-        to be integrated must match the number of additional columns in the
-        ``K`` matrix.
+        action in addition to state feedback.  The value of the
+        `integral_action` keyword should be an ndarray that will be
+        multiplied by the current and desired state to generate the error
+        for the internal integrator states of the control law.
 
     estimator : InputOutputSystem, optional
         If an estimator is provided, use the states of the estimator as
         the system inputs for the controller.
 
-    gainsched_indices : list of int or str, optional
+    gainsched_indices : int, slice, or list of int or str, optional
         If a gain scheduled controller is specified, specify the indices of
         the controller input to use for scheduling the gain. The input to
         the controller is the desired state xd, the desired input ud, and
         the system state x (or state estimate xhat, if an estimator is
-        given). The indices can either be specified as integer offsets into
-        the input vector or as strings matching the signal names of the
-        input vector. The default is to use the desire state xd.
+        given). If value is an integer `q`, the first `q` values of the
+        [xd, ud, x] vector are used.  Otherwise, the value should be a
+        slice or a list of indices.  The list of indices can be specified
+        as either integer offsets or as signal names.  The default is to
+        use the desired state xd.
 
     gainsched_method : str, optional
         The method to use for gain scheduling.  Possible values are 'linear'
         (default), 'nearest', and 'cubic'.  More information is available in
         :func:`scipy.interpolate.griddata`. For points outside of the convex
         hull of the scheduling points, the gain at the nearest point is
         used.
 
-    type : 'linear' or 'nonlinear', optional
+    controller_type : 'linear' or 'nonlinear', optional
         Set the type of controller to create. The default for a linear gain
         is a linear controller implementing the LQR regulator. If the type
         is 'nonlinear', a :class:NonlinearIOSystem is created instead, with
-        the gain ``K`` as a parameter (allowing modifications of the gain at
+        the gain `K` as a parameter (allowing modifications of the gain at
         runtime). If the gain parameter is a tuple, then a nonlinear,
         gain-scheduled controller is created.
 
     Returns
     -------
     ctrl : InputOutputSystem
-        Input/output system representing the controller.  This system takes
-        as inputs the desired state ``xd``, the desired input ``ud``, and
-        either the system state ``x`` or the estimated state ``xhat``.  It
-        outputs the controller action u according to the formula :math:`u =
-        u_d - K(x - x_d)`.  If the keyword ``integral_action`` is specified,
-        then an additional set of integrators is included in the control
-        system (with the gain matrix ``K`` having the integral gains
-        appended after the state gains).  If a gain scheduled controller is
-        specified, the gain (proportional and integral) are evaluated using
-        the scheduling variables specified by ``gainsched_indices``.
+        Input/output system representing the controller.  This system
+        takes as inputs the desired state `xd`, the desired input
+        `ud`, and either the system state `x` or the estimated state
+        `xhat`.  It outputs the controller action `u` according to the
+        formula :math:`u = u_d - K(x - x_d)`.  If the keyword
+        `integral_action` is specified, then an additional set of
+        integrators is included in the control system (with the gain
+        matrix `K` having the integral gains appended after the state
+        gains).  If a gain scheduled controller is specified, the gain
+        (proportional and integral) are evaluated using the scheduling
+        variables specified by `gainsched_indices`.
 
     clsys : InputOutputSystem
         Input/output system representing the closed loop system.  This
-        systems takes as inputs the desired trajectory ``(xd, ud)`` and
-        outputs the system state ``x`` and the applied input ``u``
+        systems takes as inputs the desired trajectory `(xd, ud)` and
+        outputs the system state `x` and the applied input `u`
         (vertically stacked).
 
     Other Parameters
     ----------------
+    control_indices : int, slice, or list of int or str, optional
+        Specify the indices of the system inputs that should be determined
+        by the state feedback controller.  If value is an integer `m`, the
+        first `m` system inputs are used.  Otherwise, the value should be a
+        slice or a list of indices.  The list of indices can be specified
+        as either integer offsets or as system input signal names.  If not
+        specified, defaults to the system inputs.
+
+    state_indices : int, slice, or list of int or str, optional
+        Specify the indices of the system (or estimator) outputs that should
+        be used by the state feedback controller.  If value is an integer
+        `n`, the first `n` system states are used.  Otherwise, the value
+        should be a slice or a list of indices.  The list of indices can be
+        specified as either integer offsets or as estimator/system output
+        signal names.  If not specified, defaults to the system states.
+
     inputs, outputs : str, or list of str, optional
         List of strings that name the individual signals of the transformed
         system.  If not given, the inputs and outputs are the same as the
         original system.
-    
+
     name : string, optional
         System name. If unspecified, a generic name <sys[id]> is generated
         with a unique integer id.
 
     """
     # Make sure that we were passed an I/O system as an input
     if not isinstance(sys, InputOutputSystem):
         raise ControlArgument("Input system must be I/O system")
 
-    # See whether we were give an estimator
-    if estimator is not None:
-        # Check to make sure the estimator is the right size
-        if estimator.noutputs != sys.nstates:
-            raise ControlArgument("Estimator output size must match state")
-    elif sys.noutputs != sys.nstates:
-        # If no estimator, make sure that the system has all states as outputs
-        # TODO: check to make sure output map is the identity
-        raise ControlArgument("System output must be the full state")
-    else:
-        # Use the system directly instead of an estimator
+    # Process (legacy) keywords
+    controller_type = _process_legacy_keyword(
+        kwargs, 'type', 'controller_type', controller_type)
+    if kwargs:
+        raise TypeError("unrecognized keywords: ", str(kwargs))
+
+    # Figure out what inputs to the system to use
+    control_indices = _process_indices(
+        control_indices, 'control', sys.input_labels, sys.ninputs)
+    sys_ninputs = len(control_indices)
+
+    # Decide what system is going to pass the states to the controller
+    if estimator is None:
         estimator = sys
 
+    # Figure out what outputs (states) from the system/estimator to use
+    state_indices = _process_indices(
+        state_indices, 'state', estimator.state_labels, sys.nstates)
+    sys_nstates = len(state_indices)
+
+    # Make sure the system/estimator states are proper dimension
+    if estimator.noutputs < sys_nstates:
+        # If no estimator, make sure that the system has all states as outputs
+        raise ControlArgument(
+            ("system" if estimator == sys else "estimator") +
+            " output must include the full state")
+    elif estimator == sys:
+        # Issue a warning if we can't verify state output
+        if (isinstance(sys, NonlinearIOSystem) and sys.outfcn is not None) or \
+           (isinstance(sys, StateSpace) and
+            not (np.all(sys.C[np.ix_(state_indices, state_indices)] ==
+                        np.eye(sys_nstates)) and
+                 np.all(sys.D[state_indices, :] == 0))):
+            warnings.warn("cannot verify system output is system state")
+
     # See whether we should implement integral action
     nintegrators = 0
     if integral_action is not None:
         if not isinstance(integral_action, np.ndarray):
             raise ControlArgument("Integral action must pass an array")
-        elif integral_action.shape[1] != sys.nstates:
+        elif integral_action.shape[1] != sys_nstates:
             raise ControlArgument(
                 "Integral gain size must match system state size")
         else:
             nintegrators = integral_action.shape[0]
             C = integral_action
     else:
         # Create a C matrix with no outputs, just in case update gets called
-        C = np.zeros((0, sys.nstates))
+        C = np.zeros((0, sys_nstates))
 
     # Check to make sure that state feedback has the right shape
     if isinstance(gain, np.ndarray):
         K = gain
-        if K.shape != (sys.ninputs, estimator.noutputs + nintegrators):
+        if K.shape != (sys_ninputs, estimator.noutputs + nintegrators):
             raise ControlArgument(
-                f'Control gain must be an array of size {sys.ninputs}'
-                f'x {sys.nstates}' +
+                f'control gain must be an array of size {sys_ninputs}'
+                f' x {sys_nstates}' +
                 (f'+{nintegrators}' if nintegrators > 0 else ''))
         gainsched = False
 
     elif isinstance(gain, tuple):
         # Check for gain scheduled controller
         if len(gain) != 2:
             raise ControlArgument("gain must be a 2-tuple for gain scheduling")
@@ -777,58 +818,60 @@
         points = np.stack(points)
         gainsched=True
 
     else:
         raise ControlArgument("gain must be an array or a tuple")
 
     # Decide on the type of system to create
-    if gainsched and type == 'linear':
+    if gainsched and controller_type == 'linear':
         raise ControlArgument(
-            "type 'linear' not allowed for gain scheduled controller")
-    elif type is None:
-        type = 'nonlinear' if gainsched else 'linear'
-    elif type not in {'linear', 'nonlinear'}:
-        raise ControlArgument(f"unknown type '{type}'")
+            "controller_type 'linear' not allowed for"
+            " gain scheduled controller")
+    elif controller_type is None:
+        controller_type = 'nonlinear' if gainsched else 'linear'
+    elif controller_type not in {'linear', 'nonlinear'}:
+        raise ControlArgument(f"unknown controller_type '{controller_type}'")
 
     # Figure out the labels to use
-    if isinstance(xd_labels, str):
-        # Generate the list of labels using the argument as a format string
-        xd_labels = [xd_labels.format(i=i) for i in range(sys.nstates)]
-
-    if isinstance(ud_labels, str):
-        # Generate the list of labels using the argument as a format string
-        ud_labels = [ud_labels.format(i=i) for i in range(sys.ninputs)]
+    xd_labels = _process_labels(
+        xd_labels, 'xd', ['xd[{i}]'.format(i=i) for i in range(sys_nstates)])
+    ud_labels = _process_labels(
+        ud_labels, 'ud', ['ud[{i}]'.format(i=i) for i in range(sys_ninputs)])
 
     # Create the signal and system names
     if inputs is None:
         inputs = xd_labels + ud_labels + estimator.output_labels
     if outputs is None:
-        outputs = list(sys.input_index.keys())
+        outputs = [sys.input_labels[i] for i in control_indices]
     if states is None:
         states = nintegrators
 
     # Process gainscheduling variables, if present
     if gainsched:
         # Create a copy of the scheduling variable indices (default = xd)
-        gainsched_indices = range(sys.nstates) if gainsched_indices is None \
-            else list(gainsched_indices)
+        gainsched_indices = _process_indices(
+            gainsched_indices, 'gainsched', inputs, sys_nstates)
+
+        # If points is a 1D list, convert to 2D
+        if points.ndim == 1:
+            points = points.reshape(-1, 1)
 
         # Make sure the scheduling variable indices are the right length
         if len(gainsched_indices) != points.shape[1]:
             raise ControlArgument(
                 "length of gainsched_indices must match dimension of"
                 " scheduling variables")
 
-        # Process scheduling variables
-        for i, idx in enumerate(gainsched_indices):
-            if isinstance(idx, str):
-                gainsched_indices[i] = inputs.index(gainsched_indices[i])
-
         # Create interpolating function
-        if gainsched_method == 'nearest':
+        if points.shape[1] < 2:
+            _interp = sp.interpolate.interp1d(
+                points[:, 0], gains, axis=0, kind=gainsched_method)
+            _nearest = sp.interpolate.interp1d(
+                points[:, 0], gains, axis=0, kind='nearest')
+        elif gainsched_method == 'nearest':
             _interp = sp.interpolate.NearestNDInterpolator(points, gains)
             def _nearest(mu):
                 raise SystemError(f"could not find nearest gain at mu = {mu}")
         elif gainsched_method == 'linear':
             _interp = sp.interpolate.LinearNDInterpolator(points, gains)
             _nearest = sp.interpolate.NearestNDInterpolator(points, gains)
         elif gainsched_method == 'cubic':
@@ -841,76 +884,80 @@
         def _compute_gain(mu):
             K = _interp(mu)
             if np.isnan(K).any():
                 K = _nearest(mu)
             return K
 
     # Define the controller system
-    if type == 'nonlinear':
+    if controller_type == 'nonlinear':
         # Create an I/O system for the state feedback gains
         def _control_update(t, states, inputs, params):
             # Split input into desired state, nominal input, and current state
-            xd_vec = inputs[0:sys.nstates]
-            x_vec = inputs[-estimator.nstates:]
+            xd_vec = inputs[0:sys_nstates]
+            x_vec = inputs[-sys_nstates:]
 
             # Compute the integral error in the xy coordinates
             return C @ (x_vec - xd_vec)
 
         def _control_output(t, states, inputs, params):
             if gainsched:
                 mu = inputs[gainsched_indices]
                 K_ = _compute_gain(mu)
             else:
                 K_ = params.get('K')
 
             # Split input into desired state, nominal input, and current state
-            xd_vec = inputs[0:sys.nstates]
-            ud_vec = inputs[sys.nstates:sys.nstates + sys.ninputs]
-            x_vec = inputs[-sys.nstates:]
+            xd_vec = inputs[0:sys_nstates]
+            ud_vec = inputs[sys_nstates:sys_nstates + sys_ninputs]
+            x_vec = inputs[-sys_nstates:]
 
             # Compute the control law
-            u = ud_vec - K_[:, 0:sys.nstates] @ (x_vec - xd_vec)
+            u = ud_vec - K_[:, 0:sys_nstates] @ (x_vec - xd_vec)
             if nintegrators > 0:
-                u -= K_[:, sys.nstates:] @ states
+                u -= K_[:, sys_nstates:] @ states
 
             return u
 
         params = {} if gainsched else {'K': K}
         ctrl = NonlinearIOSystem(
             _control_update, _control_output, name=name, inputs=inputs,
             outputs=outputs, states=states, params=params)
 
-    elif type == 'linear' or type is None:
+    elif controller_type == 'linear' or controller_type is None:
         # Create the matrices implementing the controller
         if isctime(sys):
             # Continuous time: integrator
             A_lqr = np.zeros((C.shape[0], C.shape[0]))
         else:
             # Discrete time: summer
             A_lqr = np.eye(C.shape[0])
-        B_lqr = np.hstack([-C, np.zeros((C.shape[0], sys.ninputs)), C])
-        C_lqr = -K[:, sys.nstates:]
+        B_lqr = np.hstack([-C, np.zeros((C.shape[0], sys_ninputs)), C])
+        C_lqr = -K[:, sys_nstates:]
         D_lqr = np.hstack([
-            K[:, 0:sys.nstates], np.eye(sys.ninputs), -K[:, 0:sys.nstates]
+            K[:, 0:sys_nstates], np.eye(sys_ninputs), -K[:, 0:sys_nstates]
         ])
 
         ctrl = ss(
             A_lqr, B_lqr, C_lqr, D_lqr, dt=sys.dt, name=name,
             inputs=inputs, outputs=outputs, states=states)
 
     else:
-        raise ControlArgument(f"unknown type '{type}'")
+        raise ControlArgument(f"unknown controller_type '{controller_type}'")
 
     # Define the closed loop system
+    inplist=inputs[:-sys.nstates]
+    input_labels=inputs[:-sys.nstates]
+    outlist=sys.output_labels + [sys.input_labels[i] for i in control_indices]
+    output_labels=sys.output_labels + \
+        [sys.input_labels[i] for i in control_indices]
     closed = interconnect(
         [sys, ctrl] if estimator == sys else [sys, ctrl, estimator],
-        name=sys.name + "_" + ctrl.name,
-        inplist=inputs[:-sys.nstates], inputs=inputs[:-sys.nstates],
-        outlist=sys.output_labels + sys.input_labels,
-        outputs=sys.output_labels + sys.input_labels
+        name=sys.name + "_" + ctrl.name, add_unused=True,
+        inplist=inplist, inputs=input_labels,
+        outlist=outlist, outputs=output_labels
     )
     return ctrl, closed
 
 
 def ctrb(A, B):
     """Controllabilty matrix
 
@@ -927,15 +974,18 @@
     Notes
     -----
     The return type for 2D arrays depends on the default class set for
     state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> C = ctrb(A, B)
+    >>> G = ct.tf2ss([1], [1, 2, 3])
+    >>> C = ct.ctrb(G.A, G.B)
+    >>> np.linalg.matrix_rank(C)
+    2
 
     """
 
     # Convert input parameters to matrices (if they aren't already)
     amat = _ssmatrix(A)
     bmat = _ssmatrix(B)
     n = np.shape(amat)[0]
@@ -963,15 +1013,19 @@
     Notes
     -----
     The return type for 2D arrays depends on the default class set for
     state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> O = obsv(A, C)
+    >>> G = ct.tf2ss([1], [1, 2, 3])
+    >>> C = ct.obsv(G.A, G.C)
+    >>> np.linalg.matrix_rank(C)
+    2
+
     """
 
     # Convert input parameters to matrices (if they aren't already)
     amat = _ssmatrix(A)
     cmat = _ssmatrix(C)
     n = np.shape(amat)[0]
 
@@ -1012,18 +1066,19 @@
     Notes
     -----
     The return type for 2D arrays depends on the default class set for
     state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> Wc = gram(sys, 'c')
-    >>> Wo = gram(sys, 'o')
-    >>> Rc = gram(sys, 'cf'), where Wc = Rc' * Rc
-    >>> Ro = gram(sys, 'of'), where Wo = Ro' * Ro
+    >>> G = ct.rss(4)
+    >>> Wc = ct.gram(G, 'c')
+    >>> Wo = ct.gram(G, 'o')
+    >>> Rc = ct.gram(G, 'cf')  # where Wc = Rc' * Rc
+    >>> Ro = ct.gram(G, 'of')  # where Wo = Ro' * Ro
 
     """
 
     # Check for ss system object
     if not isinstance(sys, statesp.StateSpace):
         raise ValueError("System must be StateSpace!")
     if type not in ['c', 'o', 'cf', 'of']:
```

### Comparing `control-0.9.3.post2/control/statesp.py` & `control-0.9.4/control/statesp.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,17 @@
 class StateSpace(LTI):
     r"""StateSpace(A, B, C, D[, dt])
 
     A class for representing state-space models.
 
     The StateSpace class is used to represent state-space realizations of
     linear time-invariant (LTI) systems:
-    
+
     .. math::
-    
+
           dx/dt &= A x + B u \\
               y &= C x + D u
 
     where `u` is the input, `y` is the output, and `x` is the state.
 
     Parameters
     ----------
@@ -1213,16 +1213,16 @@
             return StateSpace(self)
 
     def returnScipySignalLTI(self, strict=True):
         """Return a list of a list of :class:`scipy.signal.lti` objects.
 
         For instance,
 
-        >>> out = ssobject.returnScipySignalLTI()
-        >>> out[3][5]
+        >>> out = ssobject.returnScipySignalLTI()               # doctest: +SKIP
+        >>> out[3][5]                                           # doctest: +SKIP
 
         is a :class:`scipy.signal.lti` object corresponding to the transfer
         function from the 6th input to the 4th output.
 
         Parameters
         ----------
         strict : bool, optional
@@ -1358,38 +1358,36 @@
 
         Notes
         -----
         Uses :func:`scipy.signal.cont2discrete`
 
         Examples
         --------
-        >>> sys = StateSpace(0, 1, 1, 0)
-        >>> sysd = sys.sample(0.5, method='bilinear')
+        >>> G = ct.ss(0, 1, 1, 0)
+        >>> sysd = G.sample(0.5, method='bilinear')
 
         """
         if not self.isctime():
             raise ValueError("System must be continuous time system")
-
-        if (method == 'bilinear' or (method == 'gbt' and alpha == 0.5)) and \
-                prewarp_frequency is not None:
-            Twarp = 2 * np.tan(prewarp_frequency * Ts/2)/prewarp_frequency
+        if prewarp_frequency is not None:
+            if method in ('bilinear', 'tustin') or \
+                    (method == 'gbt' and alpha == 0.5):
+                Twarp = 2*np.tan(prewarp_frequency*Ts/2)/prewarp_frequency
+            else:
+                warn('prewarp_frequency ignored: incompatible conversion')
+                Twarp = Ts
         else:
             Twarp = Ts
         sys = (self.A, self.B, self.C, self.D)
         Ad, Bd, C, D, _ = cont2discrete(sys, Twarp, method, alpha)
         sysd = StateSpace(Ad, Bd, C, D, Ts)
         # copy over the system name, inputs, outputs, and states
         if copy_names:
-            sysd._copy_names(self)
-            if name is None:
-                sysd.name = \
-                    config.defaults['namedio.sampled_system_name_prefix'] +\
-                    sysd.name + \
-                    config.defaults['namedio.sampled_system_name_suffix']
-            else:
+            sysd._copy_names(self, prefix_suffix_name='sampled')
+            if name is not None:
                 sysd.name = name
         # pass desired signal names if names were provided
         return StateSpace(sysd, **kwargs)
 
     def dcgain(self, warn_infinite=False):
         """Return the zero-frequency gain
 
@@ -1517,27 +1515,20 @@
             if np.size(u) != self.ninputs:
                 raise ValueError("len(u) must be equal to number of inputs")
             return (self.C @ x).reshape((-1,)) \
                 + (self.D @ u).reshape((-1,))  # return as row vector
 
 
 # TODO: add discrete time check
-def _convert_to_statespace(sys):
+def _convert_to_statespace(sys, use_prefix_suffix=False):
     """Convert a system to state space form (if needed).
 
     If sys is already a state space, then it is returned.  If sys is a
     transfer function object, then it is converted to a state space and
-    returned.  If sys is a scalar, then the number of inputs and outputs can
-    be specified manually, as in:
-
-    >>> sys = _convert_to_statespace(3.) # Assumes inputs = outputs = 1
-    >>> sys = _convert_to_statespace(1., inputs=3, outputs=2)
-
-    In the latter example, A = B = C = 0 and D = [[1., 1., 1.]
-                                                  [1., 1., 1.]].
+    returned.
 
     Note: no renaming of inputs and outputs is performed; this should be done
     by the calling function.
 
     """
     from .xferfcn import TransferFunction
     import itertools
@@ -1561,56 +1552,59 @@
             num, den, denorder = sys.minreal()._common_den()
 
             # transfer function to state space conversion now should work!
             ssout = td04ad('C', sys.ninputs, sys.noutputs,
                            denorder, den, num, tol=0)
 
             states = ssout[0]
-            return StateSpace(
+            newsys = StateSpace(
                 ssout[1][:states, :states], ssout[2][:states, :sys.ninputs],
-                ssout[3][:sys.noutputs, :states], ssout[4], sys.dt,
-                inputs=sys.input_labels, outputs=sys.output_labels)
+                ssout[3][:sys.noutputs, :states], ssout[4], sys.dt)
+
         except ImportError:
             # No Slycot.  Scipy tf->ss can't handle MIMO, but static
             # MIMO is an easy special case we can check for here
             maxn = max(max(len(n) for n in nrow)
                        for nrow in sys.num)
             maxd = max(max(len(d) for d in drow)
                        for drow in sys.den)
             if 1 == maxn and 1 == maxd:
                 D = empty((sys.noutputs, sys.ninputs), dtype=float)
                 for i, j in itertools.product(range(sys.noutputs),
                                               range(sys.ninputs)):
                     D[i, j] = sys.num[i][j][0] / sys.den[i][j][0]
-                return StateSpace([], [], [], D, sys.dt)
+                newsys = StateSpace([], [], [], D, sys.dt)
             else:
                 if sys.ninputs != 1 or sys.noutputs != 1:
                     raise TypeError("No support for MIMO without slycot")
 
                 # TODO: do we want to squeeze first and check dimenations?
                 # I think this will fail if num and den aren't 1-D after
                 # the squeeze
                 A, B, C, D = \
                     sp.signal.tf2ss(squeeze(sys.num), squeeze(sys.den))
-                return StateSpace(
-                    A, B, C, D, sys.dt, inputs=sys.input_labels,
-                    outputs=sys.output_labels)
+                newsys = StateSpace(A, B, C, D, sys.dt)
+
+        # Copy over the signal (and system) names
+        newsys._copy_names(
+            sys,
+            prefix_suffix_name='converted' if use_prefix_suffix else None)
+        return newsys
 
     elif isinstance(sys, FrequencyResponseData):
         raise TypeError("Can't convert FRD to StateSpace system.")
 
     # If this is a matrix, try to create a constant feedthrough
     try:
         D = _ssmatrix(np.atleast_2d(sys))
         return StateSpace([], [], [], D, dt=None)
 
     except Exception:
         raise TypeError("Can't convert given type to StateSpace system.")
 
-
 # TODO: add discrete time option
 def _rss_generate(
         states, inputs, outputs, cdtype, strictly_proper=False, name=None):
     """Generate a random state space.
 
     This does the actual random state space generation expected from rss and
     drss.  cdtype is 'c' for continuous systems and 'd' for discrete systems.
@@ -1780,15 +1774,17 @@
                  "Only input {i} and output {o} are used."
                  .format(i=input, o=output))
         # $X = A*X + B*U
         #  Y = C*X + D*U
         new_B = sys.B[:, input]
         new_C = sys.C[output, :]
         new_D = sys.D[output, input]
-        sys = StateSpace(sys.A, new_B, new_C, new_D, sys.dt)
+        sys = StateSpace(sys.A, new_B, new_C, new_D, sys.dt,
+                         name=sys.name,
+                         inputs=sys.input_labels[input], outputs=sys.output_labels[output])
 
     return sys
 
 
 def _mimo2simo(sys, input, warn_conversion=False):
     # pylint: disable=W0622
     """
@@ -1829,15 +1825,17 @@
         if warn_conversion:
             warn("Converting MIMO system to SIMO system. "
                  "Only input {i} is used." .format(i=input))
         # $X = A*X + B*U
         #  Y = C*X + D*U
         new_B = sys.B[:, input:input+1]
         new_D = sys.D[:, input:input+1]
-        sys = StateSpace(sys.A, new_B, sys.C, new_D, sys.dt)
+        sys = StateSpace(sys.A, new_B, sys.C, new_D, sys.dt,
+                         name=sys.name,
+                         inputs=sys.input_labels[input], outputs=sys.output_labels)
 
     return sys
 
 
 def tf2ss(*args, **kwargs):
     """tf2ss(sys)
 
@@ -1894,33 +1892,37 @@
     tf
     ss2tf
 
     Examples
     --------
     >>> num = [[[1., 2.], [3., 4.]], [[5., 6.], [7., 8.]]]
     >>> den = [[[9., 8., 7.], [6., 5., 4.]], [[3., 2., 1.], [-1., -2., -3.]]]
-    >>> sys1 = tf2ss(num, den)
+    >>> sys1 = ct.tf2ss(num, den)
 
-    >>> sys_tf = tf(num, den)
-    >>> sys2 = tf2ss(sys_tf)
+    >>> sys_tf = ct.tf(num, den)
+    >>> sys2 = ct.tf2ss(sys_tf)
 
     """
 
     from .xferfcn import TransferFunction
     if len(args) == 2 or len(args) == 3:
         # Assume we were given the num, den
         return StateSpace(
             _convert_to_statespace(TransferFunction(*args)), **kwargs)
 
     elif len(args) == 1:
         sys = args[0]
         if not isinstance(sys, TransferFunction):
             raise TypeError("tf2ss(sys): sys must be a TransferFunction "
                             "object.")
-        return StateSpace(_convert_to_statespace(sys), **kwargs)
+        return StateSpace(
+            _convert_to_statespace(
+                sys,
+                use_prefix_suffix=not sys._generic_name_check()),
+            **kwargs)
     else:
         raise ValueError("Needs 1 or 2 arguments; received %i." % len(args))
 
 
 def ssdata(sys):
     """
     Return state space data objects for a system
```

### Comparing `control-0.9.3.post2/control/stochsys.py` & `control-0.9.4/control/stochsys.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,17 +19,20 @@
 import numpy as np
 import scipy as sp
 from math import sqrt
 
 from .iosys import InputOutputSystem, LinearIOSystem, NonlinearIOSystem
 from .lti import LTI
 from .namedio import isctime, isdtime
+from .namedio import _process_indices, _process_labels, \
+    _process_control_disturbance_indices
 from .mateqn import care, dare, _check_shape
 from .statesp import StateSpace, _ssmatrix
 from .exception import ControlArgument, ControlNotImplemented
+from .config import _process_legacy_keyword
 
 __all__ = ['lqe', 'dlqe', 'create_estimator_iosystem', 'white_noise',
            'correlation']
 
 
 # contributed by Sawyer B. Fuller <minster@uw.edu>
 def lqe(*args, **kwargs):
@@ -104,16 +107,16 @@
        function will be called.
 
     2. The return type for 2D arrays depends on the default class set for
        state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> L, P, E = lqe(A, G, C, QN, RN)
-    >>> L, P, E = lqe(A, G, C, Q, RN, NN)
+    >>> L, P, E = lqe(A, G, C, QN, RN)                          # doctest: +SKIP
+    >>> L, P, E = lqe(A, G, C, Q, RN, NN)                       # doctest: +SKIP
 
     See Also
     --------
     lqr, dlqe, dlqr
 
     """
 
@@ -236,16 +239,16 @@
     Notes
     -----
     The return type for 2D arrays depends on the default class set for
     state space operations.  See :func:`~control.use_numpy_matrix`.
 
     Examples
     --------
-    >>> L, P, E = dlqe(A, G, C, QN, RN)
-    >>> L, P, E = dlqe(A, G, C, QN, RN, NN)
+    >>> L, P, E = dlqe(A, G, C, QN, RN)                         # doctest: +SKIP
+    >>> L, P, E = dlqe(A, G, C, QN, RN, NN)                     # doctest: +SKIP
 
     See Also
     --------
     dlqr, lqe, lqr
 
     """
 
@@ -303,148 +306,223 @@
     # Compute the result (dimension and symmetry checking done in dare())
     P, E, LT = dare(A.T, C.T, G @ QN @ G.T, RN, method=method,
                     B_s="C", Q_s="QN", R_s="RN", S_s="NN")
     return _ssmatrix(LT.T), _ssmatrix(P), E
 
 
 # Function to create an estimator
+#
+# TODO: create predictor/corrector, UKF, and other variants (?)
+#
 def create_estimator_iosystem(
         sys, QN, RN, P0=None, G=None, C=None,
-        state_labels='xhat[{i}]', output_labels='xhat[{i}]',
-        covariance_labels='P[{i},{j}]', sensor_labels=None):
+        control_indices=None, disturbance_indices=None,
+        estimate_labels='xhat[{i}]', covariance_labels='P[{i},{j}]',
+        measurement_labels=None, control_labels=None,
+        inputs=None, outputs=None, states=None, **kwargs):
     r"""Create an I/O system implementing a linear quadratic estimator
 
     This function creates an input/output system that implements a
     continuous time state estimator of the form
 
     .. math::
-    
+
         d \hat{x}/dt &= A \hat{x} + B u - L (C \hat{x} - y) \\
            dP/dt &= A P + P A^T + F Q_N F^T - P C^T R_N^{-1} C P \\
-               L &= P C^T R_N^{-1} 
+               L &= P C^T R_N^{-1}
 
     or a discrete time state estimator of the form
 
     .. math::
-    
+
         \hat{x}[k+1] &= A \hat{x}[k] + B u[k] - L (C \hat{x}[k] - y[k]) \\
                P[k+1] &= A P A^T + F Q_N F^T - A P C^T R_e^{-1} C P A \\
                     L &= A P C^T R_e^{-1}
 
     where :math:`R_e = R_N + C P C^T`.  It can be called in the form::
 
         estim = ct.create_estimator_iosystem(sys, QN, RN)
 
     where `sys` is the process dynamics and `QN` and `RN` are the covariance
-    of the disturbance noise and sensor noise.  The function returns the
-    estimator `estim` as I/O system with a parameter `correct` that can
+    of the disturbance noise and measurement noise.  The function returns
+    the estimator `estim` as I/O system with a parameter `correct` that can
     be used to turn off the correction term in the estimation (for forward
     predictions).
 
     Parameters
     ----------
-    sys : InputOutputSystem
-        The I/O system that represents the process dynamics.  If no estimator
-        is given, the output of this system should represent the full state.
+    sys : LinearIOSystem
+        The linear I/O system that represents the process dynamics.
     QN, RN : ndarray
-        Process and sensor noise covariance matrices.
+        Disturbance and measurement noise covariance matrices.
     P0 : ndarray, optional
         Initial covariance matrix.  If not specified, defaults to the steady
         state covariance.
     G : ndarray, optional
         Disturbance matrix describing how the disturbances enters the
         dynamics.  Defaults to sys.B.
     C : ndarray, optional
-        If the system has all full states output, define the measured values
-        to be used by the estimator.  Otherwise, use the system output as the
+        If the system has full state output, define the measured values to
+        be used by the estimator.  Otherwise, use the system output as the
         measured values.
-    {state, covariance, sensor, output}_labels : str or list of str, optional
-        Set the name of the signals to use for the internal state, covariance,
-        sensors, and outputs (state estimate).  If a single string is
-        specified, it should be a format string using the variable `i` as an
-        index (or `i` and `j` for covariance).  Otherwise, a list of
-        strings matching the size of the respective signal should be used.
-        Default is ``'xhat[{i}]'`` for state and output labels, ``'y[{i}]'``
-        for output labels and ``'P[{i},{j}]'`` for covariance labels.
 
     Returns
     -------
     estim : InputOutputSystem
         Input/output system representing the estimator.  This system takes
         the system output y and input u and generates the estimated state
         xhat.
 
+    Other Parameters
+    ----------------
+    control_indices : int, slice, or list of int or string, optional
+        Specify the indices in the system input vector that correspond to
+        the control inputs.  These inputs will be used as known control
+        inputs for the estimator. If value is an integer `m`, the first `m`
+        system inputs are used.  Otherwise, the value should be a slice or
+        a list of indices.  The list of indices can be specified as either
+        integer offsets or as system input signal names.  If not specified,
+        defaults to the system inputs.
+    disturbance_indices : int, list of int, or slice, optional
+        Specify the indices in the system input vector that correspond to
+        the unknown disturbances.  These inputs are assumed to be white
+        noise with noise intensity QN.  If value is an integer `m`, the
+        last `m` system inputs are used.  Otherwise, the value should be a
+        slice or a list of indices.  The list of indices can be specified
+        as either integer offsets or as system input signal names.  If not
+        specified, the disturbances are assumed to be added to the system
+        inputs.
+    estimate_labels : str or list of str, optional
+        Set the names of the state estimate variables (estimator outputs).
+        If a single string is specified, it should be a format string using
+        the variable `i` as an index.  Otherwise, a list of strings matching
+        the number of system states should be used.  Default is "xhat[{i}]".
+    covariance_labels : str or list of str, optional
+        Set the name of the the covariance state variables.  If a single
+        string is specified, it should be a format string using the
+        variables `i` and `j` as indices.  Otherwise, a list of strings
+        matching the size of the covariance matrix should be used.  Default
+        is "P[{i},{j}]".
+    measurement_labels, control_labels : str or list of str, optional
+        Set the name of the measurement and control signal names (estimator
+        inputs).  If a single string is specified, it should be a format
+        string using the variable ``i`` as an index.  Otherwise, a list of
+        strings matching the size of the system inputs and outputs should be
+        used.  Default is the signal names for the system measurements and
+        known control inputs. These settings can also be overriden using the
+        `inputs` keyword.
+    inputs, outputs, states : int or list of str, optional
+        Set the names of the inputs, outputs, and states, as described in
+        :func:`~control.InputOutputSystem`.  Overrides signal labels.
+    name : string, optional
+        System name (used for specifying signals). If unspecified, a generic
+        name <sys[id]> is generated with a unique integer id.
+
     Notes
     -----
     This function can be used with the ``create_statefbk_iosystem()`` function
     to create a closed loop, output-feedback, state space controller::
 
         K, _, _ = ct.lqr(sys, Q, R)
         est = ct.create_estimator_iosystem(sys, QN, RN, P0)
         ctrl, clsys = ct.create_statefbk_iosystem(sys, K, estimator=est)
 
     The estimator can also be run on its own to process a noisy signal::
 
         resp = ct.input_output_response(est, T, [Y, U], [X0, P0])
 
     If desired, the ``correct`` parameter can be set to ``False`` to allow
-    prediction with no additional sensor information::
+    prediction with no additional measurement information::
 
         resp = ct.input_output_response(
            est, T, 0, [X0, P0], param={'correct': False)
 
     """
 
     # Make sure that we were passed an I/O system as an input
     if not isinstance(sys, LinearIOSystem):
         raise ControlArgument("Input system must be a linear I/O system")
 
-    # Extract the matrices that we need for easy reference
-    A, B = sys.A, sys.B
+    # Process legacy keywords
+    estimate_labels = _process_legacy_keyword(
+        kwargs, 'output_labels', 'estimate_labels', estimate_labels)
+    measurement_labels = _process_legacy_keyword(
+        kwargs, 'sensor_labels', 'measurement_labels', measurement_labels)
+
+    # Separate state_labels no longer supported => special processing required
+    if kwargs.get('state_labels'):
+        if estimate_labels is None:
+            estimate_labels = _process_legacy_keyword(
+                kwargs, 'state_labels', estimate_labels)
+        else:
+            warnings.warn(
+                "deprecated 'state_labels' ignored; use 'states' instead")
+            kwargs.pop('state_labels')
+
+    # Set the state matrix for later use
+    A = sys.A
+
+    # Determine the control and disturbance indices
+    ctrl_idx, dist_idx = _process_control_disturbance_indices(
+        sys, control_indices, disturbance_indices)
+
+    # Set the input and direct matrices
+    B = sys.B[:, ctrl_idx]
+    if not np.allclose(sys.D, 0):
+        raise NotImplemented("nonzero 'D' matrix not yet implemented")
 
-    # Set the disturbance and output matrices
-    G = sys.B if G is None else G
+    # Set the output matrices
     if C is not None:
         # Make sure that we have the full system output
         if not np.array_equal(sys.C, np.eye(sys.nstates)):
             raise ValueError("System output must be full state")
 
         # Make sure that the output matches the size of RN
         if C.shape[0] != RN.shape[0]:
             raise ValueError("System output is the wrong size for C")
     else:
-        # Use the system outputs as the sensor outputs
+        # Use the system outputs as the measurements
         C = sys.C
-        if sensor_labels is None:
-            sensor_labels = sys.output_labels
+
+    # Generate the disturbance matrix (G)
+    if G is None:
+        G = sys.B if len(dist_idx) == 0 else sys.B[:, dist_idx]
 
     # Initialize the covariance matrix
     if P0 is None:
         # Initalize P0 to the steady state value
-        L0, P0, _ = lqe(A, G, C, QN, RN)
+        _, P0, _ = lqe(A, G, C, QN, RN)
 
     # Figure out the labels to use
-    if isinstance(state_labels, str):
-        # Generate the list of labels using the argument as a format string
-        state_labels = [state_labels.format(i=i) for i in range(sys.nstates)]
+    estimate_labels = _process_labels(
+        estimate_labels, 'estimate',
+        [f'xhat[{i}]' for i in range(sys.nstates)])
+    outputs = estimate_labels if outputs is None else outputs
+
+    if C is None:
+        # System outputs are the input to the estimator
+        measurement_labels = _process_labels(
+            measurement_labels, 'measurement', sys.output_labels)
+    else:
+        # Generate labels corresponding to measured values from C
+        measurement_labels = _process_labels(
+            measurement_labels, 'measurement', 
+            [f'y[{i}]' for i in range(C.shape[0])])
+    control_labels = _process_labels(
+        control_labels, 'control',
+        [sys.input_labels[i] for i in ctrl_idx])
+    inputs = measurement_labels + control_labels if inputs is None \
+        else inputs
 
     if isinstance(covariance_labels, str):
         # Generate the list of labels using the argument as a format string
         covariance_labels = [
             covariance_labels.format(i=i, j=j) \
             for i in range(sys.nstates) for j in range(sys.nstates)]
-
-    if isinstance(output_labels, str):
-        # Generate the list of labels using the argument as a format string
-        output_labels = [output_labels.format(i=i) for i in range(sys.nstates)]
-
-    sensor_labels = 'y[{i}]' if sensor_labels is None else sensor_labels
-    if isinstance(sensor_labels, str):
-        # Generate the list of labels using the argument as a format string
-        sensor_labels = [sensor_labels.format(i=i) for i in range(C.shape[0])]
+    states = estimate_labels + covariance_labels if states is None else states
 
     if isctime(sys):
         # Create an I/O system for the state feedback gains
         # Note: reshape vectors into column vectors for legacy np.matrix
 
         R_inv = np.linalg.inv(RN)
         Reps_inv = C.T @ R_inv @ C
@@ -461,15 +539,15 @@
             y = u[0:C.shape[0]].reshape(-1, 1)
             u = u[C.shape[0]:].reshape(-1, 1)
 
             # Compute the optimal gain
             L = P @ C.T @ R_inv
 
             # Update the state estimate
-            dxhat = A @ xhat + B @ u            # prediction
+            dxhat = A @ xhat + B @ u                    # prediction
             if correct:
                 dxhat -= L @ (C @ xhat - y)     # correction
 
             # Update the covariance
             dP = A @ P + P @ A.T + G @ QN @ G.T
             if correct:
                 dP -= P @ Reps_inv @ P
@@ -491,15 +569,15 @@
             u = u[C.shape[0]:].reshape(-1, 1)
 
             # Compute the optimal gain
             Reps_inv = np.linalg.inv(RN + C @ P @ C.T)
             L = A @ P @ C.T @ Reps_inv
 
             # Update the state estimate
-            dxhat = A @ xhat + B @ u            # prediction
+            dxhat = A @ xhat + B @ u                    # prediction
             if correct:
                 dxhat -= L @ (C @ xhat - y)     # correction
 
             # Update the covariance
             dP = A @ P @ A.T + G @ QN @ G.T
             if correct:
                 dP -= A @ P @ C.T @ Reps_inv @ C @ P @ A.T
@@ -508,17 +586,16 @@
             return np.hstack([dxhat.reshape(-1), dP.reshape(-1)])
 
     def _estim_output(t, x, u, params):
         return x[0:sys.nstates]
 
     # Define the estimator system
     return NonlinearIOSystem(
-        _estim_update, _estim_output, states=state_labels + covariance_labels,
-        inputs=sensor_labels + sys.input_labels, outputs=output_labels,
-        dt=sys.dt)
+        _estim_update, _estim_output, dt=sys.dt,
+        states=states, inputs=inputs, outputs=outputs,  **kwargs)
 
 
 def white_noise(T, Q, dt=0):
     """Generate a white noise signal with specified intensity.
 
     This function generates a (multi-variable) white noise signal of
     specified intensity as either a sampled continous time signal or a
@@ -560,14 +637,15 @@
     # Generate independent white noise sources for each input
     W = np.array([
         np.random.normal(0, 1/sqrt(dt), T.size) for i in range(Q.shape[0])])
 
     # Return a linear combination of the noise sources
     return sp.linalg.sqrtm(Q) @ W
 
+
 def correlation(T, X, Y=None, squeeze=True):
     """Compute the correlation of time signals.
 
     For a time series X(t) (and optionally Y(t)), the correlation() function
     computes the correlation matrix E(X'(t+tau) X(t)) or the cross-correlation
     matrix E(X'(t+tau) Y(t)]:
```

### Comparing `control-0.9.3.post2/control/tests/bdalg_test.py` & `control-0.9.4/control/tests/bdalg_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/bspline_test.py` & `control-0.9.4/control/tests/bspline_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/canonical_test.py` & `control-0.9.4/control/tests/canonical_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,16 @@
 def test_bdschur_sort(eigvals, sorted_blk_eigvals, sort):
     # use block diagonal form to prevent numerical complications
     # for discrete case, exp and log introduce round-off, can't test as compeletely
     a = block_diag_from_eig(eigvals)
 
     b, t, blksizes = bdschur(a, sort=sort)
     assert len(blksizes) == len(sorted_blk_eigvals)
+    np.testing.assert_allclose(a, t @ b @ t.T)
+    np.testing.assert_allclose(t.T, np.linalg.inv(t))
 
     blocks = extract_bdiag(b, blksizes)
     for block, blk_eigval in zip(blocks, sorted_blk_eigvals):
         test_eigvals = np.linalg.eigvals(block)
         np.testing.assert_allclose(test_eigvals.real,
                                    blk_eigval.real)
```

### Comparing `control-0.9.3.post2/control/tests/config_test.py` & `control-0.9.4/control/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/conftest.py` & `control-0.9.4/control/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 
 
 @pytest.fixture(scope="function")
 def editsdefaults():
     """Make sure any changes to the defaults only last during a test."""
     restore = control.config.defaults.copy()
     yield
-    control.config.defaults = restore.copy()
+    control.config.defaults.clear()
+    control.config.defaults.update(restore)
 
 
 @pytest.fixture(scope="function")
 def mplcleanup():
     """Clean up any plots and changes a test may have made to matplotlib.
 
     compare matplotlib.testing.decorators.cleanup() but as a fixture instead
@@ -114,7 +115,12 @@
     save = mpl.units.registry.copy()
     try:
         yield
     finally:
         mpl.units.registry.clear()
         mpl.units.registry.update(save)
         mpl.pyplot.close("all")
+
+
+# Allow pytest.mark.slow to mark slow tests (skip with pytest -m "not slow")
+def pytest_configure(config):
+    config.addinivalue_line("markers", "slow: mark test as slow to run")
```

### Comparing `control-0.9.3.post2/control/tests/convert_test.py` & `control-0.9.4/control/tests/convert_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/ctrlutil_test.py` & `control-0.9.4/control/tests/ctrlutil_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ctrlutil_test.py"""
 
 import numpy as np
-
+import pytest
+import control as ct
 from control.ctrlutil import db2mag, mag2db, unwrap
 
 class TestUtils:
 
     mag = np.array([1, 10, 100, 2, 0.1, 0.01])
     db = np.array([0, 20, 40, 6.0205999, -20, -40])
 
@@ -54,7 +55,12 @@
     def test_mag2db(self):
         for db, mag in zip(self.db, self.mag):
             np.testing.assert_almost_equal(db, mag2db(mag))
 
     def test_mag2db_array(self):
         db_array = mag2db(self.mag)
         np.testing.assert_array_almost_equal(db_array, self.db)
+
+    def test_issys(self):
+        sys = ct.rss(2, 1, 1)
+        with pytest.warns(FutureWarning, match="deprecated; use isinstance"):
+            ct.issys(sys)
```

### Comparing `control-0.9.3.post2/control/tests/delay_test.py` & `control-0.9.4/control/tests/delay_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/descfcn_test.py` & `control-0.9.4/control/tests/descfcn_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/discrete_test.py` & `control-0.9.4/control/tests/discrete_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,36 +372,59 @@
         for sysc in (tsys.siso_tf1, tsys.siso_tf1c):
             sysd = sample_system(sysc, 1, method="matched")
             assert sysd.dt == 1
 
     @pytest.mark.parametrize("plantname",
                              ["siso_ss1c",
                               "siso_tf1c"])
-    def test_sample_system_prewarp(self, tsys, plantname):
+    @pytest.mark.parametrize("wwarp",
+                             [.1, 1, 3])
+    @pytest.mark.parametrize("Ts",
+                             [.1, 1])
+    @pytest.mark.parametrize("discretization_type",
+                             ['bilinear', 'tustin', 'gbt'])
+    def test_sample_system_prewarp(self, tsys, plantname, discretization_type, wwarp, Ts):
         """bilinear approximation with prewarping test"""
-        wwarp = 50
-        Ts = 0.025
         # test state space version
         plant = getattr(tsys, plantname)
         plant_fr = plant(wwarp * 1j)
+        alpha = 0.5 if discretization_type == 'gbt' else None
 
-        plant_d_warped = plant.sample(Ts, 'bilinear', prewarp_frequency=wwarp)
+        plant_d_warped = plant.sample(Ts, discretization_type,
+            prewarp_frequency=wwarp, alpha=alpha)
         dt = plant_d_warped.dt
         plant_d_fr = plant_d_warped(np.exp(wwarp * 1.j * dt))
         np.testing.assert_array_almost_equal(plant_fr, plant_d_fr)
 
-        plant_d_warped = sample_system(plant, Ts, 'bilinear',
-                prewarp_frequency=wwarp)
+        plant_d_warped = sample_system(plant, Ts, discretization_type,
+            prewarp_frequency=wwarp, alpha=alpha)
         plant_d_fr = plant_d_warped(np.exp(wwarp * 1.j * dt))
         np.testing.assert_array_almost_equal(plant_fr, plant_d_fr)
 
-        plant_d_warped = c2d(plant, Ts, 'bilinear', prewarp_frequency=wwarp)
+        plant_d_warped = c2d(plant, Ts, discretization_type,
+            prewarp_frequency=wwarp, alpha=alpha)
         plant_d_fr = plant_d_warped(np.exp(wwarp * 1.j * dt))
         np.testing.assert_array_almost_equal(plant_fr, plant_d_fr)
 
+    @pytest.mark.parametrize("plantname",
+                             ["siso_ss1c",
+                              "siso_tf1c"])
+    @pytest.mark.parametrize("discretization_type",
+                             ['euler', 'backward_diff', 'zoh'])
+    def test_sample_system_prewarp_warning(self, tsys, plantname, discretization_type):
+        plant = getattr(tsys, plantname)
+        wwarp = 1
+        Ts = 0.1
+        with pytest.warns(UserWarning, match="prewarp_frequency ignored: incompatible conversion"):
+            plant_d_warped = plant.sample(Ts, discretization_type, prewarp_frequency=wwarp)
+        with pytest.warns(UserWarning, match="prewarp_frequency ignored: incompatible conversion"):
+            plant_d_warped = sample_system(plant, Ts, discretization_type, prewarp_frequency=wwarp)
+        with pytest.warns(UserWarning, match="prewarp_frequency ignored: incompatible conversion"):
+            plant_d_warped = c2d(plant, Ts, discretization_type, prewarp_frequency=wwarp)
+
     def test_sample_system_errors(self, tsys):
         # Check errors
         with pytest.raises(ValueError):
             sample_system(tsys.siso_ss1d, 1)
         with pytest.raises(ValueError):
             sample_system(tsys.siso_tf1d, 1)
         with pytest.raises(ValueError):
@@ -442,19 +465,19 @@
         sys = TransferFunction([1], [1, 0.5], 1)
         omega = [1, 2, 3]
         mag_out, phase_out, omega_out = bode(sys, omega)
         H_z = list(map(lambda w: 1./(np.exp(1.j * w) + 0.5), omega))
         np.testing.assert_array_almost_equal(omega, omega_out)
         np.testing.assert_array_almost_equal(mag_out, np.absolute(H_z))
         np.testing.assert_array_almost_equal(phase_out, np.angle(H_z))
-    
+
     def test_signal_names(self, tsys):
         "test that signal names are preserved in conversion to discrete-time"
-        ssc = StateSpace(tsys.siso_ss1c, 
-            inputs='u', outputs='y', states=['a', 'b', 'c']) 
+        ssc = StateSpace(tsys.siso_ss1c,
+            inputs='u', outputs='y', states=['a', 'b', 'c'])
         ssd = ssc.sample(0.1)
         tfc = TransferFunction(tsys.siso_tf1c, inputs='u', outputs='y')
         tfd = tfc.sample(0.1)
         assert ssd.input_labels == ['u']
         assert ssd.state_labels == ['a', 'b', 'c']
         assert ssd.output_labels == ['y']
         assert tfd.input_labels == ['u']
@@ -463,15 +486,15 @@
         ssd = sample_system(ssc, 0.1)
         tfd = sample_system(tfc, 0.1)
         assert ssd.input_labels == ['u']
         assert ssd.state_labels == ['a', 'b', 'c']
         assert ssd.output_labels == ['y']
         assert tfd.input_labels == ['u']
         assert tfd.output_labels == ['y']
-    
+
         # system names and signal name override
         sysc = StateSpace(1.1, 1, 1, 1, inputs='u', outputs='y', states='a')
 
         sysd = sample_system(sysc, 0.1, name='sampled')
         assert sysd.name == 'sampled'
         assert sysd.find_input('u') == 0
         assert sysd.find_output('y') == 0
@@ -484,21 +507,21 @@
         # If copy is False, signal names should not be copied
         sysd_nocopy = sample_system(sysc, 0.1, copy_names=False)
         assert sysd_nocopy.find_input('u') is None
         assert sysd_nocopy.find_output('y') is None
         assert sysd_nocopy.find_state('a') is None
 
         # if signal names are provided, they should override those of sysc
-        sysd_newnames = sample_system(sysc, 0.1, 
+        sysd_newnames = sample_system(sysc, 0.1,
             inputs='v', outputs='x', states='b')
         assert sysd_newnames.find_input('v') == 0
         assert sysd_newnames.find_input('u') is None
         assert sysd_newnames.find_output('x') == 0
         assert sysd_newnames.find_output('y') is None
         assert sysd_newnames.find_state('b') == 0
-        assert sysd_newnames.find_state('a') is None        
+        assert sysd_newnames.find_state('a') is None
         # test just one name
         sysd_newnames = sample_system(sysc, 0.1, inputs='v')
         assert sysd_newnames.find_input('v') == 0
         assert sysd_newnames.find_input('u') is None
         assert sysd_newnames.find_output('y') == 0
         assert sysd_newnames.find_output('x') is None
```

### Comparing `control-0.9.3.post2/control/tests/flatsys_test.py` & `control-0.9.4/control/tests/flatsys_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             # Known failure cases
             if re.match(".*precision loss.*", traj_ocp.message):
                 pytest.xfail("precision loss in some configurations")
 
             elif re.match("Iteration limit.*", traj_ocp.message) and \
                  re.match(
                      "conda ubuntu-3.* Generic", os.getenv('JOBNAME', '')) and \
-                 re.match("1.24.[01]", np.__version__):
+                 re.match("1.24.[012]", np.__version__):
                 pytest.xfail("gh820: iteration limit exceeded")
 
             else:
                 # Dump out information to allow creation of an exception
                 print("Message:", traj_ocp.message)
                 print("Platform:", platform.platform())
                 print("Python:", platform.python_version())
```

### Comparing `control-0.9.3.post2/control/tests/frd_test.py` & `control-0.9.4/control/tests/frd_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/freqresp_test.py` & `control-0.9.4/control/tests/freqresp_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -371,14 +371,26 @@
     ])
 def test_phase_wrap(TF, wrap_phase, min_phase, max_phase):
     mag, phase, omega = ctrl.bode(TF, wrap_phase=wrap_phase)
     assert(min(phase) >= min_phase)
     assert(max(phase) <= max_phase)
 
 
+def test_phase_wrap_multiple_systems():
+    sys_unstable = ctrl.zpk([],[1,1], gain=1)
+
+    mag, phase, omega = ctrl.bode(sys_unstable, plot=False)
+    assert(np.min(phase) >= -2*np.pi)
+    assert(np.max(phase) <= -1*np.pi)
+
+    mag, phase, omega = ctrl.bode((sys_unstable, sys_unstable), plot=False)
+    assert(np.min(phase) >= -2*np.pi)
+    assert(np.max(phase) <= -1*np.pi)
+
+
 def test_freqresp_warn_infinite():
     """Test evaluation warnings for transfer functions w/ pole at the origin"""
     sys_finite = ctrl.tf([1], [1, 0.01])
     sys_infinite = ctrl.tf([1], [1, 0.01, 0])
 
     # Transfer function with finite zero frequency gain
     np.testing.assert_almost_equal(sys_finite(0), 100)
```

### Comparing `control-0.9.3.post2/control/tests/input_element_int_test.py` & `control-0.9.4/control/tests/input_element_int_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/interconnect_test.py` & `control-0.9.4/control/tests/interconnect_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,21 @@
     P = ct.ss2io(
         ct.rss(2, 1, 1, strictly_proper=True),
         inputs='u', outputs='y', name='P')
     kp = ct.tf(random.uniform(1, 10), [1])
     ki = ct.tf(random.uniform(1, 10), [1, 0])
     C = ct.tf2io(kp + ki, inputs='e', outputs='u', name='C')
 
+    # same but static C2
+    C2 = ct.tf(random.uniform(1, 10), 1,
+        inputs='e', outputs='u', name='C2')
+
     # Block diagram computation
     Tss = ct.feedback(P * C, 1)
+    Tss2 = ct.feedback(P * C2, 1)
 
     # Construct the interconnection explicitly
     Tio_exp = ct.interconnect(
         (C, P),
         connections = [['P.u', 'C.u'], ['C.e', '-P.y']],
         inplist='C.e', outlist='P.y')
 
@@ -89,14 +94,23 @@
         (C, P, sumblk), inplist=['r'], outlist=['y'])
 
     np.testing.assert_almost_equal(Tio_sum.A, Tss.A)
     np.testing.assert_almost_equal(Tio_sum.B, Tss.B)
     np.testing.assert_almost_equal(Tio_sum.C, Tss.C)
     np.testing.assert_almost_equal(Tio_sum.D, Tss.D)
 
+    # test whether signal names work for static system C2
+    Tio_sum2 = ct.interconnect(
+        [C2, P, sumblk], inputs='r', outputs='y')
+
+    np.testing.assert_almost_equal(Tio_sum2.A, Tss2.A)
+    np.testing.assert_almost_equal(Tio_sum2.B, Tss2.B)
+    np.testing.assert_almost_equal(Tio_sum2.C, Tss2.C)
+    np.testing.assert_almost_equal(Tio_sum2.D, Tss2.D)
+
     # Setting connections to False should lead to an empty connection map
     empty = ct.interconnect(
         (C, P, sumblk), connections=False, inplist=['r'], outlist=['y'])
     np.testing.assert_allclose(empty.connect_map, np.zeros((4, 3)))
 
     # Implicit summation across repeated signals
     kp_io = ct.tf2io(kp, inputs='e', outputs='u', name='kp')
@@ -228,27 +242,58 @@
     P_s1 = ct.interconnect([P1_iosys, P2_iosys], inputs=['u1'], outputs='y2')
     assert P_s1.output_index == {'y2' : 0}
 
     P_s2 = ct.interconnect([P1_iosys, P2_iosys], inputs=['u1'], output='y2')
     assert P_s2.output_index == {'y2' : 0}
 
 def test_linear_interconnect():
-    tf_ctrl = ct.tf(1, (10.1, 1), inputs='e', outputs='u')
-    tf_plant = ct.tf(1, (10.1, 1), inputs='u', outputs='y')
-    ss_ctrl = ct.ss(1, 2, 1, 2, inputs='e', outputs='u')
-    ss_plant = ct.ss(1, 2, 1, 2, inputs='u', outputs='y')
+    tf_ctrl = ct.tf(1, (10.1, 1), inputs='e', outputs='u', name='ctrl')
+    tf_plant = ct.tf(1, (10.1, 1), inputs='u', outputs='y', name='plant')
+    ss_ctrl = ct.ss(1, 2, 1, 0, inputs='e', outputs='u', name='ctrl')
+    ss_plant = ct.ss(1, 2, 1, 0, inputs='u', outputs='y', name='plant')
     nl_ctrl = ct.NonlinearIOSystem(
-        lambda t, x, u, params: x*x, 
-        lambda t, x, u, params: u*x, states=1, inputs='e', outputs='u')
+        lambda t, x, u, params: x*x, lambda t, x, u, params: u*x,
+        states=1, inputs='e', outputs='u', name='ctrl')
     nl_plant = ct.NonlinearIOSystem(
-        lambda t, x, u, params: x*x, 
-        lambda t, x, u, params: u*x, states=1, inputs='u', outputs='y')
-
-    assert isinstance(ct.interconnect((tf_ctrl, tf_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert isinstance(ct.interconnect((ss_ctrl, ss_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert isinstance(ct.interconnect((tf_ctrl, ss_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert isinstance(ct.interconnect((ss_ctrl, tf_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    
-    assert ~isinstance(ct.interconnect((nl_ctrl, ss_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert ~isinstance(ct.interconnect((nl_ctrl, tf_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert ~isinstance(ct.interconnect((ss_ctrl, nl_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
-    assert ~isinstance(ct.interconnect((tf_ctrl, nl_plant), inputs='e', outputs='y'), ct.LinearIOSystem)
+        lambda t, x, u, params: x*x, lambda t, x, u, params: u*x,
+        states=1, inputs='u', outputs='y', name='plant')
+    sumblk = ct.summing_junction(inputs=['r', '-y'], outputs=['e'], name='sum')
+
+    # Interconnections of linear I/O systems should be linear I/O system
+    assert isinstance(
+        ct.interconnect([tf_ctrl, tf_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert isinstance(
+        ct.interconnect([ss_ctrl, ss_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert isinstance(
+        ct.interconnect([tf_ctrl, ss_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert isinstance(
+        ct.interconnect([ss_ctrl, tf_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+
+    # Interconnections with nonliner I/O systems should not be linear
+    assert ~isinstance(
+        ct.interconnect([nl_ctrl, ss_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert ~isinstance(
+        ct.interconnect([nl_ctrl, tf_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert ~isinstance(
+        ct.interconnect([ss_ctrl, nl_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+    assert ~isinstance(
+        ct.interconnect([tf_ctrl, nl_plant, sumblk], inputs='r', outputs='y'),
+        ct.LinearIOSystem)
+
+    # Implicit converstion of transfer function should retain name
+    clsys = ct.interconnect(
+        [tf_ctrl, ss_plant, sumblk],
+        connections=[
+            ['plant.u', 'ctrl.u'],
+            ['ctrl.e', 'sum.e'],
+            ['sum.y', 'plant.y']
+        ],
+        inplist=['sum.r'], inputs='r',
+        outlist=['plant.y'], outputs='y')
+    assert clsys.syslist[0].name == 'ctrl'
```

### Comparing `control-0.9.3.post2/control/tests/iosys_test.py` & `control-0.9.4/control/tests/iosys_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1615,14 +1615,35 @@
 
 
 def secord_output(t, x, u, params={}):
     """Second order system dynamics output"""
     return np.array([x[0]])
 
 
+def test_interconnect_name():
+    g = ct.LinearIOSystem(ct.ss(-1,1,1,0),
+                          inputs=['u'],
+                          outputs=['y'],
+                          name='g')
+    k = ct.LinearIOSystem(ct.ss(0,10,2,0),
+                          inputs=['e'],
+                          outputs=['z'],
+                          name='k')
+    h = ct.interconnect([g,k],
+                            inputs=['u','e'],
+                            outputs=['y','z'])
+    assert re.match(r'sys\[\d+\]', h.name), f"Interconnect default name does not match 'sys[]' pattern, got '{h.name}'"
+
+    h = ct.interconnect([g,k],
+                            inputs=['u','e'],
+                            outputs=['y','z'],
+                            name='ic_system')
+    assert h.name == 'ic_system', f"Interconnect name excpected 'ic_system', got '{h.name}'"
+
+
 def test_interconnect_unused_input():
     # test that warnings about unused inputs are reported, or not,
     # as required
     g = ct.LinearIOSystem(ct.ss(-1,1,1,0),
                           inputs=['u'],
                           outputs=['y'],
                           name='g')
@@ -1658,15 +1679,14 @@
                             outputs=['y'],
                             ignore_inputs=['s.n'])
 
         # no warning if auto-connect disabled
         h = ct.interconnect([g,s,k],
                             connections=False)
 
-
     # warn if explicity ignored input in fact used
     with pytest.warns(
             UserWarning,
             match=r"Input\(s\) specified as ignored is \(are\) used:") \
             as record:
         h = ct.interconnect([g,s,k],
                             inputs=['r'],
@@ -1756,14 +1776,50 @@
     with pytest.raises(ValueError):
         h = ct.interconnect([g,s,k],
                             inputs=['r'],
                             outputs=['y'],
                             ignore_outputs=['v'])
 
 
+def test_interconnect_add_unused():
+    P = ct.ss(
+        [[-1]], [[1, -1]], [[-1], [1]], 0,
+        inputs=['u1', 'u2'], outputs=['y1','y2'], name='g')
+    S = ct.summing_junction(inputs=['r','-y1'], outputs=['e'], name='s')
+    C = ct.ss(0, 10, 2, 0, inputs=['e'], outputs=['u1'], name='k')
+
+    # Try a normal interconnection
+    G1 = ct.interconnect(
+        [P, S, C], inputs=['r', 'u2'], outputs=['y1', 'y2'])
+
+    # Same system, but using add_unused
+    G2 = ct.interconnect(
+        [P, S, C], inputs=['r'], outputs=['y1'], add_unused=True)
+    assert G2.input_labels == G1.input_labels
+    assert G2.input_offset == G1.input_offset
+    assert G2.output_labels == G1.output_labels
+    assert G2.output_offset == G1.output_offset
+
+    # Ignore one of the inputs
+    G3 = ct.interconnect(
+        [P, S, C], inputs=['r'], outputs=['y1'], add_unused=True,
+        ignore_inputs=['u2'])
+    assert G3.input_labels == G1.input_labels[0:1]
+    assert G3.output_labels == G1.output_labels
+    assert G3.output_offset == G1.output_offset
+
+    # Ignore one of the outputs
+    G4 = ct.interconnect(
+        [P, S, C], inputs=['r'], outputs=['y1'], add_unused=True,
+        ignore_outputs=['y2'])
+    assert G4.input_labels == G1.input_labels
+    assert G4.input_offset == G1.input_offset
+    assert G4.output_labels == G1.output_labels[0:1]
+
+
 def test_input_output_broadcasting():
     # Create a system, time vector, and noisy input
     sys = ct.rss(6, 2, 3)
     T = np.linspace(0, 10, 10)
     U = np.zeros((sys.ninputs, T.size))
     U[0, :] = np.sin(T)
     U[1, :] = np.zeros_like(U[1, :])
@@ -1976,7 +2032,18 @@
             iy = np.s_[:] if iy is None else np.array(iy)
             np.testing.assert_allclose(
                 eqpt_out(0, xeq, ueq, {})[iy], y0[iy], atol=1e-6)
 
     # Check that we got the expected result as well
     np.testing.assert_allclose(np.array(xeq), x_expect, atol=1e-6)
     np.testing.assert_allclose(np.array(ueq), u_expect, atol=1e-6)
+
+def test_iosys_sample():
+    csys = ct.rss(2, 1, 1)
+    dsys = csys.sample(0.1)
+    assert isinstance(dsys, ct.LinearIOSystem)
+    assert dsys.dt == 0.1
+
+    csys = ct.rss(2, 1, 1)
+    dsys = ct.sample_system(csys, 0.1)
+    assert isinstance(dsys, ct.LinearIOSystem)
+    assert dsys.dt == 0.1
```

### Comparing `control-0.9.3.post2/control/tests/kwargs_test.py` & `control-0.9.4/control/tests/kwargs_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 import control
 import control.flatsys
 
 # List of all of the test modules where kwarg unit tests are defined
 import control.tests.flatsys_test as flatsys_test
 import control.tests.frd_test as frd_test
 import control.tests.interconnect_test as interconnect_test
+import control.tests.optimal_test as optimal_test
 import control.tests.statefbk_test as statefbk_test
+import control.tests.stochsys_test as stochsys_test
 import control.tests.trdata_test as trdata_test
 
-
 @pytest.mark.parametrize("module, prefix", [
-    (control, ""), (control.flatsys, "flatsys.")
+    (control, ""), (control.flatsys, "flatsys."), (control.optimal, "optimal.")
 ])
 def test_kwarg_search(module, prefix):
     # Look through every object in the package
     for name, obj in inspect.getmembers(module):
         # Skip anything that is outside of this module
         if inspect.getmodule(obj) is not None and \
            not inspect.getmodule(obj).__name__.startswith('control'):
@@ -81,30 +82,32 @@
      (control.dlqr, 1, 0, ([[1, 0], [0, 1]], [[1]]), {}),
      (control.drss, 0, 0, (2, 1, 1), {}),
      (control.input_output_response, 1, 0, ([0, 1, 2], [1, 1, 1]), {}),
      (control.lqe, 1, 0, ([[1]], [[1]]), {}),
      (control.lqr, 1, 0, ([[1, 0], [0, 1]], [[1]]), {}),
      (control.linearize, 1, 0, (0, 0), {}),
      (control.pzmap, 1, 0, (), {}),
-     (control.rlocus, 0, 1, ( ), {}),
-     (control.root_locus, 0, 1, ( ), {}),
+     (control.rlocus, 0, 1, (), {}),
+     (control.root_locus, 0, 1, (), {}),
      (control.rss, 0, 0, (2, 1, 1), {}),
      (control.set_defaults, 0, 0, ('control',), {'default_dt': True}),
      (control.ss, 0, 0, (0, 0, 0, 0), {'dt': 1}),
      (control.ss2io, 1, 0,  (), {}),
      (control.ss2tf, 1, 0, (), {}),
      (control.summing_junction, 0, 0, (2,), {}),
      (control.tf, 0, 0, ([1], [1, 1]), {}),
      (control.tf2io, 0, 1, (), {}),
      (control.tf2ss, 0, 1, (), {}),
      (control.zpk, 0, 0, ([1], [2, 3], 4), {}),
      (control.InputOutputSystem, 0, 0, (),
       {'inputs': 1, 'outputs': 1, 'states': 1}),
      (control.InputOutputSystem.linearize, 1, 0, (0, 0), {}),
-     (control.StateSpace, 0, 0, ([[-1, 0], [0, -1]], [[1], [1]], [[1, 1]], 0), {}),
+     (control.LinearIOSystem.sample, 1, 0, (0.1,), {}),
+     (control.StateSpace, 0, 0,
+      ([[-1, 0], [0, -1]], [[1], [1]], [[1, 1]], 0), {}),
      (control.TransferFunction, 0, 0, ([1], [1, 1]), {})]
 )
 def test_unrecognized_kwargs(function, nsssys, ntfsys, moreargs, kwargs,
                              mplcleanup, editsdefaults):
     # Create SISO systems for use in parameterized tests
     sssys = control.ss([[-1, 1], [0, -1]], [[0], [1]], [[1, 0]], 0, dt=None)
     tfsys = control.tf([1], [1, 1])
@@ -154,14 +157,16 @@
 # will also force people who add new functions to put in an appropriate unit
 # test.
 #
 
 kwarg_unittest = {
     'bode': test_matplotlib_kwargs,
     'bode_plot': test_matplotlib_kwargs,
+    'create_estimator_iosystem': stochsys_test.test_estimator_errors,
+    'create_statefbk_iosystem': statefbk_test.TestStatefbk.test_statefbk_errors,
     'describing_function_plot': test_matplotlib_kwargs,
     'dlqe': test_unrecognized_kwargs,
     'dlqr': test_unrecognized_kwargs,
     'drss': test_unrecognized_kwargs,
     'gangof4': test_matplotlib_kwargs,
     'gangof4_plot': test_matplotlib_kwargs,
     'input_output_response': test_unrecognized_kwargs,
@@ -181,34 +186,49 @@
     'ss2io': test_unrecognized_kwargs,
     'ss2tf': test_unrecognized_kwargs,
     'summing_junction': interconnect_test.test_interconnect_exceptions,
     'tf': test_unrecognized_kwargs,
     'tf2io' : test_unrecognized_kwargs,
     'tf2ss' : test_unrecognized_kwargs,
     'sample_system' : test_unrecognized_kwargs,
+    'c2d' : test_unrecognized_kwargs,
     'zpk': test_unrecognized_kwargs,
     'flatsys.point_to_point':
         flatsys_test.TestFlatSys.test_point_to_point_errors,
     'flatsys.solve_flat_ocp':
         flatsys_test.TestFlatSys.test_solve_flat_ocp_errors,
+    'optimal.create_mpc_iosystem': optimal_test.test_mpc_iosystem_rename,
+    'optimal.solve_ocp': optimal_test.test_ocp_argument_errors,
+    'optimal.solve_oep': optimal_test.test_oep_argument_errors,
     'FrequencyResponseData.__init__':
         frd_test.TestFRD.test_unrecognized_keyword,
     'InputOutputSystem.__init__': test_unrecognized_kwargs,
     'InputOutputSystem.linearize': test_unrecognized_kwargs,
     'InterconnectedSystem.__init__':
         interconnect_test.test_interconnect_exceptions,
     'LinearIOSystem.__init__':
         interconnect_test.test_interconnect_exceptions,
+    'LinearIOSystem.sample': test_unrecognized_kwargs,
     'NonlinearIOSystem.__init__':
         interconnect_test.test_interconnect_exceptions,
     'StateSpace.__init__': test_unrecognized_kwargs,
-    'StateSpace.sample': test_unrecognized_kwargs, 
+    'StateSpace.sample': test_unrecognized_kwargs,
     'TimeResponseData.__call__': trdata_test.test_response_copy,
     'TransferFunction.__init__': test_unrecognized_kwargs,
-    'TransferFunction.sample': test_unrecognized_kwargs, 
+    'TransferFunction.sample': test_unrecognized_kwargs,
+    'optimal.OptimalControlProblem.__init__':
+        optimal_test.test_ocp_argument_errors,
+    'optimal.OptimalControlProblem.compute_trajectory':
+        optimal_test.test_ocp_argument_errors,
+    'optimal.OptimalControlProblem.create_mpc_iosystem':
+        optimal_test.test_ocp_argument_errors,
+    'optimal.OptimalEstimationProblem.__init__':
+        optimal_test.test_oep_argument_errors,
+    'optimal.OptimalEstimationProblem.create_mhe_iosystem':
+        optimal_test.test_oep_argument_errors,
 }
 
 #
 # Look for keywords with mutable defaults
 #
 # This test goes through every function and looks for signatures that have a
 # default value for a keyword that is mutable.  An error is generated unless
@@ -217,17 +237,14 @@
 # value of the mutable is not modified in the code).
 #
 mutable_ok = {                                          # initial and date
     control.flatsys.SystemTrajectory.__init__,          # RMM, 18 Nov 2022
     control.freqplot._add_arrows_to_line2D,             # RMM, 18 Nov 2022
     control.namedio._process_dt_keyword,                # RMM, 13 Nov 2022
     control.namedio._process_namedio_keywords,          # RMM, 18 Nov 2022
-    control.optimal.OptimalControlProblem.__init__,     # RMM, 18 Nov 2022
-    control.optimal.solve_ocp,                          # RMM, 18 Nov 2022
-    control.optimal.create_mpc_iosystem,                # RMM, 18 Nov 2022
 }
 
 @pytest.mark.parametrize("module", [control, control.flatsys])
 def test_mutable_defaults(module, recurse=True):
     # Look through every object in the package
     for name, obj in inspect.getmembers(module):
         # Skip anything that is outside of this module
```

### Comparing `control-0.9.3.post2/control/tests/lti_test.py` & `control-0.9.4/control/tests/lti_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pytest
 from .conftest import editsdefaults
 
 import control as ct
 from control import c2d, tf, ss, tf2ss, NonlinearIOSystem
-from control.lti import LTI, evalfr, damp, dcgain, zeros, poles
+from control.lti import LTI, evalfr, damp, dcgain, zeros, poles, bandwidth
 from control import common_timebase, isctime, isdtime, issiso, timebaseEqual
 from control.tests.conftest import slycotonly
 from control.exception import slycot_check
 
 class TestLTI:
     @pytest.mark.parametrize("fun, args", [
         [tf, (126, [-1, 42])],
@@ -100,14 +100,46 @@
         np.testing.assert_almost_equal(p2, p2_zplane)
 
     def test_dcgain(self):
         sys = tf(84, [1, 2])
         np.testing.assert_allclose(sys.dcgain(), 42)
         np.testing.assert_allclose(dcgain(sys), 42)
 
+    def test_bandwidth(self):
+        # test a first-order system, compared with matlab
+        sys1 = tf(0.1, [1, 0.1])
+        np.testing.assert_allclose(sys1.bandwidth(), 0.099762834511098)
+        np.testing.assert_allclose(bandwidth(sys1), 0.099762834511098)
+
+        # test a second-order system, compared with matlab
+        wn2 = 1
+        zeta2 = 0.001
+        sys2 = sys1 * tf(wn2**2, [1, 2*zeta2*wn2, wn2**2])
+        np.testing.assert_allclose(sys2.bandwidth(), 0.101848388240241)
+        np.testing.assert_allclose(bandwidth(sys2), 0.101848388240241)
+
+        # test constant gain, bandwidth should be infinity
+        sysAP = tf(1,1)
+        np.testing.assert_allclose(bandwidth(sysAP), np.inf)
+
+        # test integrator, bandwidth should return np.nan
+        sysInt = tf(1, [1, 0])
+        np.testing.assert_allclose(bandwidth(sysInt), np.nan)
+
+        # test exception for system other than LTI
+        np.testing.assert_raises(TypeError, bandwidth, 1)
+
+        # test exception for system other than SISO system
+        sysMIMO = tf([[[-1, 41], [1]], [[1, 2], [3, 4]]], 
+                     [[[1, 10], [1, 20]], [[1, 30], [1, 40]]])
+        np.testing.assert_raises(TypeError, bandwidth, sysMIMO)
+
+        # test if raise exception if dbdrop is positive scalar
+        np.testing.assert_raises(ValueError, bandwidth, sys1, 3)
+
     @pytest.mark.parametrize("dt1, dt2, expected",
                              [(None, None, True),
                               (None, 0, True),
                               (None, 1, True),
                               pytest.param(None, True, True,
                                            marks=pytest.mark.xfail(
                                                reason="returns false")),
```

### Comparing `control-0.9.3.post2/control/tests/margin_test.py` & `control-0.9.4/control/tests/margin_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/mateqn_test.py` & `control-0.9.4/control/tests/mateqn_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/matlab2_test.py` & `control-0.9.4/control/tests/matlab2_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/matlab_test.py` & `control-0.9.4/control/tests/matlab_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/minreal_test.py` & `control-0.9.4/control/tests/minreal_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/modelsimp_test.py` & `control-0.9.4/control/tests/modelsimp_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/namedio_test.py` & `control-0.9.4/control/tests/namedio_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,16 +86,18 @@
     [ct.drss, (4, 1, 1), {}],
     [ct.drss, (3, 2, 1), {}],
     [ct.FRD, ([1, 2, 3,], [1, 2, 3]), {}],
     [ct.NonlinearIOSystem,
      (lambda t, x, u, params: -x, None),
      {'inputs': 2, 'outputs':2, 'states':2}],
     [ct.ss, ([[1, 2], [3, 4]], [[0], [1]], [[1, 0]], 0), {}],
+    [ct.ss, ([], [], [], 3), {}], # static system
     [ct.StateSpace, ([[1, 2], [3, 4]], [[0], [1]], [[1, 0]], 0), {}],
     [ct.tf, ([1, 2], [3, 4, 5]), {}],
+    [ct.tf, (2, 3), {}], # static system
     [ct.TransferFunction, ([1, 2], [3, 4, 5]), {}],
 ])
 def test_io_naming(fun, args, kwargs):
     # Reset the ID counter to get uniform generic names
     ct.namedio.NamedIOSystem._idCounter = 0
 
     # Create the system w/out any names
@@ -108,15 +110,15 @@
     if fun in fun_notinstance:
         assert not isinstance(sys_g, fun_notinstance[fun])
 
     # Make sure the names make sense
     assert sys_g.name == 'sys[0]'
     assert sys_g.input_labels == [f'u[{i}]' for i in range(sys_g.ninputs)]
     assert sys_g.output_labels == [f'y[{i}]' for i in range(sys_g.noutputs)]
-    if sys_g.nstates:
+    if sys_g.nstates is not None:
         assert sys_g.state_labels == [f'x[{i}]' for i in range(sys_g.nstates)]
 
     #
     # Reset the names to something else and make sure they stick
     #
     sys_r = copy(sys_g)
 
@@ -124,53 +126,58 @@
     sys_r.set_inputs(input_labels)
     assert sys_r.input_labels == input_labels
 
     output_labels = [f'y{i}' for i in range(sys_g.noutputs)]
     sys_r.set_outputs(output_labels)
     assert sys_r.output_labels == output_labels
 
-    if sys_g.nstates:
+    if sys_g.nstates is not None:
         state_labels = [f'x{i}' for i in range(sys_g.nstates)]
         sys_r.set_states(state_labels)
         assert sys_r.state_labels == state_labels
 
+    sys_r.name = 'sys'          # make sure name is non-generic
+
     #
     # Set names using keywords and make sure they stick
     #
 
     # How the keywords are used depends on the type of system
     if fun in (ct.rss, ct.drss):
         # Pass the labels instead of the numbers
         sys_k = fun(state_labels, output_labels, input_labels, name='mysys')
 
     elif sys_g.nstates is None:
-        # Don't pass state labels
+        # Don't pass state labels if TransferFunction
         sys_k = fun(
             *args, inputs=input_labels, outputs=output_labels, name='mysys')
 
     else:
         sys_k = fun(
             *args, inputs=input_labels, outputs=output_labels,
             states=state_labels, name='mysys')
 
     assert sys_k.name == 'mysys'
     assert sys_k.input_labels == input_labels
     assert sys_k.output_labels == output_labels
-    if sys_g.nstates:
+    if sys_g.nstates is not None:
         assert sys_k.state_labels == state_labels
 
     #
     # Convert the system to state space and make sure labels transfer
     #
     if ct.slycot_check() and not isinstance(
             sys_r, (ct.FrequencyResponseData, ct.NonlinearIOSystem)):
         sys_ss = ct.ss(sys_r)
         assert sys_ss != sys_r
         assert sys_ss.input_labels == input_labels
         assert sys_ss.output_labels == output_labels
+        if not isinstance(sys_r, ct.StateSpace):
+            # System should get unique name
+            assert sys_ss.name != sys_r.name
 
         # Reassign system and signal names
         sys_ss = ct.ss(
             sys_g, inputs=input_labels, outputs=output_labels, name='new')
         assert sys_ss.name == 'new'
         assert sys_ss.input_labels == input_labels
         assert sys_ss.output_labels == output_labels
@@ -189,14 +196,32 @@
         # Reassign system and signal names
         sys_tf = ct.tf(
             sys_g, inputs=input_labels, outputs=output_labels, name='new')
         assert sys_tf.name == 'new'
         assert sys_tf.input_labels == input_labels
         assert sys_tf.output_labels == output_labels
 
+    #
+    # Convert the system to a LinearIOSystem and make sure labels transfer
+    #
+    if not isinstance(
+            sys_r, (ct.FrequencyResponseData, ct.NonlinearIOSystem)) and \
+                    ct.slycot_check():
+        sys_lio = ct.LinearIOSystem(sys_r)
+        assert sys_lio != sys_r
+        assert sys_lio.input_labels == input_labels
+        assert sys_lio.output_labels == output_labels
+
+        # Reassign system and signal names
+        sys_lio = ct.LinearIOSystem(
+            sys_g, inputs=input_labels, outputs=output_labels, name='new')
+        assert sys_lio.name == 'new'
+        assert sys_lio.input_labels == input_labels
+        assert sys_lio.output_labels == output_labels
+
 
 # Internal testing of StateSpace initialization
 def test_init_namedif():
     # Set up the initial system
     sys = ct.rss(2, 1, 1)
 
     # Rename the system, inputs, and outouts
@@ -217,22 +242,37 @@
     # Make sure that passing an unrecognized keyword generates an error
     with pytest.raises(TypeError, match="unrecognized keyword"):
         ct.StateSpace.__init__(
             sys_keep, sys, inputs='u', outputs='y', init_namedio=False)
 
 # Test state space conversion
 def test_convert_to_statespace():
-    # Set up the initial system
-    sys = ct.tf(ct.rss(2, 1, 1))
+    # Set up the initial systems
+    sys = ct.tf(ct.rss(2, 1, 1), inputs='u', outputs='y', name='sys')
+    sys_static = ct.tf(1, 2, inputs='u', outputs='y', name='sys_static')
+
+    # check that name, inputs, and outputs passed through
+    sys_new = ct.ss(sys)
+    assert sys_new.name == 'sys$converted'
+    assert sys_new.input_labels == ['u']
+    assert sys_new.output_labels == ['y']
+    sys_new = ct.ss(sys_static)
+    assert sys_new.name == 'sys_static$converted'
+    assert sys_new.input_labels == ['u']
+    assert sys_new.output_labels == ['y']
 
     # Make sure we can rename system name, inputs, outputs
     sys_new = ct.ss(sys, inputs='u', outputs='y', name='new')
     assert sys_new.name == 'new'
     assert sys_new.input_labels == ['u']
     assert sys_new.output_labels == ['y']
+    sys_new = ct.ss(sys_static, inputs='u', outputs='y', name='new')
+    assert sys_new.name == 'new'
+    assert sys_new.input_labels == ['u']
+    assert sys_new.output_labels == ['y']
 
     # Try specifying the state names (via low level test)
     with pytest.warns(UserWarning, match="non-unique state space realization"):
         sys_new = ct.ss(sys, inputs='u', outputs='y', states=['x1', 'x2'])
         assert sys_new.input_labels == ['u']
         assert sys_new.output_labels == ['y']
         assert sys_new.state_labels == ['x1', 'x2']
```

### Comparing `control-0.9.3.post2/control/tests/nichols_test.py` & `control-0.9.4/control/tests/nichols_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/nyquist_test.py` & `control-0.9.4/control/tests/nyquist_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,16 +366,31 @@
 
     with pytest.warns(UserWarning, match="indented contour may miss"):
         count = ct.nyquist_plot(sys)
 
 def test_discrete_nyquist():
     # Make sure we can handle discrete time systems with negative poles
     sys = ct.tf(1, [1, -0.1], dt=1) * ct.tf(1, [1, 0.1], dt=1)
-    ct.nyquist_plot(sys)
-    
+    ct.nyquist_plot(sys, plot=False)
+
+    # system with a pole at the origin
+    sys = ct.zpk([1,], [.3, 0], 1, dt=True)
+    ct.nyquist_plot(sys, plot=False)
+    sys = ct.zpk([1,], [0], 1, dt=True)
+    ct.nyquist_plot(sys, plot=False)
+
+    # only a pole at the origin
+    sys = ct.zpk([], [0], 2, dt=True)
+    ct.nyquist_plot(sys, plot=False)
+
+    # pole at zero (pure delay)
+    sys = ct.zpk([], [1], 1, dt=True)
+    ct.nyquist_plot(sys, plot=False)
+
+
 if __name__ == "__main__":
     #
     # Interactive mode: generate plots for manual viewing
     #
     # Running this script in python (or better ipython) will show a
     # collection of figures that should all look OK on the screeen.
     #
@@ -423,9 +438,9 @@
     print("Discrete time systems")
     sys = ct.c2d(sys, 0.01)
     plt.figure()
     plt.title("Discrete-time; poles: %s" %
               np.array2string(sys.poles(), precision=2, separator=','))
     count = ct.nyquist_plot(sys)
 
-    
+
```

### Comparing `control-0.9.3.post2/control/tests/optimal_test.py` & `control-0.9.4/control/tests/optimal_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         sys, time, x0, integral_cost, trajectory_constraints,
         terminal_cost=terminal_cost, initial_guess=lqr_u)
 
     # Make sure we got a different solution
     assert np.any(np.abs(res1.inputs - res2.inputs) > 0.1)
 
 
+@pytest.mark.slow
 def test_mpc_iosystem_aircraft():
     # model of an aircraft discretized with 0.2s sampling time
     # Source: https://www.mpt3.org/UI/RegulationProblem
     A = [[0.99, 0.01, 0.18, -0.09,   0],
          [   0, 0.94,    0,  0.29,   0],
          [   0, 0.14, 0.81,  -0.9,   0],
          [   0, -0.2,    0,  0.95,   0],
@@ -210,14 +211,43 @@
         loop, np.arange(0, Nsim) * 0.2, 0, X0)
 
     # Make sure the system converged to the desired state
     np.testing.assert_allclose(
         xout[0:sys.nstates, -1], xd, atol=0.1, rtol=0.01)
 
 
+def test_mpc_iosystem_rename():
+    # Create a discrete time system (double integrator) + cost function
+    sys = ct.ss([[1, 1], [0, 1]], [[0], [1]], np.eye(2), 0, dt=True)
+    cost = opt.quadratic_cost(sys, np.eye(2), np.eye(1))
+    timepts = np.arange(0, 5)
+
+    # Create the default optimal control problem and check labels
+    mpc = opt.create_mpc_iosystem(sys, timepts, cost)
+    assert mpc.input_labels == sys.state_labels
+    assert mpc.output_labels == sys.input_labels
+
+    # Change the signal names
+    input_relabels = ['x1', 'x2']
+    output_relabels = ['u']
+    state_relabels = [f'x_[{i}]' for i in timepts]
+    mpc_relabeled = opt.create_mpc_iosystem(
+        sys, timepts, cost, inputs=input_relabels, outputs=output_relabels,
+        states=state_relabels, name='mpc_relabeled')
+    assert mpc_relabeled.input_labels == input_relabels
+    assert mpc_relabeled.output_labels == output_relabels
+    assert mpc_relabeled.state_labels == state_relabels
+    assert mpc_relabeled.name == 'mpc_relabeled'
+
+    # Make sure that unknown keywords are caught
+    # Unrecognized arguments
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        mpc = opt.create_mpc_iosystem(sys, timepts, cost, unknown=None)
+
+
 def test_mpc_iosystem_continuous():
     # Create a random state space system
     sys = ct.rss(2, 1, 1)
     T, _ = ct.step_response(sys)
 
     # provide penalties on the system signals
     Q = np.eye(sys.nstates)
@@ -488,14 +518,22 @@
             sys, time, x0, cost, constraints, initial_guess=np.zeros((4,1,1)))
 
     # Unrecognized arguments
     with pytest.raises(TypeError, match="unrecognized keyword"):
         res = opt.solve_ocp(
             sys, time, x0, cost, constraints, terminal_constraint=None)
 
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        ocp = opt.OptimalControlProblem(
+            sys, time, x0, cost, constraints, terminal_constraint=None)
+
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        ocp = opt.OptimalControlProblem(sys, time, cost, constraints)
+        ocp.compute_trajectory(x0, unknown=None)
+
     # Unrecognized trajectory constraint type
     constraints = [(None, np.eye(3), [0, 0, 0], [0, 0, 0])]
     with pytest.raises(TypeError, match="unknown trajectory constraint type"):
         res = opt.solve_ocp(
             sys, time, x0, cost, trajectory_constraints=constraints)
 
     # Unrecognized terminal constraint type
@@ -509,14 +547,15 @@
         res = opt.solve_ocp(
             sys, time, x0, cost, solve_ivp_method='LSODA')
     with pytest.raises(TypeError, match="solve_ivp method, kwargs not allowed"):
         res = opt.solve_ocp(
             sys, time, x0, cost, solve_ivp_kwargs={'eps': 0.1})
 
 
+@pytest.mark.slow
 @pytest.mark.parametrize("basis", [
     flat.PolyFamily(4), flat.PolyFamily(6),
     flat.BezierFamily(4), flat.BSplineFamily([0, 4, 8], 6)
     ])
 def test_optimal_basis_simple(basis):
     sys = ct.ss([[1, 1], [0, 1]], [[1], [0.5]], np.eye(2), 0, 1)
 
@@ -611,14 +650,15 @@
     final_point = [(None, final_point_eval, [0, 0], [0, 0])]
     with pytest.raises(TypeError, match="unknown terminal constraint type"):
         optctrl = opt.OptimalControlProblem(
             sys, time, cost, terminal_constraints=final_point)
         res = optctrl.compute_trajectory(x0, squeeze=True, return_x=True)
 
 
+@pytest.mark.slow
 @pytest.mark.parametrize(
     "method, npts, initial_guess, fail", [
         ('shooting', 3, None, 'xfail'),         # doesn't converge
         ('shooting', 3, 'zero', 'xfail'),       # doesn't converge
         ('shooting', 3, 'u0', None),            # github issue #782
         ('shooting', 3, 'input', 'endpoint'),   # doesn't converge to optimal
         ('shooting', 5, 'input', 'endpoint'),   # doesn't converge to optimal
@@ -728,7 +768,32 @@
                 t_eval=np.linspace(0, Tf, 10))
             t, y = resp
             if fail == 'openloop':
                 with pytest.raises(AssertionError):
                     np.testing.assert_almost_equal(y[:,-1], xf, decimal=1)
             else:
                 np.testing.assert_almost_equal(y[:,-1], xf, decimal=1)
+
+
+def test_oep_argument_errors():
+    sys = ct.rss(4, 2, 2)
+    timepts = np.linspace(0, 1, 10)
+    Y = np.zeros((2, timepts.size))
+    U = np.zeros_like(timepts)
+    cost = opt.gaussian_likelihood_cost(sys, np.eye(1), np.eye(2))
+
+    # Unrecognized arguments
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        res = opt.solve_oep(sys, timepts, Y, U, cost, unknown=True)
+
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        oep = opt.OptimalEstimationProblem(sys, timepts, cost, unknown=True)
+
+    with pytest.raises(TypeError, match="unrecognized keyword"):
+        sys = ct.rss(4, 2, 2, dt=True)
+        oep = opt.OptimalEstimationProblem(sys, timepts, cost)
+        oep.create_mhe_iosystem(unknown=True)
+
+    # Incorrect number of signals
+    with pytest.raises(ValueError, match="incorrect length"):
+        oep = opt.OptimalEstimationProblem(sys, timepts, cost)
+        mhe = oep.create_mhe_iosystem(estimate_labels=['x1', 'x2', 'x3'])
```

### Comparing `control-0.9.3.post2/control/tests/passivity_test.py` & `control-0.9.4/control/tests/passivity_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/phaseplot_test.py` & `control-0.9.4/control/tests/phaseplot_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/pzmap_test.py` & `control-0.9.4/control/tests/pzmap_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/rlocus_test.py` & `control-0.9.4/control/tests/rlocus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         np.testing.assert_allclose(klist, k_out)
         self.check_cl_poles(sys, roots, klist)
 
     def test_without_gains(self, sys):
         roots, kvect = root_locus(sys, plot=False)
         self.check_cl_poles(sys, roots, kvect)
 
+    @pytest.mark.slow
     @pytest.mark.parametrize('grid', [None, True, False])
     def test_root_locus_plot_grid(self, sys, grid):
         rlist, klist = root_locus(sys, grid=grid)
         ax = plt.gca()
         n_gridlines = sum([int(line.get_linestyle() in [':', 'dotted',
                                                         '--', 'dashed'])
                            for line in ax.lines])
```

### Comparing `control-0.9.3.post2/control/tests/robust_test.py` & `control-0.9.4/control/tests/robust_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/sisotool_test.py` & `control-0.9.4/control/tests/sisotool_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,20 @@
             'omega_limits': None,
             'omega_num': None,
             'sisotool': True,
             'fig': fig,
             'margins': True
         }
 
+        # Check that the xaxes of the bode plot are shared before the rlocus click
+        assert ax_mag.get_xlim() == ax_phase.get_xlim()
+        ax_mag.set_xlim(2, 12)
+        assert ax_mag.get_xlim() == (2, 12)
+        assert ax_phase.get_xlim() == (2, 12)
+
         # Move the rootlocus to another point
         event = type('test', (object,), {'xdata': 2.31206868287,
                                          'ydata': 15.5983051046,
                                          'inaxes': ax_rlocus.axes})()
         _RLClickDispatcher(event=event, sys=tsys, fig=fig,
                            ax_rlocus=ax_rlocus, sisotool=True, plotstr='-',
                            bode_plot_params=bode_plot_params, tvect=None)
@@ -112,14 +118,20 @@
         # Check if the step response has changed
         step_response_moved = np.array(
             [0.    , 0.0237, 0.1596, 0.4511, 0.884 , 1.3985, 1.9031, 2.2922,
              2.4676, 2.3606])
         assert_array_almost_equal(
             ax_step.lines[0].get_data()[1][:10], step_response_moved, 4)
 
+        # Check that the xaxes of the bode plot are still shared after the rlocus click
+        assert ax_mag.get_xlim() == ax_phase.get_xlim()
+        ax_mag.set_xlim(3, 13)
+        assert ax_mag.get_xlim() == (3, 13)
+        assert ax_phase.get_xlim() == (3, 13)
+
     @pytest.mark.skipif(plt.get_current_fig_manager().toolbar is None,
                         reason="Requires the zoom toolbar")
     @pytest.mark.parametrize('tsys', [0, True],
                              indirect=True, ids=['ctime', 'dtime'])
     def test_sisotool_tvect(self, tsys):
         # test supply tvect
         tvect = np.linspace(0, 1, 10)
@@ -166,26 +178,27 @@
     @pytest.mark.parametrize('plant', ('syscont', 'sysdisc1', 'syscont221'), indirect=True)
     @pytest.mark.parametrize('gain', ('P', 'I', 'D'))
     @pytest.mark.parametrize('sign', (1,))
     @pytest.mark.parametrize('input_signal', ('r', 'd'))
     @pytest.mark.parametrize('Kp0', (0,))
     @pytest.mark.parametrize('Ki0', (1.,))
     @pytest.mark.parametrize('Kd0', (0.1,))
+    @pytest.mark.parametrize('deltaK', (1.,))
     @pytest.mark.parametrize('tau', (0.01,))
     @pytest.mark.parametrize('C_ff', (0, 1,))
     @pytest.mark.parametrize('derivative_in_feedback_path', (True, False,))
     @pytest.mark.parametrize("kwargs", [{'plot':False},])
-    def test_pid_designer_1(self, plant, gain, sign, input_signal, Kp0, Ki0, Kd0, tau, C_ff,
+    def test_pid_designer_1(self, plant, gain, sign, input_signal, Kp0, Ki0, Kd0, deltaK, tau, C_ff,
             derivative_in_feedback_path, kwargs):
-        rootlocus_pid_designer(plant, gain, sign, input_signal, Kp0, Ki0, Kd0, tau, C_ff,
+        rootlocus_pid_designer(plant, gain, sign, input_signal, Kp0, Ki0, Kd0, deltaK, tau, C_ff,
             derivative_in_feedback_path, **kwargs)
 
     # test creation of sisotool plot
     # input from reference or disturbance
-    @pytest.mark.skip("Bode plot is incorrect; generates spurious warnings")
     @pytest.mark.parametrize('plant', ('syscont', 'syscont221'), indirect=True)
     @pytest.mark.parametrize("kwargs", [
         {'input_signal':'r', 'Kp0':0.01, 'derivative_in_feedback_path':True},
-        {'input_signal':'d', 'Kp0':0.01, 'derivative_in_feedback_path':True},])
+        {'input_signal':'d', 'Kp0':0.01, 'derivative_in_feedback_path':True},
+        {'input_signal':'r', 'Kd0':0.01, 'derivative_in_feedback_path':True}])
     def test_pid_designer_2(self, plant, kwargs):
         rootlocus_pid_designer(plant, **kwargs)
```

### Comparing `control-0.9.3.post2/control/tests/slycot_convert_test.py` & `control-0.9.4/control/tests/slycot_convert_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/statefbk_test.py` & `control-0.9.4/control/tests/statefbk_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 RMM, 30 Mar 2011 (based on TestStatefbk from v0.4a)
 """
 
 import numpy as np
 import pytest
 import itertools
+import warnings
 from math import pi, atan
 
 import control as ct
 from control import lqe, dlqe, poles, rss, ss, tf
 from control.exception import ControlDimension, ControlSlycot, \
     ControlArgument, slycot_check
 from control.mateqn import care, dare
@@ -507,28 +508,28 @@
         np.testing.assert_almost_equal(E_asys, E_expl)
 
         # Calling dlqr() with a continuous time system should raise an error
         with pytest.raises(ControlArgument, match="dsys must be discrete"):
             K, S, E = ct.dlqr(csys, Q, R)
 
     @pytest.mark.parametrize(
-        'nstates, noutputs, ninputs, nintegrators, type',
+        'nstates, noutputs, ninputs, nintegrators, type_',
         [(2,      0,        1,       0,            None),
          (2,      1,        1,       0,            None),
          (4,      0,        2,       0,            None),
          (4,      3,        2,       0,            None),
          (2,      0,        1,       1,            None),
          (4,      0,        2,       2,            None),
          (4,      3,        2,       2,            None),
          (2,      0,        1,       0,            'nonlinear'),
          (4,      0,        2,       2,            'nonlinear'),
          (4,      3,        2,       2,            'nonlinear'),
         ])
     def test_statefbk_iosys(
-            self, nstates, ninputs, noutputs, nintegrators, type):
+            self, nstates, ninputs, noutputs, nintegrators, type_):
         # Create the system to be controlled (and estimator)
         # TODO: make sure it is controllable?
         if noutputs == 0:
             # Create a system with full state output
             sys = ct.rss(nstates, nstates, ninputs, strictly_proper=True)
             sys.C = np.eye(nstates)
             est = None
@@ -565,18 +566,23 @@
 
         # Design an LQR controller
         K, _, _ = ct.lqr(aug, np.eye(nstates + nintegrators), np.eye(ninputs))
         Kp, Ki = K[:, :nstates], K[:, nstates:]
 
         # Create an I/O system for the controller
         ctrl, clsys = ct.create_statefbk_iosystem(
-            sys, K, integral_action=C_int, estimator=est, type=type)
+            sys, K, integral_action=C_int, estimator=est,
+            controller_type=type_, name=type_)
+
+        # Make sure the name got set correctly
+        if type_ is not None:
+            assert ctrl.name == type_
 
         # If we used a nonlinear controller, linearize it for testing
-        if type == 'nonlinear':
+        if type_ == 'nonlinear':
             clsys = clsys.linearize(0, 0)
 
         # Make sure the linear system elements are correct
         if noutputs == 0:
             # No estimator
             Ac = np.block([
                 [sys.A - sys.B @ Kp, -sys.B @ Ki],
@@ -618,14 +624,62 @@
 
         # Check to make sure everything matches
         np.testing.assert_array_almost_equal(clsys.A, Ac)
         np.testing.assert_array_almost_equal(clsys.B, Bc)
         np.testing.assert_array_almost_equal(clsys.C, Cc)
         np.testing.assert_array_almost_equal(clsys.D, Dc)
 
+    def test_statefbk_iosys_unused(self):
+        # Create a base system to work with
+        sys = ct.rss(2, 1, 1, strictly_proper=True)
+
+        # Create a system with extra input
+        aug = ct.rss(2, inputs=[sys.input_labels[0], 'd'],
+                     outputs=sys.output_labels, strictly_proper=True,)
+        aug.A = sys.A
+        aug.B[:, 0:1] = sys.B
+
+        # Create an estimator
+        est = ct.create_estimator_iosystem(
+            sys, np.eye(sys.ninputs), np.eye(sys.noutputs))
+
+        # Design an LQR controller
+        K, _, _ = ct.lqr(sys, np.eye(sys.nstates), np.eye(sys.ninputs))
+
+        # Create a baseline I/O control system
+        ctrl0, clsys0 = ct.create_statefbk_iosystem(sys, K, estimator=est)
+        clsys0_lin = clsys0.linearize(0, 0)
+
+        # Create an I/O system with additional inputs
+        ctrl1, clsys1 = ct.create_statefbk_iosystem(
+            aug, K, estimator=est, control_indices=[0])
+        clsys1_lin = clsys1.linearize(0, 0)
+
+        # Make sure the extra inputs are there
+        assert aug.input_labels[1] not in clsys0.input_labels
+        assert aug.input_labels[1] in clsys1.input_labels
+        np.testing.assert_allclose(clsys0_lin.A, clsys1_lin.A)
+
+        # Switch around which input we use
+        aug = ct.rss(2, inputs=['d', sys.input_labels[0]],
+                     outputs=sys.output_labels, strictly_proper=True,)
+        aug.A = sys.A
+        aug.B[:, 1:2] = sys.B
+
+        # Create an I/O system with additional inputs
+        ctrl2, clsys2 = ct.create_statefbk_iosystem(
+            aug, K, estimator=est, control_indices=[1])
+        clsys2_lin = clsys2.linearize(0, 0)
+
+        # Make sure the extra inputs are there
+        assert aug.input_labels[0] not in clsys0.input_labels
+        assert aug.input_labels[0] in clsys1.input_labels
+        np.testing.assert_allclose(clsys0_lin.A, clsys2_lin.A)
+
+
     def test_lqr_integral_continuous(self):
         # Generate a continuous time system for testing
         sys = ct.rss(4, 4, 2, strictly_proper=True)
         sys.C = np.eye(4)       # reset output to be full state
         C_int = np.eye(2, 4)    # integrate outputs for first two states
         nintegrators = C_int.shape[0]
 
@@ -744,31 +798,51 @@
                 sys, np.eye(sys.nstates), np.eye(sys.ninputs),
                 integrator=None)
 
     def test_statefbk_errors(self):
         sys = ct.rss(4, 4, 2, strictly_proper=True)
         K, _, _ = ct.lqr(sys, np.eye(sys.nstates), np.eye(sys.ninputs))
 
+        with pytest.warns(UserWarning, match="cannot verify system output"):
+            ctrl, clsys = ct.create_statefbk_iosystem(sys, K)
+
+        # reset the system output
+        sys.C = np.eye(sys.nstates)
+
         with pytest.raises(ControlArgument, match="must be I/O system"):
             sys_tf = ct.tf([1], [1, 1])
             ctrl, clsys = ct.create_statefbk_iosystem(sys_tf, K)
 
-        with pytest.raises(ControlArgument, match="output size must match"):
+        with pytest.raises(ControlArgument,
+                           match="estimator output must include the full"):
             est = ct.rss(3, 3, 2)
             ctrl, clsys = ct.create_statefbk_iosystem(sys, K, estimator=est)
 
-        with pytest.raises(ControlArgument, match="must be the full state"):
+        with pytest.raises(ControlArgument,
+                           match="system output must include the full state"):
             sys_nf = ct.rss(4, 3, 2, strictly_proper=True)
             ctrl, clsys = ct.create_statefbk_iosystem(sys_nf, K)
 
         with pytest.raises(ControlArgument, match="gain must be an array"):
             ctrl, clsys = ct.create_statefbk_iosystem(sys, "bad argument")
 
-        with pytest.raises(ControlArgument, match="unknown type"):
-            ctrl, clsys = ct.create_statefbk_iosystem(sys, K, type=1)
+        with pytest.warns(DeprecationWarning, match="'type' is deprecated"):
+            ctrl, clsys = ct.create_statefbk_iosystem(sys, K, type='nonlinear')
+
+        with pytest.raises(ControlArgument, match="duplicate keywords"):
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                ctrl, clsys = ct.create_statefbk_iosystem(
+                    sys, K, type='nonlinear', controller_type='nonlinear')
+
+        with pytest.raises(TypeError, match="unrecognized keyword"):
+            ctrl, clsys = ct.create_statefbk_iosystem(sys, K, typo='nonlinear')
+
+        with pytest.raises(ControlArgument, match="unknown controller_type"):
+            ctrl, clsys = ct.create_statefbk_iosystem(sys, K, controller_type=1)
 
         # Errors involving integral action
         C_int = np.eye(2, 4)
         K_int, _, _ = ct.lqr(
             sys, np.eye(sys.nstates + C_int.shape[0]), np.eye(sys.ninputs),
             integral_action=C_int)
 
@@ -784,19 +858,16 @@
 # Kinematic car example for testing gain scheduling
 @pytest.fixture
 def unicycle():
     # Create a simple nonlinear system to check (kinematic car)
     def unicycle_update(t, x, u, params):
         return np.array([np.cos(x[2]) * u[0], np.sin(x[2]) * u[0], u[1]])
 
-    def unicycle_output(t, x, u, params):
-        return x
-
     return ct.NonlinearIOSystem(
-        unicycle_update, unicycle_output,
+        unicycle_update, None,
         inputs = ['v', 'phi'],
         outputs = ['x', 'y', 'theta'],
         states = ['x_', 'y_', 'theta_'])
 
 from math import pi
 
 @pytest.mark.parametrize("method", ['nearest', 'linear', 'cubic'])
@@ -902,28 +973,56 @@
 
     # Run a simulation following a curved path
     resp = ct.input_output_response(clsys, timepts, [Xd, Ud], X0)
     np.testing.assert_allclose(
         resp.states[:, -1], Xd[:, -1], atol=1e-2, rtol=1e-2)
 
 
+@pytest.mark.parametrize("method", ['nearest', 'linear', 'cubic'])
+def test_gainsched_1d(method):
+    # Define a linear system to test
+    sys = ct.ss([[-1, 0.1], [0, -2]], [[0], [1]], np.eye(2), 0)
+
+    # Define gains for the first state only
+    points = [-1, 0, 1]
+
+    # Define gain to be constant
+    K, _, _ = ct.lqr(sys, np.eye(sys.nstates), np.eye(sys.ninputs))
+    gains = [K for p in points]
+
+    # Define the paramters for the simulations
+    timepts = np.linspace(0, 10, 100)
+    X0 = np.ones(sys.nstates) * 1.1     # Start outside defined range
+
+    # Create a controller and simulate the initial response
+    gs_ctrl, gs_clsys = ct.create_statefbk_iosystem(
+        sys, (gains, points), gainsched_indices=[0])
+    gs_resp = ct.input_output_response(gs_clsys, timepts, 0, X0)
+
+    # Verify that we get the same result as a constant gain
+    ck_clsys = ct.ss(sys.A - sys.B @ K, sys.B, sys.C, 0)
+    ck_resp = ct.input_output_response(ck_clsys, timepts, 0, X0)
+
+    np.testing.assert_allclose(gs_resp.states, ck_resp.states)
+
+
 def test_gainsched_default_indices():
     # Define a linear system to test
     sys = ct.ss([[-1, 0.1], [0, -2]], [[0], [1]], np.eye(2), 0)
 
     # Define gains at origin + corners of unit cube
     points = [[0, 0]] + list(itertools.product([-1, 1], [-1, 1]))
 
     # Define gain to be constant
     K, _, _ = ct.lqr(sys, np.eye(sys.nstates), np.eye(sys.ninputs))
     gains = [K for p in points]
 
     # Define the paramters for the simulations
     timepts = np.linspace(0, 10, 100)
-    X0 = np.ones(sys.nstates) * 0.9
+    X0 = np.ones(sys.nstates) * 1.1     # Start outside defined range
 
     # Create a controller and simulate the initial response
     gs_ctrl, gs_clsys = ct.create_statefbk_iosystem(sys, (gains, points))
     gs_resp = ct.input_output_response(gs_clsys, timepts, 0, X0)
 
     # Verify that we get the same result as a constant gain
     ck_clsys = ct.ss(sys.A - sys.B @ K, sys.B, sys.C, 0)
```

### Comparing `control-0.9.3.post2/control/tests/statesp_test.py` & `control-0.9.4/control/tests/statesp_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/timebase_test.py` & `control-0.9.4/control/tests/timebase_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/timeresp_test.py` & `control-0.9.4/control/tests/timeresp_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/trdata_test.py` & `control-0.9.4/control/tests/trdata_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,23 +192,28 @@
     t, y = response_mimo()
     t, y, x = response_mimo(return_x=True)
     with pytest.raises(ValueError, match="too many"):
         t, y = response_mimo(return_x=True)
     with pytest.raises(ValueError, match="not enough"):
         t, y, x = response_mimo
 
-    # Labels
-    assert response_mimo.output_labels is None
-    assert response_mimo.state_labels is None
-    assert response_mimo.input_labels is None
+    # Make sure labels are transferred to the response
+    assert response_siso.output_labels == sys_siso.output_labels
+    assert response_siso.state_labels == sys_siso.state_labels
+    assert response_siso.input_labels == sys_siso.input_labels
+    assert response_mimo.output_labels == sys_mimo.output_labels
+    assert response_mimo.state_labels == sys_mimo.state_labels
+    assert response_mimo.input_labels == sys_mimo.input_labels
+
+    # Check relabelling
     response = response_mimo(
         output_labels=['y1', 'y2'], input_labels='u',
-        state_labels=["x[%d]" % i for i in range(4)])
+        state_labels=["x%d" % i for i in range(4)])
     assert response.output_labels == ['y1', 'y2']
-    assert response.state_labels == ['x[0]', 'x[1]', 'x[2]', 'x[3]']
+    assert response.state_labels == ['x0', 'x1', 'x2', 'x3']
     assert response.input_labels == ['u']
 
     # Unknown keyword
     with pytest.raises(TypeError, match="unrecognized keywords"):
         response_bad_kw = response_mimo(input=0)
 
 
@@ -227,14 +232,25 @@
     np.testing.assert_equal(
         response.output_labels, ["y[%d]" % i for i in range(sys.noutputs)])
     np.testing.assert_equal(
         response.state_labels, ["x[%d]" % i for i in range(sys.nstates)])
     np.testing.assert_equal(
         response.input_labels, ["u[%d]" % i for i in range(sys.ninputs)])
 
+    # Make sure the selected input and output are both correctly transferred to the response
+    for nu in range(sys.ninputs):
+        for ny in range(sys.noutputs):
+            step_response = ct.step_response(sys, T, input=nu, output=ny)
+            assert step_response.input_labels == [sys.input_labels[nu]]
+            assert step_response.output_labels == [sys.output_labels[ny]]
+
+            init_response = ct.initial_response(sys, T, input=nu, output=ny)
+            assert init_response.input_labels == None
+            assert init_response.output_labels == [sys.output_labels[ny]]
+
 
 def test_trdata_multitrace():
     #
     # Output signal processing
     #
 
     # Proper call of multi-trace data w/ ambiguous 2D output
```

### Comparing `control-0.9.3.post2/control/tests/type_conversion_test.py` & `control-0.9.4/control/tests/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/xferfcn_input_test.py` & `control-0.9.4/control/tests/xferfcn_input_test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/control/tests/xferfcn_test.py` & `control-0.9.4/control/tests/xferfcn_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 import numpy as np
 import pytest
 import operator
 
 import control as ct
 from control import StateSpace, TransferFunction, rss, evalfr
-from control import ss, ss2tf, tf, tf2ss
-from control import isctime, isdtime, sample_system, defaults
+from control import ss, ss2tf, tf, tf2ss, zpk
+from control import isctime, isdtime, sample_system
+from control import defaults, reset_defaults, set_defaults
 from control.statesp import _convert_to_statespace
 from control.xferfcn import _convert_to_transfer_function
 from control.tests.conftest import slycotonly, matrixfilter
 
 
 class TestXferFcn:
     """Test functionality and correct reporting of the transfer function class.
@@ -902,14 +903,136 @@
     @slycotonly
     def test_printing_mimo(self):
         """Print MIMO, continuous time"""
         sys = ss2tf(rss(4, 2, 3))
         assert isinstance(str(sys), str)
         assert isinstance(sys._repr_latex_(), str)
 
+    @pytest.mark.parametrize(
+        "zeros, poles, gain, output",
+        [([0], [-1], 1,
+          '\n'
+          '  s\n'
+          '-----\n'
+          's + 1\n'),
+         ([-1], [-1], 1,
+          '\n'
+          's + 1\n'
+          '-----\n'
+          's + 1\n'),
+         ([-1], [1], 1,
+          '\n'
+          's + 1\n'
+          '-----\n'
+          's - 1\n'),
+         ([1], [-1], 1,
+          '\n'
+          's - 1\n'
+          '-----\n'
+          's + 1\n'),
+         ([-1], [-1], 2,
+          '\n'
+          '2 (s + 1)\n'
+          '---------\n'
+          '  s + 1\n'),
+         ([-1], [-1], 0,
+          '\n'
+          '0\n'
+          '-\n'
+          '1\n'),
+         ([-1], [1j, -1j], 1,
+          '\n'
+          '      s + 1\n'
+          '-----------------\n'
+          '(s - 1j) (s + 1j)\n'),
+         ([4j, -4j], [2j, -2j], 2,
+          '\n'
+          '2 (s - 4j) (s + 4j)\n'
+          '-------------------\n'
+          ' (s - 2j) (s + 2j)\n'),
+         ([1j, -1j], [-1, -4], 2,
+          '\n'
+          '2 (s - 1j) (s + 1j)\n'
+          '-------------------\n'
+          '  (s + 1) (s + 4)\n'),
+         ([1], [-1 + 1j, -1 - 1j], 1,
+          '\n'
+          '          s - 1\n'
+          '-------------------------\n'
+          '(s + (1-1j)) (s + (1+1j))\n'),
+         ([1], [1 + 1j, 1 - 1j], 1,
+          '\n'
+          '          s - 1\n'
+          '-------------------------\n'
+          '(s - (1+1j)) (s - (1-1j))\n'),
+         ])
+    def test_printing_zpk(self, zeros, poles, gain, output):
+        """Test _tf_polynomial_to_string for constant systems"""
+        G = zpk(zeros, poles, gain, display_format='zpk')
+        res = str(G)
+        assert res == output
+
+    @pytest.mark.parametrize(
+        "zeros, poles, gain, format, output",
+        [([1], [1 + 1j, 1 - 1j], 1, ".2f",
+          '\n'
+          '                1.00\n'
+          '-------------------------------------\n'
+          '(s + (1.00-1.41j)) (s + (1.00+1.41j))\n'),
+         ([1], [1 + 1j, 1 - 1j], 1, ".3f",
+          '\n'
+           '                  1.000\n'
+           '-----------------------------------------\n'
+           '(s + (1.000-1.414j)) (s + (1.000+1.414j))\n'),
+         ([1], [1 + 1j, 1 - 1j], 1, ".6g",
+          '\n'
+          '                  1\n'
+          '-------------------------------------\n'
+          '(s + (1-1.41421j)) (s + (1+1.41421j))\n')
+         ])
+    def test_printing_zpk_format(self, zeros, poles, gain, format, output):
+        """Test _tf_polynomial_to_string for constant systems"""
+        G = tf([1], [1,2,3], display_format='zpk')
+
+        set_defaults('xferfcn', floating_point_format=format)
+        res = str(G)
+        reset_defaults()
+
+        assert res == output
+
+    @pytest.mark.parametrize(
+        "num, den, output",
+        [([[[11], [21]], [[12], [22]]],
+         [[[1, -3, 2], [1, 1, -6]], [[1, 0, 1], [1, -1, -20]]],
+         ('\n'
+          'Input 1 to output 1:\n'
+          '      11\n'
+          '---------------\n'
+          '(s - 2) (s - 1)\n'
+          '\n'
+          'Input 1 to output 2:\n'
+          '       12\n'
+          '-----------------\n'
+          '(s - 1j) (s + 1j)\n'
+          '\n'
+          'Input 2 to output 1:\n'
+          '      21\n'
+          '---------------\n'
+          '(s - 2) (s + 3)\n'
+          '\n'
+          'Input 2 to output 2:\n'
+          '      22\n'
+          '---------------\n'
+          '(s - 5) (s + 4)\n'))])
+    def test_printing_zpk_mimo(self, num, den, output):
+        """Test _tf_polynomial_to_string for constant systems"""
+        G = tf(num, den, display_format='zpk')
+        res = str(G)
+        assert res == output
+
     @slycotonly
     def test_size_mismatch(self):
         """Test size mismacht"""
         sys1 = ss2tf(rss(2, 2, 2))
 
         # Different number of inputs
         sys2 = ss2tf(rss(3, 1, 2))
@@ -1127,19 +1250,25 @@
     (TransferFunction, ([1], [1, 1]), dict(inputs='i', outputs='o'), tf2ss),
     (TransferFunction, ([1], [1, 1]), dict(inputs=1, outputs=1), tf2ss),
     (TransferFunction, ([1], [1, 1]), dict(inputs='i', outputs='o'), tf),
     (TransferFunction, ([1], [1, 1]), dict(inputs='i', outputs='o'), ss),
 ])
 def test_copy_names(create, args, kwargs, convert):
     # Convert a system with no renaming
-    sys = create(*args, **kwargs)
+    sys = create(*args, **kwargs, name='sys')
     cpy = convert(sys)
 
     assert cpy.input_labels == sys.input_labels
     assert cpy.input_labels == sys.input_labels
     if cpy.nstates is not None and sys.nstates is not None:
         assert cpy.state_labels == sys.state_labels
 
+    # Make sure that names aren't the same if system changed type
+    if not isinstance(cpy, create):
+        assert cpy.name == sys.name + '$converted'
+    else:
+        assert cpy.name == sys.name
+
     # Relabel inputs and outputs
     cpy = convert(sys, inputs='myin', outputs='myout')
     assert cpy.input_labels == ['myin']
     assert cpy.output_labels == ['myout']
```

### Comparing `control-0.9.3.post2/control/timeresp.py` & `control-0.9.4/control/timeresp.py`

 * *Files 3% similar despite different names*

```diff
@@ -690,15 +690,18 @@
         try:
             # Turn into a list
             labels = [ivd[n] for n in range(len(labels))]
         except KeyError:
             raise ValueError("Name dictionary for %s is incomplete" % signal)
 
     # Convert labels to a list
-    labels = list(labels)
+    if isinstance(labels, str):
+        labels = [labels]
+    else:
+        labels = list(labels)
 
     # Make sure the signal list is the right length and type
     if len(labels) != length:
         raise ValueError("List of %s labels is the wrong length" % signal)
     elif not all([isinstance(label, str) for label in labels]):
         raise ValueError("List of %s labels must all  be strings" % signal)
 
@@ -813,15 +816,15 @@
 
     return out_array
 
 
 # Forced response of a linear system
 def forced_response(sys, T=None, U=0., X0=0., transpose=False,
                     interpolate=False, return_x=None, squeeze=None):
-    """Simulate the output of a linear system.
+    """Compute the output of a linear system given the input.
 
     As a convenience for parameters `U`, `X0`:
     Numbers (scalars) are converted to constant arrays with the correct shape.
     The correct shape is inferred from arguments `sys` and `T`.
 
     For information on the **shape** of parameters `U`, `T`, `X0` and
     return values `T`, `yout`, `xout`, see :ref:`time-series-convention`.
@@ -912,15 +915,17 @@
 
     For continuous time systems, the output is computed using the matrix
     exponential `exp(A t)` and assuming linear interpolation of the inputs
     between time points.
 
     Examples
     --------
-    >>> T, yout, xout = forced_response(sys, T, u, X0)
+    >>> G = ct.rss(4)
+    >>> T = np.linspace(0, 10)
+    >>> T, yout = ct.forced_response(G, T=T)
 
     See :ref:`time-series-convention` and
     :ref:`package-configuration-parameters`.
 
     """
     if not isinstance(sys, (StateSpace, TransferFunction)):
         raise TypeError('Parameter ``sys``: must be a ``StateSpace`` or'
@@ -1105,14 +1110,16 @@
 
         # Transpose the output and state vectors to match local convention
         xout = np.transpose(xout)
         yout = np.transpose(yout)
 
     return TimeResponseData(
         tout, yout, xout, U, issiso=sys.issiso(),
+        output_labels=sys.output_labels, input_labels=sys.input_labels,
+        state_labels=sys.state_labels,
         transpose=transpose, return_x=return_x, squeeze=squeeze)
 
 
 # Process time responses in a uniform way
 def _process_time_response(
         tout, yout, issiso=False, transpose=None, squeeze=None):
     """Process time response signals.
@@ -1324,15 +1331,16 @@
     Notes
     -----
     This function uses the `forced_response` function with the input set to a
     unit step.
 
     Examples
     --------
-    >>> T, yout = step_response(sys, T, X0)
+    >>> G = ct.rss(4)
+    >>> T, yout = ct.step_response(G)
 
     """
     # Create the time and input vectors
     if T is None or np.asarray(T).size == 1:
         T = _default_time_vector(sys, N=T_num, tfinal=T, is_step=True)
     U = np.ones_like(T)
 
@@ -1367,28 +1375,36 @@
         yout[:, inpidx, :] = response.y
         xout[:, inpidx, :] = response.x
         uout[:, inpidx, :] = U
 
     # Figure out if the system is SISO or not
     issiso = sys.issiso() or (input is not None and output is not None)
 
+    # Select only the given input and output, if any
+    input_labels = sys.input_labels if input is None \
+        else sys.input_labels[input]
+    output_labels = sys.output_labels if output is None \
+        else sys.output_labels[output]
+
     return TimeResponseData(
         response.time, yout, xout, uout, issiso=issiso,
+        output_labels=output_labels, input_labels=input_labels,
+        state_labels=sys.state_labels,
         transpose=transpose, return_x=return_x, squeeze=squeeze)
 
 
 def step_info(sysdata, T=None, T_num=None, yfinal=None,
               SettlingTimeThreshold=0.02, RiseTimeLimits=(0.1, 0.9)):
     """
     Step response characteristics (Rise time, Settling Time, Peak and others).
 
     Parameters
     ----------
     sysdata : StateSpace or TransferFunction or array_like
-        The system data. Either LTI system to similate (StateSpace,
+        The system data. Either LTI system to simulate (StateSpace,
         TransferFunction), or a time series of step response data.
     T : array_like or float, optional
         Time vector, or simulation time duration if a number (time vector is
         autocomputed if not given, see :func:`step_response` for more detail).
         Required, if sysdata is a time series of response data.
     T_num : int, optional
         Number of time steps to use in simulation if T is not provided as an
@@ -1436,17 +1452,16 @@
 
     See Also
     --------
     step, lsim, initial, impulse
 
     Examples
     --------
-    >>> from control import step_info, TransferFunction
-    >>> sys = TransferFunction([-1, 1], [1, 1, 1])
-    >>> S = step_info(sys)
+    >>> sys = ct.TransferFunction([-1, 1], [1, 1, 1])
+    >>> S = ct.step_info(sys)
     >>> for k in S:
     ...     print(f"{k}: {S[k]:3.4}")
     ...
     RiseTime: 1.256
     SettlingTime: 9.071
     SettlingMin: 0.9011
     SettlingMax: 1.208
@@ -1456,23 +1471,22 @@
     PeakTime: 4.187
     SteadyStateValue: 1.0
 
     MIMO System: Simulate until a final time of 10. Get the step response
     characteristics for the second input and specify a 5% error until the
     signal is considered settled.
 
-    >>> from numpy import sqrt
-    >>> from control import step_info, StateSpace
-    >>> sys = StateSpace([[-1., -1.],
+    >>> from math import sqrt
+    >>> sys = ct.StateSpace([[-1., -1.],
     ...                   [1., 0.]],
     ...                  [[-1./sqrt(2.), 1./sqrt(2.)],
     ...                   [0, 0]],
     ...                  [[sqrt(2.), -sqrt(2.)]],
     ...                  [[0, 0]])
-    >>> S = step_info(sys, T=10., SettlingTimeThreshold=0.05)
+    >>> S = ct.step_info(sys, T=10., SettlingTimeThreshold=0.05)
     >>> for k, v in S[0][1].items():
     ...     print(f"{k}: {float(v):3.4}")
     RiseTime: 1.212
     SettlingTime: 6.061
     SettlingMin: -1.209
     SettlingMax: -0.9184
     Overshoot: 20.87
@@ -1598,15 +1612,15 @@
 
     return ret[0][0] if retsiso else ret
 
 
 def initial_response(sys, T=None, X0=0., input=0, output=None, T_num=None,
                      transpose=False, return_x=False, squeeze=None):
     # pylint: disable=W0622
-    """Initial condition response of a linear system
+    """Compute the initial condition response for a linear system.
 
     If the system has multiple outputs (MIMO), optionally, one output
     may be selected. If no selection is made for the output, all
     outputs are given.
 
     For information on the **shape** of parameters `T`, `X0` and
     return values `T`, `yout`, see :ref:`time-series-convention`.
@@ -1682,15 +1696,16 @@
     Notes
     -----
     This function uses the `forced_response` function with the input set to
     zero.
 
     Examples
     --------
-    >>> T, yout = initial_response(sys, T, X0)
+    >>> G = ct.rss(4)
+    >>> T, yout = ct.initial_response(G)
 
     """
     squeeze, sys = _get_ss_simo(sys, input, output, squeeze=squeeze)
 
     # Create time and input vectors; checking is done in forced_response(...)
     # The initial vector X0 is created in forced_response(...) if necessary
     if T is None or np.asarray(T).size == 1:
@@ -1698,17 +1713,23 @@
 
     # Compute the forced response
     response = forced_response(sys, T, 0, X0)
 
     # Figure out if the system is SISO or not
     issiso = sys.issiso() or (input is not None and output is not None)
 
+    # Select only the given output, if any
+    output_labels = sys.output_labels if output is None \
+        else sys.output_labels[0]
+
     # Store the response without an input
     return TimeResponseData(
         response.t, response.y, response.x, None, issiso=issiso,
+        output_labels=output_labels, input_labels=None,
+        state_labels=sys.state_labels,
         transpose=transpose, return_x=return_x, squeeze=squeeze)
 
 
 def impulse_response(sys, T=None, X0=0., input=None, output=None, T_num=None,
                      transpose=False, return_x=False, squeeze=None):
     # pylint: disable=W0622
     """Compute the impulse response for a linear system.
@@ -1792,20 +1813,21 @@
     --------
     forced_response, initial_response, step_response
 
     Notes
     -----
     This function uses the `forced_response` function to compute the time
     response. For continuous time systems, the initial condition is altered to
-    account for the initial impulse. For discrete-time aystems, the impulse is 
+    account for the initial impulse. For discrete-time aystems, the impulse is
     sized so that it has unit area.
 
     Examples
     --------
-    >>> T, yout = impulse_response(sys, T, X0)
+    >>> G = ct.rss(4)
+    >>> T, yout = ct.impulse_response(G)
 
     """
     # Convert to state space so that we can simulate
     sys = _convert_to_statespace(sys)
 
     # Check to make sure there is not a direct term
     if np.any(sys.D != 0) and isctime(sys):
@@ -1862,16 +1884,24 @@
         inpidx = i if input is None else 0
         yout[:, inpidx, :] = response.y
         xout[:, inpidx, :] = response.x
 
     # Figure out if the system is SISO or not
     issiso = sys.issiso() or (input is not None and output is not None)
 
+    # Select only the given input and output, if any
+    input_labels = sys.input_labels if input is None \
+        else sys.input_labels[input]
+    output_labels = sys.output_labels if output is None \
+        else sys.output_labels[output]
+
     return TimeResponseData(
         response.time, yout, xout, uout, issiso=issiso,
+        output_labels=output_labels, input_labels=input_labels,
+        state_labels=sys.state_labels,
         transpose=transpose, return_x=return_x, squeeze=squeeze)
 
 
 # utility function to find time period and time increment using pole locations
 def _ideal_tfinal_and_dt(sys, is_step=True):
     """helper function to compute ideal simulation duration tfinal and dt, the
     time increment. Usually called by _default_time_vector, whose job it is to
```

### Comparing `control-0.9.3.post2/control/xferfcn.py` & `control-0.9.4/control/xferfcn.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,23 @@
 from .frdata import FrequencyResponseData
 from . import config
 
 __all__ = ['TransferFunction', 'tf', 'zpk', 'ss2tf', 'tfdata']
 
 
 # Define module default parameter values
-_xferfcn_defaults = {}
+_xferfcn_defaults = {
+    'xferfcn.display_format': 'poly',
+    'xferfcn.floating_point_format': '.4g'
+}
+
+
+def _float2str(value):
+    _num_format = config.defaults.get('xferfcn.floating_point_format', ':.4g')
+    return f"{value:{_num_format}}"
 
 
 class TransferFunction(LTI):
     """TransferFunction(num, den[, dt])
 
     A class for representing transfer functions.
 
@@ -88,14 +96,18 @@
         Polynomial coefficients of the denominator
     dt : None, True or float, optional
         System timebase. 0 (default) indicates continuous
         time, True indicates discrete time with unspecified sampling
         time, positive number is discrete time with specified
         sampling time, None indicates unspecified timebase (either
         continuous or discrete time).
+    display_format: None, 'poly' or 'zpk'
+        Set the display format used in printing the TransferFunction object.
+        Default behavior is polynomial display and can be changed by
+        changing config.defaults['xferfcn.display_format'].
 
     Attributes
     ----------
     ninputs, noutputs, nstates : int
         Number of input, output and state variables.
     num, den : 2D list of array
         Polynomial coefficients of the numerator and denominator.
@@ -106,15 +118,15 @@
         timebase (either continuous or discrete time).
 
     Notes
     -----
     The attribues 'num' and 'den' are 2-D lists of arrays containing MIMO
     numerator and denominator coefficients.  For example,
 
-    >>> num[2][5] = numpy.array([1., 4., 8.])
+    >>> num[2][5] = numpy.array([1., 4., 8.])                   # doctest: +SKIP
 
     means that the numerator of the transfer function from the 6th input to
     the 3rd output is set to s^2 + 4s + 8.
 
     A discrete time transfer function is created by specifying a nonzero
     'timebase' dt when the system is constructed:
 
@@ -137,15 +149,15 @@
     :meth:`~control.TransferFunction.__call__` for a more detailed description.
 
     The TransferFunction class defines two constants ``s`` and ``z`` that
     represent the differentiation and delay operators in continuous and
     discrete time.  These can be used to create variables that allow algebraic
     creation of transfer functions.  For example,
 
-    >>> s = TransferFunction.s
+    >>> s = ct.TransferFunction.s
     >>> G = (s + 1)/(s**2 + 2*s + 1)
 
     """
 
     # Give TransferFunction._rmul_() priority for ndarray * TransferFunction
     __array_priority__ = 11     # override ndarray and matrix types
 
@@ -194,14 +206,25 @@
 
         num = _clean_part(num)
         den = _clean_part(den)
 
         #
         # Process keyword arguments
         #
+        # During module init, TransferFunction.s and TransferFunction.z
+        # get initialized when defaults are not fully initialized yet.
+        # Use 'poly' in these cases.
+
+        self.display_format = kwargs.pop(
+            'display_format',
+            config.defaults.get('xferfcn.display_format', 'poly'))
+
+        if self.display_format not in ('poly', 'zpk'):
+            raise ValueError("display_format must be 'poly' or 'zpk',"
+                             " got '%s'" % self.display_format)
 
         # Determine if the transfer function is static (needed for dt)
         static = True
         for col in num + den:
             for poly in col:
                 if len(poly) > 1:
                     static = False
@@ -428,47 +451,54 @@
                         data[p][i][j] = zeros(1)
                     else:
                         # Truncate the trivial coefficients.
                         data[p][i][j] = data[p][i][j][nonzero:]
         [self.num, self.den] = data
 
     def __str__(self, var=None):
-        """String representation of the transfer function."""
+        """String representation of the transfer function.
 
-        mimo = self.ninputs > 1 or self.noutputs > 1
+        Based on the display_format property, the output will be formatted as
+        either polynomials or in zpk form.
+        """
+        mimo = not self.issiso()
         if var is None:
-            # TODO: replace with standard calls to lti functions
-            var = 's' if self.dt is None or self.dt == 0 else 'z'
+            var = 's' if self.isctime() else 'z'
         outstr = ""
 
-        for i in range(self.ninputs):
-            for j in range(self.noutputs):
+        for ni in range(self.ninputs):
+            for no in range(self.noutputs):
                 if mimo:
-                    outstr += "\nInput %i to output %i:" % (i + 1, j + 1)
+                    outstr += "\nInput %i to output %i:" % (ni + 1, no + 1)
 
                 # Convert the numerator and denominator polynomials to strings.
-                numstr = _tf_polynomial_to_string(self.num[j][i], var=var)
-                denstr = _tf_polynomial_to_string(self.den[j][i], var=var)
+                if self.display_format == 'poly':
+                    numstr = _tf_polynomial_to_string(self.num[no][ni], var=var)
+                    denstr = _tf_polynomial_to_string(self.den[no][ni], var=var)
+                elif self.display_format == 'zpk':
+                    z, p, k = tf2zpk(self.num[no][ni], self.den[no][ni])
+                    numstr = _tf_factorized_polynomial_to_string(
+                        z, gain=k, var=var)
+                    denstr = _tf_factorized_polynomial_to_string(p, var=var)
 
                 # Figure out the length of the separating line
                 dashcount = max(len(numstr), len(denstr))
                 dashes = '-' * dashcount
 
                 # Center the numerator or denominator
                 if len(numstr) < dashcount:
                     numstr = ' ' * ((dashcount - len(numstr)) // 2) + numstr
                 if len(denstr) < dashcount:
                     denstr = ' ' * ((dashcount - len(denstr)) // 2) + denstr
 
                 outstr += "\n" + numstr + "\n" + dashes + "\n" + denstr + "\n"
 
-        # See if this is a discrete time system with specific sampling time
-        if not (self.dt is None) and type(self.dt) != bool and self.dt > 0:
-            # TODO: replace with standard calls to lti functions
-            outstr += "\ndt = " + self.dt.__str__() + "\n"
+        # If this is a strict discrete time system, print the sampling time
+        if type(self.dt) != bool and self.isdtime(strict=True):
+            outstr += "\ndt = " + str(self.dt) + "\n"
 
         return outstr
 
     # represent to implement a re-loadable version
     def __repr__(self):
         """Print transfer function in loadable form"""
         if self.issiso():
@@ -481,37 +511,43 @@
                 num=self.num.__repr__(), den=self.den.__repr__(),
                 dt=', {}'.format(self.dt) if isdtime(self, strict=True)
                 else '')
 
     def _repr_latex_(self, var=None):
         """LaTeX representation of transfer function, for Jupyter notebook"""
 
-        mimo = self.ninputs > 1 or self.noutputs > 1
+        mimo = not self.issiso()
 
         if var is None:
             # ! TODO: replace with standard calls to lti functions
             var = 's' if self.dt is None or self.dt == 0 else 'z'
 
         out = ['$$']
 
         if mimo:
             out.append(r"\begin{bmatrix}")
 
-        for i in range(self.noutputs):
-            for j in range(self.ninputs):
+        for no in range(self.noutputs):
+            for ni in range(self.ninputs):
                 # Convert the numerator and denominator polynomials to strings.
-                numstr = _tf_polynomial_to_string(self.num[i][j], var=var)
-                denstr = _tf_polynomial_to_string(self.den[i][j], var=var)
+                if self.display_format == 'poly':
+                    numstr = _tf_polynomial_to_string(self.num[no][ni], var=var)
+                    denstr = _tf_polynomial_to_string(self.den[no][ni], var=var)
+                elif self.display_format == 'zpk':
+                    z, p, k = tf2zpk(self.num[no][ni], self.den[no][ni])
+                    numstr = _tf_factorized_polynomial_to_string(
+                        z, gain=k, var=var)
+                    denstr = _tf_factorized_polynomial_to_string(p, var=var)
 
                 numstr = _tf_string_to_latex(numstr, var=var)
                 denstr = _tf_string_to_latex(denstr, var=var)
 
                 out += [r"\frac{", numstr, "}{", denstr, "}"]
 
-                if mimo and j < self.noutputs - 1:
+                if mimo and ni < self.ninputs - 1:
                     out.append("&")
 
             if mimo:
                 out.append(r"\\")
 
         if mimo:
             out.append(r" \end{bmatrix}")
@@ -870,16 +906,16 @@
         return TransferFunction(num, den, self.dt)
 
     def returnScipySignalLTI(self, strict=True):
         """Return a list of a list of :class:`scipy.signal.lti` objects.
 
         For instance,
 
-        >>> out = tfobject.returnScipySignalLTI()
-        >>> out[3][5]
+        >>> out = tfobject.returnScipySignalLTI()               # doctest: +SKIP
+        >>> out[3][5]                                           # doctest: +SKIP
 
         is a :class:`scipy.signal.lti` object corresponding to the
         transfer function from the 6th input to the 4th output.
 
         Parameters
         ----------
         strict : bool, optional
@@ -959,15 +995,15 @@
 
         denorder: array of int, orders of den, one per input
 
 
 
         Examples
         --------
-        >>> num, den, denorder = sys._common_den()
+        >>> num, den, denorder = sys._common_den()              # doctest: +SKIP
 
         """
 
         # Machine precision for floats.
         eps = finfo(float).eps
         real_tol = sqrt(eps * self.ninputs * self.noutputs)
 
@@ -1094,15 +1130,15 @@
         Ts : float
             Sampling period
         method : {"gbt", "bilinear", "euler", "backward_diff",
                   "zoh", "matched"}
             Method to use for sampling:
 
             * gbt: generalized bilinear transformation
-            * bilinear: Tustin's approximation ("gbt" with alpha=0.5)
+            * bilinear or tustin: Tustin's approximation ("gbt" with alpha=0.5)
             * euler: Euler (or forward difference) method ("gbt" with alpha=0)
             * backward_diff: Backwards difference ("gbt" with alpha=1.0)
             * zoh: zero-order hold (default)
         alpha : float within [0, 1]
             The generalized bilinear transformation weighting parameter, which
             should only be specified with method="gbt", and is ignored
             otherwise. See :func:`scipy.signal.cont2discrete`.
@@ -1141,42 +1177,41 @@
         -----
         1. Available only for SISO systems
 
         2. Uses :func:`scipy.signal.cont2discrete`
 
         Examples
         --------
-        >>> sys = TransferFunction(1, [1,1])
+        >>> sys = ct.tf(1, [1, 1])
         >>> sysd = sys.sample(0.5, method='bilinear')
 
         """
         if not self.isctime():
             raise ValueError("System must be continuous time system")
         if not self.issiso():
             raise ControlMIMONotImplemented("Not implemented for MIMO systems")
         if method == "matched":
             return _c2d_matched(self, Ts)
         sys = (self.num[0][0], self.den[0][0])
-        if (method == 'bilinear' or (method == 'gbt' and alpha == 0.5)) and \
-                prewarp_frequency is not None:
-            Twarp = 2*np.tan(prewarp_frequency*Ts/2)/prewarp_frequency
+        if prewarp_frequency is not None:
+            if method in ('bilinear', 'tustin') or \
+                    (method == 'gbt' and alpha == 0.5):
+                Twarp = 2*np.tan(prewarp_frequency*Ts/2)/prewarp_frequency
+            else:
+                warn('prewarp_frequency ignored: incompatible conversion')
+                Twarp = Ts
         else:
             Twarp = Ts
         numd, dend, _ = cont2discrete(sys, Twarp, method, alpha)
 
         sysd = TransferFunction(numd[0, :], dend, Ts)
         # copy over the system name, inputs, outputs, and states
         if copy_names:
-            sysd._copy_names(self)
-            if name is None:
-                sysd.name = \
-                    config.defaults['namedio.sampled_system_name_prefix'] +\
-                    sysd.name + \
-                    config.defaults['namedio.sampled_system_name_suffix']
-            else:
+            sysd._copy_names(self, prefix_suffix_name='sampled')
+            if name is not None:
                 sysd.name = name
         # pass desired signal names if names were provided
         return TransferFunction(sysd, name=name, **kwargs)
 
     def dcgain(self, warn_infinite=False):
         """Return the zero-frequency (or DC) gain
 
@@ -1198,14 +1233,21 @@
             The value of the array elements or the scalar is either the
             zero-frequency (or DC) gain, or `inf`, if the frequency response
             is singular.
 
             For real valued systems, the empty imaginary part of the
             complex zero-frequency response is discarded and a real array or
             scalar is returned.
+
+        Examples
+        --------
+        >>> G = ct.tf([1], [1, 4])
+        >>> G.dcgain()
+        0.25
+
         """
         return self._dcgain(warn_infinite)
 
     def _isstatic(self):
         """returns True if and only if all of the numerator and denominator
         polynomials of the (possibly MIMO) transfer function are zeroth order,
         that is, if the system has no dynamics. """
@@ -1226,29 +1268,29 @@
     #: Differentation operator (continuous time)
     #:
     #: The ``s`` constant can be used to create continuous time transfer
     #: functions using algebraic expressions.
     #:
     #: Example
     #: -------
-    #: >>> s = TransferFunction.s
-    #: >>> G  = (s + 1)/(s**2 + 2*s + 1)
+    #: >>> s = TransferFunction.s                               # doctest: +SKIP
+    #: >>> G  = (s + 1)/(s**2 + 2*s + 1)                        # doctest: +SKIP
     #:
     #: :meta hide-value:
     s = None
 
     #: Delay operator (discrete time)
     #:
     #: The ``z`` constant can be used to create discrete time transfer
     #: functions using algebraic expressions.
     #:
     #: Example
     #: -------
-    #: >>> z = TransferFunction.z
-    #: >>> G  = 2 * z / (4 * z**3 + 3*z - 1)
+    #: >>> z = TransferFunction.z                               # doctest: +SKIP
+    #: >>> G  = 2 * z / (4 * z**3 + 3*z - 1)                    # doctest: +SKIP
     #:
     #: :meta hide-value:
     z = None
 
 
 # c2d function contributed by Benjamin White, Oct 2012
 def _c2d_matched(sysC, Ts):
@@ -1281,15 +1323,15 @@
 
     thestr = "0"
 
     # Compute the number of coefficients
     N = len(coeffs) - 1
 
     for k in range(len(coeffs)):
-        coefstr = '%.4g' % abs(coeffs[k])
+        coefstr = _float2str(abs(coeffs[k]))
         power = (N - k)
         if power == 0:
             if coefstr != '0':
                 newstr = '%s' % (coefstr,)
             else:
                 if k == 0:
                     newstr = '0'
@@ -1319,14 +1361,57 @@
         elif (k == 0) and (newstr != '') and (coeffs[k] < 0):
             thestr = "-%s" % (newstr,)
         else:
             thestr = newstr
     return thestr
 
 
+def _tf_factorized_polynomial_to_string(roots, gain=1, var='s'):
+    """Convert a factorized polynomial to a string"""
+
+    if roots.size == 0:
+        return _float2str(gain)
+
+    factors = []
+    for root in sorted(roots, reverse=True):
+        if np.isreal(root):
+            if root == 0:
+                factor = f"{var}"
+                factors.append(factor)
+            elif root > 0:
+                factor = f"{var} - {_float2str(np.abs(root))}"
+                factors.append(factor)
+            else:
+                factor = f"{var} + {_float2str(np.abs(root))}"
+                factors.append(factor)
+        elif np.isreal(root * 1j):
+            if root.imag > 0:
+                factor = f"{var} - {_float2str(np.abs(root))}j"
+                factors.append(factor)
+            else:
+                factor = f"{var} + {_float2str(np.abs(root))}j"
+                factors.append(factor)
+        else:
+            if root.real > 0:
+                factor = f"{var} - ({_float2str(root)})"
+                factors.append(factor)
+            else:
+                factor = f"{var} + ({_float2str(-root)})"
+                factors.append(factor)
+
+    multiplier = ''
+    if round(gain, 4) != 1.0:
+        multiplier = _float2str(gain) + " "
+
+    if len(factors) > 1 or multiplier:
+        factors = [f"({factor})" for factor in factors]
+
+    return multiplier + " ".join(factors)
+
+
 def _tf_string_to_latex(thestr, var='s'):
     """ make sure to superscript all digits in a polynomial string
         and convert float coefficients in scientific notation
         to prettier LaTeX representation """
     # TODO: make the multiplication sign configurable
     expmul = r' \\times'
     thestr = sub(var + r'\^(\d{2,})', var + r'^{\1}', thestr)
@@ -1344,15 +1429,16 @@
 
     num = polyadd(polymul(num1, den2), polymul(num2, den1))
     den = polymul(den1, den2)
 
     return num, den
 
 
-def _convert_to_transfer_function(sys, inputs=1, outputs=1):
+def _convert_to_transfer_function(
+        sys, inputs=1, outputs=1, use_prefix_suffix=False):
     """Convert a system to transfer function form (if needed).
 
     If sys is already a transfer function, then it is returned.  If sys is a
     state space object, then it is converted to a transfer function and
     returned.  If sys is a scalar, then the number of inputs and outputs can be
     specified manually, as in:
 
@@ -1420,15 +1506,18 @@
 
                 # Do the conversion using sp.signal.ss2tf
                 # Note that this returns a 2D array for the numerator
                 num, den = sp.signal.ss2tf(sys.A, sys.B, sys.C, sys.D)
                 num = squeeze(num)  # Convert to 1D array
                 den = squeeze(den)  # Probably not needed
 
-        return TransferFunction(num, den, sys.dt)
+        newsys = TransferFunction(num, den, sys.dt)
+        if use_prefix_suffix:
+            newsys._copy_names(sys, prefix_suffix_name='converted')
+        return newsys
 
     elif isinstance(sys, (int, float, complex, np.number)):
         num = [[[sys] for j in range(inputs)] for i in range(outputs)]
         den = [[[1] for j in range(inputs)] for i in range(outputs)]
 
         return TransferFunction(num, den)
 
@@ -1482,14 +1571,18 @@
     ----------
     sys: LTI (StateSpace or TransferFunction)
         A linear system
     num: array_like, or list of list of array_like
         Polynomial coefficients of the numerator
     den: array_like, or list of list of array_like
         Polynomial coefficients of the denominator
+    display_format: None, 'poly' or 'zpk'
+        Set the display format used in printing the TransferFunction object.
+        Default behavior is polynomial display and can be changed by
+        changing config.defaults['xferfcn.display_format']..
 
     Returns
     -------
     out: :class:`TransferFunction`
         The new linear system
 
     Other Parameters
@@ -1530,23 +1623,23 @@
     Examples
     --------
     >>> # Create a MIMO transfer function object
     >>> # The transfer function from the 2nd input to the 1st output is
     >>> # (3s + 4) / (6s^2 + 5s + 4).
     >>> num = [[[1., 2.], [3., 4.]], [[5., 6.], [7., 8.]]]
     >>> den = [[[9., 8., 7.], [6., 5., 4.]], [[3., 2., 1.], [-1., -2., -3.]]]
-    >>> sys1 = tf(num, den)
+    >>> sys1 = ct.tf(num, den)
 
     >>> # Create a variable 's' to allow algebra operations for SISO systems
-    >>> s = tf('s')
+    >>> s = ct.tf('s')
     >>> G  = (s + 1)/(s**2 + 2*s + 1)
 
     >>> # Convert a StateSpace to a TransferFunction object.
-    >>> sys_ss = ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
-    >>> sys2 = tf(sys1)
+    >>> sys_ss = ct.ss("1. -2; 3. -4", "5.; 7", "6. 8", "9.")
+    >>> sys2 = ct.tf(sys1)
 
     """
 
     if len(args) == 2 or len(args) == 3:
         return TransferFunction(*args, **kwargs)
 
     elif len(args) == 1 and isinstance(args[0], str):
@@ -1605,20 +1698,33 @@
         List of strings that name the individual signals.  If this parameter
         is not given or given as `None`, the signal names will be of the
         form `s[i]` (where `s` is one of `u`, `y`, or `x`). See
         :class:`InputOutputSystem` for more information.
     name : string, optional
         System name (used for specifying signals). If unspecified, a generic
         name <sys[id]> is generated with a unique integer id.
+    display_format: None, 'poly' or 'zpk'
+        Set the display format used in printing the TransferFunction object.
+        Default behavior is polynomial display and can be changed by
+        changing config.defaults['xferfcn.display_format'].
 
     Returns
     -------
     out: :class:`TransferFunction`
         Transfer function with given zeros, poles, and gain.
 
+    Examples
+    --------
+    >>> G = ct.zpk([1], [2, 3], gain=1, display_format='zpk')
+    >>> print(G)                                                # doctest: +SKIP
+
+         s - 1
+    ---------------
+    (s - 2) (s - 3)
+
     """
     num, den = zpk2tf(zeros, poles, gain)
     return TransferFunction(num, den, *args, **kwargs)
 
 
 def ss2tf(*args, **kwargs):
 
@@ -1678,22 +1784,22 @@
     --------
     tf
     ss
     tf2ss
 
     Examples
     --------
-    >>> A = [[1., -2], [3, -4]]
-    >>> B = [[5.], [7]]
-    >>> C = [[6., 8]]
-    >>> D = [[9.]]
-    >>> sys1 = ss2tf(A, B, C, D)
+    >>> A = [[-1, -2], [3, -4]]
+    >>> B = [[5], [6]]
+    >>> C = [[7, 8]]
+    >>> D = [[9]]
+    >>> sys1 = ct.ss2tf(A, B, C, D)
 
-    >>> sys_ss = ss(A, B, C, D)
-    >>> sys2 = ss2tf(sys_ss)
+    >>> sys_ss = ct.ss(A, B, C, D)
+    >>> sys2 = ct.ss2tf(sys_ss)
 
     """
 
     from .statesp import StateSpace
     if len(args) == 4 or len(args) == 5:
         # Assume we were given the A, B, C, D matrix and (optional) dt
         return _convert_to_transfer_function(StateSpace(*args, **kwargs))
@@ -1703,15 +1809,17 @@
         if isinstance(sys, StateSpace):
             kwargs = kwargs.copy()
             if not kwargs.get('inputs'):
                 kwargs['inputs'] = sys.input_labels
             if not kwargs.get('outputs'):
                 kwargs['outputs'] = sys.output_labels
             return TransferFunction(
-                _convert_to_transfer_function(sys), **kwargs)
+                _convert_to_transfer_function(
+                    sys, use_prefix_suffix=not sys._generic_name_check()),
+                **kwargs)
         else:
             raise TypeError(
                 "ss2tf(sys): sys must be a StateSpace object.  It is %s."
                 % type(sys))
     else:
         raise ValueError("Needs 1 or 4 arguments; received %i." % len(args))
```

### Comparing `control-0.9.3.post2/control.egg-info/PKG-INFO` & `control-0.9.4/control.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control
-Version: 0.9.3.post2
+Version: 0.9.4
 Summary: Python Control Systems Library
 Author-email: Python Control Developers <python-control-developers@lists.sourceforge.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://python-control.org
 Project-URL: source, https://github.com/python-control/python-control
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -48,103 +48,113 @@
 
 Python Control Systems Library
 ==============================
 
 The Python Control Systems Library is a Python module that implements basic
 operations for analysis and design of feedback control systems.
 
-
 Have a go now!
-==============
+--------------
 Try out the examples in the examples folder using the binder service.
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/python-control/python-control/HEAD
 
+The package can also be installed on Google Colab using the commands::
+
+  !pip install control
+  import control as ct
 
 Features
 --------
 
 - Linear input/output systems in state-space and frequency domain
 - Block diagram algebra: serial, parallel, feedback, and other interconnections
 - Time response: initial, step, impulse
 - Frequency response: Bode, Nyquist, and Nichols plots
 - Control analysis: stability, reachability, observability, stability margins, root locus
 - Control design: eigenvalue placement, linear quadratic regulator, sisotool, hinfsyn, rootlocus_pid_designer
 - Estimator design: linear quadratic estimator (Kalman filter)
 - Nonlinear systems: optimization-based control, describing functions, differential flatness
 
 Links
-=====
+-----
 
 - Project home page: http://python-control.org
 - Source code repository: https://github.com/python-control/python-control
 - Documentation: http://python-control.readthedocs.org/
 - Issue tracker: https://github.com/python-control/python-control/issues
 - Mailing list: http://sourceforge.net/p/python-control/mailman/
 
-
 Dependencies
-============
+------------
 
 The package requires numpy, scipy, and matplotlib.  In addition, some routines
 use a module called slycot, that is a Python wrapper around some FORTRAN
 routines.  Many parts of python-control will work without slycot, but some
 functionality is limited or absent, and installation of slycot is recommended
 (see below). The Slycot wrapper can be found at:
 
 https://github.com/python-control/Slycot
 
+
 Installation
 ============
 
 Conda and conda-forge
 ---------------------
 
 The easiest way to get started with the Control Systems library is
 using `Conda <https://conda.io>`_.
 
-The Control Systems library has been packages for the `conda-forge
+The Control Systems library has packages available using the `conda-forge
 <https://conda-forge.org>`_ Conda channel, and as of Slycot version
 0.3.4, binaries for that package are available for 64-bit Windows,
 OSX, and Linux.
 
 To install both the Control Systems library and Slycot in an existing
 conda environment, run::
 
   conda install -c conda-forge control slycot
 
+Mixing packages from conda-forge and the default conda channel can
+sometimes cause problems with dependencies, so it is usually best to
+instally NumPy, SciPy, and Matplotlib from conda-forge as well.
+
 Pip
 ---
 
 To install using pip::
 
   pip install slycot   # optional; see below
   pip install control
 
 If you install Slycot using pip you'll need a development environment
-(e.g., Python development files, C and Fortran compilers).
+(e.g., Python development files, C and Fortran compilers).  Pip
+installation can be particularly complicated for Windows.
 
 Installing from source
 ----------------------
 
 To install from source, get the source code of the desired branch or release
 from the github repository or archive, unpack, and run from within the
 toplevel `python-control` directory::
 
   pip install .
   
 Article and Citation Information
 ================================
 
-An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
+An `article <https://ieeexplore.ieee.org/abstract/document/9683368>`_ about
+the library is available on IEEE Explore. If the Python Control Systems Library helped you in your research, please cite::
 
   @inproceedings{python-control2021,
     title={The Python Control Systems Library (python-control)},
-    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
+    author={Fuller, Sawyer and Greiner, Ben and Moore, Jason and
+            Murray, Richard and van Paassen, Ren{\'e} and Yorke, Rory},
     booktitle={60th IEEE Conference on Decision and Control (CDC)},
     pages={4875--4881},
     year={2021},
     organization={IEEE}
   }
 
 or the GitHub site: https://github.com/python-control/python-control
```

### Comparing `control-0.9.3.post2/control.egg-info/SOURCES.txt` & `control-0.9.4/control.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 LICENSE
 MANIFEST.in
 Pending
 README.rst
 asv.conf.json
 pyproject.toml
 .github/conda-env/build-env.yml
+.github/conda-env/doctest-env.yml
 .github/conda-env/test-env.yml
 .github/scripts/set-conda-test-matrix.py
 .github/scripts/set-pip-test-matrix.py
 .github/workflows/control-slycot-src.yml
+.github/workflows/doctest.yml
 .github/workflows/install_examples.yml
 .github/workflows/os-blas-test-matrix.yml
 .github/workflows/python-package-conda.yml
 benchmarks/README
 benchmarks/__init__.py
 benchmarks/flatsys_bench.py
+benchmarks/optestim_bench.py
 benchmarks/optimal_bench.py
 conda-recipe/bld.bat
 conda-recipe/meta.yaml
 control/__init__.py
 control/_version.py
 control/bdalg.py
 control/canonical.py
@@ -117,14 +120,15 @@
 control/tests/xferfcn_input_test.py
 control/tests/xferfcn_test.py
 doc/.gitignore
 doc/Makefile
 doc/README
 doc/classes.fig
 doc/classes.pdf
+doc/classes.png
 doc/classes.rst
 doc/conf.py
 doc/control.rst
 doc/conventions.rst
 doc/cruise-control.py
 doc/cruise-control.rst
 doc/cruise.ipynb
@@ -135,32 +139,38 @@
 doc/index.rst
 doc/intro.rst
 doc/iosys.rst
 doc/kincar-flatsys.py
 doc/kincar-flatsys.rst
 doc/kincar-fusion.ipynb
 doc/matlab.rst
+doc/mhe-pvtol.ipynb
 doc/mpc-overview.png
 doc/mpc_aircraft.ipynb
 doc/optimal.rst
 doc/phaseplots.py
 doc/phaseplots.rst
 doc/pvtol-lqr-nested.ipynb
 doc/pvtol-lqr.py
 doc/pvtol-lqr.rst
 doc/pvtol-nested.py
 doc/pvtol-nested.rst
 doc/pvtol-outputfbk.ipynb
+doc/pvtol.py
 doc/requirements.txt
 doc/robust_mimo.py
 doc/robust_mimo.rst
 doc/robust_siso.py
 doc/robust_siso.rst
 doc/rss-balred.py
 doc/rss-balred.rst
+doc/scherer_etal_ex7_H2_h2syn.py
+doc/scherer_etal_ex7_H2_h2syn.rst
+doc/scherer_etal_ex7_Hinf_hinfsyn.py
+doc/scherer_etal_ex7_Hinf_hinfsyn.rst
 doc/secord-matlab.py
 doc/secord-matlab.rst
 doc/steering-gainsched.py
 doc/steering-gainsched.rst
 doc/steering-optimal.png
 doc/steering-optimal.py
 doc/steering-optimal.rst
@@ -171,30 +181,35 @@
 examples/bdalg-matlab.py
 examples/bode-and-nyquist-plots.ipynb
 examples/check-controllability-and-observability.py
 examples/cruise-control.py
 examples/cruise.ipynb
 examples/describing_functions.ipynb
 examples/genswitch.py
+examples/interconnect_tutorial.ipynb
 examples/kincar-flatsys.py
 examples/kincar-fusion.ipynb
+examples/mhe-pvtol.ipynb
 examples/mpc_aircraft.ipynb
 examples/phaseplots.py
 examples/pvtol-lqr-nested.ipynb
 examples/pvtol-lqr.py
 examples/pvtol-nested-ss.py
 examples/pvtol-nested.py
 examples/pvtol-outputfbk.ipynb
 examples/pvtol.py
 examples/robust_mimo.py
 examples/robust_siso.py
 examples/rss-balred.py
 examples/run_examples.sh
 examples/run_notebooks.sh
+examples/scherer_etal_ex7_H2_h2syn.py
+examples/scherer_etal_ex7_Hinf_hinfsyn.py
 examples/secord-matlab.py
+examples/simulating_discrete_nonlinear.ipynb
 examples/singular-values-plot.ipynb
 examples/sisotool_example.py
 examples/slycot-import-test.py
 examples/steering-gainsched.py
 examples/steering-optimal.py
 examples/steering.ipynb
 examples/stochresp.ipynb
```

### Comparing `control-0.9.3.post2/doc/Makefile` & `control-0.9.4/doc/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Rules to create figures
 FIGS = classes.pdf
-classes.pdf: classes.fig;	fig2dev -Lpdf $< $@
+classes.pdf: classes.fig
+	fig2dev -Lpdf $< $@
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-html pdf clean: Makefile $(FIGS)
+html pdf clean doctest: Makefile $(FIGS)
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `control-0.9.3.post2/doc/README` & `control-0.9.4/doc/README`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/classes.fig` & `control-0.9.4/doc/classes.fig`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/classes.pdf` & `control-0.9.4/doc/classes.pdf`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/classes.rst` & `control-0.9.4/doc/classes.rst`

 * *Files 10% similar despite different names*

```diff
@@ -54,7 +54,12 @@
    flatsys.BasisFamily
    flatsys.FlatSystem
    flatsys.LinearFlatSystem
    flatsys.PolyFamily
    flatsys.SystemTrajectory
    optimal.OptimalControlProblem
    optimal.OptimalControlResult
+   optimal.OptimalEstimationProblem
+   optimal.OptimalEstimationResult
+
+The use of these classes is described in more detail in the
+:ref:`flatsys-module` module and the :ref:`optimal-module` module
```

### Comparing `control-0.9.3.post2/doc/conf.py` & `control-0.9.4/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,34 +33,36 @@
 copyright = u'2022, python-control.org'
 author = u'Python Control Developers'
 
 # Version information - read from the source code
 import re
 import control
 
+# Get the version number for this commmit (including alpha/beta/rc tags)
+release = re.sub('^v', '', os.popen('git describe').read().strip())
+
 # The short X.Y.Z version
-version = re.sub(r'(\d+\.\d+\.\d+)(.*)', r'\1', control.__version__)
+version = re.sub(r'(\d+\.\d+\.\d+(.post\d+)?)(.*)', r'\1', release)
 
-# The full version, including alpha/beta/rc tags
-release = control.__version__
 print("version %s, release %s" % (version, release))
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '3.1'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc', 'sphinx.ext.todo', 'sphinx.ext.napoleon',
     'sphinx.ext.intersphinx', 'sphinx.ext.imgmath',
-    'sphinx.ext.autosummary', 'nbsphinx', 'numpydoc', 'sphinx.ext.linkcode'
+    'sphinx.ext.autosummary', 'nbsphinx', 'numpydoc',
+    'sphinx.ext.linkcode', 'sphinx.ext.doctest'
 ]
 
 # scan documents for autosummary directives and generate stub pages for each.
 autosummary_generate = True
 
 # list of autodoc directive flags that should be automatically applied
 # to all autodoc directives.
@@ -123,15 +125,18 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-# html_static_path = ['_static']
+
+html_static_path = ['_static']
+def setup(app):
+    app.add_css_file('css/custom.css')
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
@@ -198,19 +203,18 @@
 
     if lineno:
         linespec = "#L%d-L%d" % (lineno, lineno + len(source) - 1)
     else:
         linespec = ""
 
     base_url = "https://github.com/python-control/python-control/blob/"
-    if 'dev' in control.__version__:
+    if release != version:      # development release
         return base_url + "main/control/%s%s" % (fn, linespec)
-    else:
-        return base_url + "%s/control/%s%s" % (
-           control.__version__, fn, linespec)
+    else:                       # specific version
+        return base_url + "%s/control/%s%s" % (version, fn, linespec)
 
 # Don't automaticall show all members of class in Methods & Attributes section
 numpydoc_show_class_members = False
 
 # Don't create a Sphinx TOC for the lists of class methods and attributes
 numpydoc_class_members_toctree = False
 
@@ -265,7 +269,18 @@
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'PythonControlLibrary', u'Python Control Library Documentation',
      author, 'PythonControlLibrary', 'One line description of project.',
      'Miscellaneous'),
 ]
+
+# -- Options for doctest ----------------------------------------------
+
+# Import control as ct
+doctest_global_setup = """
+import numpy as np
+import control as ct
+import control.optimal as obc
+import control.flatsys as fs
+ct.reset_defaults()
+"""
```

### Comparing `control-0.9.3.post2/doc/control.rst` & `control-0.9.4/doc/control.rst`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     describing_function
     frequency_response
     get_input_ff_index
     get_output_fb_index
     ispassive
     margin
     stability_margins
+    step_info
     phase_crossover_frequencies
     poles
     zeros
     pzmap
     root_locus
     sisotool
     StateSpace.__call__
@@ -181,14 +182,16 @@
     mag2db
     modal_form
     observable_form
     pade
     reachable_form
     reset_defaults
     sample_system
+    set_defaults
+    similarity_transform
     ss2tf
     ssdata
     tf2ss
     tfdata
     timebase
     timebaseEqual
     unwrap
```

### Comparing `control-0.9.3.post2/doc/conventions.rst` & `control-0.9.4/doc/conventions.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 .. currentmodule:: control
 
 *******************
 Library conventions
 *******************
 
-The python-control library uses a set of standard conventions for the way
-that different types of standard information used by the library.
+The python-control library uses a set of standard conventions for the
+way that different types of standard information used by the library.
+Throughout this manual, we assume the `control` package has been
+imported as `ct`.
 
 LTI system representation
 =========================
 
 Linear time invariant (LTI) systems are represented in python-control in
 state space, transfer function, or frequency response data (FRD) form.  Most
 functions in the toolbox will operate on any of these data types and
@@ -25,15 +27,15 @@
 .. math::
 
   \frac{dx}{dt} &= A x + B u \\
   y &= C x + D u
 
 where u is the input, y is the output, and x is the state.
 
-To create a state space system, use the :func:`ss` function:
+To create a state space system, use the :func:`ss` function::
 
   sys = ct.ss(A, B, C, D)
 
 State space systems can be manipulated using standard arithmetic operations
 as well as the :func:`feedback`, :func:`parallel`, and :func:`series`
 function.  A full list of functions can be found in :ref:`function-ref`.
 
@@ -47,15 +49,15 @@
   G(s) = \frac{\text{num}(s)}{\text{den}(s)}
        = \frac{a_0 s^m + a_1 s^{m-1} + \cdots + a_m}
               {b_0 s^n + b_1 s^{n-1} + \cdots + b_n},
 
 where n is generally greater than or equal to m (for a proper transfer
 function).
 
-To create a transfer function, use the :func:`tf` function:
+To create a transfer function, use the :func:`tf` function::
 
   sys = ct.tf(num, den)
 
 Transfer functions can be manipulated using standard arithmetic operations
 as well as the :func:`feedback`, :func:`parallel`, and :func:`series`
 function.  A full list of functions can be found in :ref:`function-ref`.
 
@@ -73,71 +75,100 @@
 FRD systems have a somewhat more limited set of functions that are
 available, although all of the standard algebraic manipulations can be
 performed.
 
 The FRD class is also used as the return type for the
 :func:`frequency_response` function (and the equivalent method for the
 :class:`StateSpace` and :class:`TransferFunction` classes).  This
-object can be assigned to a tuple using
+object can be assigned to a tuple using::
 
     mag, phase, omega = response
 
 where `mag` is the magnitude (absolute value, not dB or log10) of the
 system frequency response, `phase` is the wrapped phase in radians of
 the system frequency response, and `omega` is the (sorted) frequencies
 at which the response was evaluated.  If the system is SISO and the
 `squeeze` argument to :func:`frequency_response` is not True,
 `magnitude` and `phase` are 1D, indexed by frequency.  If the system
 is not SISO or `squeeze` is False, the array is 3D, indexed by the
 output, input, and frequency.  If `squeeze` is True then
 single-dimensional axes are removed.  The processing of the `squeeze`
 keyword can be changed by calling the response function with a new
-argument:
+argument::
 
     mag, phase, omega = response(squeeze=False)
 
 
 Discrete time systems
 ---------------------
 A discrete time system is created by specifying a nonzero 'timebase', dt.
 The timebase argument can be given when a system is constructed:
 
-* dt = 0: continuous time system (default)
-* dt > 0: discrete time system with sampling period 'dt'
-* dt = True: discrete time with unspecified sampling period
-* dt = None: no timebase specified
+* `dt = 0`: continuous time system (default)
+* `dt > 0`: discrete time system with sampling period 'dt'
+* `dt = True`: discrete time with unspecified sampling period
+* `dt = None`: no timebase specified
 
 Only the :class:`StateSpace`, :class:`TransferFunction`, and
 :class:`InputOutputSystem` classes allow explicit representation of
 discrete time systems.
 
 Systems must have compatible timebases in order to be combined. A discrete
 time system with unspecified sampling time (`dt = True`) can be combined with
 a system having a specified sampling time; the result will be a discrete time
 system with the sample time of the latter system.  Similarly, a system with
 timebase `None` can be combined with a system having a specified timebase; the
 result will have the timebase of the latter system. For continuous time
 systems, the :func:`sample_system` function or the :meth:`StateSpace.sample`
 and :meth:`TransferFunction.sample` methods can be used to create a discrete
 time system from a continuous time system.  See
-:ref:`utility-and-conversions`. The default value of 'dt' can be changed by
-changing the value of ``control.config.defaults['control.default_dt']``.
+:ref:`utility-and-conversions`. The default value of `dt` can be changed by
+changing the value of `control.config.defaults['control.default_dt']`.
 
 Conversion between representations
 ----------------------------------
 LTI systems can be converted between representations either by calling the
 constructor for the desired data type using the original system as the sole
 argument or using the explicit conversion functions :func:`ss2tf` and
 :func:`tf2ss`.
 
+Simulating LTI systems
+======================
+
+A number of functions are available for computing the output (and
+state) response of an LTI systems:
+
+.. autosummary::
+   :toctree: generated/
+   :template: custom-class-template.rst
+
+    initial_response
+    step_response
+    impulse_response
+    forced_response
+
+Each of these functions returns a :class:`TimeResponseData` object
+that contains the data for the time response (described in more detail
+in the next section).
+
+The :func:`forced_response` system is the most general and allows by
+the zero initial state response to be simulated as well as the
+response from a non-zero intial condition.
+
+In addition the :func:`input_output_response` function, which handles
+simulation of nonlinear systems and interconnected systems, can be
+used.  For an LTI system, results are generally more accurate using
+the LTI simulation functions above.  The :func:`input_output_response`
+function is described in more detail in the :ref:`iosys-module` section.
+
 .. currentmodule:: control
 .. _time-series-convention:
 
 Time series data
-================
+----------------
 A variety of functions in the library return time series data: sequences of
 values that change over time.  A common set of conventions is used for
 returning such data: columns represent different points in time, rows are
 different components (e.g., inputs, outputs or states).  For return
 arguments, an array of times is given as the first returned argument,
 followed by one or more arrays of variable values.  This convention is used
 throughout the library, for example in the functions
@@ -161,18 +192,17 @@
 
       U = [[u1(t1), u1(t2), u1(t3), ..., u1(tn)]
            [u2(t1), u2(t2), u2(t3), ..., u2(tn)]
            ...
            ...
            [ui(t1), ui(t2), ui(t3), ..., ui(tn)]]
 
-      Same for X, Y
-
-So, U[:,2] is the system's input at the third point in time; and U[1] or U[1,:]
-is the sequence of values for the system's second input.
+(and similarly for `X`, `Y`).  So, `U[:, 2]` is the system's input at the
+third point in time; and `U[1]` or `U[1, :]` is the sequence of values for
+the system's second input.
 
 When there is only one row, a 1D object is accepted or returned, which adds
 convenience for SISO systems:
 
 The initial conditions are either 1D, or 2D with shape (j, 1)::
 
      X0 = [[x1]
@@ -181,16 +211,18 @@
            ...
            [xj]]
 
 Functions that return time responses (e.g., :func:`forced_response`,
 :func:`impulse_response`, :func:`input_output_response`,
 :func:`initial_response`, and :func:`step_response`) return a
 :class:`TimeResponseData` object that contains the data for the time
-response.  These data can be accessed via the ``time``, ``outputs``,
-``states`` and ``inputs`` properties::
+response.  These data can be accessed via the
+:attr:`~TimeResponseData.time`, :attr:`~TimeResponseData.outputs`,
+:attr:`~TimeResponseData.states` and :attr:`~TimeResponseData.inputs`
+properties::
 
     sys = ct.rss(4, 1, 1)
     response = ct.step_response(sys)
     plot(response.time, response.outputs)
 
 The dimensions of the response properties depend on the function being
 called and whether the system is SISO or MIMO.  In addition, some time
@@ -209,21 +241,21 @@
 The output of a MIMO LTI system can be plotted like this::
 
     t, y = ct.forced_response(sys, t, u)
     plot(t, y[0], label='y_0')
     plot(t, y[1], label='y_1')
 
 The convention also works well with the state space form of linear
-systems. If ``D`` is the feedthrough matrix (2D array) of a linear system,
-and ``U`` is its input (array), then the feedthrough part of the system's
+systems. If `D` is the feedthrough matrix (2D array) of a linear system,
+and `U` is its input (array), then the feedthrough part of the system's
 response, can be computed like this::
 
     ft = D @ U
 
-Finally, the `to_pandas()` function can be used to create a pandas dataframe:
+Finally, the `to_pandas()` function can be used to create a pandas dataframe::
 
     df = response.to_pandas()
 
 The column labels for the data frame are `time` and the labels for the input,
 output, and state signals (`u[i]`, `y[i]`, and `x[i]` by default, but these
 can be changed using the `inputs`, `outputs`, and `states` keywords when
 constructing the system, as described in :func:`ss`, :func:`tf`, and other
@@ -238,44 +270,40 @@
 
 The python-control library can be customized to allow for different default
 values for selected parameters.  This includes the ability to set the style
 for various types of plots and establishing the underlying representation for
 state space matrices.
 
 To set the default value of a configuration variable, set the appropriate
-element of the `control.config.defaults` dictionary:
-
-.. code-block:: python
+element of the `control.config.defaults` dictionary::
 
     ct.config.defaults['module.parameter'] = value
 
 The `~control.config.set_defaults` function can also be used to set multiple
-configuration parameters at the same time:
-
-.. code-block:: python
+configuration parameters at the same time::
 
     ct.config.set_defaults('module', param1=val1, param2=val2, ...]
 
 Finally, there are also functions available set collections of variables based
 on standard configurations.
 
 Selected variables that can be configured, along with their default values:
 
   * freqplot.dB (False): Bode plot magnitude plotted in dB (otherwise powers
     of 10)
-    
+
   * freqplot.deg (True): Bode plot phase plotted in degrees (otherwise radians)
-    
+
   * freqplot.Hz (False): Bode plot frequency plotted in Hertz (otherwise
     rad/sec)
-    
+
   * freqplot.grid (True): Include grids for magnitude and phase plots
-    
+
   * freqplot.number_of_samples (1000): Number of frequency points in Bode plots
-    
+
   * freqplot.feature_periphery_decade (1.0): How many decades to include in
     the frequency range on both sides of features (poles, zeros).
 
   * statesp.use_numpy_matrix (True): set the return type for state space
     matrices to `numpy.matrix` (verus numpy.ndarray)
 
   * statesp.default_dt and xferfcn.default_dt (None): set the default value
```

### Comparing `control-0.9.3.post2/doc/cruise-control.py` & `control-0.9.4/doc/cruise-control.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/cruise.ipynb` & `control-0.9.4/doc/cruise.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/descfcn.rst` & `control-0.9.4/doc/descfcn.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/describing_functions.ipynb` & `control-0.9.4/doc/describing_functions.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/flatsys.rst` & `control-0.9.4/doc/flatsys.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/index.rst` & `control-0.9.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/intro.rst` & `control-0.9.4/doc/intro.rst`

 * *Files 10% similar despite different names*

```diff
@@ -27,66 +27,72 @@
 
 In terms of the python-control package more specifically, here are
 some thing to keep in mind:
 
 * You must include commas in vectors.  So [1 2 3] must be [1, 2, 3].
 * Functions that return multiple arguments use tuples.  
 * You cannot use braces for collections; use tuples instead.
+* Time series data have time as the final index (see
+  :ref:`time-series-convention`).
 
 Installation
 ============
 
-The `python-control` package can be installed using pip, conda or the
-standard setuptools mechanisms.  The package requires `numpy`_ and
-`scipy`_, and the plotting routines require `matplotlib
-<https://matplotlib.org>`_.  In addition, some routines require the `slycot
-<https://github.com/python-control/Slycot>`_ library in order to implement
-more advanced features (including some MIMO functionality).
+The `python-control` package can be installed using conda or pip.  The
+package requires `NumPy`_ and `SciPy`_, and the plotting routines
+require `Matplotlib <https://matplotlib.org>`_.  In addition, some
+routines require the `Slycot
+<https://github.com/python-control/Slycot>`_ library in order to
+implement more advanced features (including some MIMO functionality).
 
+For users with the Anaconda distribution of Python, the following
+command can be used::
+
+  conda install -c conda-forge control slycot
+
+This installs `slycot` and `python-control` from conda-forge, including the
+`openblas` package.  NumPy, SciPy, and Matplotlib will also be installed if
+they are not already present.
+
+.. note::
+   Mixing packages from conda-forge and the default conda channel
+   can sometimes cause problems with dependencies, so it is usually best to
+   instally NumPy, SciPy, and Matplotlib from conda-forge as well.)
 
 To install using pip::
 
   pip install slycot   # optional
   pip install control
 
+.. note::
+   If you install Slycot using pip you'll need a development
+   environment (e.g., Python development files, C and Fortran compilers).
+   Pip installation can be particularly complicated for Windows.
+
 Many parts of `python-control` will work without `slycot`, but some
 functionality is limited or absent, and installation of `slycot` is
 recommended. Users can check to insure that slycot is installed
 correctly by running the command::
 
   python -c "import slycot"
 
 and verifying that no error message appears. More information on the 
-slycot package can be obtained from the `slycot project page
+Slycot package can be obtained from the `Slycot project page
 <https://github.com/python-control/Slycot>`_.
 
-For users with the Anaconda distribution of Python, the following
-commands can be used::
-
-  conda install numpy scipy matplotlib    # if not yet installed
-  conda install -c conda-forge control slycot
-
-This installs `slycot` and `python-control` from conda-forge, including the
-`openblas` package.
-
-Alternatively, to use setuptools, first `download the source
+Alternatively, to install from source, first `download the source
 <https://github.com/python-control/python-control/releases>`_ and unpack it.
 To install in your home directory, use::
 
-  python setup.py install --user
-
-or to install for all users (on Linux or Mac OS)::
-
-  python setup.py build
-  sudo python setup.py install
+  pip install .
 
 Getting started
 ===============
 
 There are two different ways to use the package.  For the default interface
 described in :ref:`function-ref`, simply import the control package as follows::
 
-    >>> import control
+    >>> import control as ct
 
 If you want to have a MATLAB-like environment, use the :ref:`matlab-module`::
 
     >>> from control.matlab import *
```

### Comparing `control-0.9.3.post2/doc/iosys.rst` & `control-0.9.4/doc/iosys.rst`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
       r = params.get('r', 1.6)
 
       # Map the states into local variable names
       H = x[0]
       L = x[1]
 
       # Compute the control action (only allow addition of food)
-      u_0 = u if u > 0 else 0
+      u_0 = u[0] if u[0] > 0 else 0
 
       # Compute the discrete updates
       dH = (r + u_0) * H * (1 - H/k) - (a * H * L)/(c + H)
       dL = b * (a * H *  L)/(c + H) - d * L
 
-      return [dH, dL]
+      return np.array([dH, dL])
 
 We now create an input/output system using these dynamics:
 
 .. code-block:: python
 
   io_predprey = ct.NonlinearIOSystem(
       predprey_rhs, None, inputs=('u'), outputs=('H', 'L'),
```

### Comparing `control-0.9.3.post2/doc/kincar-flatsys.py` & `control-0.9.4/doc/kincar-flatsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # kinematic (bicycle) model of a car changing lanes.
 
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import control as ct
 import control.flatsys as fs
-import control.optimal as opt
+import control.optimal as obc
 
 #
 # System model and utility functions
 #
 
 # Function to take states, inputs and return the flat flag
 def vehicle_flat_forward(x, u, params={}):
@@ -143,15 +143,15 @@
 #
 
 # Define timepoints for evaluation plus basis function to use
 timepts = np.linspace(0, Tf, 10)
 basis = fs.PolyFamily(8)
 
 # Define the cost function (penalize lateral error and steering)
-traj_cost = opt.quadratic_cost(
+traj_cost = obc.quadratic_cost(
     vehicle_flat, np.diag([0, 0.1, 0]), np.diag([0.1, 1]), x0=xf, u0=uf)
 
 # Solve for an optimal solution
 traj2 = fs.point_to_point(
     vehicle_flat, timepts, x0, u0, xf, uf, cost=traj_cost, basis=basis,
 )
 xd, ud = traj2.eval(T)
@@ -164,15 +164,15 @@
 # Approach #3: optimal cost with trajectory constraints
 #
 # Resolve the problem with constraints on the inputs
 #
 
 # Constraint the input values
 constraints = [
-    opt.input_range_constraint(vehicle_flat, [8, -0.1], [12, 0.1]) ]
+    obc.input_range_constraint(vehicle_flat, [8, -0.1], [12, 0.1]) ]
 
 # TEST: Change the basis to use B-splines
 basis = fs.BSplineFamily([0, Tf/2, Tf], 6)
 
 # Solve for an optimal solution
 traj3 = fs.point_to_point(
     vehicle_flat, timepts, x0, u0, xf, uf, cost=traj_cost,
@@ -194,19 +194,19 @@
 #
 # Resolve the problem with constraints on the inputs and also replacing the
 # point to point problem with one using a terminal cost to set the final
 # state.
 #
 
 # Define the cost function (mainly penalize steering angle)
-traj_cost = opt.quadratic_cost(
+traj_cost = obc.quadratic_cost(
     vehicle_flat, None, np.diag([0.1, 10]), x0=xf, u0=uf)
 
 # Set terminal cost to bring us close to xf
-terminal_cost = opt.quadratic_cost(vehicle_flat, 1e3 * np.eye(3), None, x0=xf)
+terminal_cost = obc.quadratic_cost(vehicle_flat, 1e3 * np.eye(3), None, x0=xf)
 
 # Change the basis to use B-splines
 basis = fs.BSplineFamily([0, Tf/2, Tf], [4, 6], vars=2)
 
 # Use a straight line as an initial guess for the trajectory
 initial_guess = np.array(
     [x0[i] + (xf[i] - x0[i]) * timepts/Tf for i in (0, 1)])
```

### Comparing `control-0.9.3.post2/doc/kincar-fusion.ipynb` & `control-0.9.4/doc/kincar-fusion.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/matlab.rst` & `control-0.9.4/doc/matlab.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/mpc-overview.png` & `control-0.9.4/doc/mpc-overview.png`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/mpc_aircraft.ipynb` & `control-0.9.4/doc/mpc_aircraft.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import control.optimal as obc\\n')], delete: [2]}}, 3: "*

 * *            "{'source': {insert: [(8, 'constraints = [obc.input_range_constraint(sys, [-5, -6], "*

 * *            "[5, 6])]\\n'), (13, 'cost = obc.quadratic_cost(model, Q, R, x0=xd, u0=ud)\\n'), (16, "*

 * *            "'ctrl = obc.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)')], "*

 * *            'delete: [16, 13, 8]}}}'}*

```diff
@@ -15,15 +15,15 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import control as ct\n",
                 "import numpy as np\n",
-                "import control.optimal as opt\n",
+                "import control.optimal as obc\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
@@ -66,23 +66,23 @@
                 "# steady state which can be added using \"reference\" filter\n",
                 "# model.u.with('reference');\n",
                 "# model.u.reference = us;\n",
                 "# model.y.with('reference');\n",
                 "# model.y.reference = ys;\n",
                 "\n",
                 "# provide constraints on the system signals\n",
-                "constraints = [opt.input_range_constraint(sys, [-5, -6], [5, 6])]\n",
+                "constraints = [obc.input_range_constraint(sys, [-5, -6], [5, 6])]\n",
                 "\n",
                 "# provide penalties on the system signals\n",
                 "Q = model.C.transpose() @ np.diag([10, 10, 10, 10]) @ model.C\n",
                 "R = np.diag([3, 2])\n",
-                "cost = opt.quadratic_cost(model, Q, R, x0=xd, u0=ud)\n",
+                "cost = obc.quadratic_cost(model, Q, R, x0=xd, u0=ud)\n",
                 "\n",
                 "# online MPC controller object is constructed with a horizon 6\n",
-                "ctrl = opt.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)"
+                "ctrl = obc.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
```

### Comparing `control-0.9.3.post2/doc/optimal.rst` & `control-0.9.4/doc/optimal.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .. _optimal-module:
 
-***************
-Optimal control
-***************
+**************************
+Optimization-based control
+**************************
 
 .. automodule:: control.optimal
    :no-members:
    :no-inherited-members:
    :no-special-members:
 
-Problem setup
-=============
+Optimal control problem setup
+=============================
 
 Consider the *optimal control problem*:
 
 .. math::
 
-  \min_{u(\cdot)} 
+  \min_{u(\cdot)}
   \int_0^T L(x,u)\, dt + V \bigl( x(T) \bigr)
 
 subject to the constraint
 
 .. math::
 
   \dot x = f(x, u), \qquad x\in\mathbb{R}^n,\, u\in\mathbb{R}^m.
@@ -40,27 +40,27 @@
 final (or terminal) cost.
 
 It is often convenient to ask that the final value of the trajectory,
 denoted :math:`x_\text{f}`, be specified.  We can do this by requiring that
 :math:`x(T) = x_\text{f}` or by using a more general form of constraint:
 
 .. math::
-   
+
   \psi_i(x(T)) = 0, \qquad i = 1, \dots, q.
 
 The fully constrained case is obtained by setting :math:`q = n` and defining
 :math:`\psi_i(x(T)) = x_i(T) - x_{i,\text{f}}`.  For a control problem with
 a full set of terminal constraints, :math:`V(x(T))` can be omitted (since
 its value is fixed).
 
 Finally, we may wish to consider optimizations in which either the state or
 the inputs are constrained by a set of nonlinear functions of the form
 
 .. math::
-   
+
   \text{lb}_i \leq g_i(x, u) \leq \text{ub}_i, \qquad i = 1, \dots, k.
 
 where :math:`\text{lb}_i` and :math:`\text{ub}_i` represent lower and upper
 bounds on the constraint function :math:`g_i`.  Note that these constraints
 can be on the input, the state, or combinations of input and state,
 depending on the form of :math:`g_i`.  Furthermore, these constraints are
 intended to hold at all instants in time along the trajectory.
@@ -87,23 +87,127 @@
 In reality, the system will not follow the predicted path exactly, so that
 the red (computed) and blue (actual) trajectories will diverge.  We thus
 recompute the optimal path from the new state at time :math:`t + \Delta T`,
 extending our horizon by an additional :math:`\Delta T` units of time.  This
 approach can be shown to generate stabilizing control laws under suitable
 conditions (see, for example, the FBS2e supplement on `Optimization-Based
 Control <https://fbswiki.org/wiki/index.php/OBC>`_.
-  
+
+Optimal estimation problem setup
+================================
+
+Consider a nonlinear system with discrete time dynamics of the form
+
+.. math::
+  :label: eq_fusion_nlsys-oep
+
+  X[k+1] = f(X[k], u[k], V[k]), \qquad Y[k] = h(X[k]) + W[k],
+
+where :math:`X[k] \in \mathbb{R}^n`, :math:`u[k] \in \mathbb{R}^m`, and
+:math:`Y[k] \in \mathbb{R}^p`, and :math:`V[k] \in \mathbb{R}^q` and
+:math:`W[k] \in \mathbb{R}^p` represent random processes that are not
+necessarily Gaussian white noise processes.  The estimation problem that we
+wish to solve is to find the estimate :math:`\hat x[\cdot]` that matches
+the measured outputs :math:`y[\cdot]` with "likely" disturbances and
+noise.
+
+For a fixed horizon of length :math:`N`, this problem can be formulated as
+an optimization problem where we define the likelihood of a given estimate
+(and the resulting noise and disturbances predicted by the model) as a cost
+function. Suppose we model the likelihood using a conditional probability
+density function :math:`p(x[0], \dots, x[N] \mid y[0], \dots, y[N-1])`.
+Then we can pose the state estimation problem as
+
+.. math::
+  :label: eq_fusion_oep
+
+  \hat x[0], \dots, \hat x[N] =
+  \arg \max_{\hat x[0], \dots, \hat x[N]}
+  p(\hat x[0], \dots, \hat x[N] \mid y[0], \dots, y[N-1])
+
+subject to the constraints given by equation :eq:`eq_fusion_nlsys-oep`.
+The result of this optimization gives us the estimated state for the
+previous :math:`N` steps in time, including the "current" time
+:math:`x[N]`.  The basic idea is thus to compute the state estimate that is
+most consistent with our model and penalize the noise and disturbances
+according to how likely the are (based on the given stochastic system 
+model for each).
+
+Given a solution to this fixed-horizon optimal estimation problem, we can
+create an estimator for the state over all times by repeatedly applying the
+optimization problem :eq:`eq_fusion_oep` over a moving horizon.  At each
+time :math:`k`, we take the measurements for the last :math:`N` time steps
+along with the previously estimated state at the start of the horizon,
+:math:`x[k-N]` and reapply the optimization in equation
+:eq:`eq_fusion_oep`.  This approach is known as a \define{moving horizon
+estimator} (MHE).
+
+The formulation for the moving horizon estimation problem is very general
+and various situations can be captured using the conditional probability
+function :math:`p(x[0], \dots, x[N] \mid y[0], \dots, y[N-1]`.  We start by
+noting that if the disturbances are independent of the underlying states of
+the system, we can write the conditional probability as
+
+.. math::
+
+  p \bigl(x[0], \dots, x[N] \mid y[0], \dots, y[N-1]\bigr) =
+  p_{X[0]}(x[0])\, \prod_{k=0}^{N-1} p_V\bigl(y[k] - h(x[k])\bigr)\,
+    p\bigl(x[k+1] \mid x[k]\bigr).
+
+This expression can be further simplified by taking the log of the
+expression and maximizing the function
+
+.. math::
+  :label: eq_fusion_log-likelihood
+
+  \log p_{X[0]}(x[0]) + \sum_{k=0}^{N-1} \log
+  p_W \bigl(y[k] - h(x[k])\bigr) + \log p_V(v[k]).
+
+The first term represents the likelihood of the initial state, the
+second term captures the likelihood of the noise signal, and the final
+term captures the likelihood of the disturbances.
+
+If we return to the case where :math:`V` and :math:`W` are modeled as
+Gaussian processes, then it can be shown that maximizing equation
+:eq:`eq_fusion_log-likelihood` is equivalent to solving the optimization
+problem given by
+
+.. math::
+  :label: eq_fusion_oep-gaussian
+
+  \min_{x[0], \{v[0], \dots, v[N-1]\}}
+  \|x[0] - \bar x[0]\|_{P_0^{-1}} + \sum_{k=0}^{N-1}
+  \|y[k] - h(x_k)\|_{R_W^{-1}}^2 +
+  \|v[k] \|_{R_V^{-1}}^2,
+
+where :math:`P_0`, :math:`R_V`, and :math:`R_W` are the covariances of the
+initial state, disturbances, and measurement noise.
+
+Note that while the optimization is carried out only over the estimated
+initial state :math:`\hat x[0]`, the entire history of estimated states can
+be reconstructed using the system dynamics:
+
+.. math::
+
+  \hat x[k+1] = f(\hat x[k], u[k], v[k]), \quad k = 0, \dots, N-1.
+
+In particular, we can obtain the estimated state at the end of the moving
+horizon window, corresponding to the current time, and we can thus
+implement an estimator by repeatedly solving the optimization of a window
+of length :math:`N` backwards in time.
+
 Module usage
 ============
 
-The optimal control module provides a means of computing optimal
-trajectories for nonlinear systems and implementing optimization-based
-controllers, including model predictive control.  It follows the basic
-problem setup described above, but carries out all computations in *discrete
-time* (so that integrals become sums) and over a *finite horizon*.  To local
+The optimization-based control module provides a means of computing
+optimal trajectories for nonlinear systems and implementing
+optimization-based controllers, including model predictive control and
+moving horizon estimation.  It follows the basic problem setups
+described above, but carries out all computations in *discrete time*
+(so that integrals become sums) and over a *finite horizon*.  To local
 the optimal control modules, import `control.optimal`:
 
   import control.optimal as obc
 
 To describe an optimal control problem we need an input/output system, a
 time horizon, a cost function, and (optionally) a set of constraints on the
 state and/or input, either along the trajectory and at the terminal time.
@@ -159,26 +263,54 @@
   * `res.states`: state trajectory (if `return_x` was `True`)
   * `res.time`: copy of the time timepts vector
 
 In addition, the results from :func:`scipy.optimize.minimize` are also
 available.
 
 To simplify the specification of cost functions and constraints, the
-:mod:`~control.ios` module defines a number of utility functions:
+:mod:`~control.ios` module defines a number of utility functions for
+optimal control problems:
 
 .. autosummary::
 
    ~control.optimal.quadratic_cost
    ~control.optimal.input_poly_constraint
    ~control.optimal.input_range_constraint
    ~control.optimal.output_poly_constraint
    ~control.optimal.output_range_constraint
    ~control.optimal.state_poly_constraint
    ~control.optimal.state_range_constraint
 
+The optimization-based control module also implements functions for solving
+optimal estimation problems.  The
+:class:`~control.optimal.OptimalEstimationProblem` class is used to define
+an optimal estimation problem over a finite horizon::
+
+  oep = OptimalEstimationProblem(sys, timepts, cost[, constraints])
+
+Given noisy measurements :math:`y` and control inputs :math:`u`, an
+estimate of the states over the time points can be computed using the
+:func:`~control.optimal.OptimalEstimationProblem.compute_estimate` method::
+
+  estim = oep.compute_optimal(Y, U[, X0=x0, initial_guess=(xhat, v)])
+  xhat, v, w = estim.states, estim.inputs, estim.outputs
+
+For discrete time systems, the
+:func:`~control.optimal.OptimalEstimationProblem.create_mhe_iosystem`
+method can be used to generate an input/output system that implements a
+moving horizon estimator.
+
+Several functions are available to help set up standard optimal estimation
+problems:
+
+.. autosummary::
+
+   ~control.optimal.gaussian_likelihood_cost
+   ~control.optimal.disturbance_range_constraint
+
 Example
 =======
 
 Consider the vehicle steering example described in FBS2e.  The dynamics of
 the system can be defined as a nonlinear input/output system using the
 following code::
 
@@ -221,26 +353,26 @@
 
 To set up the optimal control problem we design a cost function that
 penalizes the state and input using quadratic cost functions::
 
   Q = np.diag([0, 0, 0.1])          # don't turn too sharply
   R = np.diag([1, 1])               # keep inputs small
   P = np.diag([1000, 1000, 1000])   # get close to final point
-  traj_cost = opt.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
-  term_cost = opt.quadratic_cost(vehicle, P, 0, x0=xf)
+  traj_cost = obc.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
+  term_cost = obc.quadratic_cost(vehicle, P, 0, x0=xf)
 
 We also constraint the maximum turning rate to 0.1 radians (about 6 degees)
 and constrain the velocity to be in the range of 9 m/s to 11 m/s::
 
-  constraints = [ opt.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
+  constraints = [ obc.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
 
 Finally, we solve for the optimal inputs::
 
   timepts = np.linspace(0, Tf, 10, endpoint=True)
-  result = opt.solve_ocp(
+  result = obc.solve_ocp(
       vehicle, timepts, x0, traj_cost, constraints,
       terminal_cost=term_cost, initial_guess=u0)
 
 Plotting the results::
 
   # Simulate the system dynamics (open loop)
   resp = ct.input_output_response(
@@ -270,14 +402,19 @@
   plt.tight_layout()
   plt.show()
 
 yields
 
 .. image:: steering-optimal.png
 
+
+An example showing the use of the optimal estimation problem and moving
+horizon estimation (MHE) is given in the :doc:`mhe-pvtol Jupyter
+notebook <mhe-pvtol>`.
+
 Optimization Tips
 =================
 
 The python-control optimization module makes use of the SciPy optimization
 toolbox and it can sometimes be tricky to get the optimization to converge.
 If you are getting errors when solving optimal control problems or your
 solutions do not seem close to optimal, here are a few things to try:
@@ -325,19 +462,24 @@
 ============================
 .. autosummary::
    :toctree: generated/
    :template: custom-class-template.rst
 
    ~control.optimal.OptimalControlProblem
    ~control.optimal.OptimalControlResult
+   ~control.optimal.OptimalEstimationProblem
+   ~control.optimal.OptimalEstimationResult
 
 .. autosummary::
    :toctree: generated/
 
-   ~control.optimal.solve_ocp
    ~control.optimal.create_mpc_iosystem
+   ~control.optimal.disturbance_range_constraint
+   ~control.optimal.gaussian_likelihood_cost
    ~control.optimal.input_poly_constraint
    ~control.optimal.input_range_constraint
    ~control.optimal.output_poly_constraint
    ~control.optimal.output_range_constraint
+   ~control.optimal.quadratic_cost
+   ~control.optimal.solve_ocp
    ~control.optimal.state_poly_constraint
    ~control.optimal.state_range_constraint
```

### Comparing `control-0.9.3.post2/doc/phaseplots.py` & `control-0.9.4/doc/phaseplots.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-lqr-nested.ipynb` & `control-0.9.4/doc/pvtol-lqr-nested.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-lqr.py` & `control-0.9.4/doc/pvtol-lqr.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-lqr.rst` & `control-0.9.4/doc/pvtol-lqr.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-nested.py` & `control-0.9.4/doc/pvtol-nested.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-nested.rst` & `control-0.9.4/doc/pvtol-nested.rst`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/pvtol-outputfbk.ipynb` & `control-0.9.4/doc/pvtol-outputfbk.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995920762029509%*

 * *Differences: {"'cells'": "{4: {'outputs': {0: {'text': {insert: [(5, 'Object: pvtol_noisy\\n')], delete: "*

 * *            "[5]}}}, 'source': {insert: [(1, '# pvtol_noisy = pvtol w/ process disturbances and "*

 * *            "sensor noise\\n'), (2, 'from pvtol import pvtol, pvtol_noisy, plot_results\\n'), (20, "*

 * *            "'print(pvtol_noisy)')], delete: [20, 2, 1]}}, 8: {'source': {insert: [(33, '    "*

 * *            "inputs= pvtol_noisy.state_labels[0:3] \\\\\\n'), (34, '        + "*

 * *            "pvtol_noisy.input_labels[0:pvto […]*

```diff
@@ -72,25 +72,25 @@
                     "output_type": "stream",
                     "text": [
                         "Object: pvtol\n",
                         "Inputs (2): F1, F2, \n",
                         "Outputs (6): x0, x1, x2, x3, x4, x5, \n",
                         "States (6): x0, x1, x2, x3, x4, x5,  \n",
                         "\n",
-                        "Object: noisy_pvtol\n",
+                        "Object: pvtol_noisy\n",
                         "Inputs (7): F1, F2, Dx, Dy, Nx, Ny, Nth, \n",
                         "Outputs (6): x0, x1, x2, x3, x4, x5, \n",
                         "States (6): x0, x1, x2, x3, x4, x5, \n"
                     ]
                 }
             ],
             "source": [
                 "# pvtol = nominal system (no disturbances or noise)\n",
-                "# noisy_pvtol = pvtol w/ process disturbances and sensor noise\n",
-                "from pvtol import pvtol, noisy_pvtol, plot_results\n",
+                "# pvtol_noisy = pvtol w/ process disturbances and sensor noise\n",
+                "from pvtol import pvtol, pvtol_noisy, plot_results\n",
                 "\n",
                 "# Find the equiblirum point corresponding to the origin\n",
                 "xe, ue = ct.find_eqpt(\n",
                 "    pvtol, np.zeros(pvtol.nstates),\n",
                 "    np.zeros(pvtol.ninputs), [0, 0, 0, 0, 0, 0],\n",
                 "    iu=range(2, pvtol.ninputs), iy=[0, 1])\n",
                 "\n",
@@ -100,15 +100,15 @@
                 "    iu=range(2, pvtol.ninputs), iy=[0, 1])\n",
                 "\n",
                 "# Extract the linearization for use in LQR design\n",
                 "pvtol_lin = pvtol.linearize(xe, ue)\n",
                 "A, B = pvtol_lin.A, pvtol_lin.B\n",
                 "\n",
                 "print(pvtol, \"\\n\")\n",
-                "print(noisy_pvtol)"
+                "print(pvtol_noisy)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "be6ec05c",
             "metadata": {},
             "source": [
@@ -188,16 +188,16 @@
                 "\n",
                 "    # Return the derivative\n",
                 "    return np.hstack([xhatdot, Pdot.reshape(-1)])\n",
                 "\n",
                 "estimator = ct.NonlinearIOSystem(\n",
                 "    estimator_update, lambda t, x, u, params: x[0:pvtol.nstates],\n",
                 "    states=pvtol.nstates + pvtol.nstates**2,\n",
-                "    inputs= noisy_pvtol.state_labels[0:3] \\\n",
-                "        + noisy_pvtol.input_labels[0:pvtol.ninputs],\n",
+                "    inputs= pvtol_noisy.state_labels[0:3] \\\n",
+                "        + pvtol_noisy.input_labels[0:pvtol.ninputs],\n",
                 "    outputs=[f'xh{i}' for i in range(pvtol.nstates)],\n",
                 ")\n",
                 "print(estimator)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -237,15 +237,15 @@
                         "       1.31948923e-06 -3.16227766e+00  2.32324805e-07  2.36396241e-06\n",
                         "      -4.97998224e+00 -7.90913288e-08]]\n",
                         " \n",
                         "\n",
                         "Object: xh5\n",
                         "Inputs (13): xd[0], xd[1], xd[2], xd[3], xd[4], xd[5], ud[0], ud[1], Dx, Dy, Nx, Ny, Nth, \n",
                         "Outputs (14): x0, x1, x2, x3, x4, x5, F1, F2, xh0, xh1, xh2, xh3, xh4, xh5, \n",
-                        "States (48): noisy_pvtol_x0, noisy_pvtol_x1, noisy_pvtol_x2, noisy_pvtol_x3, noisy_pvtol_x4, noisy_pvtol_x5, sys[3]_x[0], sys[3]_x[1], sys[3]_x[2], sys[3]_x[3], sys[3]_x[4], sys[3]_x[5], sys[3]_x[6], sys[3]_x[7], sys[3]_x[8], sys[3]_x[9], sys[3]_x[10], sys[3]_x[11], sys[3]_x[12], sys[3]_x[13], sys[3]_x[14], sys[3]_x[15], sys[3]_x[16], sys[3]_x[17], sys[3]_x[18], sys[3]_x[19], sys[3]_x[20], sys[3]_x[21], sys[3]_x[22], sys[3]_x[23], sys[3]_x[24], sys[3]_x[25], sys[3]_x[26], sys[3]_x[27], sys[3]_x[28], sys[3]_x[29], sys[3]_x[30], sys[3]_x[31], sys[3]_x[32], sys[3]_x[33], sys[3]_x[34], sys[3]_x[35], sys[3]_x[36], sys[3]_x[37], sys[3]_x[38], sys[3]_x[39], sys[3]_x[40], sys[3]_x[41], \n"
+                        "States (48): pvtol_noisy_x0, pvtol_noisy_x1, pvtol_noisy_x2, pvtol_noisy_x3, pvtol_noisy_x4, pvtol_noisy_x5, sys[3]_x[0], sys[3]_x[1], sys[3]_x[2], sys[3]_x[3], sys[3]_x[4], sys[3]_x[5], sys[3]_x[6], sys[3]_x[7], sys[3]_x[8], sys[3]_x[9], sys[3]_x[10], sys[3]_x[11], sys[3]_x[12], sys[3]_x[13], sys[3]_x[14], sys[3]_x[15], sys[3]_x[16], sys[3]_x[17], sys[3]_x[18], sys[3]_x[19], sys[3]_x[20], sys[3]_x[21], sys[3]_x[22], sys[3]_x[23], sys[3]_x[24], sys[3]_x[25], sys[3]_x[26], sys[3]_x[27], sys[3]_x[28], sys[3]_x[29], sys[3]_x[30], sys[3]_x[31], sys[3]_x[32], sys[3]_x[33], sys[3]_x[34], sys[3]_x[35], sys[3]_x[36], sys[3]_x[37], sys[3]_x[38], sys[3]_x[39], sys[3]_x[40], sys[3]_x[41], \n"
                     ]
                 }
             ],
             "source": [
                 "# Shoot for 1 cm error in x, 10 cm error in y.  Try to keep the angle\n",
                 "# less than 5 degrees in making the adjustments.  Penalize side forces\n",
                 "# due to loss in efficiency.\n",
@@ -265,19 +265,19 @@
                 "# Construct the state feedback controller with estimated state as input\n",
                 "statefbk, _ = ct.create_statefbk_iosystem(pvtol, K, estimator=estimator)\n",
                 "print(statefbk, \"\\n\")\n",
                 "\n",
                 "# Reconstruct the control system with the noisy version of the process\n",
                 "# Create a closed loop system around the controller\n",
                 "clsys = ct.interconnect(\n",
-                "    [noisy_pvtol, statefbk, estimator],\n",
+                "    [pvtol_noisy, statefbk, estimator],\n",
                 "    inplist = statefbk.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    inputs = statefbk.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    outlist = pvtol.output_labels + statefbk.output_labels + estimator.output_labels,\n",
                 "    outputs = pvtol.output_labels + statefbk.output_labels + estimator.output_labels\n",
                 ")\n",
                 "print(clsys)"
             ]
         },
         {
@@ -445,19 +445,19 @@
                 }
             ],
             "source": [
                 "# Compute the full state feedback solution\n",
                 "lqr_ctrl, _ = ct.create_statefbk_iosystem(pvtol, K)\n",
                 "\n",
                 "lqr_clsys = ct.interconnect(\n",
-                "    [noisy_pvtol, lqr_ctrl],\n",
+                "    [pvtol_noisy, lqr_ctrl],\n",
                 "    inplist = lqr_ctrl.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    inputs = lqr_ctrl.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    outlist = pvtol.output_labels + lqr_ctrl.output_labels,\n",
                 "    outputs = pvtol.output_labels + lqr_ctrl.output_labels\n",
                 ")\n",
                 "\n",
                 "# Put together the input for the system\n",
                 "U = np.vstack([\n",
                 "    np.outer(xe, np.ones_like(T)),      # xd\n",
```

### Comparing `control-0.9.3.post2/doc/robust_mimo.py` & `control-0.9.4/doc/robust_mimo.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/robust_siso.py` & `control-0.9.4/doc/robust_siso.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/rss-balred.py` & `control-0.9.4/doc/rss-balred.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/secord-matlab.py` & `control-0.9.4/doc/secord-matlab.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/steering-gainsched.py` & `control-0.9.4/doc/steering-gainsched.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/steering-optimal.png` & `control-0.9.4/doc/steering-optimal.png`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/steering-optimal.py` & `control-0.9.4/doc/steering-optimal.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file works through an optimal control example for the vehicle
 # steering system.  It is intended to demonstrate the functionality for
 # optimal control module (control.optimal) in the python-control package.
 
 import numpy as np
 import math
 import control as ct
-import control.optimal as opt
+import control.optimal as obc
 import matplotlib.pyplot as plt
 import logging
 import time
 import os
 
 #
 # Vehicle steering dynamics
@@ -102,15 +102,15 @@
 # exerting too much control effort to achieve our goal.
 #
 print("Approach 1: standard quadratic cost")
 
 # Set up the cost functions
 Q = np.diag([.1, 10, .1])       # keep lateral error low
 R = np.diag([.1, 1])            # minimize applied inputs
-quad_cost = opt.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
+quad_cost = obc.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
 
 # Define the time horizon (and spacing) for the optimization
 timepts = np.linspace(0, Tf, 20, endpoint=True)
 
 # Provide an initial guess
 straight_line = (
     np.array([x0 + (xf - x0) * time/Tf for time in timepts]).transpose(),
@@ -120,15 +120,15 @@
 # Turn on debug level logging so that we can see what the optimizer is doing
 logging.basicConfig(
     level=logging.DEBUG, filename="steering-integral_cost.log",
     filemode='w', force=True)
 
 # Compute the optimal control, setting step size for gradient calculation (eps)
 start_time = time.process_time()
-result1 = opt.solve_ocp(
+result1 = obc.solve_ocp(
     vehicle, timepts, x0, quad_cost, initial_guess=straight_line, log=True,
     # minimize_method='trust-constr',
     # minimize_options={'finite_diff_rel_step': 0.01},
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
 # If we are running CI tests, make sure we succeeded
@@ -154,32 +154,32 @@
 # cost on the inputs, resuling in a more graduate lane change.
 #
 # We also set the solver explicitly.
 #
 print("\nApproach 2: input cost and constraints plus terminal cost")
 
 # Add input constraint, input cost, terminal cost
-constraints = [ opt.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
-traj_cost = opt.quadratic_cost(vehicle, None, np.diag([0.1, 1]), u0=uf)
-term_cost = opt.quadratic_cost(vehicle, np.diag([1, 10, 10]), None, x0=xf)
+constraints = [ obc.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
+traj_cost = obc.quadratic_cost(vehicle, None, np.diag([0.1, 1]), u0=uf)
+term_cost = obc.quadratic_cost(vehicle, np.diag([1, 10, 10]), None, x0=xf)
 
 # Change logging to keep less information
 logging.basicConfig(
     level=logging.INFO, filename="./steering-terminal_cost.log",
     filemode='w', force=True)
 
 # Use a straight line between initial and final position as initial guesss
 input_guess = np.outer(u0, np.ones((1, timepts.size)))
 state_guess = np.array([
     x0 + (xf - x0) * time/Tf for time in timepts]).transpose()
 straight_line = (state_guess, input_guess)
 
 # Compute the optimal control
 start_time = time.process_time()
-result2 = opt.solve_ocp(
+result2 = obc.solve_ocp(
     vehicle, timepts, x0, traj_cost, constraints, terminal_cost=term_cost,
     initial_guess=straight_line, log=True,
     # minimize_method='SLSQP', minimize_options={'eps': 0.01}
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
 # If we are running CI tests, make sure we succeeded
@@ -203,27 +203,27 @@
 # with a terminal *constraint* on the state.  If a solution is found,
 # it guarantees we get to exactly the final state.
 #
 print("\nApproach 3: terminal constraints")
 
 # Input cost and terminal constraints
 R = np.diag([1, 1])                 # minimize applied inputs
-cost3 = opt.quadratic_cost(vehicle, np.zeros((3,3)), R, u0=uf)
+cost3 = obc.quadratic_cost(vehicle, np.zeros((3,3)), R, u0=uf)
 constraints = [
-    opt.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
-terminal = [ opt.state_range_constraint(vehicle, xf, xf) ]
+    obc.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
+terminal = [ obc.state_range_constraint(vehicle, xf, xf) ]
 
 # Reset logging to its default values
 logging.basicConfig(
     level=logging.DEBUG, filename="./steering-terminal_constraint.log",
     filemode='w', force=True)
 
 # Compute the optimal control
 start_time = time.process_time()
-result3 = opt.solve_ocp(
+result3 = obc.solve_ocp(
     vehicle, timepts, x0, cost3, constraints,
     terminal_constraints=terminal, initial_guess=straight_line, log=False,
     # solve_ivp_kwargs={'atol': 1e-3, 'rtol': 1e-2},
     # minimize_method='trust-constr',
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
@@ -250,15 +250,15 @@
 # for a much more time resolved set of inputs.
 
 print("\nApproach 4: Bezier basis")
 import control.flatsys as flat
 
 # Compute the optimal control
 start_time = time.process_time()
-result4 = opt.solve_ocp(
+result4 = obc.solve_ocp(
     vehicle, timepts, x0, quad_cost,
     constraints,
     terminal_constraints=terminal,
     initial_guess=straight_line,
     basis=flat.BezierFamily(6, T=Tf),
     # solve_ivp_kwargs={'method': 'RK45', 'atol': 1e-2, 'rtol': 1e-2},
     # solve_ivp_kwargs={'atol': 1e-3, 'rtol': 1e-2},
```

### Comparing `control-0.9.3.post2/doc/steering.ipynb` & `control-0.9.4/doc/steering.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/doc/stochresp.ipynb` & `control-0.9.4/doc/stochresp.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/bode-and-nyquist-plots.ipynb` & `control-0.9.4/examples/bode-and-nyquist-plots.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/check-controllability-and-observability.py` & `control-0.9.4/examples/check-controllability-and-observability.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/cruise-control.py` & `control-0.9.4/examples/cruise-control.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/cruise.ipynb` & `control-0.9.4/examples/cruise.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/describing_functions.ipynb` & `control-0.9.4/examples/describing_functions.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/genswitch.py` & `control-0.9.4/examples/genswitch.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/kincar-flatsys.py` & `control-0.9.4/examples/kincar-flatsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # kinematic (bicycle) model of a car changing lanes.
 
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import control as ct
 import control.flatsys as fs
-import control.optimal as opt
+import control.optimal as obc
 
 #
 # System model and utility functions
 #
 
 # Function to take states, inputs and return the flat flag
 def vehicle_flat_forward(x, u, params={}):
@@ -143,15 +143,15 @@
 #
 
 # Define timepoints for evaluation plus basis function to use
 timepts = np.linspace(0, Tf, 10)
 basis = fs.PolyFamily(8)
 
 # Define the cost function (penalize lateral error and steering)
-traj_cost = opt.quadratic_cost(
+traj_cost = obc.quadratic_cost(
     vehicle_flat, np.diag([0, 0.1, 0]), np.diag([0.1, 1]), x0=xf, u0=uf)
 
 # Solve for an optimal solution
 traj2 = fs.point_to_point(
     vehicle_flat, timepts, x0, u0, xf, uf, cost=traj_cost, basis=basis,
 )
 xd, ud = traj2.eval(T)
@@ -164,15 +164,15 @@
 # Approach #3: optimal cost with trajectory constraints
 #
 # Resolve the problem with constraints on the inputs
 #
 
 # Constraint the input values
 constraints = [
-    opt.input_range_constraint(vehicle_flat, [8, -0.1], [12, 0.1]) ]
+    obc.input_range_constraint(vehicle_flat, [8, -0.1], [12, 0.1]) ]
 
 # TEST: Change the basis to use B-splines
 basis = fs.BSplineFamily([0, Tf/2, Tf], 6)
 
 # Solve for an optimal solution
 traj3 = fs.point_to_point(
     vehicle_flat, timepts, x0, u0, xf, uf, cost=traj_cost,
@@ -194,19 +194,19 @@
 #
 # Resolve the problem with constraints on the inputs and also replacing the
 # point to point problem with one using a terminal cost to set the final
 # state.
 #
 
 # Define the cost function (mainly penalize steering angle)
-traj_cost = opt.quadratic_cost(
+traj_cost = obc.quadratic_cost(
     vehicle_flat, None, np.diag([0.1, 10]), x0=xf, u0=uf)
 
 # Set terminal cost to bring us close to xf
-terminal_cost = opt.quadratic_cost(vehicle_flat, 1e3 * np.eye(3), None, x0=xf)
+terminal_cost = obc.quadratic_cost(vehicle_flat, 1e3 * np.eye(3), None, x0=xf)
 
 # Change the basis to use B-splines
 basis = fs.BSplineFamily([0, Tf/2, Tf], [4, 6], vars=2)
 
 # Use a straight line as an initial guess for the trajectory
 initial_guess = np.array(
     [x0[i] + (xf[i] - x0[i]) * timepts/Tf for i in (0, 1)])
```

### Comparing `control-0.9.3.post2/examples/kincar-fusion.ipynb` & `control-0.9.4/examples/kincar-fusion.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/mpc_aircraft.ipynb` & `control-0.9.4/examples/mpc_aircraft.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import control.optimal as obc\\n')], delete: [2]}}, 3: "*

 * *            "{'source': {insert: [(8, 'constraints = [obc.input_range_constraint(sys, [-5, -6], "*

 * *            "[5, 6])]\\n'), (13, 'cost = obc.quadratic_cost(model, Q, R, x0=xd, u0=ud)\\n'), (16, "*

 * *            "'ctrl = obc.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)')], "*

 * *            'delete: [16, 13, 8]}}}'}*

```diff
@@ -15,15 +15,15 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import control as ct\n",
                 "import numpy as np\n",
-                "import control.optimal as opt\n",
+                "import control.optimal as obc\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
@@ -66,23 +66,23 @@
                 "# steady state which can be added using \"reference\" filter\n",
                 "# model.u.with('reference');\n",
                 "# model.u.reference = us;\n",
                 "# model.y.with('reference');\n",
                 "# model.y.reference = ys;\n",
                 "\n",
                 "# provide constraints on the system signals\n",
-                "constraints = [opt.input_range_constraint(sys, [-5, -6], [5, 6])]\n",
+                "constraints = [obc.input_range_constraint(sys, [-5, -6], [5, 6])]\n",
                 "\n",
                 "# provide penalties on the system signals\n",
                 "Q = model.C.transpose() @ np.diag([10, 10, 10, 10]) @ model.C\n",
                 "R = np.diag([3, 2])\n",
-                "cost = opt.quadratic_cost(model, Q, R, x0=xd, u0=ud)\n",
+                "cost = obc.quadratic_cost(model, Q, R, x0=xd, u0=ud)\n",
                 "\n",
                 "# online MPC controller object is constructed with a horizon 6\n",
-                "ctrl = opt.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)"
+                "ctrl = obc.create_mpc_iosystem(model, np.arange(0, 6) * 0.2, cost, constraints)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
```

### Comparing `control-0.9.3.post2/examples/phaseplots.py` & `control-0.9.4/examples/phaseplots.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/pvtol-lqr-nested.ipynb` & `control-0.9.4/examples/pvtol-lqr-nested.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/pvtol-lqr.py` & `control-0.9.4/examples/pvtol-lqr.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/pvtol-nested-ss.py` & `control-0.9.4/examples/pvtol-nested-ss.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/pvtol-nested.py` & `control-0.9.4/examples/pvtol-nested.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/pvtol-outputfbk.ipynb` & `control-0.9.4/examples/pvtol-outputfbk.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995920762029509%*

 * *Differences: {"'cells'": "{4: {'outputs': {0: {'text': {insert: [(5, 'Object: pvtol_noisy\\n')], delete: "*

 * *            "[5]}}}, 'source': {insert: [(1, '# pvtol_noisy = pvtol w/ process disturbances and "*

 * *            "sensor noise\\n'), (2, 'from pvtol import pvtol, pvtol_noisy, plot_results\\n'), (20, "*

 * *            "'print(pvtol_noisy)')], delete: [20, 2, 1]}}, 8: {'source': {insert: [(33, '    "*

 * *            "inputs= pvtol_noisy.state_labels[0:3] \\\\\\n'), (34, '        + "*

 * *            "pvtol_noisy.input_labels[0:pvto […]*

```diff
@@ -72,25 +72,25 @@
                     "output_type": "stream",
                     "text": [
                         "Object: pvtol\n",
                         "Inputs (2): F1, F2, \n",
                         "Outputs (6): x0, x1, x2, x3, x4, x5, \n",
                         "States (6): x0, x1, x2, x3, x4, x5,  \n",
                         "\n",
-                        "Object: noisy_pvtol\n",
+                        "Object: pvtol_noisy\n",
                         "Inputs (7): F1, F2, Dx, Dy, Nx, Ny, Nth, \n",
                         "Outputs (6): x0, x1, x2, x3, x4, x5, \n",
                         "States (6): x0, x1, x2, x3, x4, x5, \n"
                     ]
                 }
             ],
             "source": [
                 "# pvtol = nominal system (no disturbances or noise)\n",
-                "# noisy_pvtol = pvtol w/ process disturbances and sensor noise\n",
-                "from pvtol import pvtol, noisy_pvtol, plot_results\n",
+                "# pvtol_noisy = pvtol w/ process disturbances and sensor noise\n",
+                "from pvtol import pvtol, pvtol_noisy, plot_results\n",
                 "\n",
                 "# Find the equiblirum point corresponding to the origin\n",
                 "xe, ue = ct.find_eqpt(\n",
                 "    pvtol, np.zeros(pvtol.nstates),\n",
                 "    np.zeros(pvtol.ninputs), [0, 0, 0, 0, 0, 0],\n",
                 "    iu=range(2, pvtol.ninputs), iy=[0, 1])\n",
                 "\n",
@@ -100,15 +100,15 @@
                 "    iu=range(2, pvtol.ninputs), iy=[0, 1])\n",
                 "\n",
                 "# Extract the linearization for use in LQR design\n",
                 "pvtol_lin = pvtol.linearize(xe, ue)\n",
                 "A, B = pvtol_lin.A, pvtol_lin.B\n",
                 "\n",
                 "print(pvtol, \"\\n\")\n",
-                "print(noisy_pvtol)"
+                "print(pvtol_noisy)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "be6ec05c",
             "metadata": {},
             "source": [
@@ -188,16 +188,16 @@
                 "\n",
                 "    # Return the derivative\n",
                 "    return np.hstack([xhatdot, Pdot.reshape(-1)])\n",
                 "\n",
                 "estimator = ct.NonlinearIOSystem(\n",
                 "    estimator_update, lambda t, x, u, params: x[0:pvtol.nstates],\n",
                 "    states=pvtol.nstates + pvtol.nstates**2,\n",
-                "    inputs= noisy_pvtol.state_labels[0:3] \\\n",
-                "        + noisy_pvtol.input_labels[0:pvtol.ninputs],\n",
+                "    inputs= pvtol_noisy.state_labels[0:3] \\\n",
+                "        + pvtol_noisy.input_labels[0:pvtol.ninputs],\n",
                 "    outputs=[f'xh{i}' for i in range(pvtol.nstates)],\n",
                 ")\n",
                 "print(estimator)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -237,15 +237,15 @@
                         "       1.31948923e-06 -3.16227766e+00  2.32324805e-07  2.36396241e-06\n",
                         "      -4.97998224e+00 -7.90913288e-08]]\n",
                         " \n",
                         "\n",
                         "Object: xh5\n",
                         "Inputs (13): xd[0], xd[1], xd[2], xd[3], xd[4], xd[5], ud[0], ud[1], Dx, Dy, Nx, Ny, Nth, \n",
                         "Outputs (14): x0, x1, x2, x3, x4, x5, F1, F2, xh0, xh1, xh2, xh3, xh4, xh5, \n",
-                        "States (48): noisy_pvtol_x0, noisy_pvtol_x1, noisy_pvtol_x2, noisy_pvtol_x3, noisy_pvtol_x4, noisy_pvtol_x5, sys[3]_x[0], sys[3]_x[1], sys[3]_x[2], sys[3]_x[3], sys[3]_x[4], sys[3]_x[5], sys[3]_x[6], sys[3]_x[7], sys[3]_x[8], sys[3]_x[9], sys[3]_x[10], sys[3]_x[11], sys[3]_x[12], sys[3]_x[13], sys[3]_x[14], sys[3]_x[15], sys[3]_x[16], sys[3]_x[17], sys[3]_x[18], sys[3]_x[19], sys[3]_x[20], sys[3]_x[21], sys[3]_x[22], sys[3]_x[23], sys[3]_x[24], sys[3]_x[25], sys[3]_x[26], sys[3]_x[27], sys[3]_x[28], sys[3]_x[29], sys[3]_x[30], sys[3]_x[31], sys[3]_x[32], sys[3]_x[33], sys[3]_x[34], sys[3]_x[35], sys[3]_x[36], sys[3]_x[37], sys[3]_x[38], sys[3]_x[39], sys[3]_x[40], sys[3]_x[41], \n"
+                        "States (48): pvtol_noisy_x0, pvtol_noisy_x1, pvtol_noisy_x2, pvtol_noisy_x3, pvtol_noisy_x4, pvtol_noisy_x5, sys[3]_x[0], sys[3]_x[1], sys[3]_x[2], sys[3]_x[3], sys[3]_x[4], sys[3]_x[5], sys[3]_x[6], sys[3]_x[7], sys[3]_x[8], sys[3]_x[9], sys[3]_x[10], sys[3]_x[11], sys[3]_x[12], sys[3]_x[13], sys[3]_x[14], sys[3]_x[15], sys[3]_x[16], sys[3]_x[17], sys[3]_x[18], sys[3]_x[19], sys[3]_x[20], sys[3]_x[21], sys[3]_x[22], sys[3]_x[23], sys[3]_x[24], sys[3]_x[25], sys[3]_x[26], sys[3]_x[27], sys[3]_x[28], sys[3]_x[29], sys[3]_x[30], sys[3]_x[31], sys[3]_x[32], sys[3]_x[33], sys[3]_x[34], sys[3]_x[35], sys[3]_x[36], sys[3]_x[37], sys[3]_x[38], sys[3]_x[39], sys[3]_x[40], sys[3]_x[41], \n"
                     ]
                 }
             ],
             "source": [
                 "# Shoot for 1 cm error in x, 10 cm error in y.  Try to keep the angle\n",
                 "# less than 5 degrees in making the adjustments.  Penalize side forces\n",
                 "# due to loss in efficiency.\n",
@@ -265,19 +265,19 @@
                 "# Construct the state feedback controller with estimated state as input\n",
                 "statefbk, _ = ct.create_statefbk_iosystem(pvtol, K, estimator=estimator)\n",
                 "print(statefbk, \"\\n\")\n",
                 "\n",
                 "# Reconstruct the control system with the noisy version of the process\n",
                 "# Create a closed loop system around the controller\n",
                 "clsys = ct.interconnect(\n",
-                "    [noisy_pvtol, statefbk, estimator],\n",
+                "    [pvtol_noisy, statefbk, estimator],\n",
                 "    inplist = statefbk.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    inputs = statefbk.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    outlist = pvtol.output_labels + statefbk.output_labels + estimator.output_labels,\n",
                 "    outputs = pvtol.output_labels + statefbk.output_labels + estimator.output_labels\n",
                 ")\n",
                 "print(clsys)"
             ]
         },
         {
@@ -445,19 +445,19 @@
                 }
             ],
             "source": [
                 "# Compute the full state feedback solution\n",
                 "lqr_ctrl, _ = ct.create_statefbk_iosystem(pvtol, K)\n",
                 "\n",
                 "lqr_clsys = ct.interconnect(\n",
-                "    [noisy_pvtol, lqr_ctrl],\n",
+                "    [pvtol_noisy, lqr_ctrl],\n",
                 "    inplist = lqr_ctrl.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    inputs = lqr_ctrl.input_labels[0:pvtol.ninputs + pvtol.nstates] + \\\n",
-                "        noisy_pvtol.input_labels[pvtol.ninputs:],\n",
+                "        pvtol_noisy.input_labels[pvtol.ninputs:],\n",
                 "    outlist = pvtol.output_labels + lqr_ctrl.output_labels,\n",
                 "    outputs = pvtol.output_labels + lqr_ctrl.output_labels\n",
                 ")\n",
                 "\n",
                 "# Put together the input for the system\n",
                 "U = np.vstack([\n",
                 "    np.outer(xe, np.ones_like(T)),      # xd\n",
```

### Comparing `control-0.9.3.post2/examples/pvtol.py` & `control-0.9.4/doc/pvtol.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import control as ct
 import control.flatsys as fs
 from math import sin, cos
 from warnings import warn
 
+__all__ = ['pvtol', 'pvtol_windy', 'pvtol_noisy']
+
 # PVTOL dynamics
-def pvtol_update(t, x, u, params):
+def _pvtol_update(t, x, u, params):
     # Get the parameter values
     m = params.get('m', 4.)             # mass of aircraft
     J = params.get('J', 0.0475)         # inertia around pitch axis
     r = params.get('r', 0.25)           # distance to center of force
     g = params.get('g', 9.8)            # gravitational constant
     c = params.get('c', 0.05)           # damping factor (estimated)
 
@@ -34,19 +36,19 @@
     # Dynamics
     xddot = (F1 * cos(theta) - F2 * sin(theta) - c * xdot) / m
     yddot = (F1 * sin(theta) + F2 * cos(theta) - m * g - c * ydot) / m
     thddot = (r * F1) / J
 
     return np.array([xdot, ydot, thetadot, xddot, yddot, thddot])
 
-def pvtol_output(t, x, u, params):
+def _pvtol_output(t, x, u, params):
     return x
 
 # PVTOL flat system mappings
-def pvtol_flat_forward(states, inputs, params={}):
+def _pvtol_flat_forward(states, inputs, params={}):
     # Get the parameter values
     m = params.get('m', 4.)             # mass of aircraft
     J = params.get('J', 0.0475)         # inertia around pitch axis
     r = params.get('r', 0.25)           # distance to center of force
     g = params.get('g', 9.8)            # gravitational constant
     c = params.get('c', 0.05)           # damping factor (estimated)
 
@@ -98,26 +100,22 @@
         + (-F1 * sin(theta) - F2 * cos(theta)) * (thdot**2 / m) \
         - 6 * (J / (m * r)) * sin(theta) * thdot**2 * thddot \
         - 3 * (J / (m * r)) * cos(theta) * thddot**2 \
         + (J / (m * r)) * cos(theta) * thdot**4
 
     return zflag
 
-def pvtol_flat_reverse(zflag, params={}):
+def _pvtol_flat_reverse(zflag, params={}):
     # Get the parameter values
     m = params.get('m', 4.)             # mass of aircraft
     J = params.get('J', 0.0475)         # inertia around pitch axis
     r = params.get('r', 0.25)           # distance to center of force
     g = params.get('g', 9.8)            # gravitational constant
     c = params.get('c', 0.05)           # damping factor (estimated)
 
-    # Create a vector to store the state and inputs
-    x = np.zeros(6)
-    u = np.zeros(2)
-
     # Given the flat variables, solve for the state
     theta = np.arctan2(-zflag[0][2],  zflag[1][2] + g)
     x = zflag[0][0] + (J / (m * r)) * sin(theta)
     y = zflag[1][0] - (J / (m * r)) * cos(theta)
 
     # Solve for thdot using next derivative
     thdot = (zflag[0][3] * cos(theta) + zflag[1][3] * sin(theta)) \
@@ -128,28 +126,25 @@
     ydot = zflag[1][1] + (J / (m * r)) * sin(theta) * thdot
 
     # Solve for the input forces
     F2 = m * ((zflag[1][2] + g) * cos(theta) - zflag[0][2] * sin(theta)
               + (J / (m * r)) * thdot**2)
     F1 = (J / r) * \
         (zflag[0][4] * cos(theta) + zflag[1][4] * sin(theta)
-#         - 2 * (zflag[0][3] * sin(theta) - zflag[1][3] * cos(theta)) * thdot \
          - 2 * zflag[0][3] * sin(theta) * thdot \
          + 2 * zflag[1][3] * cos(theta) * thdot \
-#         - (zflag[0][2] * cos(theta)
-#            + (zflag[1][2] + g) * sin(theta)) * thdot**2) \
          - zflag[0][2] * cos(theta) * thdot**2
          - (zflag[1][2] + g) * sin(theta) * thdot**2) \
         / (zflag[0][2] * sin(theta) - (zflag[1][2] + g) * cos(theta))
 
     return np.array([x, y, theta, xdot, ydot, thdot]), np.array([F1, F2])
 
 pvtol = fs.FlatSystem(
-    pvtol_flat_forward, pvtol_flat_reverse, name='pvtol',
-    updfcn=pvtol_update, outfcn=pvtol_output,
+    _pvtol_flat_forward, _pvtol_flat_reverse, name='pvtol',
+    updfcn=_pvtol_update, outfcn=_pvtol_output,
     states = [f'x{i}' for i in range(6)],
     inputs = ['F1', 'F2'],
     outputs = [f'x{i}' for i in range(6)],
     params = {
         'm': 4.,                # mass of aircraft
         'J': 0.0475,            # inertia around pitch axis
         'r': 0.25,              # distance to center of force
@@ -158,89 +153,93 @@
     }
 )
 
 #
 # PVTOL dynamics with wind
 # 
 
-def windy_update(t, x, u, params):
+def _windy_update(t, x, u, params):
     # Get the input vector
     F1, F2, d = u
 
     # Get the system response from the original dynamics
     xdot, ydot, thetadot, xddot, yddot, thddot = \
-        pvtol_update(t, x, u[0:2], params)
+        _pvtol_update(t, x, u[0:2], params)
 
     # Now add the wind term
     m = params.get('m', 4.)             # mass of aircraft
     xddot += d / m
 
     return np.array([xdot, ydot, thetadot, xddot, yddot, thddot])
 
-windy_pvtol = ct.NonlinearIOSystem(
-    windy_update, pvtol_output, name="windy_pvtol",
+pvtol_windy = ct.NonlinearIOSystem(
+    _windy_update, _pvtol_output, name="pvtol_windy",
     states = [f'x{i}' for i in range(6)],
     inputs = ['F1', 'F2', 'd'],
     outputs = [f'x{i}' for i in range(6)]
 )
 
 #
 # PVTOL dynamics with noise and disturbances
 # 
 
-def noisy_update(t, x, u, params):
+def _noisy_update(t, x, u, params):
     # Get the inputs
-    F1, F2, Dx, Dy, Nx, Ny, Nth = u
+    F1, F2, Dx, Dy = u[:4]
+    if u.shape[0] > 4:
+        Nx, Ny, Nth = u[4:]
+    else:
+        Nx, Ny, Nth = 0, 0, 0
 
     # Get the system response from the original dynamics
     xdot, ydot, thetadot, xddot, yddot, thddot = \
-        pvtol_update(t, x, u[0:2], params)
+        _pvtol_update(t, x, u[0:2], params)
 
     # Get the parameter values we need
     m = params.get('m', 4.)             # mass of aircraft
     J = params.get('J', 0.0475)         # inertia around pitch axis
 
     # Now add the disturbances
     xddot += Dx / m
     yddot += Dy / m
 
     return np.array([xdot, ydot, thetadot, xddot, yddot, thddot])
 
-def noisy_output(t, x, u, params):
+def _noisy_output(t, x, u, params):
     F1, F2, dx, Dy, Nx, Ny, Nth = u
     return x + np.array([Nx, Ny, Nth, 0, 0, 0])
 
-noisy_pvtol = ct.NonlinearIOSystem(
-    noisy_update, noisy_output, name="noisy_pvtol",
+pvtol_noisy = ct.NonlinearIOSystem(
+    _noisy_update, _noisy_output, name="pvtol_noisy",
     states = [f'x{i}' for i in range(6)],
     inputs = ['F1', 'F2'] + ['Dx', 'Dy'] + ['Nx', 'Ny', 'Nth'],
     outputs = pvtol.state_labels
 )
 
-# Add the linearitizations to the dynamics as additional methods
-def noisy_pvtol_A(x, u, params={}):
+# Add the linearitizations to the dynamics as an additional method
+def pvtol_noisy_A(x, u, params={}):
     # Get the parameter values we need
     m = params.get('m', 4.)             # mass of aircraft
     J = params.get('J', 0.0475)         # inertia around pitch axis
     c = params.get('c', 0.05)           # damping factor (estimated)
 
     # Get the angle and compute sine and cosine
-    theta = x[[2]]
+    theta = x[2]
     cth, sth = cos(theta), sin(theta)
 
     # Return the linearized dynamics matrix
     return np.array([
         [0, 0, 0, 1, 0, 0],
         [0, 0, 0, 0, 1, 0],
         [0, 0, 0, 0, 0, 1],
         [0, 0, (-u[0] * sth - u[1] * cth)/m, -c/m, 0, 0],
         [0, 0, ( u[0] * cth - u[1] * sth)/m, 0, -c/m, 0],
         [0, 0, 0, 0, 0, 0]
     ])
-pvtol.A = noisy_pvtol_A
+pvtol.A = pvtol_noisy_A
 
 # Plot the trajectory in xy coordinates
 def plot_results(t, x, u):
     # Set the size of the figure
     plt.figure(figsize=(10, 6))
 
     # Top plot: xy trajectory
@@ -298,18 +297,17 @@
         ]
     elif isinstance(test_points, tuple):
         # If we only got one test point, convert to a list
         test_points = [test_points]
 
     for x, u in test_points:
         x, u = np.array(x), np.array(u)
-        flag = pvtol_flat_forward(x, u)
-        xc, uc = pvtol_flat_reverse(flag)
+        flag = _pvtol_flat_forward(x, u)
+        xc, uc = _pvtol_flat_reverse(flag)
         print(f'({x}, {u}): ', end='')
         if verbose:
             print(f'\n  flag: {flag}')
             print(f'  check: ({xc}, {uc}): ', end='')
         if np.allclose(x, xc) and np.allclose(u, uc):
             print("OK")
         else:
             print("ERR")
-
```

### Comparing `control-0.9.3.post2/examples/robust_mimo.py` & `control-0.9.4/examples/robust_mimo.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/robust_siso.py` & `control-0.9.4/examples/robust_siso.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/rss-balred.py` & `control-0.9.4/examples/rss-balred.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/run_examples.sh` & `control-0.9.4/examples/run_examples.sh`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/run_notebooks.sh` & `control-0.9.4/examples/run_notebooks.sh`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/secord-matlab.py` & `control-0.9.4/examples/secord-matlab.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/singular-values-plot.ipynb` & `control-0.9.4/examples/singular-values-plot.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/sisotool_example.py` & `control-0.9.4/examples/sisotool_example.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/slycot-import-test.py` & `control-0.9.4/examples/slycot-import-test.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/steering-gainsched.py` & `control-0.9.4/examples/steering-gainsched.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/steering-optimal.py` & `control-0.9.4/examples/steering-optimal.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file works through an optimal control example for the vehicle
 # steering system.  It is intended to demonstrate the functionality for
 # optimal control module (control.optimal) in the python-control package.
 
 import numpy as np
 import math
 import control as ct
-import control.optimal as opt
+import control.optimal as obc
 import matplotlib.pyplot as plt
 import logging
 import time
 import os
 
 #
 # Vehicle steering dynamics
@@ -102,15 +102,15 @@
 # exerting too much control effort to achieve our goal.
 #
 print("Approach 1: standard quadratic cost")
 
 # Set up the cost functions
 Q = np.diag([.1, 10, .1])       # keep lateral error low
 R = np.diag([.1, 1])            # minimize applied inputs
-quad_cost = opt.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
+quad_cost = obc.quadratic_cost(vehicle, Q, R, x0=xf, u0=uf)
 
 # Define the time horizon (and spacing) for the optimization
 timepts = np.linspace(0, Tf, 20, endpoint=True)
 
 # Provide an initial guess
 straight_line = (
     np.array([x0 + (xf - x0) * time/Tf for time in timepts]).transpose(),
@@ -120,15 +120,15 @@
 # Turn on debug level logging so that we can see what the optimizer is doing
 logging.basicConfig(
     level=logging.DEBUG, filename="steering-integral_cost.log",
     filemode='w', force=True)
 
 # Compute the optimal control, setting step size for gradient calculation (eps)
 start_time = time.process_time()
-result1 = opt.solve_ocp(
+result1 = obc.solve_ocp(
     vehicle, timepts, x0, quad_cost, initial_guess=straight_line, log=True,
     # minimize_method='trust-constr',
     # minimize_options={'finite_diff_rel_step': 0.01},
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
 # If we are running CI tests, make sure we succeeded
@@ -154,32 +154,32 @@
 # cost on the inputs, resuling in a more graduate lane change.
 #
 # We also set the solver explicitly.
 #
 print("\nApproach 2: input cost and constraints plus terminal cost")
 
 # Add input constraint, input cost, terminal cost
-constraints = [ opt.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
-traj_cost = opt.quadratic_cost(vehicle, None, np.diag([0.1, 1]), u0=uf)
-term_cost = opt.quadratic_cost(vehicle, np.diag([1, 10, 10]), None, x0=xf)
+constraints = [ obc.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
+traj_cost = obc.quadratic_cost(vehicle, None, np.diag([0.1, 1]), u0=uf)
+term_cost = obc.quadratic_cost(vehicle, np.diag([1, 10, 10]), None, x0=xf)
 
 # Change logging to keep less information
 logging.basicConfig(
     level=logging.INFO, filename="./steering-terminal_cost.log",
     filemode='w', force=True)
 
 # Use a straight line between initial and final position as initial guesss
 input_guess = np.outer(u0, np.ones((1, timepts.size)))
 state_guess = np.array([
     x0 + (xf - x0) * time/Tf for time in timepts]).transpose()
 straight_line = (state_guess, input_guess)
 
 # Compute the optimal control
 start_time = time.process_time()
-result2 = opt.solve_ocp(
+result2 = obc.solve_ocp(
     vehicle, timepts, x0, traj_cost, constraints, terminal_cost=term_cost,
     initial_guess=straight_line, log=True,
     # minimize_method='SLSQP', minimize_options={'eps': 0.01}
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
 # If we are running CI tests, make sure we succeeded
@@ -203,27 +203,27 @@
 # with a terminal *constraint* on the state.  If a solution is found,
 # it guarantees we get to exactly the final state.
 #
 print("\nApproach 3: terminal constraints")
 
 # Input cost and terminal constraints
 R = np.diag([1, 1])                 # minimize applied inputs
-cost3 = opt.quadratic_cost(vehicle, np.zeros((3,3)), R, u0=uf)
+cost3 = obc.quadratic_cost(vehicle, np.zeros((3,3)), R, u0=uf)
 constraints = [
-    opt.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
-terminal = [ opt.state_range_constraint(vehicle, xf, xf) ]
+    obc.input_range_constraint(vehicle, [8, -0.1], [12, 0.1]) ]
+terminal = [ obc.state_range_constraint(vehicle, xf, xf) ]
 
 # Reset logging to its default values
 logging.basicConfig(
     level=logging.DEBUG, filename="./steering-terminal_constraint.log",
     filemode='w', force=True)
 
 # Compute the optimal control
 start_time = time.process_time()
-result3 = opt.solve_ocp(
+result3 = obc.solve_ocp(
     vehicle, timepts, x0, cost3, constraints,
     terminal_constraints=terminal, initial_guess=straight_line, log=False,
     # solve_ivp_kwargs={'atol': 1e-3, 'rtol': 1e-2},
     # minimize_method='trust-constr',
 )
 print("* Total time = %5g seconds\n" % (time.process_time() - start_time))
 
@@ -250,15 +250,15 @@
 # for a much more time resolved set of inputs.
 
 print("\nApproach 4: Bezier basis")
 import control.flatsys as flat
 
 # Compute the optimal control
 start_time = time.process_time()
-result4 = opt.solve_ocp(
+result4 = obc.solve_ocp(
     vehicle, timepts, x0, quad_cost,
     constraints,
     terminal_constraints=terminal,
     initial_guess=straight_line,
     basis=flat.BezierFamily(6, T=Tf),
     # solve_ivp_kwargs={'method': 'RK45', 'atol': 1e-2, 'rtol': 1e-2},
     # solve_ivp_kwargs={'atol': 1e-3, 'rtol': 1e-2},
```

### Comparing `control-0.9.3.post2/examples/steering.ipynb` & `control-0.9.4/examples/steering.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/stochresp.ipynb` & `control-0.9.4/examples/stochresp.ipynb`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/test-response.py` & `control-0.9.4/examples/test-response.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/tfvis.py` & `control-0.9.4/examples/tfvis.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/type2_type3.py` & `control-0.9.4/examples/type2_type3.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/vehicle-steering.png` & `control-0.9.4/examples/vehicle-steering.png`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/examples/vehicle.py` & `control-0.9.4/examples/vehicle.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/external/controls.py` & `control-0.9.4/external/controls.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/external/yottalab.py` & `control-0.9.4/external/yottalab.py`

 * *Files identical despite different names*

### Comparing `control-0.9.3.post2/pyproject.toml` & `control-0.9.4/pyproject.toml`

 * *Files identical despite different names*

