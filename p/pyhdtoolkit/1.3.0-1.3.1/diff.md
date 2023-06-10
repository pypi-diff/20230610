# Comparing `tmp/pyhdtoolkit-1.3.0.tar.gz` & `tmp/pyhdtoolkit-1.3.1.tar.gz`

## Comparing `pyhdtoolkit-1.3.0.tar` & `pyhdtoolkit-1.3.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/.codeclimate.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/.zenodo.json
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/version.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/__init__.py
--rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/_generators.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/constants.py
--rw-r--r--   0        0        0    14165 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/coupling.py
--rw-r--r--   0        0        0    17934 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/matching.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/parameters.py
--rw-r--r--   0        0        0    20681 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/ptc.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/track.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/tune.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/twiss.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/__init__.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_elements.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_errors.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_misc.py
--rw-r--r--   0        0        0    17925 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_powering.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_queries.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_routines.py
--rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_setup.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/maths/__init__.py
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/maths/nonconvex_phase_sync.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/maths/stats_fitting.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/maths/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/models/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/models/beam.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/models/htc.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/models/madx.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/optics/__init__.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/optics/beam.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/optics/ripken.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/optics/twiss.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/__init__.py
--rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/aperture.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/crossing.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/envelope.py
--rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/lattice.py
--rw-r--r--   0        0        0    20179 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/layout.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/phasespace.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/tune.py
--rw-r--r--   0        0        0    19836 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/utils.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/sbs/coupling.py
--rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/sbs/phase.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/__init__.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/paper.py
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/thesis.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/__init__.py
--rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/_misc.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/cmdline.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/contexts.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/executors.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/htc_monitor.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/logging.py
--rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/operations.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyhdtoolkit/utils/printutil.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/LICENSE
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/README.md
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/.codeclimate.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/.zenodo.json
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/__init__.py
+-rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/_generators.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/constants.py
+-rw-r--r--   0        0        0    14165 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/coupling.py
+-rw-r--r--   0        0        0    17934 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/matching.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/parameters.py
+-rw-r--r--   0        0        0    20681 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/ptc.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/track.py
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/tune.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/twiss.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/__init__.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_coupling.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_elements.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_errors.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_misc.py
+-rw-r--r--   0        0        0    17925 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_powering.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_queries.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_routines.py
+-rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_setup.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_twiss.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/maths/__init__.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/maths/nonconvex_phase_sync.py
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/maths/stats_fitting.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/maths/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/models/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/models/beam.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/models/htc.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/models/madx.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/optics/__init__.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/optics/beam.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/optics/ripken.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/optics/twiss.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/__init__.py
+-rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/aperture.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/crossing.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/envelope.py
+-rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/lattice.py
+-rw-r--r--   0        0        0    20361 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/layout.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/phasespace.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/tune.py
+-rw-r--r--   0        0        0    19836 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/utils.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/sbs/coupling.py
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/sbs/phase.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/__init__.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/paper.py
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/thesis.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/_misc.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/cmdline.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/contexts.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/executors.py
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/htc_monitor.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/logging.py
+-rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/operations.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyhdtoolkit/utils/printutil.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/README.md
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.1/PKG-INFO
```

### Comparing `pyhdtoolkit-1.3.0/.codeclimate.yml` & `pyhdtoolkit-1.3.1/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/Makefile` & `pyhdtoolkit-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/__init__.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/version.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 
 
 def version_info() -> str:
     """Debug convenience function to give version, platform and runtime information."""
     import platform
     import sys
```

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/_generators.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/_generators.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/constants.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/constants.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/coupling.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/matching.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/matching.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/parameters.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/parameters.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/ptc.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/ptc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/track.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/track.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/tune.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/tune.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/twiss.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/utils.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/__init__.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_elements.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_elements.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_errors.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_errors.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_misc.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_misc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_powering.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_powering.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_queries.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_queries.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_routines.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_routines.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_setup.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_setup.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/cpymadtools/lhc/_twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/maths/nonconvex_phase_sync.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/maths/nonconvex_phase_sync.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/maths/stats_fitting.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/maths/stats_fitting.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/maths/utils.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/maths/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/models/beam.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/models/beam.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/models/htc.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/models/htc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/models/madx.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/models/madx.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/optics/beam.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/optics/beam.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/optics/ripken.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/optics/ripken.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/optics/twiss.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/optics/twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/aperture.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/aperture.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/crossing.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/crossing.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/envelope.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/envelope.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/lattice.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/lattice.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/layout.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,20 @@
     dipoles_df = element_dfs["dipoles"]
     quadrupoles_df = element_dfs["quadrupoles"]
     sextupoles_df = element_dfs["sextupoles"]
     octupoles_df = element_dfs["octupoles"]
     bpms_df = element_dfs["bpms"]
 
     logger.trace("Determining the ylimits for k0l and k1l patches")
+    # Assume lattice doesnt mix 'k0l' and 'angle' for dipoles powering
+    dipoles_power_column = "k0l" if dipoles_df.k0l.any() else "angle"
     k0l_lim = (
         _ylim_from_input(k0l_lim, "k0l_lim")
         if k0l_lim is not None
-        else _determine_default_knl_lim(dipoles_df, col="k0l", coeff=2)
+        else _determine_default_knl_lim(dipoles_df, col=dipoles_power_column, coeff=2)
     )
     k1l_lim = (
         _ylim_from_input(k1l_lim, "k1l_lim")
         if k1l_lim is not None
         else _determine_default_knl_lim(quadrupoles_df, col="k1l", coeff=1.3)
     )
 
@@ -178,15 +180,15 @@
     dipole_patches_axis.grid(False)
 
     if plot_dipoles:  # beware 'sbend' and 'rbend' have an 'angle' value and not a 'k0l'
         logger.trace("Plotting dipole patches")
         plotted_elements = 0  # will help us not declare a label for legend at every patch
         for dipole_name, dipole in dipoles_df.iterrows():
             logger.trace(f"Plotting dipole element '{dipole_name}'")
-            bend_value = dipole.k0l if dipole.k0l != 0 else dipole.angle
+            bend_value = dipole.k0l if dipole.k0l != 0 else dipole.angle  # check for each element
             _plot_lattice_series(
                 dipole_patches_axis,
                 dipole,
                 height=bend_value,
                 v_offset=bend_value / 2,
                 color="royalblue",
                 label="MB" if plotted_elements == 0 else None,  # avoid duplicating legend labels
```

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/phasespace.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/phasespace.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/tune.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/tune.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/utils.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/sbs/coupling.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/sbs/coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/sbs/phase.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/sbs/phase.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/__init__.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/paper.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/paper.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/plotting/styles/thesis.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/plotting/styles/thesis.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/__init__.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/_misc.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/cmdline.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/contexts.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/executors.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/executors.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/htc_monitor.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/htc_monitor.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/logging.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/operations.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/operations.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyhdtoolkit/utils/printutil.py` & `pyhdtoolkit-1.3.1/pyhdtoolkit/utils/printutil.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/.gitignore` & `pyhdtoolkit-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/LICENSE` & `pyhdtoolkit-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/README.md` & `pyhdtoolkit-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/pyproject.toml` & `pyhdtoolkit-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.0/PKG-INFO` & `pyhdtoolkit-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhdtoolkit
-Version: 1.3.0
+Version: 1.3.1
 Summary: An all-in-one toolkit package to ease my Python work in my PhD.
 Project-URL: homepage, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: repository, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: documentation, https://fsoubelet.github.io/PyhDToolkit
 Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/release.html
 Author-email: Felix Soubelet <felix.soubelet@cern.ch>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.3.0 Summary: An all-in-one
+Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.3.1 Summary: An all-in-one
 toolkit package to ease my Python work in my PhD. Project-URL: homepage, https:
 //github.com/fsoubelet/PyhDToolkit Project-URL: repository, https://github.com/
 fsoubelet/PyhDToolkit Project-URL: documentation, https://fsoubelet.github.io/
 PyhDToolkit Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/
 release.html Author-email: Felix Soubelet
 soubelet@cern.ch> License-Expression: MIT License-File: LICENSE Keywords:
 Accelerator Physics,Docker,PHD,Physics Simulation,Visualisation Classifier:
```

