# Comparing `tmp/qm-sim-0.1.1.tar.gz` & `tmp/qm-sim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm-sim-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "qm-sim-0.1.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `qm-sim-0.1.1.tar` & `qm-sim-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/build_package.yml
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.gitignore
--rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.gitmodules
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 qm-sim-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 qm-sim-0.1.1/LICENSE
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 qm-sim-0.1.1/README.md
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/make.bat
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1219 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/api.rst
--rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/contribution.rst
--rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/examples.rst
--rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/01_zero_potential.py
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/02_quadratic_potential.py
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/03_2D_potential.py
--rw-r--r--   0        0        0     1643 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/04_adiabatic_evolution.py
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/05_temporal_evolution.py
--rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/06_2D_temporal_evolution.py
--rw-r--r--   0        0        0     1405 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/07_hydrogen_atom.py
--rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 qm-sim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 qm-sim-0.1.1/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/__init__.py
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/CMakeLists.txt
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/__init__.py
--rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/CMakeLists.txt
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/__init__.py
--rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/eigensolver.hpp
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/scripts/generate_init.py
--rw-r--r--   0        0        0     2436 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/eigensolver.cpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/CMakeLists.txt
--rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp
--rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/__init__.py
--rw-r--r--   0        0        0     1342 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/pytorch_eigen.py
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/scipy_eigen.py
--rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/hamiltonian/__init__.py
--rw-r--r--   0        0        0    14888 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/hamiltonian/spatial_hamiltonian.py
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/nature_constants.py
--rw-r--r--   0        0        0     3571 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/plot.py
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/spatial_derivative/__init__.py
--rw-r--r--   0        0        0     6820 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/spatial_derivative/cartesian.py
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/__init__.py
--rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/base.py
--rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/crank_nicolson.py
--rw-r--r--   0        0        0     1582 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/leapfrog.py
--rw-r--r--   0        0        0     2114 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/scipy_solvers.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/__init__.py
--rw-r--r--   0        0        0     3655 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/scipy_backend.py
--rw-r--r--   0        0        0     3890 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/test_eigensolvers.py
--rw-r--r--   0        0        0     4630 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_hamiltonian.py
--rw-r--r--   0        0        0     3918 2022-11-09 12:37:21.000000 qm-sim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.2/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 qm-sim-0.1.2/.github/workflows/build_package.yml
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 qm-sim-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.2/.gitignore
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 qm-sim-0.1.2/.gitmodules
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 qm-sim-0.1.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 qm-sim-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 qm-sim-0.1.2/README.md
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1219 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/api.rst
+-rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/contribution.rst
+-rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 qm-sim-0.1.2/docs/source/usage.rst
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/01_zero_potential.py
+-rw-r--r--   0        0        0      592 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/02_quadratic_potential.py
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/03_2D_potential.py
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/04_adiabatic_evolution.py
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/05_temporal_evolution.py
+-rw-r--r--   0        0        0     1263 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/06_2D_temporal_evolution.py
+-rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 qm-sim-0.1.2/examples/07_hydrogen_atom.py
+-rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 qm-sim-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 qm-sim-0.1.2/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/__init__.py
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/__init__.py
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/CMakeLists.txt
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/__init__.py
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/include/eigensolver.hpp
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/scripts/generate_init.py
+-rw-r--r--   0        0        0     2436 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/src/eigensolver.cpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/wrapper/CMakeLists.txt
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp
+-rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/eigensolvers/__init__.py
+-rw-r--r--   0        0        0     1342 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/eigensolvers/pytorch_eigen.py
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/eigensolvers/scipy_eigen.py
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/hamiltonian/__init__.py
+-rw-r--r--   0        0        0    14583 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/hamiltonian/spatial_hamiltonian.py
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/nature_constants.py
+-rw-r--r--   0        0        0     3571 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/plot.py
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/spatial_derivative/__init__.py
+-rw-r--r--   0        0        0    11051 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/spatial_derivative/cartesian.py
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/temporal_solver/__init__.py
+-rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/temporal_solver/base.py
+-rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/temporal_solver/crank_nicolson.py
+-rw-r--r--   0        0        0     1582 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/temporal_solver/leapfrog.py
+-rw-r--r--   0        0        0     2114 2022-11-09 12:37:21.000000 qm-sim-0.1.2/src/qm_sim/temporal_solver/scipy_solvers.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.2/tests/test_eigensolvers/__init__.py
+-rw-r--r--   0        0        0     3655 2022-11-09 12:37:21.000000 qm-sim-0.1.2/tests/test_eigensolvers/scipy_backend.py
+-rw-r--r--   0        0        0     3890 2022-11-09 12:37:21.000000 qm-sim-0.1.2/tests/test_eigensolvers/test_eigensolvers.py
+-rw-r--r--   0        0        0     4630 2022-11-09 12:37:21.000000 qm-sim-0.1.2/tests/test_hamiltonian.py
+-rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 qm-sim-0.1.2/PKG-INFO
```

### Comparing `qm-sim-0.1.1/.github/workflows/build_docs.yml` & `qm-sim-0.1.2/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/.github/workflows/build_package.yml` & `qm-sim-0.1.2/.github/workflows/build_package.yml`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/.github/workflows/linting.yml` & `qm-sim-0.1.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/LICENSE` & `qm-sim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/README.md` & `qm-sim-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # QM_sim
 
-Python library for simulation of quantum mechanical systems.
+Python library for simulation of quantum mechanical systems. The documentation is available on [GitHub pages](https://viljarjf.github.io/QM_sim/).
 
 [![Build docs](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
 
 [//]: # (This is a comment. This comment should be on line 7. If this changes, also change the hard-coded line number for the start-line for the mdinclude at the top of docs/source/index.rst )
 
 ## Features 
 - 1D, 2D, and 3D systems
```

### Comparing `qm-sim-0.1.1/docs/Makefile` & `qm-sim-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/docs/make.bat` & `qm-sim-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/docs/source/_templates/custom-class-template.rst` & `qm-sim-0.1.2/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/docs/source/_templates/custom-module-template.rst` & `qm-sim-0.1.2/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/docs/source/conf.py` & `qm-sim-0.1.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'QM sim'
 copyright = '2023, Viljar Femoen'
 author = 'Viljar Femoen'
-release = '0.1.1'
+release = '0.1.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
```

### Comparing `qm-sim-0.1.1/docs/source/contribution.rst` & `qm-sim-0.1.2/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/docs/source/examples.rst` & `qm-sim-0.1.2/docs/source/usage.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,27 @@
-Examples
+Usage
 ========
 
+Installation
+------------
+
+To use QM sim, first install it using pip:
+
+.. code-block:: console
+
+    $ pip install qm-sim
+
+
+To run calculations on a GPU, install the PyTorch version for your system at the 
+`PyTorch website <https://pytorch.org/get-started/locally/>`_ as well
+
+
+Examples
+--------
+
 No potential
 ------------
 
 .. literalinclude:: ../../examples/01_zero_potential.py
    :language: python
 
 Quadratic potential
@@ -34,11 +51,11 @@
 Temporal evolution of a 2D system
 ---------------------------------
 
 .. literalinclude:: ../../examples/06_2D_temporal_evolution.py
    :language: python
 
 Hydrogen atom
----------------------------------
+-------------
 
 .. literalinclude:: ../../examples/07_hydrogen_atom.py
    :language: python
```

### Comparing `qm-sim-0.1.1/examples/02_quadratic_potential.py` & `qm-sim-0.1.2/examples/02_quadratic_potential.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 m = m_e         # Mass of the particle, here chosen as electron mass
 n = 4           # The amount of eigenstates to find
 
 # Set hamiltonian
 H = Hamiltonian(N, L, m)
 
 # Set potential
-x = np.linspace(-L/2, L/2, N)
+x, = H.get_coordinate_arrays()
 
 def V(t):
     k = 200
     return 1/2*(k+t)*x**2
 H.V = V
 
 # Plot
```

### Comparing `qm-sim-0.1.1/examples/03_2D_potential.py` & `qm-sim-0.1.2/examples/03_2D_potential.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/examples/05_temporal_evolution.py` & `qm-sim-0.1.2/examples/05_temporal_evolution.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 t_end = 10e-15          # Simulation time
 dt = 1e-17              # Simulation data storage stepsize
 
 # Initialize the hamiltonian
 H = Hamiltonian(N, L, m, temporal_scheme="leapfrog")
 
 # Set the potential to a quadratic potential oscilating from side to side
-z = np.linspace(-L/2, L/2, N)
+z, = H.get_coordinate_arrays()
 H.V = lambda t: 6*z**2 + 3*z*np.abs(z)*np.sin(4e15*t)
 
 # Plot
 H.plot_temporal(t_end, dt)
```

### Comparing `qm-sim-0.1.1/examples/06_2D_temporal_evolution.py` & `qm-sim-0.1.2/examples/06_2D_temporal_evolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 # Initialize the hamiltonian.
 H = Hamiltonian(N, L, m, temporal_scheme="scipy-Runge-Kutta 3(2)")
 
 # Set the potential. Use a cool elipse cross that rotates over time
 a = 2e-9
 b = 5e-9
-x = np.linspace(-L[0]/2, L[0]/2, N[0])
-y = np.linspace(-L[1]/2, L[1]/2, N[1])
-X, Y = np.meshgrid(x, y)
+X, Y = H.get_coordinate_arrays()
 def V(theta: float) -> np.ndarray:
     ct, st = np.cos(theta), np.sin(theta)
 
     V = np.ones(N) * e_0
     V[((X*ct + Y*st) / a)**2 + ((X*st - Y*ct) / b)**2 <= 1] = 0
     V[((X*ct + Y*st) / b)**2 + ((X*st - Y*ct) / a)**2 <= 1] = 0
```

### Comparing `qm-sim-0.1.1/examples/07_hydrogen_atom.py` & `qm-sim-0.1.2/examples/07_hydrogen_atom.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 nx, ny = 2, 2               # Used for the plot
 n = nx * ny                 # Number of orbitals to find
 
 # Initialize the hamiltonian.
 H = Hamiltonian(N, L, m)
 
 # Define the potential: -e^2 / (4*pi*𝜀_0*r)
-x, y, z = np.meshgrid(*(np.linspace(-L[i]/2, L[i]/2, N[i]) for i in range(3)))
+x, y, z = H.get_coordinate_arrays()
 r = (x**2 + y**2 + z**2)**0.5
 H.V = -e_0**2 / (4 * np.pi * 𝜀_0 * r)
 
 # Find a couple eigenvalues
 energies, orbitals = H.eigen(n)
 orbitals = np.abs(orbitals**2)
```

### Comparing `qm-sim-0.1.1/pyproject.toml` & `qm-sim-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qm_sim"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Viljar Femoen", email="author@example.com" },
 ]
 description = "Quantum mechanics simulation library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/CMakeLists.txt` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/scripts/generate_init.py` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/scripts/generate_init.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/eigensolver.cpp` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/src/eigensolver.cpp`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp` & `qm-sim-0.1.2/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/eigensolvers/__init__.py` & `qm-sim-0.1.2/src/qm_sim/eigensolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/eigensolvers/pytorch_eigen.py` & `qm-sim-0.1.2/src/qm_sim/eigensolvers/pytorch_eigen.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/eigensolvers/scipy_eigen.py` & `qm-sim-0.1.2/src/qm_sim/eigensolvers/scipy_eigen.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/hamiltonian/spatial_hamiltonian.py` & `qm-sim-0.1.2/src/qm_sim/hamiltonian/spatial_hamiltonian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 
 Real-space discretized Hamiltonian class, with solving and plotting functionality
 
 """
 
-from collections.abc import Iterable
 from typing import Any, Callable
 
 import numpy as np
 from scipy.sparse import dia_matrix
 from scipy.sparse.linalg import eigsh as adiabatic_eigsh
 from tqdm import tqdm
 
 from .. import plot
 from ..eigensolvers import get_eigensolver
 from ..nature_constants import h_bar
 from ..spatial_derivative import get_scheme_order
-from ..spatial_derivative.cartesian import laplacian, nabla
+from ..spatial_derivative.cartesian import (
+    CartesianDiscretization,
+    laplacian,
+    nabla,
+)
 from ..temporal_solver import TemporalSolver, get_temporal_solver
 
 
 class SpatialHamiltonian:
     def __init__(
         self,
         N: tuple[int] | int,
@@ -80,70 +83,53 @@
 
             - zero
             - periodic
 
             Defaults to "zero"
         :type boundary_condition: str, optional
         """
-        # 1D inputs
-        if isinstance(N, int):
-            N = (N,)
-        if isinstance(L, (float, int)):
-            L = (L,)
-
-        # Allow any iterable that can be converted to a tuple
-        if isinstance(N, Iterable):
-            N = tuple(N)
-        if isinstance(L, Iterable):
-            L = tuple(L)
-
-        # Check type
-        if not isinstance(N, tuple) or not all(isinstance(i, int) for i in N):
-            raise ValueError(f"Param `N` must be int or tuple of ints, got {type(N)}")
-        if not isinstance(L, tuple) or not all(isinstance(i, (float, int)) for i in L):
-            raise ValueError(f"Param `L` must be float or tuple, got {type(L)}")
-
-        if len(N) != len(L):
-            raise ValueError("`N`and `L`must have same length")
-
-        self.N = N
-        self.L = L
+        # Creating this object performs the necessary type checking
+        self.discretization = CartesianDiscretization(L, N)
+        self.N = self.discretization.N
+        self.L = self.discretization.L
+        self.deltas = self.discretization.dx
 
         self.eigensolver = get_eigensolver(eigensolver)
         if self.eigensolver is None:
             raise ValueError(f"Eigensolver {eigensolver} not found")
 
         order = get_scheme_order(spatial_scheme)
         if order is None:
             raise ValueError("Requested finite difference is invalid")
 
-        self._dim = len(N)
-        self.delta = [Li / Ni for Li, Ni in zip(L, N)]
-
         # Handle non-isotropic effective mass
         if isinstance(m, np.ndarray) and np.all(m == m.flat[0]):
             m = m.flatten()[0]
         if isinstance(m, np.ndarray):
             print("Warning: Continuity is NOT satisfied (yet) with non-isotropic mass")
             if m.shape != self.N:
                 raise ValueError(
                     f"Inconsistent shape of `m`: {m.shape}, should be {self.N}"
                 )
             m_inv = 1 / m.flatten()
 
-            _n = nabla(N, L, order=order, boundary_condition=boundary_condition)
-            _n2 = laplacian(N, L, order=order, boundary_condition=boundary_condition)
+            _n = nabla(
+                self.discretization, order=order, boundary_condition=boundary_condition
+            )
+            _n2 = laplacian(
+                self.discretization, order=order, boundary_condition=boundary_condition
+            )
 
             # nabla m_inv nabla + m_inv nabla^2
             _n.data *= _n @ m_inv  # First term
             _n2.data *= m_inv  # Second term
             self.mat = _n + _n2
         else:
             self.mat = laplacian(
-                N, L, order=order, boundary_condition=boundary_condition
+                self.discretization, order=order, boundary_condition=boundary_condition
             )
             self.mat *= 1 / m
 
         self._centerline_index = list(self.mat.offsets).index(0)
         self._default_data = None
 
         # Multiply the laplacian with the remaining factors
@@ -423,7 +409,14 @@
     def asarray(self) -> np.ndarray:
         """Return the data matrix as a dense array
 
         :return: Dense array of the discretized Hamiltonian
         :rtype: np.ndarray
         """
         return self.mat.toarray()
+
+    def get_coordinate_arrays(self) -> tuple[np.ndarray]:
+        return self.discretization.get_coordinate_arrays()
+
+    get_coordinate_arrays.__doc__ = (
+        CartesianDiscretization.get_coordinate_arrays.__doc__
+    )
```

### Comparing `qm-sim-0.1.1/src/qm_sim/nature_constants.py` & `qm-sim-0.1.2/src/qm_sim/nature_constants.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/plot.py` & `qm-sim-0.1.2/src/qm_sim/plot.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/temporal_solver/base.py` & `qm-sim-0.1.2/src/qm_sim/temporal_solver/base.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/temporal_solver/crank_nicolson.py` & `qm-sim-0.1.2/src/qm_sim/temporal_solver/crank_nicolson.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/temporal_solver/leapfrog.py` & `qm-sim-0.1.2/src/qm_sim/temporal_solver/leapfrog.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/src/qm_sim/temporal_solver/scipy_solvers.py` & `qm-sim-0.1.2/src/qm_sim/temporal_solver/scipy_solvers.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/tests/test_eigensolvers/scipy_backend.py` & `qm-sim-0.1.2/tests/test_eigensolvers/scipy_backend.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/tests/test_eigensolvers/test_eigensolvers.py` & `qm-sim-0.1.2/tests/test_eigensolvers/test_eigensolvers.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/tests/test_hamiltonian.py` & `qm-sim-0.1.2/tests/test_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qm-sim-0.1.1/PKG-INFO` & `qm-sim-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-sim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quantum mechanics simulation library
 Author-Email: Viljar Femoen <author@example.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 Provides-Extra: torch
 Provides-Extra: docs
 Provides-Extra: linting
 Description-Content-Type: text/markdown
 
 # QM_sim
 
-Python library for simulation of quantum mechanical systems.
+Python library for simulation of quantum mechanical systems. The documentation is available on [GitHub pages](https://viljarjf.github.io/QM_sim/).
 
 [![Build docs](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
 
 [//]: # (This is a comment. This comment should be on line 7. If this changes, also change the hard-coded line number for the start-line for the mdinclude at the top of docs/source/index.rst )
 
 ## Features 
 - 1D, 2D, and 3D systems
```

