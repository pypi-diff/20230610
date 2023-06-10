# Comparing `tmp/cibuildwheel-2.8.1.tar.gz` & `tmp/cibuildwheel-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cibuildwheel-2.8.1.tar", last modified: Mon Jul 18 20:43:00 2022, max compression
+gzip compressed data, was "cibuildwheel-2.9.0.tar", last modified: Thu Aug 11 18:44:37 2022, max compression
```

## Comparing `cibuildwheel-2.8.1.tar` & `cibuildwheel-2.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 20:43:00.317803 cibuildwheel-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    20894 2022-07-18 20:43:00.317803 cibuildwheel-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19564 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 20:43:00.313804 cibuildwheel-2.8.1/cibuildwheel/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11704 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/architecture.py
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/bashlex_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/extra.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/functools_cached_property_38.py
--rw-r--r--   0 runner    (1001) docker     (121)    17175 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/linux.py
--rw-r--r--   0 runner    (1001) docker     (121)     8748 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    24034 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/macos.py
--rw-r--r--   0 runner    (1001) docker     (121)    11751 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/oci_container.py
--rw-r--r--   0 runner    (1001) docker     (121)    22035 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/projectfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 20:43:00.313804 cibuildwheel-2.8.1/cibuildwheel/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    10711 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/build-platforms.toml
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python310.txt
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python311.txt
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python36.txt
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python37.txt
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python38.txt
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python39.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints.in
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/defaults.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/install_certifi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/pinned_docker_images.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/resources/virtualenv.toml
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)    20639 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    17043 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/cibuildwheel/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 20:43:00.313804 cibuildwheel-2.8.1/cibuildwheel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20894 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-18 20:43:00.000000 cibuildwheel-2.8.1/cibuildwheel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-07-18 20:43:00.317803 cibuildwheel-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 20:43:00.317803 cibuildwheel-2.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_0_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5288 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_abi_variants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_before_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_before_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_before_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_build_skip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_container_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_cpp_standards.py
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_dependency_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_emulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     5081 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_from_sdist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_macos_archs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_manylinuxXXXX_only.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_pep518.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_podman.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_pure_wheel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_same_wheel.py
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_subdir_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_troubleshooting.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-07-18 20:42:52.000000 cibuildwheel-2.8.1/test/test_wheel_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:37.974050 cibuildwheel-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    20906 2022-08-11 18:44:37.974050 cibuildwheel-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19626 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:37.970050 cibuildwheel-2.9.0/cibuildwheel/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11700 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/bashlex_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/functools_cached_property_38.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17200 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/linux.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8739 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24069 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/macos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11742 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/oci_container.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22428 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/projectfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:37.970050 cibuildwheel-2.9.0/cibuildwheel/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)    10717 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/build-platforms.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python310.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python311.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python36.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python37.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python38.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python39.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints.in
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/defaults.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/install_certifi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/pinned_docker_images.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/resources/virtualenv.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20573 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17049 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/cibuildwheel/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:37.970050 cibuildwheel-2.9.0/cibuildwheel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    20906 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-11 18:44:37.000000 cibuildwheel-2.9.0/cibuildwheel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-08-11 18:44:37.974050 cibuildwheel-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 18:44:37.974050 cibuildwheel-2.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_abi_variants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_before_all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_before_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_before_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_build_skip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_container_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_cpp_standards.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_dependency_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5117 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_from_sdist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_macos_archs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4895 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_manylinuxXXXX_only.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_pep518.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_podman.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_pure_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_same_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_subdir_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_troubleshooting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-11 18:44:30.000000 cibuildwheel-2.9.0/test/test_wheel_tag.py
```

### Comparing `cibuildwheel-2.8.1/LICENSE` & `cibuildwheel-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cibuildwheel-2.8.1/PKG-INFO` & `cibuildwheel-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: cibuildwheel
-Version: 2.8.1
+Version: 2.9.0
 Summary: Build Python wheels on CI with minimal configuration.
 Home-page: https://github.com/pypa/cibuildwheel
 Author: Joe Rickerby
 Author-email: joerick@mac.com
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/pypa/cibuildwheel#changelog
 Project-URL: Documentation, https://cibuildwheel.readthedocs.io/
 Keywords: ci,wheel,packaging,pypi,travis,appveyor,macos,linux,windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: bin
 Provides-Extra: mypy
 Provides-Extra: dev
 Provides-Extra: all
@@ -59,23 +58,22 @@
 |   | macOS Intel | macOS Apple Silicon | Windows 64bit | Windows 32bit | Windows Arm64 | manylinux<br/>musllinux x86_64 | manylinux<br/>musllinux i686 | manylinux<br/>musllinux aarch64 | manylinux<br/>musllinux ppc64le | manylinux<br/>musllinux s390x |
 |---------------|----|-----|-----|-----|-----|----|-----|----|-----|-----|
 | CPython 3.6   | ✅ | N/A | ✅  | ✅  | N/A | ✅  | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.7   | ✅ | N/A | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.8   | ✅ | ✅  | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.9   | ✅ | ✅  | ✅  | ✅  | ✅² | ✅³ | ✅ | ✅ | ✅  | ✅  |
 | CPython 3.10  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
-| CPython 3.11⁴ | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
+| CPython 3.11  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
 | PyPy 3.7 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.8 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.9 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 
 <sup>¹ PyPy is only supported for manylinux wheels.</sup><br>
 <sup>² Windows arm64 support is experimental.</sup><br>
 <sup>³ Alpine 3.14 and very briefly 3.15's default python3 [was not able to load](https://github.com/pypa/cibuildwheel/issues/934) musllinux wheels. This has been fixed; please upgrade the python package if using Alpine from before the fix.</sup><br>
-<sup>⁴ CPython 3.11 is available using the [CIBW_PRERELEASE_PYTHONS](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) option.</sup><br>
 
 - Builds manylinux, musllinux, macOS 10.9+, and Windows wheels for CPython and PyPy
 - Works on GitHub Actions, Azure Pipelines, Travis CI, AppVeyor, CircleCI, and GitLab CI
 - Bundles shared library dependencies on Linux and macOS through [auditwheel](https://github.com/pypa/auditwheel) and [delocate](https://github.com/matthew-brett/delocate)
 - Runs your library's tests against the wheel-installed version of your library
 
 See the [cibuildwheel 1 documentation](https://cibuildwheel.readthedocs.io/en/1.x/) if you need to build unsupported versions of Python, such as Python 2.
@@ -119,15 +117,15 @@
     steps:
       - uses: actions/checkout@v3
 
       # Used to host cibuildwheel
       - uses: actions/setup-python@v3
 
       - name: Install cibuildwheel
-        run: python -m pip install cibuildwheel==2.8.1
+        run: python -m pip install cibuildwheel==2.9.0
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         # to supply options, put them in 'env', like:
         # env:
         #   CIBW_SOME_OPTION: value
 
@@ -234,14 +232,23 @@
 Changelog
 =========
 
 <!-- START bin/update_readme_changelog.py -->
 
 <!-- this section was generated by bin/update_readme_changelog.py -- do not edit manually -->
 
+### v2.9.0
+
+_11 August 2022_
+
+- 🌟 CPython 3.11 wheels are now built by default - without the CIBW_PRERELEASE_PYTHONS flag. It's time to build and upload these wheels to PyPI! This release includes CPython 3.11.0rc1, which is guaranteed to be ABI compatible with the final release. (#1226)
+- ⚠️ Removed support for running cibuildwheel in Python 3.6. Python 3.6 is EOL. However, cibuildwheel continues to build CPython 3.6 wheels for the moment. (#1175)
+- ✨ Improved error messages when misspelling TOML options, suggesting close matches (#1205)
+- 🛠 When running on Apple Silicon (so far, an unsupported mode of operation), cibuildwheel no longer builds universal2 wheels by default - just arm64. See [#1204](https://github.com/pypa/cibuildwheel/issues/1204) for discussion. We hope to release official support for native builds on Apple Silicon soon! (#1217)
+
 ### v2.8.1
 
 _18 July 2022_
 
 - 🐛 Fix a bug when building CPython 3.8 wheels on an Apple Silicon machine where testing would always fail. cibuildwheel will no longer attempt to test the arm64 part of CPython 3.8 wheels because we use the x86_64 installer of CPython 3.8 due to its macOS system version backward-compatibility. See [#1169](https://github.com/pypa/cibuildwheel/pull/1169) for more details. (#1171)
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b4. (#1180)
 - 🛠 The GitHub Action will ensure a compatible version of Python is installed on the runner (#1114)
@@ -271,21 +278,14 @@
 
 ### v2.6.1
 
 _7 June 2022_
 
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b3
 
-### v2.6.0
-
-_25 May 2022_
-
-- 🌟 Added the ability to test building wheels on CPython 3.11! Because CPython 3.11 is in beta, these wheels should not be distributed, because they might not be compatible with the final release, but it's available to build for testing purposes. Use the flag [`--prerelease-pythons` or `CIBW_PRERELEASE_PYTHONS`](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) to test. This version of cibuildwheel includes CPython 3.11.0b1. (#1109)
-- 📚 Added an interactive diagram showing how cibuildwheel works to the [docs](https://cibuildwheel.readthedocs.io/en/stable/#how-it-works) (#1100)
-
 <!-- END bin/update_readme_changelog.py -->
 
 ---
 
 That's the last few versions.
 
 ℹ️ **Want more changelog? Head over to [the changelog page in the docs](https://cibuildwheel.readthedocs.io/en/stable/changelog/).**
```

### Comparing `cibuildwheel-2.8.1/README.md` & `cibuildwheel-2.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,23 +25,22 @@
 |   | macOS Intel | macOS Apple Silicon | Windows 64bit | Windows 32bit | Windows Arm64 | manylinux<br/>musllinux x86_64 | manylinux<br/>musllinux i686 | manylinux<br/>musllinux aarch64 | manylinux<br/>musllinux ppc64le | manylinux<br/>musllinux s390x |
 |---------------|----|-----|-----|-----|-----|----|-----|----|-----|-----|
 | CPython 3.6   | ✅ | N/A | ✅  | ✅  | N/A | ✅  | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.7   | ✅ | N/A | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.8   | ✅ | ✅  | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.9   | ✅ | ✅  | ✅  | ✅  | ✅² | ✅³ | ✅ | ✅ | ✅  | ✅  |
 | CPython 3.10  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
-| CPython 3.11⁴ | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
+| CPython 3.11  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
 | PyPy 3.7 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.8 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.9 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 
 <sup>¹ PyPy is only supported for manylinux wheels.</sup><br>
 <sup>² Windows arm64 support is experimental.</sup><br>
 <sup>³ Alpine 3.14 and very briefly 3.15's default python3 [was not able to load](https://github.com/pypa/cibuildwheel/issues/934) musllinux wheels. This has been fixed; please upgrade the python package if using Alpine from before the fix.</sup><br>
-<sup>⁴ CPython 3.11 is available using the [CIBW_PRERELEASE_PYTHONS](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) option.</sup><br>
 
 - Builds manylinux, musllinux, macOS 10.9+, and Windows wheels for CPython and PyPy
 - Works on GitHub Actions, Azure Pipelines, Travis CI, AppVeyor, CircleCI, and GitLab CI
 - Bundles shared library dependencies on Linux and macOS through [auditwheel](https://github.com/pypa/auditwheel) and [delocate](https://github.com/matthew-brett/delocate)
 - Runs your library's tests against the wheel-installed version of your library
 
 See the [cibuildwheel 1 documentation](https://cibuildwheel.readthedocs.io/en/1.x/) if you need to build unsupported versions of Python, such as Python 2.
@@ -85,15 +84,15 @@
     steps:
       - uses: actions/checkout@v3
 
       # Used to host cibuildwheel
       - uses: actions/setup-python@v3
 
       - name: Install cibuildwheel
-        run: python -m pip install cibuildwheel==2.8.1
+        run: python -m pip install cibuildwheel==2.9.0
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         # to supply options, put them in 'env', like:
         # env:
         #   CIBW_SOME_OPTION: value
 
@@ -200,14 +199,23 @@
 Changelog
 =========
 
 <!-- START bin/update_readme_changelog.py -->
 
 <!-- this section was generated by bin/update_readme_changelog.py -- do not edit manually -->
 
+### v2.9.0
+
+_11 August 2022_
+
+- 🌟 CPython 3.11 wheels are now built by default - without the CIBW_PRERELEASE_PYTHONS flag. It's time to build and upload these wheels to PyPI! This release includes CPython 3.11.0rc1, which is guaranteed to be ABI compatible with the final release. (#1226)
+- ⚠️ Removed support for running cibuildwheel in Python 3.6. Python 3.6 is EOL. However, cibuildwheel continues to build CPython 3.6 wheels for the moment. (#1175)
+- ✨ Improved error messages when misspelling TOML options, suggesting close matches (#1205)
+- 🛠 When running on Apple Silicon (so far, an unsupported mode of operation), cibuildwheel no longer builds universal2 wheels by default - just arm64. See [#1204](https://github.com/pypa/cibuildwheel/issues/1204) for discussion. We hope to release official support for native builds on Apple Silicon soon! (#1217)
+
 ### v2.8.1
 
 _18 July 2022_
 
 - 🐛 Fix a bug when building CPython 3.8 wheels on an Apple Silicon machine where testing would always fail. cibuildwheel will no longer attempt to test the arm64 part of CPython 3.8 wheels because we use the x86_64 installer of CPython 3.8 due to its macOS system version backward-compatibility. See [#1169](https://github.com/pypa/cibuildwheel/pull/1169) for more details. (#1171)
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b4. (#1180)
 - 🛠 The GitHub Action will ensure a compatible version of Python is installed on the runner (#1114)
@@ -237,21 +245,14 @@
 
 ### v2.6.1
 
 _7 June 2022_
 
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b3
 
-### v2.6.0
-
-_25 May 2022_
-
-- 🌟 Added the ability to test building wheels on CPython 3.11! Because CPython 3.11 is in beta, these wheels should not be distributed, because they might not be compatible with the final release, but it's available to build for testing purposes. Use the flag [`--prerelease-pythons` or `CIBW_PRERELEASE_PYTHONS`](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) to test. This version of cibuildwheel includes CPython 3.11.0b1. (#1109)
-- 📚 Added an interactive diagram showing how cibuildwheel works to the [docs](https://cibuildwheel.readthedocs.io/en/stable/#how-it-works) (#1100)
-
 <!-- END bin/update_readme_changelog.py -->
 
 ---
 
 That's the last few versions.
 
 ℹ️ **Want more changelog? Head over to [the changelog page in the docs](https://cibuildwheel.readthedocs.io/en/stable/changelog/).**
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/__main__.py` & `cibuildwheel-2.9.0/cibuildwheel/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from __future__ import annotations
+
 import argparse
 import os
 import shutil
 import sys
 import tarfile
 import tempfile
 import textwrap
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import List, Set, Union
 
 import cibuildwheel
 import cibuildwheel.linux
 import cibuildwheel.macos
 import cibuildwheel.util
 import cibuildwheel.windows
 from cibuildwheel.architecture import Architecture, allowed_architectures_check
@@ -253,15 +254,15 @@
                 assert_never(platform)
     finally:
         shutil.rmtree(tmp_path, ignore_errors=sys.platform.startswith("win"))
         if tmp_path.exists():
             log.warning(f"Can't delete temporary folder '{str(tmp_path)}'")
 
 
-def print_preamble(platform: str, options: Options, identifiers: List[str]) -> None:
+def print_preamble(platform: str, options: Options, identifiers: list[str]) -> None:
     print(
         textwrap.dedent(
             """
                  _ _       _ _   _       _           _
              ___|_| |_ _ _|_| |_| |_ _ _| |_ ___ ___| |
             |  _| | . | | | | | . | | | |   | -_| -_| |
             |___|_|___|___|_|_|___|_____|_|_|___|___|_|
@@ -283,21 +284,21 @@
         for warning in warnings:
             print("  " + warning)
 
     print("\nHere we go!\n")
 
 
 def get_build_identifiers(
-    platform: PlatformName, build_selector: BuildSelector, architectures: Set[Architecture]
-) -> List[str]:
-    python_configurations: Union[
-        List[cibuildwheel.linux.PythonConfiguration],
-        List[cibuildwheel.windows.PythonConfiguration],
-        List[cibuildwheel.macos.PythonConfiguration],
-    ]
+    platform: PlatformName, build_selector: BuildSelector, architectures: set[Architecture]
+) -> list[str]:
+    python_configurations: (
+        list[cibuildwheel.linux.PythonConfiguration]
+        | list[cibuildwheel.windows.PythonConfiguration]
+        | list[cibuildwheel.macos.PythonConfiguration]
+    )
 
     if platform == "linux":
         python_configurations = cibuildwheel.linux.get_python_configurations(
             build_selector, architectures
         )
     elif platform == "windows":
         python_configurations = cibuildwheel.windows.get_python_configurations(
@@ -309,15 +310,15 @@
         )
     else:
         assert_never(platform)
 
     return [config.identifier for config in python_configurations]
 
 
-def detect_warnings(*, options: Options, identifiers: List[str]) -> List[str]:
+def detect_warnings(*, options: Options, identifiers: list[str]) -> list[str]:
     warnings = []
 
     # warn about deprecated {python} and {pip}
     for option_name in ["test_command", "before_build"]:
         option_values = [getattr(options.build_options(i), option_name) for i in identifiers]
 
         if any(o and ("{python}" in o or "{pip}" in o) for o in option_values):
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/architecture.py` & `cibuildwheel-2.9.0/cibuildwheel/architecture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
 import functools
 import platform as platform_module
 import re
 from enum import Enum
-from typing import Set
 
 from .typing import Final, Literal, PlatformName, assert_never
 
 PRETTY_NAMES: Final = {"linux": "Linux", "macos": "macOS", "windows": "Windows"}
 
 
 @functools.total_ordering
@@ -28,19 +29,19 @@
 
     # windows archs
     x86 = "x86"
     AMD64 = "AMD64"
     ARM64 = "ARM64"
 
     # Allow this to be sorted
-    def __lt__(self, other: "Architecture") -> bool:
+    def __lt__(self, other: Architecture) -> bool:
         return self.value < other.value
 
     @staticmethod
-    def parse_config(config: str, platform: PlatformName) -> "Set[Architecture]":
+    def parse_config(config: str, platform: PlatformName) -> set[Architecture]:
         result = set()
         for arch_str in re.split(r"[\s,]+", config):
             if arch_str == "auto":
                 result |= Architecture.auto_archs(platform=platform)
             elif arch_str == "native":
                 result.add(Architecture(platform_module.machine()))
             elif arch_str == "all":
@@ -50,62 +51,58 @@
             elif arch_str == "auto32":
                 result |= Architecture.bitness_archs(platform=platform, bitness="32")
             else:
                 result.add(Architecture(arch_str))
         return result
 
     @staticmethod
-    def auto_archs(platform: PlatformName) -> "Set[Architecture]":
+    def auto_archs(platform: PlatformName) -> set[Architecture]:
         native_architecture = Architecture(platform_module.machine())
         result = {native_architecture}
 
         if platform == "linux" and native_architecture == Architecture.x86_64:
             # x86_64 machines can run i686 containers
             result.add(Architecture.i686)
 
         if platform == "windows" and native_architecture == Architecture.AMD64:
             result.add(Architecture.x86)
 
-        if platform == "macos" and native_architecture == Architecture.arm64:
-            # arm64 can build and test both archs of a universal2 wheel.
-            result.add(Architecture.universal2)
-
         return result
 
     @staticmethod
-    def all_archs(platform: PlatformName) -> "Set[Architecture]":
+    def all_archs(platform: PlatformName) -> set[Architecture]:
         all_archs_map = {
             "linux": {
                 Architecture.x86_64,
                 Architecture.i686,
                 Architecture.aarch64,
                 Architecture.ppc64le,
                 Architecture.s390x,
             },
             "macos": {Architecture.x86_64, Architecture.arm64, Architecture.universal2},
             "windows": {Architecture.x86, Architecture.AMD64, Architecture.ARM64},
         }
         return all_archs_map[platform]
 
     @staticmethod
-    def bitness_archs(platform: PlatformName, bitness: Literal["64", "32"]) -> "Set[Architecture]":
+    def bitness_archs(platform: PlatformName, bitness: Literal["64", "32"]) -> set[Architecture]:
         archs_32 = {Architecture.i686, Architecture.x86}
         auto_archs = Architecture.auto_archs(platform)
 
         if bitness == "64":
             return auto_archs - archs_32
         elif bitness == "32":
             return auto_archs & archs_32
         else:
             assert_never(bitness)
 
 
 def allowed_architectures_check(
     platform: PlatformName,
-    architectures: Set[Architecture],
+    architectures: set[Architecture],
 ) -> None:
 
     allowed_architectures = Architecture.all_archs(platform)
 
     msg = f"{PRETTY_NAMES[platform]} only supports {sorted(allowed_architectures)} at the moment."
 
     if platform != "linux":
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/bashlex_eval.py` & `cibuildwheel-2.9.0/cibuildwheel/bashlex_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+from __future__ import annotations
+
 import subprocess
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Optional, Sequence
+from typing import Callable, Dict, List, Sequence
 
 import bashlex
 
 # a function that takes a command and the environment, and returns the result
 EnvironmentExecutor = Callable[[List[str], Dict[str, str]], str]
 
 
-def local_environment_executor(command: List[str], env: Dict[str, str]) -> str:
-    return subprocess.run(
-        command, env=env, universal_newlines=True, stdout=subprocess.PIPE, check=True
-    ).stdout
+def local_environment_executor(command: list[str], env: dict[str, str]) -> str:
+    return subprocess.run(command, env=env, text=True, stdout=subprocess.PIPE, check=True).stdout
 
 
 @dataclass(frozen=True)
 class NodeExecutionContext:
-    environment: Dict[str, str]
+    environment: dict[str, str]
     input: str
     executor: EnvironmentExecutor
 
 
 def evaluate(
-    value: str, environment: Dict[str, str], executor: Optional[EnvironmentExecutor] = None
+    value: str, environment: dict[str, str], executor: EnvironmentExecutor | None = None
 ) -> str:
     if not value:
         # empty string evaluates to empty string
         # (but trips up bashlex)
         return ""
 
     command_node = bashlex.parsesingle(value)
@@ -99,15 +99,15 @@
         else:
             raise ValueError(f'Unsupported bash node in compound command: "{node.kind}"')
 
     return result
 
 
 def evaluate_nodes_as_simple_command(
-    nodes: List[bashlex.ast.node], context: NodeExecutionContext
+    nodes: list[bashlex.ast.node], context: NodeExecutionContext
 ) -> str:
     command = [evaluate_node(part, context=context) for part in nodes]
     return context.executor(command, context.environment)
 
 
 def evaluate_parameter_node(node: bashlex.ast.node, context: NodeExecutionContext) -> str:
     return context.environment.get(node.value, "")
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/environment.py` & `cibuildwheel-2.9.0/cibuildwheel/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 import dataclasses
-from typing import Any, Dict, List, Mapping, Optional, Sequence
+from typing import Any, Mapping, Sequence
 
 import bashlex
 
 from cibuildwheel.typing import Protocol
 
 from . import bashlex_eval
 
 
 class EnvironmentParseError(Exception):
     pass
 
 
-def split_env_items(env_string: str) -> List[str]:
+def split_env_items(env_string: str) -> list[str]:
     """Splits space-separated variable assignments into a list of individual assignments.
 
     >>> split_env_items('VAR=abc')
     ['VAR=abc']
     >>> split_env_items('VAR="a string" THING=3')
     ['VAR="a string"', 'THING=3']
     >>> split_env_items('VAR="a string" THING=\\'single "quotes"\\'')
@@ -43,16 +45,16 @@
 
 class EnvironmentAssignment(Protocol):
     name: str
 
     def evaluated_value(
         self,
         *,
-        environment: Dict[str, str],
-        executor: Optional[bashlex_eval.EnvironmentExecutor] = None,
+        environment: dict[str, str],
+        executor: bashlex_eval.EnvironmentExecutor | None = None,
     ) -> str:
         """Returns the value of this assignment, as evaluated in the environment"""
 
 
 class EnvironmentAssignmentRaw:
     """
     An environment variable - a simple name/value pair
@@ -80,40 +82,40 @@
         if not equals:
             raise EnvironmentParseError(assignment)
         self.name = name
         self.value = value
 
     def evaluated_value(
         self,
-        environment: Dict[str, str],
-        executor: Optional[bashlex_eval.EnvironmentExecutor] = None,
+        environment: dict[str, str],
+        executor: bashlex_eval.EnvironmentExecutor | None = None,
     ) -> str:
         return bashlex_eval.evaluate(self.value, environment=environment, executor=executor)
 
     def __repr__(self) -> str:
         return f"{self.name}={self.value}"
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, EnvironmentAssignmentBash):
             return self.name == other.name and self.value == other.value
         return False
 
 
 @dataclasses.dataclass
 class ParsedEnvironment:
-    assignments: List[EnvironmentAssignment]
+    assignments: list[EnvironmentAssignment]
 
     def __init__(self, assignments: Sequence[EnvironmentAssignment]) -> None:
         self.assignments = list(assignments)
 
     def as_dictionary(
         self,
         prev_environment: Mapping[str, str],
-        executor: Optional[bashlex_eval.EnvironmentExecutor] = None,
-    ) -> Dict[str, str]:
+        executor: bashlex_eval.EnvironmentExecutor | None = None,
+    ) -> dict[str, str]:
         environment = dict(**prev_environment)
 
         for assignment in self.assignments:
             value = assignment.evaluated_value(environment=environment, executor=executor)
             environment[assignment.name] = value
 
         return environment
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/extra.py` & `cibuildwheel-2.9.0/cibuildwheel/extra.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 These are utilities for the `/bin` scripts, not for the `cibuildwheel` program.
 """
 
+from __future__ import annotations
+
 from io import StringIO
-from typing import Dict, List
 
 from .typing import Protocol
 
 __all__ = ("Printable", "dump_python_configurations")
 
 
 class Printable(Protocol):
     def __str__(self) -> str:
         ...
 
 
-def dump_python_configurations(inp: Dict[str, Dict[str, List[Dict[str, Printable]]]]) -> str:
+def dump_python_configurations(inp: dict[str, dict[str, list[dict[str, Printable]]]]) -> str:
     output = StringIO()
     for header, values in inp.items():
         output.write(f"[{header}]\n")
         for inner_header, listing in values.items():
             output.write(f"{inner_header} = [\n")
             for item in listing:
                 output.write("  { ")
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/functools_cached_property_38.py` & `cibuildwheel-2.9.0/cibuildwheel/functools_cached_property_38.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+from __future__ import annotations
+
 from threading import RLock
-from typing import Any, Callable, Generic, Optional, Type, TypeVar, overload
+from typing import Any, Callable, Generic, TypeVar, overload
 
 __all__ = ["cached_property"]
 
 _NOT_FOUND = object()
 
 _T = TypeVar("_T")
 
 
 class cached_property(Generic[_T]):
     def __init__(self, func: Callable[[Any], _T]):
         self.func = func
-        self.attrname: Optional[str] = None
+        self.attrname: str | None = None
         self.__doc__ = func.__doc__
         self.lock = RLock()
 
-    def __set_name__(self, owner: Type[Any], name: str) -> None:
+    def __set_name__(self, owner: type[Any], name: str) -> None:
         if self.attrname is None:
             self.attrname = name
         elif name != self.attrname:
             raise TypeError(
                 "Cannot assign the same cached_property to two different names "
                 f"({self.attrname!r} and {name!r})."
             )
 
     @overload
-    def __get__(self, instance: None, owner: Optional[Type[Any]] = ...) -> "cached_property[_T]":
+    def __get__(self, instance: None, owner: type[Any] | None = ...) -> cached_property[_T]:
         ...
 
     @overload
-    def __get__(self, instance: object, owner: Optional[Type[Any]] = ...) -> _T:
+    def __get__(self, instance: object, owner: type[Any] | None = ...) -> _T:
         ...
 
-    def __get__(self, instance: Optional[object], owner: Optional[Type[Any]] = None) -> Any:
+    def __get__(self, instance: object | None, owner: type[Any] | None = None) -> Any:
         if instance is None:
             return self
         if self.attrname is None:
             raise TypeError(
                 "Cannot use cached_property instance without calling __set_name__ on it."
             )
         try:
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/linux.py` & `cibuildwheel-2.9.0/cibuildwheel/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import subprocess
 import sys
 import textwrap
 from dataclasses import dataclass
 from pathlib import Path, PurePath, PurePosixPath
-from typing import Iterator, List, Set, Tuple
+from typing import Iterator, Tuple
 
 from .architecture import Architecture
 from .logger import log
 from .oci_container import OCIContainer
 from .options import Options
 from .typing import OrderedDict, PathOrStr, assert_never
 from .util import (
@@ -31,23 +33,23 @@
     @property
     def path(self) -> PurePosixPath:
         return PurePosixPath(self.path_str)
 
 
 @dataclass(frozen=True)
 class BuildStep:
-    platform_configs: List[PythonConfiguration]
+    platform_configs: list[PythonConfiguration]
     platform_tag: str
     container_image: str
 
 
 def get_python_configurations(
     build_selector: BuildSelector,
-    architectures: Set[Architecture],
-) -> List[PythonConfiguration]:
+    architectures: set[Architecture],
+) -> list[PythonConfiguration]:
 
     full_python_configs = read_python_configs("linux")
 
     python_configurations = [PythonConfiguration(**item) for item in full_python_configs]
 
     # return all configurations whose arch is in our `architectures` set,
     # and match the build/skip rules
@@ -75,15 +77,15 @@
         build_options.manylinux_images[platform_arch]
         if platform_tag.startswith("manylinux")
         else build_options.musllinux_images[platform_arch]
     )
 
 
 def get_build_steps(
-    options: Options, python_configurations: List[PythonConfiguration]
+    options: Options, python_configurations: list[PythonConfiguration]
 ) -> Iterator[BuildStep]:
     """
     Groups PythonConfigurations into BuildSteps. Each BuildStep represents a
     separate container instance.
     """
     steps = OrderedDict[Tuple[str, str, str], BuildStep]()
 
@@ -106,15 +108,15 @@
 
     yield from steps.values()
 
 
 def build_in_container(
     *,
     options: Options,
-    platform_configs: List[PythonConfiguration],
+    platform_configs: list[PythonConfiguration],
     container: OCIContainer,
     container_project_path: PurePath,
     container_package_dir: PurePath,
 ) -> None:
     container_output_dir = PurePosixPath("/output")
 
     log.step("Copying project into container...")
@@ -136,21 +138,21 @@
         before_all_prepared = prepare_command(
             before_all_options.before_all,
             project=container_project_path,
             package=container_package_dir,
         )
         container.call(["sh", "-c", before_all_prepared], env=env)
 
-    built_wheels: List[PurePosixPath] = []
+    built_wheels: list[PurePosixPath] = []
 
     for config in platform_configs:
         log.build_start(config.identifier)
         build_options = options.build_options(config.identifier)
 
-        dependency_constraint_flags: List[PathOrStr] = []
+        dependency_constraint_flags: list[PathOrStr] = []
 
         if build_options.dependency_constraints:
             constraints_file = build_options.dependency_constraints.get_for_python_version(
                 config.version
             )
             container_constraints_file = PurePath("/constraints.txt")
 
@@ -391,15 +393,15 @@
             log.step_end_with_error(
                 f"Command {error.cmd} failed with code {error.returncode}. {error.stdout}"
             )
             troubleshoot(options, error)
             sys.exit(1)
 
 
-def _matches_prepared_command(error_cmd: List[str], command_template: str) -> bool:
+def _matches_prepared_command(error_cmd: list[str], command_template: str) -> bool:
     if len(error_cmd) < 3 or error_cmd[0:2] != ["sh", "-c"]:
         return False
     command_prefix = command_template.split("{", maxsplit=1)[0].strip()
     return error_cmd[2].startswith(command_prefix)
 
 
 def troubleshoot(options: Options, error: Exception) -> None:
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/logger.py` & `cibuildwheel-2.9.0/cibuildwheel/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import codecs
 import os
 import re
 import sys
 import time
-from typing import IO, AnyStr, Optional, Union
+from typing import IO, AnyStr
 
 from cibuildwheel.typing import Final
 from cibuildwheel.util import CIProvider, detect_ci_provider
 
 DEFAULT_FOLD_PATTERN: Final = ("{name}", "")
 FOLD_PATTERNS: Final = {
     "azure": ("##[group]{name}", "##[endgroup]"),
@@ -35,18 +37,18 @@
 }
 
 
 class Logger:
     fold_mode: str
     colors_enabled: bool
     unicode_enabled: bool
-    active_build_identifier: Optional[str] = None
-    build_start_time: Optional[float] = None
-    step_start_time: Optional[float] = None
-    active_fold_group_name: Optional[str] = None
+    active_build_identifier: str | None = None
+    build_start_time: float | None = None
+    step_start_time: float | None = None
+    active_fold_group_name: str | None = None
 
     def __init__(self) -> None:
         if sys.platform == "win32" and hasattr(sys.stdout, "reconfigure"):
             # the encoding on Windows can be a 1-byte charmap, but all CIs
             # support utf8, so we hardcode that
             sys.stdout.reconfigure(encoding="utf8")
 
@@ -116,26 +118,26 @@
             if success:
                 print(f"{c.green}{s.done} {c.end}{duration:.2f}s".rjust(78))
             else:
                 print(f"{c.red}{s.error} {c.end}{duration:.2f}s".rjust(78))
 
             self.step_start_time = None
 
-    def step_end_with_error(self, error: Union[BaseException, str]) -> None:
+    def step_end_with_error(self, error: BaseException | str) -> None:
         self.step_end(success=False)
         self.error(error)
 
     def warning(self, message: str) -> None:
         if self.fold_mode == "github":
             print(f"::warning::{message}\n", file=sys.stderr)
         else:
             c = self.colors
             print(f"{c.yellow}Warning{c.end}: {message}\n", file=sys.stderr)
 
-    def error(self, error: Union[BaseException, str]) -> None:
+    def error(self, error: BaseException | str) -> None:
         if self.fold_mode == "github":
             print(f"::error::{error}\n", file=sys.stderr)
         else:
             c = self.colors
             print(f"{c.bright_red}Error{c.end}: {error}\n", file=sys.stderr)
 
     def _start_fold_group(self, name: str) -> None:
@@ -170,19 +172,19 @@
         identifier = re.sub(r"[^A-Za-z\d_]+", "", identifier)
         # trim underscores
         identifier = identifier.strip("_")
         # lowercase, shorten
         return identifier.lower()[:20]
 
     @property
-    def colors(self) -> "Colors":
+    def colors(self) -> Colors:
         return Colors(enabled=self.colors_enabled)
 
     @property
-    def symbols(self) -> "Symbols":
+    def symbols(self) -> Symbols:
         return Symbols(unicode=self.unicode_enabled)
 
 
 def build_description_from_identifier(identifier: str) -> str:
     python_identifier, _, platform_identifier = identifier.partition("-")
 
     build_description = ""
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/macos.py` & `cibuildwheel-2.9.0/cibuildwheel/macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import functools
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, List, Sequence, Set, Tuple, cast
+from typing import Sequence, Tuple, cast
 
 from filelock import FileLock
 
 from .architecture import Architecture
 from .environment import ParsedEnvironment
 from .logger import log
 from .options import Options
@@ -33,43 +35,43 @@
     read_python_configs,
     shell,
     unwrap,
     virtualenv,
 )
 
 
-def get_macos_version() -> Tuple[int, int]:
+def get_macos_version() -> tuple[int, int]:
     """
     Returns the macOS major/minor version, as a tuple, e.g. (10, 15) or (11, 0)
 
     These tuples can be used in comparisons, e.g.
         (10, 14) <= (11, 0) == True
         (10, 14) <= (10, 16) == True
         (11, 2) <= (11, 0) != True
     """
     version_str, _, _ = platform.mac_ver()
     version = tuple(map(int, version_str.split(".")[:2]))
     return cast(Tuple[int, int], version)
 
 
-def get_macos_sdks() -> List[str]:
+def get_macos_sdks() -> list[str]:
     output = call("xcodebuild", "-showsdks", capture_stdout=True)
     return [m.group(1) for m in re.finditer(r"-sdk (macosx\S+)", output)]
 
 
 @dataclass(frozen=True)
 class PythonConfiguration:
     version: str
     identifier: str
     url: str
 
 
 def get_python_configurations(
-    build_selector: BuildSelector, architectures: Set[Architecture]
-) -> List[PythonConfiguration]:
+    build_selector: BuildSelector, architectures: set[Architecture]
+) -> list[PythonConfiguration]:
 
     full_python_configs = read_python_configs("macos")
 
     python_configurations = [PythonConfiguration(**item) for item in full_python_configs]
 
     # filter out configs that don't match any of the selected architectures
     python_configurations = [
@@ -130,15 +132,15 @@
 
 def setup_python(
     tmp: Path,
     python_configuration: PythonConfiguration,
     dependency_constraint_flags: Sequence[PathOrStr],
     environment: ParsedEnvironment,
     build_frontend: BuildFrontend,
-) -> Dict[str, str]:
+) -> dict[str, str]:
     tmp.mkdir()
     implementation_id = python_configuration.identifier.split("-")[0]
     log.step(f"Installing Python {implementation_id}...")
     if implementation_id.startswith("cp"):
         base_python = install_cpython(tmp, python_configuration.version, python_configuration.url)
     elif implementation_id.startswith("pp"):
         base_python = install_pypy(tmp, python_configuration.url)
@@ -291,15 +293,15 @@
             env = before_all_options.environment.as_dictionary(prev_environment=os.environ)
             env.setdefault("MACOSX_DEPLOYMENT_TARGET", "10.9")
             before_all_prepared = prepare_command(
                 before_all_options.before_all, project=".", package=before_all_options.package_dir
             )
             shell(before_all_prepared, env=env)
 
-        built_wheels: List[Path] = []
+        built_wheels: list[Path] = []
 
         for config in python_configurations:
             build_options = options.build_options(config.identifier)
             log.build_start(config.identifier)
 
             identifier_tmp_dir = tmp_path / config.identifier
             identifier_tmp_dir.mkdir()
@@ -414,15 +416,15 @@
                 if repaired_wheel.name in {wheel.name for wheel in built_wheels}:
                     raise AlreadyBuiltWheelError(repaired_wheel.name)
 
                 log.step_end()
 
             if build_options.test_command and build_options.test_selector(config.identifier):
                 machine_arch = platform.machine()
-                testing_archs: List[Literal["x86_64", "arm64"]]
+                testing_archs: list[Literal["x86_64", "arm64"]]
 
                 if config_is_arm64:
                     testing_archs = ["arm64"]
                 elif config_is_universal2:
                     testing_archs = ["x86_64", "arm64"]
                 else:
                     testing_archs = ["x86_64"]
@@ -501,15 +503,15 @@
                             arch_prefix = ["arch", "-x86_64"]
                         else:
                             msg = f"don't know how to emulate {testing_arch} on {machine_arch}"
                             raise RuntimeError(msg)
 
                     # define a custom 'call' function that adds the arch prefix each time
                     call_with_arch = functools.partial(call, *arch_prefix)
-                    shell_with_arch = functools.partial(shell, *arch_prefix)
+                    shell_with_arch = functools.partial(call, *arch_prefix, "/bin/sh", "-c")
 
                     # Use --no-download to ensure determinism by using seed libraries
                     # built into virtualenv
                     call_with_arch("python", "-m", "virtualenv", "--no-download", venv_dir, env=env)
 
                     virtualenv_env = env.copy()
                     virtualenv_env["PATH"] = os.pathsep.join(
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/oci_container.py` & `cibuildwheel-2.9.0/cibuildwheel/oci_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 import io
 import json
 import os
 import platform
 import shlex
 import shutil
 import subprocess
 import sys
 import uuid
 from pathlib import Path, PurePath, PurePosixPath
 from types import TracebackType
-from typing import IO, Dict, List, Optional, Sequence, Type, cast
+from typing import IO, Dict, Sequence, cast
 
 from cibuildwheel.util import CIProvider, detect_ci_provider
 
 from .typing import Literal, PathOrStr, PopenBytes
 
 ContainerEngine = Literal["docker", "podman"]
 
@@ -48,27 +50,27 @@
     bash_stdout: IO[bytes]
 
     def __init__(
         self,
         *,
         image: str,
         simulate_32_bit: bool = False,
-        cwd: Optional[PathOrStr] = None,
+        cwd: PathOrStr | None = None,
         engine: ContainerEngine = "docker",
     ):
         if not image:
             raise ValueError("Must have a non-empty image to run.")
 
         self.image = image
         self.simulate_32_bit = simulate_32_bit
         self.cwd = cwd
-        self.name: Optional[str] = None
+        self.name: str | None = None
         self.engine = engine
 
-    def __enter__(self) -> "OCIContainer":
+    def __enter__(self) -> OCIContainer:
 
         self.name = f"cibuildwheel-{uuid.uuid4()}"
 
         # work-around for Travis-CI PPC64le Docker runs since 2021:
         # this avoids network splits
         # https://github.com/pypa/cibuildwheel/issues/904
         # https://github.com/conda-forge/conda-smithy/pull/1520
@@ -118,17 +120,17 @@
             # to setup a workdir for a container running in podman.
             self.call(["mkdir", "-p", os.fspath(self.cwd)], cwd="/")
 
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
 
         self.bash_stdin.write(b"exit 0\n")
         self.bash_stdin.flush()
         self.process.wait(timeout=30)
         self.bash_stdin.close()
         self.bash_stdout.close()
@@ -213,15 +215,15 @@
                 shell=True,
                 check=True,
                 cwd=to_path,
             )
         else:
             raise KeyError(self.engine)
 
-    def glob(self, path: PurePosixPath, pattern: str) -> List[PurePosixPath]:
+    def glob(self, path: PurePosixPath, pattern: str) -> list[PurePosixPath]:
         glob_pattern = path.joinpath(pattern)
 
         path_strings = json.loads(
             self.call(
                 [
                     self.UTILITY_PYTHON,
                     "-c",
@@ -232,17 +234,17 @@
         )
 
         return [PurePosixPath(p) for p in path_strings]
 
     def call(
         self,
         args: Sequence[PathOrStr],
-        env: Optional[Dict[str, str]] = None,
+        env: dict[str, str] | None = None,
         capture_output: bool = False,
-        cwd: Optional[PathOrStr] = None,
+        cwd: PathOrStr | None = None,
     ) -> str:
 
         if cwd is None:
             # Podman does not start the a container in a specific working dir
             # so we always need to specify it when making calls.
             cwd = self.cwd
 
@@ -310,28 +312,28 @@
             output = ""
 
         if return_code != 0:
             raise subprocess.CalledProcessError(return_code, args, output)
 
         return output
 
-    def get_environment(self) -> Dict[str, str]:
+    def get_environment(self) -> dict[str, str]:
         env = json.loads(
             self.call(
                 [
                     self.UTILITY_PYTHON,
                     "-c",
                     "import sys, json, os; json.dump(os.environ.copy(), sys.stdout)",
                 ],
                 capture_output=True,
             )
         )
         return cast(Dict[str, str], env)
 
-    def environment_executor(self, command: List[str], environment: Dict[str, str]) -> str:
+    def environment_executor(self, command: list[str], environment: dict[str, str]) -> str:
         # used as an EnvironmentExecutor to evaluate commands and capture output
         return self.call(command, env=environment, capture_output=True)
 
     def debug_info(self) -> str:
         if self.engine == "podman":
             command = f"{self.engine} info --debug"
         else:
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/options.py` & `cibuildwheel-2.9.0/cibuildwheel/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,19 @@
+from __future__ import annotations
+
+import difflib
 import functools
 import os
 import sys
 import traceback
 from configparser import ConfigParser
 from contextlib import contextmanager
 from dataclasses import asdict, dataclass
 from pathlib import Path
-from typing import (
-    Any,
-    Dict,
-    Generator,
-    List,
-    Mapping,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-    cast,
-)
+from typing import Any, Dict, Generator, List, Mapping, Union, cast
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 from packaging.specifiers import SpecifierSet
@@ -46,46 +38,46 @@
     unwrap,
 )
 
 
 @dataclass
 class CommandLineArguments:
     platform: Literal["auto", "linux", "macos", "windows"]
-    archs: Optional[str]
+    archs: str | None
     output_dir: Path
     config_file: str
     package_dir: Path
     print_build_identifiers: bool
     allow_empty: bool
     prerelease_pythons: bool
 
 
 @dataclass(frozen=True)
 class GlobalOptions:
     package_dir: Path
     output_dir: Path
     build_selector: BuildSelector
     test_selector: TestSelector
-    architectures: Set[Architecture]
+    architectures: set[Architecture]
     container_engine: ContainerEngine
 
 
 @dataclass(frozen=True)
 class BuildOptions:
     globals: GlobalOptions
     environment: ParsedEnvironment
     before_all: str
-    before_build: Optional[str]
+    before_build: str | None
     repair_command: str
-    manylinux_images: Optional[Dict[str, str]]
-    musllinux_images: Optional[Dict[str, str]]
-    dependency_constraints: Optional[DependencyConstraints]
-    test_command: Optional[str]
-    before_test: Optional[str]
-    test_requires: List[str]
+    manylinux_images: dict[str, str] | None
+    musllinux_images: dict[str, str] | None
+    dependency_constraints: DependencyConstraints | None
+    test_command: str | None
+    before_test: str | None
+    test_requires: list[str]
     test_extras: str
     build_verbosity: int
     build_frontend: BuildFrontend
 
     @property
     def package_dir(self) -> Path:
         return self.globals.package_dir
@@ -99,25 +91,25 @@
         return self.globals.build_selector
 
     @property
     def test_selector(self) -> TestSelector:
         return self.globals.test_selector
 
     @property
-    def architectures(self) -> Set[Architecture]:
+    def architectures(self) -> set[Architecture]:
         return self.globals.architectures
 
 
 Setting = Union[Dict[str, str], List[str], str, int]
 
 
 @dataclass(frozen=True)
 class Override:
     select_pattern: str
-    options: Dict[str, Setting]
+    options: dict[str, Setting]
 
 
 MANYLINUX_OPTIONS = {f"manylinux-{build_platform}-image" for build_platform in MANYLINUX_ARCHS}
 MUSLLINUX_OPTIONS = {f"musllinux-{build_platform}-image" for build_platform in MUSLLINUX_ARCHS}
 DISALLOWED_OPTIONS = {
     "linux": {"dependency-versions"},
     "macos": MANYLINUX_OPTIONS | MUSLLINUX_OPTIONS,
@@ -130,15 +122,15 @@
     sep: str
 
 
 class ConfigOptionError(KeyError):
     pass
 
 
-def _dig_first(*pairs: Tuple[Mapping[str, Setting], str], ignore_empty: bool = False) -> Setting:
+def _dig_first(*pairs: tuple[Mapping[str, Setting], str], ignore_empty: bool = False) -> Setting:
     """
     Return the first dict item that matches from pairs of dicts and keys.
     Will throw a KeyError if missing.
 
     _dig_first((dict1, "key1"), (dict2, "key2"), ...)
     """
     if not pairs:
@@ -172,138 +164,146 @@
       from `config_file`, or from cibuildwheel/resources/defaults.toml. An
       error is thrown if there are any unexpected keys or sections in
       tool.cibuildwheel.
     """
 
     def __init__(
         self,
-        config_file_path: Optional[Path] = None,
+        config_file_path: Path | None = None,
         *,
         platform: PlatformName,
-        disallow: Optional[Dict[str, Set[str]]] = None,
+        disallow: dict[str, set[str]] | None = None,
     ) -> None:
         self.platform = platform
         self.disallow = disallow or {}
 
         # Open defaults.toml, loading both global and platform sections
         defaults_path = resources_dir / "defaults.toml"
         self.default_options, self.default_platform_options = self._load_file(defaults_path)
 
         # Load the project config file
-        config_options: Dict[str, Any] = {}
-        config_platform_options: Dict[str, Any] = {}
+        config_options: dict[str, Any] = {}
+        config_platform_options: dict[str, Any] = {}
 
         if config_file_path is not None:
             config_options, config_platform_options = self._load_file(config_file_path)
 
         # Validate project config
         for option_name in config_options:
-            if not self._is_valid_global_option(option_name):
-                raise ConfigOptionError(f'Option "{option_name}" not supported in a config file')
+            self._validate_global_option(option_name)
 
         for option_name in config_platform_options:
-            if not self._is_valid_platform_option(option_name):
-                raise ConfigOptionError(
-                    f'Option "{option_name}" not supported in the "{self.platform}" section'
-                )
+            self._validate_platform_option(option_name)
 
         self.config_options = config_options
         self.config_platform_options = config_platform_options
 
-        self.overrides: List[Override] = []
-        self.current_identifier: Optional[str] = None
+        self.overrides: list[Override] = []
+        self.current_identifier: str | None = None
 
         config_overrides = self.config_options.get("overrides")
 
         if config_overrides is not None:
             if not isinstance(config_overrides, list):
-                raise ConfigOptionError('"tool.cibuildwheel.overrides" must be a list')
+                raise ConfigOptionError("'tool.cibuildwheel.overrides' must be a list")
 
             for config_override in config_overrides:
                 select = config_override.pop("select", None)
 
                 if not select:
-                    raise ConfigOptionError('"select" must be set in an override')
+                    raise ConfigOptionError("'select' must be set in an override")
 
                 if isinstance(select, list):
                     select = " ".join(select)
 
                 self.overrides.append(Override(select, config_override))
 
-    def _is_valid_global_option(self, name: str) -> bool:
+    def _validate_global_option(self, name: str) -> None:
         """
-        Returns True if an option with this name is allowed in the
+        Raises an error if an option with this name is not allowed in the
         [tool.cibuildwheel] section of a config file.
         """
         allowed_option_names = self.default_options.keys() | PLATFORMS | {"overrides"}
 
-        return name in allowed_option_names
+        if name not in allowed_option_names:
+            msg = f"Option {name!r} not supported in a config file."
+            matches = difflib.get_close_matches(name, allowed_option_names, 1, 0.7)
+            if matches:
+                msg += f" Perhaps you meant {matches[0]!r}?"
+            raise ConfigOptionError(msg)
 
-    def _is_valid_platform_option(self, name: str) -> bool:
+    def _validate_platform_option(self, name: str) -> None:
         """
-        Returns True if an option with this name is allowed in the
+        Raises an error if an option with this name is not allowed in the
         [tool.cibuildwheel.<current-platform>] section of a config file.
         """
         disallowed_platform_options = self.disallow.get(self.platform, set())
         if name in disallowed_platform_options:
-            return False
+            msg = f"{name!r} is not allowed in {disallowed_platform_options}"
+            raise ConfigOptionError(msg)
 
         allowed_option_names = self.default_options.keys() | self.default_platform_options.keys()
 
-        return name in allowed_option_names
+        if name not in allowed_option_names:
+            msg = f"Option {name!r} not supported in the {self.platform!r} section"
+            matches = difflib.get_close_matches(name, allowed_option_names, 1, 0.7)
+            if matches:
+                msg += f" Perhaps you meant {matches[0]!r}?"
+            raise ConfigOptionError(msg)
 
-    def _load_file(self, filename: Path) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+    def _load_file(self, filename: Path) -> tuple[dict[str, Any], dict[str, Any]]:
         """
         Load a toml file, returns global and platform as separate dicts.
         """
         with filename.open("rb") as f:
             config = tomllib.load(f)
 
         global_options = config.get("tool", {}).get("cibuildwheel", {})
         platform_options = global_options.get(self.platform, {})
 
         return global_options, platform_options
 
     @property
-    def active_config_overrides(self) -> List[Override]:
+    def active_config_overrides(self) -> list[Override]:
         if self.current_identifier is None:
             return []
         return [
             o for o in self.overrides if selector_matches(o.select_pattern, self.current_identifier)
         ]
 
     @contextmanager
-    def identifier(self, identifier: Optional[str]) -> Generator[None, None, None]:
+    def identifier(self, identifier: str | None) -> Generator[None, None, None]:
         self.current_identifier = identifier
         try:
             yield
         finally:
             self.current_identifier = None
 
     def get(
         self,
         name: str,
         *,
         env_plat: bool = True,
-        sep: Optional[str] = None,
-        table: Optional[TableFmt] = None,
+        sep: str | None = None,
+        table: TableFmt | None = None,
         ignore_empty: bool = False,
     ) -> str:
         """
         Get and return the value for the named option from environment,
         configuration file, or the default. If env_plat is False, then don't
         accept platform versions of the environment variable. If this is an
         array it will be merged with "sep" before returning. If it is a table,
         it will be formatted with "table['item']" using {k} and {v} and merged
         with "table['sep']". Empty variables will not override if ignore_empty
         is True.
         """
 
         if name not in self.default_options and name not in self.default_platform_options:
-            raise ConfigOptionError(f"{name} must be in cibuildwheel/resources/defaults.toml file")
+            msg = f"{name!r} must be in cibuildwheel/resources/defaults.toml file to be accessed."
+            raise ConfigOptionError(msg)
 
         # Environment variable form
         envvar = f"CIBW_{name.upper().replace('-', '_')}"
         plat_envvar = f"{envvar}_{self.platform.upper()}"
 
         # later overrides take precedence over earlier ones, so reverse the list
         active_config_overrides = reversed(self.active_config_overrides)
@@ -319,20 +319,20 @@
             (self.default_platform_options, name),
             (self.default_options, name),
             ignore_empty=ignore_empty,
         )
 
         if isinstance(result, dict):
             if table is None:
-                raise ConfigOptionError(f"{name} does not accept a table")
+                raise ConfigOptionError(f"{name!r} does not accept a table")
             return table["sep"].join(table["item"].format(k=k, v=v) for k, v in result.items())
 
         if isinstance(result, list):
             if sep is None:
-                raise ConfigOptionError(f"{name} does not accept a list")
+                raise ConfigOptionError(f"{name!r} does not accept a list")
             return sep.join(result)
 
         if isinstance(result, int):
             return str(result)
 
         return result
 
@@ -345,29 +345,29 @@
         self.reader = OptionsReader(
             self.config_file_path,
             platform=platform,
             disallow=DISALLOWED_OPTIONS,
         )
 
     @property
-    def config_file_path(self) -> Optional[Path]:
+    def config_file_path(self) -> Path | None:
         args = self.command_line_arguments
 
         if args.config_file:
             return Path(format_safe(args.config_file, package=args.package_dir))
 
         # return pyproject.toml, if it's available
         pyproject_toml_path = Path(args.package_dir) / "pyproject.toml"
         if pyproject_toml_path.exists():
             return pyproject_toml_path
 
         return None
 
     @cached_property
-    def package_requires_python_str(self) -> Optional[str]:
+    def package_requires_python_str(self) -> str | None:
         args = self.command_line_arguments
         return get_requires_python_str(Path(args.package_dir))
 
     @property
     def globals(self) -> GlobalOptions:
         args = self.command_line_arguments
         package_dir = args.package_dir
@@ -379,15 +379,15 @@
 
         prerelease_pythons = args.prerelease_pythons or strtobool(
             os.environ.get("CIBW_PRERELEASE_PYTHONS", "0")
         )
 
         # This is not supported in tool.cibuildwheel, as it comes from a standard location.
         # Passing this in as an environment variable will override pyproject.toml, setup.cfg, or setup.py
-        requires_python_str: Optional[str] = (
+        requires_python_str: str | None = (
             os.environ.get("CIBW_PROJECT_REQUIRES_PYTHON") or self.package_requires_python_str
         )
         requires_python = None if requires_python_str is None else SpecifierSet(requires_python_str)
 
         build_selector = BuildSelector(
             build_config=build_config,
             skip_config=skip_config,
@@ -398,30 +398,30 @@
 
         archs_config_str = args.archs or self.reader.get("archs", sep=" ")
         architectures = Architecture.parse_config(archs_config_str, platform=self.platform)
 
         container_engine_str = self.reader.get("container-engine")
 
         if container_engine_str not in ["docker", "podman"]:
-            msg = f"cibuildwheel: Unrecognised container_engine '{container_engine_str}', only 'docker' and 'podman' are supported"
+            msg = f"cibuildwheel: Unrecognised container_engine {container_engine_str!r}, only 'docker' and 'podman' are supported"
             print(msg, file=sys.stderr)
             sys.exit(2)
 
         container_engine = cast(ContainerEngine, container_engine_str)
 
         return GlobalOptions(
             package_dir=package_dir,
             output_dir=output_dir,
             build_selector=build_selector,
             test_selector=test_selector,
             architectures=architectures,
             container_engine=container_engine,
         )
 
-    def build_options(self, identifier: Optional[str]) -> BuildOptions:
+    def build_options(self, identifier: str | None) -> BuildOptions:
         """
         Compute BuildOptions for a single run configuration.
         """
 
         with self.reader.identifier(identifier):
             before_all = self.reader.get("before-all", sep=" && ")
 
@@ -442,56 +442,56 @@
 
             build_frontend: BuildFrontend
             if build_frontend_str == "build":
                 build_frontend = "build"
             elif build_frontend_str == "pip":
                 build_frontend = "pip"
             else:
-                msg = f"cibuildwheel: Unrecognised build frontend '{build_frontend_str}', only 'pip' and 'build' are supported"
+                msg = f"cibuildwheel: Unrecognised build frontend {build_frontend_str!r}, only 'pip' and 'build' are supported"
                 print(msg, file=sys.stderr)
                 sys.exit(2)
 
             try:
                 environment = parse_environment(environment_config)
             except (EnvironmentParseError, ValueError):
                 print(
-                    f'cibuildwheel: Malformed environment option "{environment_config}"',
+                    f"cibuildwheel: Malformed environment option {environment_config!r}",
                     file=sys.stderr,
                 )
                 traceback.print_exc(None, sys.stderr)
                 sys.exit(2)
 
             # Pass through environment variables
             if self.platform == "linux":
                 for env_var_name in environment_pass:
                     try:
                         environment.add(env_var_name, os.environ[env_var_name])
                     except KeyError:
                         pass
 
             if dependency_versions == "pinned":
-                dependency_constraints: Optional[
+                dependency_constraints: None | (
                     DependencyConstraints
-                ] = DependencyConstraints.with_defaults()
+                ) = DependencyConstraints.with_defaults()
             elif dependency_versions == "latest":
                 dependency_constraints = None
             else:
                 dependency_versions_path = Path(dependency_versions)
                 dependency_constraints = DependencyConstraints(dependency_versions_path)
 
             if test_extras:
                 test_extras = f"[{test_extras}]"
 
             try:
                 build_verbosity = min(3, max(-3, int(build_verbosity_str)))
             except ValueError:
                 build_verbosity = 0
 
-            manylinux_images: Dict[str, str] = {}
-            musllinux_images: Dict[str, str] = {}
+            manylinux_images: dict[str, str] = {}
+            musllinux_images: dict[str, str] = {}
             if self.platform == "linux":
                 all_pinned_container_images = _get_pinned_container_images()
 
                 for build_platform in MANYLINUX_ARCHS:
                     pinned_images = all_pinned_container_images[build_platform]
 
                     config_value = self.reader.get(
@@ -535,15 +535,15 @@
                 environment=environment,
                 dependency_constraints=dependency_constraints,
                 manylinux_images=manylinux_images or None,
                 musllinux_images=musllinux_images or None,
                 build_frontend=build_frontend,
             )
 
-    def check_for_invalid_configuration(self, identifiers: List[str]) -> None:
+    def check_for_invalid_configuration(self, identifiers: list[str]) -> None:
         if self.platform in ["macos", "windows"]:
             before_all_values = {self.build_options(i).before_all for i in identifiers}
 
             if len(before_all_values) > 1:
                 raise ValueError(
                     unwrap(
                         f"""
@@ -558,15 +558,15 @@
         build_selector = self.globals.build_selector
         test_selector = self.globals.test_selector
 
         deprecated_selectors("CIBW_BUILD", build_selector.build_config, error=True)
         deprecated_selectors("CIBW_SKIP", build_selector.skip_config)
         deprecated_selectors("CIBW_TEST_SKIP", test_selector.skip_config)
 
-    def summary(self, identifiers: List[str]) -> str:
+    def summary(self, identifiers: list[str]) -> str:
         lines = [
             f"{option_name}: {option_value!r}"
             for option_name, option_value in sorted(asdict(self.globals).items())
         ]
 
         build_option_defaults = self.build_options(identifier=None)
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/projectfiles.py` & `cibuildwheel-2.9.0/cibuildwheel/projectfiles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import ast
 import sys
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 if sys.version_info < (3, 8):
@@ -20,15 +22,15 @@
 
     def get_constant(x: ast.Constant) -> Any:
         return x.value
 
 
 class Analyzer(ast.NodeVisitor):
     def __init__(self) -> None:
-        self.requires_python: Optional[str] = None
+        self.requires_python: str | None = None
 
     def visit(self, node: ast.AST) -> None:
         for inner_node in ast.walk(node):
             for child in ast.iter_child_nodes(inner_node):
                 child.parent = inner_node  # type: ignore[attr-defined]
         super().visit(node)
 
@@ -39,25 +41,25 @@
             # This will be Module -> Expr -> Call -> keyword
             if not hasattr(node.parent.parent.parent, "parent") and isinstance(  # type: ignore[attr-defined]
                 node.value, Constant
             ):
                 self.requires_python = get_constant(node.value)
 
 
-def setup_py_python_requires(content: str) -> Optional[str]:
+def setup_py_python_requires(content: str) -> str | None:
     try:
         tree = ast.parse(content)
         analyzer = Analyzer()
         analyzer.visit(tree)
         return analyzer.requires_python or None
     except Exception:  # pylint: disable=broad-except
         return None
 
 
-def get_requires_python_str(package_dir: Path) -> Optional[str]:
+def get_requires_python_str(package_dir: Path) -> str | None:
     """Return the python requires string from the most canonical source available, or None"""
 
     # Read in from pyproject.toml:project.requires-python
     try:
         with (package_dir / "pyproject.toml").open("rb") as f1:
             info = tomllib.load(f1)
         return str(info["project"]["requires-python"])
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/build-platforms.toml` & `cibuildwheel-2.9.0/cibuildwheel/resources/build-platforms.toml`

 * *Files 1% similar despite different names*

```diff
@@ -77,20 +77,20 @@
   { identifier = "cp37-macosx_x86_64", version = "3.7", url = "https://www.python.org/ftp/python/3.7.9/python-3.7.9-macosx10.9.pkg" },
   { identifier = "cp38-macosx_x86_64", version = "3.8", url = "https://www.python.org/ftp/python/3.8.10/python-3.8.10-macosx10.9.pkg" },
   { identifier = "cp38-macosx_arm64", version = "3.8", url = "https://www.python.org/ftp/python/3.8.10/python-3.8.10-macosx10.9.pkg" },
   { identifier = "cp38-macosx_universal2", version = "3.8", url = "https://www.python.org/ftp/python/3.8.10/python-3.8.10-macosx10.9.pkg" },
   { identifier = "cp39-macosx_x86_64", version = "3.9", url = "https://www.python.org/ftp/python/3.9.13/python-3.9.13-macos11.pkg" },
   { identifier = "cp39-macosx_arm64", version = "3.9", url = "https://www.python.org/ftp/python/3.9.13/python-3.9.13-macos11.pkg" },
   { identifier = "cp39-macosx_universal2", version = "3.9", url = "https://www.python.org/ftp/python/3.9.13/python-3.9.13-macos11.pkg" },
-  { identifier = "cp310-macosx_x86_64", version = "3.10", url = "https://www.python.org/ftp/python/3.10.5/python-3.10.5-macos11.pkg" },
-  { identifier = "cp310-macosx_arm64", version = "3.10", url = "https://www.python.org/ftp/python/3.10.5/python-3.10.5-macos11.pkg" },
-  { identifier = "cp310-macosx_universal2", version = "3.10", url = "https://www.python.org/ftp/python/3.10.5/python-3.10.5-macos11.pkg" },
-  { identifier = "cp311-macosx_x86_64", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0b4-macos11.pkg" },
-  { identifier = "cp311-macosx_arm64", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0b4-macos11.pkg" },
-  { identifier = "cp311-macosx_universal2", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0b4-macos11.pkg" },
+  { identifier = "cp310-macosx_x86_64", version = "3.10", url = "https://www.python.org/ftp/python/3.10.6/python-3.10.6-macos11.pkg" },
+  { identifier = "cp310-macosx_arm64", version = "3.10", url = "https://www.python.org/ftp/python/3.10.6/python-3.10.6-macos11.pkg" },
+  { identifier = "cp310-macosx_universal2", version = "3.10", url = "https://www.python.org/ftp/python/3.10.6/python-3.10.6-macos11.pkg" },
+  { identifier = "cp311-macosx_x86_64", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0rc1-macos11.pkg" },
+  { identifier = "cp311-macosx_arm64", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0rc1-macos11.pkg" },
+  { identifier = "cp311-macosx_universal2", version = "3.11", url = "https://www.python.org/ftp/python/3.11.0/python-3.11.0rc1-macos11.pkg" },
   { identifier = "pp37-macosx_x86_64", version = "3.7", url = "https://downloads.python.org/pypy/pypy3.7-v7.3.9-osx64.tar.bz2" },
   { identifier = "pp38-macosx_x86_64", version = "3.8", url = "https://downloads.python.org/pypy/pypy3.8-v7.3.9-osx64.tar.bz2" },
   { identifier = "pp39-macosx_x86_64", version = "3.9", url = "https://downloads.python.org/pypy/pypy3.9-v7.3.9-osx64.tar.bz2" },
 ]
 
 [windows]
 python_configurations = [
@@ -98,18 +98,18 @@
   { identifier = "cp36-win_amd64", version = "3.6.8", arch = "64" },
   { identifier = "cp37-win32", version = "3.7.9", arch = "32" },
   { identifier = "cp37-win_amd64", version = "3.7.9", arch = "64" },
   { identifier = "cp38-win32", version = "3.8.10", arch = "32" },
   { identifier = "cp38-win_amd64", version = "3.8.10", arch = "64" },
   { identifier = "cp39-win32", version = "3.9.13", arch = "32" },
   { identifier = "cp39-win_amd64", version = "3.9.13", arch = "64" },
-  { identifier = "cp310-win32", version = "3.10.5", arch = "32" },
-  { identifier = "cp310-win_amd64", version = "3.10.5", arch = "64" },
-  { identifier = "cp311-win32", version = "3.11.0-b4", arch = "32" },
-  { identifier = "cp311-win_amd64", version = "3.11.0-b4", arch = "64" },
+  { identifier = "cp310-win32", version = "3.10.6", arch = "32" },
+  { identifier = "cp310-win_amd64", version = "3.10.6", arch = "64" },
+  { identifier = "cp311-win32", version = "3.11.0-rc1", arch = "32" },
+  { identifier = "cp311-win_amd64", version = "3.11.0-rc1", arch = "64" },
   { identifier = "cp39-win_arm64", version = "3.9.10", arch = "ARM64" },
-  { identifier = "cp310-win_arm64", version = "3.10.5", arch = "ARM64" },
-  { identifier = "cp311-win_arm64", version = "3.11.0-b4", arch = "ARM64" },
+  { identifier = "cp310-win_arm64", version = "3.10.6", arch = "ARM64" },
+  { identifier = "cp311-win_arm64", version = "3.11.0-rc1", arch = "ARM64" },
   { identifier = "pp37-win_amd64", version = "3.7", arch = "64", url = "https://downloads.python.org/pypy/pypy3.7-v7.3.9-win64.zip" },
   { identifier = "pp38-win_amd64", version = "3.8", arch = "64", url = "https://downloads.python.org/pypy/pypy3.8-v7.3.9-win64.zip" },
   { identifier = "pp39-win_amd64", version = "3.9", arch = "64", url = "https://downloads.python.org/pypy/pypy3.9-v7.3.9-win64.zip" },
 ]
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python310.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python310.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #
 # This file is autogenerated by pip-compile with python 3.10
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.10
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
+filelock==3.8.0
     # via virtualenv
 platformdirs==2.5.2
     # via virtualenv
-six==1.16.0
-    # via virtualenv
 typing-extensions==4.3.0
     # via delocate
-virtualenv==20.15.1
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python311.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python311.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #
 # This file is autogenerated by pip-compile with python 3.11
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.11
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
+filelock==3.8.0
     # via virtualenv
 platformdirs==2.5.2
     # via virtualenv
-six==1.16.0
-    # via virtualenv
 typing-extensions==4.3.0
     # via delocate
-virtualenv==20.15.1
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python36.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python39.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 #
-# This file is autogenerated by pip-compile with python 3.6
+# This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.9
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.4.1
+filelock==3.8.0
     # via virtualenv
-importlib-metadata==4.8.3
+platformdirs==2.5.2
     # via virtualenv
-importlib-resources==5.4.0
-    # via virtualenv
-platformdirs==2.4.0
-    # via virtualenv
-six==1.16.0
-    # via virtualenv
-typing-extensions==4.1.1
-    # via
-    #   delocate
-    #   importlib-metadata
-virtualenv==20.15.1
+typing-extensions==4.3.0
+    # via delocate
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
-zipp==3.6.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==21.3.1
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==59.6.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python37.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 #
-# This file is autogenerated by pip-compile with python 3.7
+# This file is autogenerated by pip-compile with python 3.11
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.11
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
-    # via virtualenv
-importlib-metadata==4.12.0
+filelock==3.8.0
     # via virtualenv
 platformdirs==2.5.2
     # via virtualenv
-six==1.16.0
-    # via virtualenv
 typing-extensions==4.3.0
-    # via
-    #   delocate
-    #   importlib-metadata
-virtualenv==20.15.1
+    # via delocate
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
-zipp==3.8.1
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python38.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python38.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.8
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
+filelock==3.8.0
     # via virtualenv
 platformdirs==2.5.2
     # via virtualenv
-six==1.16.0
-    # via virtualenv
 typing-extensions==4.3.0
     # via delocate
-virtualenv==20.15.1
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints-python39.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python36.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
+# This file is autogenerated by pip-compile with python 3.6
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.6
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
+filelock==3.4.1
     # via virtualenv
-platformdirs==2.5.2
+importlib-metadata==4.8.3
     # via virtualenv
-six==1.16.0
+importlib-resources==5.4.0
     # via virtualenv
-typing-extensions==4.3.0
-    # via delocate
-virtualenv==20.15.1
+platformdirs==2.4.0
+    # via virtualenv
+typing-extensions==4.1.1
+    # via
+    #   delocate
+    #   importlib-metadata
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
+zipp==3.6.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==21.3.1
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==59.6.0
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/constraints.txt` & `cibuildwheel-2.9.0/cibuildwheel/resources/constraints-python37.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
+# This file is autogenerated by pip-compile with python 3.7
 # To update, run:
 #
-#    bin/update_dependencies.py
+#    nox -s update_constraints-3.7
 #
 delocate==0.10.2
     # via -r cibuildwheel/resources/constraints.in
 distlib==0.3.5
     # via virtualenv
-filelock==3.7.1
+filelock==3.8.0
     # via virtualenv
-platformdirs==2.5.2
+importlib-metadata==4.12.0
     # via virtualenv
-six==1.16.0
+platformdirs==2.5.2
     # via virtualenv
 typing-extensions==4.3.0
-    # via delocate
-virtualenv==20.15.1
+    # via
+    #   delocate
+    #   importlib-metadata
+virtualenv==20.16.3
     # via -r cibuildwheel/resources/constraints.in
 wheel==0.37.1
     # via
     #   -r cibuildwheel/resources/constraints.in
     #   delocate
+zipp==3.8.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==22.2.2
     # via -r cibuildwheel/resources/constraints.in
-setuptools==63.2.0
+setuptools==63.4.2
     # via -r cibuildwheel/resources/constraints.in
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/defaults.toml` & `cibuildwheel-2.9.0/cibuildwheel/resources/defaults.toml`

 * *Files identical despite different names*

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/install_certifi.py` & `cibuildwheel-2.9.0/cibuildwheel/resources/install_certifi.py`

 * *Files identical despite different names*

### Comparing `cibuildwheel-2.8.1/cibuildwheel/resources/pinned_docker_images.cfg` & `cibuildwheel-2.9.0/cibuildwheel/resources/pinned_docker_images.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [x86_64]
-manylinux1 = quay.io/pypa/manylinux1_x86_64:2022-07-17-f8ddacc
-manylinux2010 = quay.io/pypa/manylinux2010_x86_64:2022-07-17-51324db
-manylinux2014 = quay.io/pypa/manylinux2014_x86_64:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_x86_64:2022-07-17-51324db
-manylinux_2_28 = quay.io/pypa/manylinux_2_28_x86_64:2022-07-17-51324db
-musllinux_1_1 = quay.io/pypa/musllinux_1_1_x86_64:2022-07-17-51324db
+manylinux1 = quay.io/pypa/manylinux1_x86_64:2022-08-08-7292f33
+manylinux2010 = quay.io/pypa/manylinux2010_x86_64:2022-08-05-4535177
+manylinux2014 = quay.io/pypa/manylinux2014_x86_64:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_x86_64:2022-08-09-51a01be
+manylinux_2_28 = quay.io/pypa/manylinux_2_28_x86_64:2022-08-09-51a01be
+musllinux_1_1 = quay.io/pypa/musllinux_1_1_x86_64:2022-08-09-51a01be
 
 [i686]
-manylinux1 = quay.io/pypa/manylinux1_i686:2022-07-17-f8ddacc
-manylinux2010 = quay.io/pypa/manylinux2010_i686:2022-07-17-51324db
-manylinux2014 = quay.io/pypa/manylinux2014_i686:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_i686:2022-07-17-51324db
-musllinux_1_1 = quay.io/pypa/musllinux_1_1_i686:2022-07-17-51324db
+manylinux1 = quay.io/pypa/manylinux1_i686:2022-08-08-7292f33
+manylinux2010 = quay.io/pypa/manylinux2010_i686:2022-08-05-4535177
+manylinux2014 = quay.io/pypa/manylinux2014_i686:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_i686:2022-08-09-51a01be
+musllinux_1_1 = quay.io/pypa/musllinux_1_1_i686:2022-08-09-51a01be
 
 [pypy_x86_64]
-manylinux2010 = quay.io/pypa/manylinux2010_x86_64:2022-07-17-51324db
-manylinux2014 = quay.io/pypa/manylinux2014_x86_64:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_x86_64:2022-07-17-51324db
-manylinux_2_28 = quay.io/pypa/manylinux_2_28_x86_64:2022-07-17-51324db
+manylinux2010 = quay.io/pypa/manylinux2010_x86_64:2022-08-05-4535177
+manylinux2014 = quay.io/pypa/manylinux2014_x86_64:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_x86_64:2022-08-09-51a01be
+manylinux_2_28 = quay.io/pypa/manylinux_2_28_x86_64:2022-08-09-51a01be
 
 [pypy_i686]
-manylinux2010 = quay.io/pypa/manylinux2010_i686:2022-07-17-51324db
-manylinux2014 = quay.io/pypa/manylinux2014_i686:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_i686:2022-07-17-51324db
+manylinux2010 = quay.io/pypa/manylinux2010_i686:2022-08-05-4535177
+manylinux2014 = quay.io/pypa/manylinux2014_i686:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_i686:2022-08-09-51a01be
 
 [aarch64]
-manylinux2014 = quay.io/pypa/manylinux2014_aarch64:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_aarch64:2022-07-17-51324db
-manylinux_2_28 = quay.io/pypa/manylinux_2_28_aarch64:2022-07-17-51324db
-musllinux_1_1 = quay.io/pypa/musllinux_1_1_aarch64:2022-07-17-51324db
+manylinux2014 = quay.io/pypa/manylinux2014_aarch64:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_aarch64:2022-08-09-51a01be
+manylinux_2_28 = quay.io/pypa/manylinux_2_28_aarch64:2022-08-09-51a01be
+musllinux_1_1 = quay.io/pypa/musllinux_1_1_aarch64:2022-08-09-51a01be
 
 [ppc64le]
-manylinux2014 = quay.io/pypa/manylinux2014_ppc64le:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_ppc64le:2022-07-17-51324db
-manylinux_2_28 = quay.io/pypa/manylinux_2_28_ppc64le:2022-07-17-51324db
-musllinux_1_1 = quay.io/pypa/musllinux_1_1_ppc64le:2022-07-17-51324db
+manylinux2014 = quay.io/pypa/manylinux2014_ppc64le:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_ppc64le:2022-08-09-51a01be
+manylinux_2_28 = quay.io/pypa/manylinux_2_28_ppc64le:2022-08-09-51a01be
+musllinux_1_1 = quay.io/pypa/musllinux_1_1_ppc64le:2022-08-09-51a01be
 
 [s390x]
-manylinux2014 = quay.io/pypa/manylinux2014_s390x:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_s390x:2022-07-17-51324db
-musllinux_1_1 = quay.io/pypa/musllinux_1_1_s390x:2022-07-17-51324db
+manylinux2014 = quay.io/pypa/manylinux2014_s390x:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_s390x:2022-08-09-51a01be
+musllinux_1_1 = quay.io/pypa/musllinux_1_1_s390x:2022-08-09-51a01be
 
 [pypy_aarch64]
-manylinux2014 = quay.io/pypa/manylinux2014_aarch64:2022-07-17-51324db
-manylinux_2_24 = quay.io/pypa/manylinux_2_24_aarch64:2022-07-17-51324db
-manylinux_2_28 = quay.io/pypa/manylinux_2_28_aarch64:2022-07-17-51324db
+manylinux2014 = quay.io/pypa/manylinux2014_aarch64:2022-08-09-51a01be
+manylinux_2_24 = quay.io/pypa/manylinux_2_24_aarch64:2022-08-09-51a01be
+manylinux_2_28 = quay.io/pypa/manylinux_2_28_aarch64:2022-08-09-51a01be
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/typing.py` & `cibuildwheel-2.9.0/cibuildwheel/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import subprocess
 import sys
 from typing import TYPE_CHECKING, NoReturn, Set, Union
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final, Literal, OrderedDict, Protocol, TypedDict
@@ -32,12 +34,12 @@
     PathOrStr = Union[str, os.PathLike[str]]
 else:
     PopenBytes = subprocess.Popen
     PathOrStr = Union[str, "os.PathLike[str]"]
 
 
 PlatformName = Literal["linux", "macos", "windows"]
-PLATFORMS: Final[Set[PlatformName]] = {"linux", "macos", "windows"}
+PLATFORMS: Final[set[PlatformName]] = {"linux", "macos", "windows"}
 
 
 def assert_never(value: NoReturn) -> NoReturn:
     assert False, f"Unhandled value: {value} ({type(value).__name__})"  # noqa: B011
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/util.py` & `cibuildwheel-2.9.0/cibuildwheel/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import contextlib
 import fnmatch
 import itertools
 import os
 import re
 import shlex
 import ssl
@@ -14,23 +16,19 @@
 from enum import Enum
 from functools import lru_cache
 from pathlib import Path, PurePath
 from time import sleep
 from typing import (
     Any,
     ClassVar,
-    Dict,
     Generator,
     Iterable,
-    List,
-    Optional,
     Sequence,
     TextIO,
     TypeVar,
-    Union,
     cast,
     overload,
 )
 
 import bracex
 import certifi
 
@@ -94,59 +92,57 @@
 
 IS_WIN: Final = sys.platform.startswith("win")
 
 
 @overload
 def call(
     *args: PathOrStr,
-    env: Optional[Dict[str, str]] = None,
-    cwd: Optional[PathOrStr] = None,
+    env: dict[str, str] | None = None,
+    cwd: PathOrStr | None = None,
     capture_stdout: Literal[False] = ...,
 ) -> None:
     ...
 
 
 @overload
 def call(
     *args: PathOrStr,
-    env: Optional[Dict[str, str]] = None,
-    cwd: Optional[PathOrStr] = None,
+    env: dict[str, str] | None = None,
+    cwd: PathOrStr | None = None,
     capture_stdout: Literal[True],
 ) -> str:
     ...
 
 
 def call(
     *args: PathOrStr,
-    env: Optional[Dict[str, str]] = None,
-    cwd: Optional[PathOrStr] = None,
+    env: dict[str, str] | None = None,
+    cwd: PathOrStr | None = None,
     capture_stdout: bool = False,
-) -> Optional[str]:
+) -> str | None:
     """
     Run subprocess.run, but print the commands first. Takes the commands as
     *args. Uses shell=True on Windows due to a bug. Also converts to
     Paths to strings, due to Windows behavior at least on older Pythons.
     https://bugs.python.org/issue8557
     """
     args_ = [str(arg) for arg in args]
     # print the command executing for the logs
     print("+ " + " ".join(shlex.quote(a) for a in args_))
-    kwargs: Dict[str, Any] = {}
+    kwargs: dict[str, Any] = {}
     if capture_stdout:
         kwargs["universal_newlines"] = True
         kwargs["stdout"] = subprocess.PIPE
     result = subprocess.run(args_, check=True, shell=IS_WIN, env=env, cwd=cwd, **kwargs)
     if not capture_stdout:
         return None
     return cast(str, result.stdout)
 
 
-def shell(
-    *commands: str, env: Optional[Dict[str, str]] = None, cwd: Optional[PathOrStr] = None
-) -> None:
+def shell(*commands: str, env: dict[str, str] | None = None, cwd: PathOrStr | None = None) -> None:
     command = " ".join(commands)
     print(f"+ {command}")
     subprocess.run(command, env=env, cwd=cwd, shell=True, check=True)
 
 
 def format_safe(template: str, **kwargs: Any) -> str:
     """
@@ -196,28 +192,28 @@
 
     For example, used in the test_command option to specify the path to the
     project's root. Unmatched syntax will mostly be allowed through.
     """
     return format_safe(command, python="python", pip="pip", **kwargs)
 
 
-def get_build_verbosity_extra_flags(level: int) -> List[str]:
+def get_build_verbosity_extra_flags(level: int) -> list[str]:
     if level > 0:
         return ["-" + level * "v"]
     elif level < 0:
         return ["-" + -level * "q"]
     else:
         return []
 
 
-def read_python_configs(config: PlatformName) -> List[Dict[str, str]]:
+def read_python_configs(config: PlatformName) -> list[dict[str, str]]:
     input_file = resources_dir / "build-platforms.toml"
     with input_file.open("rb") as f:
         loaded_file = tomllib.load(f)
-    results: List[Dict[str, str]] = list(loaded_file[config]["python_configurations"])
+    results: list[dict[str, str]] = list(loaded_file[config]["python_configurations"])
     return results
 
 
 def selector_matches(patterns: str, string: str) -> bool:
     """
     Returns True if `string` is matched by any of the wildcard patterns in
     `patterns`.
@@ -239,18 +235,18 @@
     build identifier, and it returns True if that identifier should be
     included. Only call this on valid identifiers, ones that have at least 2
     numeric digits before the first dash.
     """
 
     build_config: str
     skip_config: str
-    requires_python: Optional[SpecifierSet] = None
+    requires_python: SpecifierSet | None = None
 
     # a pattern that skips prerelease versions, when include_prereleases is False.
-    PRERELEASE_SKIP: ClassVar[str] = "cp311-*"
+    PRERELEASE_SKIP: ClassVar[str] = ""
     prerelease_pythons: bool = False
 
     def __call__(self, build_id: str) -> bool:
         # Filter build selectors by python_requires if set
         if self.requires_python is not None:
             py_ver_str = build_id.split("-")[0]
             major = int(py_ver_str[2])
@@ -324,15 +320,15 @@
 
 class DependencyConstraints:
     def __init__(self, base_file_path: Path):
         assert base_file_path.exists()
         self.base_file_path = base_file_path.resolve()
 
     @staticmethod
-    def with_defaults() -> "DependencyConstraints":
+    def with_defaults() -> DependencyConstraints:
         return DependencyConstraints(base_file_path=resources_dir / "constraints.txt")
 
     def get_for_python_version(self, version: str) -> Path:
         version_parts = version.split(".")
 
         # try to find a version-specific dependency file e.g. if
         # ./constraints.txt is the base, look for ./constraints-python36.txt
@@ -396,15 +392,15 @@
     circle_ci = "circle_ci"
     azure_pipelines = "azure_pipelines"
     github_actions = "github_actions"
     gitlab = "gitlab"
     other = "other"
 
 
-def detect_ci_provider() -> Optional[CIProvider]:
+def detect_ci_provider() -> CIProvider | None:
     if "TRAVIS" in os.environ:
         return CIProvider.travis_ci
     elif "APPVEYOR" in os.environ:
         return CIProvider.appveyor
     elif "CIRCLECI" in os.environ:
         return CIProvider.circle_ci
     elif "AZURE_HTTP_USER_AGENT" in os.environ:
@@ -469,15 +465,15 @@
         *sorted(
             f"  {f.name:<{max_name_len}s}   {f.size:>{max_size_len}s} kB" for f in new_contents
         ),
         sep="\n",
     )
 
 
-def get_pip_version(env: Dict[str, str]) -> str:
+def get_pip_version(env: dict[str, str]) -> str:
     versions_output_text = call(
         "python", "-m", "pip", "freeze", "--all", capture_stdout=True, env=env
     )
     (pip_version,) = (
         version[5:]
         for version in versions_output_text.strip().splitlines()
         if version.startswith("pip==")
@@ -497,15 +493,15 @@
         if not path.exists():
             download(url, path)
     return path
 
 
 def _parse_constraints_for_virtualenv(
     dependency_constraint_flags: Sequence[PathOrStr],
-) -> Dict[str, str]:
+) -> dict[str, str]:
     """
     Parses the constraints file referenced by `dependency_constraint_flags` and returns a dict where
     the key is the package name, and the value is the constraint version.
     If a package version cannot be found, its value is "embed" meaning that virtualenv will install
     its bundled version, already available locally.
     The function does not try to be too smart and just handles basic constraints.
     If it can't get an exact version, the real constraint will be handled by the
@@ -543,15 +539,15 @@
                 except InvalidRequirement:
                     continue
     return constraints_dict
 
 
 def virtualenv(
     python: Path, venv_path: Path, dependency_constraint_flags: Sequence[PathOrStr]
-) -> Dict[str, str]:
+) -> dict[str, str]:
     assert python.exists()
     virtualenv_app = _ensure_virtualenv()
     constraints = _parse_constraints_for_virtualenv(dependency_constraint_flags)
     additional_flags = [f"--{package}={version}" for package, version in constraints.items()]
 
     # Using symlinks to pre-installed seed packages is really the fastest way to get a virtual
     # environment. The initial cost is a bit higher but reusing is much faster.
@@ -585,15 +581,15 @@
     env["PATH"] = os.pathsep.join(paths + [env["PATH"]])
     return env
 
 
 T = TypeVar("T", bound=PurePath)
 
 
-def find_compatible_wheel(wheels: Sequence[T], identifier: str) -> Optional[T]:
+def find_compatible_wheel(wheels: Sequence[T], identifier: str) -> T | None:
     """
     Finds a wheel with an abi3 or a none ABI tag in `wheels` compatible with the Python interpreter
     specified by `identifier` that is previously built.
     """
 
     interpreter, platform = identifier.split("-")
     for wheel in wheels:
@@ -637,15 +633,15 @@
     from functools import cached_property
 else:
     from .functools_cached_property_38 import cached_property
 
 
 # Can be replaced by contextlib.chdir in Python 3.11
 @contextlib.contextmanager
-def chdir(new_path: Union[Path, str]) -> Generator[None, None, None]:
+def chdir(new_path: Path | str) -> Generator[None, None, None]:
     """Non thread-safe context manager to change the current working directory."""
 
     cwd = os.getcwd()
     try:
         os.chdir(new_path)
         yield
     finally:
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel/windows.py` & `cibuildwheel-2.9.0/cibuildwheel/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import os
 import shutil
 import subprocess
 import sys
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Set
+from typing import Sequence
 from zipfile import ZipFile
 
 from filelock import FileLock
 from packaging.version import Version
 
 from .architecture import Architecture
 from .environment import ParsedEnvironment
@@ -30,15 +32,15 @@
     prepare_command,
     read_python_configs,
     shell,
     virtualenv,
 )
 
 
-def get_nuget_args(version: str, arch: str, output_directory: Path) -> List[str]:
+def get_nuget_args(version: str, arch: str, output_directory: Path) -> list[str]:
     platform_suffix = {"32": "x86", "64": "", "ARM64": "arm64"}
     python_name = "python" + platform_suffix[arch]
     return [
         python_name,
         "-Version",
         version,
         "-FallbackSource",
@@ -49,21 +51,21 @@
 
 
 @dataclass(frozen=True)
 class PythonConfiguration:
     version: str
     arch: str
     identifier: str
-    url: Optional[str] = None
+    url: str | None = None
 
 
 def get_python_configurations(
     build_selector: BuildSelector,
-    architectures: Set[Architecture],
-) -> List[PythonConfiguration]:
+    architectures: set[Architecture],
+) -> list[PythonConfiguration]:
 
     full_python_configs = read_python_configs("windows")
 
     python_configurations = [PythonConfiguration(**item) for item in full_python_configs]
 
     map_arch = {"32": Architecture.x86, "64": Architecture.AMD64, "ARM64": Architecture.ARM64}
 
@@ -120,15 +122,15 @@
 
 def setup_python(
     tmp: Path,
     python_configuration: PythonConfiguration,
     dependency_constraint_flags: Sequence[PathOrStr],
     environment: ParsedEnvironment,
     build_frontend: BuildFrontend,
-) -> Dict[str, str]:
+) -> dict[str, str]:
     tmp.mkdir()
     implementation_id = python_configuration.identifier.split("-")[0]
     log.step(f"Installing Python {implementation_id}...")
     if implementation_id.startswith("cp"):
         base_python = install_cpython(python_configuration.version, python_configuration.arch)
     elif implementation_id.startswith("pp"):
         assert python_configuration.url is not None
@@ -249,15 +251,15 @@
             log.step("Running before_all...")
             env = before_all_options.environment.as_dictionary(prev_environment=os.environ)
             before_all_prepared = prepare_command(
                 before_all_options.before_all, project=".", package=options.globals.package_dir
             )
             shell(before_all_prepared, env=env)
 
-        built_wheels: List[Path] = []
+        built_wheels: list[Path] = []
 
         for config in python_configurations:
             build_options = options.build_options(config.identifier)
             log.build_start(config.identifier)
 
             identifier_tmp_dir = tmp_path / config.identifier
             identifier_tmp_dir.mkdir()
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel.egg-info/PKG-INFO` & `cibuildwheel-2.9.0/cibuildwheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: cibuildwheel
-Version: 2.8.1
+Version: 2.9.0
 Summary: Build Python wheels on CI with minimal configuration.
 Home-page: https://github.com/pypa/cibuildwheel
 Author: Joe Rickerby
 Author-email: joerick@mac.com
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/pypa/cibuildwheel#changelog
 Project-URL: Documentation, https://cibuildwheel.readthedocs.io/
 Keywords: ci,wheel,packaging,pypi,travis,appveyor,macos,linux,windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: bin
 Provides-Extra: mypy
 Provides-Extra: dev
 Provides-Extra: all
@@ -59,23 +58,22 @@
 |   | macOS Intel | macOS Apple Silicon | Windows 64bit | Windows 32bit | Windows Arm64 | manylinux<br/>musllinux x86_64 | manylinux<br/>musllinux i686 | manylinux<br/>musllinux aarch64 | manylinux<br/>musllinux ppc64le | manylinux<br/>musllinux s390x |
 |---------------|----|-----|-----|-----|-----|----|-----|----|-----|-----|
 | CPython 3.6   | ✅ | N/A | ✅  | ✅  | N/A | ✅  | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.7   | ✅ | N/A | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.8   | ✅ | ✅  | ✅  | ✅  | N/A | ✅ | ✅  | ✅ | ✅  | ✅  |
 | CPython 3.9   | ✅ | ✅  | ✅  | ✅  | ✅² | ✅³ | ✅ | ✅ | ✅  | ✅  |
 | CPython 3.10  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
-| CPython 3.11⁴ | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
+| CPython 3.11  | ✅ | ✅  | ✅  | ✅  | ✅² | ✅ | ✅  | ✅ | ✅  | ✅  |
 | PyPy 3.7 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.8 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 | PyPy 3.9 v7.3 | ✅ | N/A | ✅  | N/A | N/A | ✅¹ | ✅¹  | ✅¹ | N/A | N/A |
 
 <sup>¹ PyPy is only supported for manylinux wheels.</sup><br>
 <sup>² Windows arm64 support is experimental.</sup><br>
 <sup>³ Alpine 3.14 and very briefly 3.15's default python3 [was not able to load](https://github.com/pypa/cibuildwheel/issues/934) musllinux wheels. This has been fixed; please upgrade the python package if using Alpine from before the fix.</sup><br>
-<sup>⁴ CPython 3.11 is available using the [CIBW_PRERELEASE_PYTHONS](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) option.</sup><br>
 
 - Builds manylinux, musllinux, macOS 10.9+, and Windows wheels for CPython and PyPy
 - Works on GitHub Actions, Azure Pipelines, Travis CI, AppVeyor, CircleCI, and GitLab CI
 - Bundles shared library dependencies on Linux and macOS through [auditwheel](https://github.com/pypa/auditwheel) and [delocate](https://github.com/matthew-brett/delocate)
 - Runs your library's tests against the wheel-installed version of your library
 
 See the [cibuildwheel 1 documentation](https://cibuildwheel.readthedocs.io/en/1.x/) if you need to build unsupported versions of Python, such as Python 2.
@@ -119,15 +117,15 @@
     steps:
       - uses: actions/checkout@v3
 
       # Used to host cibuildwheel
       - uses: actions/setup-python@v3
 
       - name: Install cibuildwheel
-        run: python -m pip install cibuildwheel==2.8.1
+        run: python -m pip install cibuildwheel==2.9.0
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         # to supply options, put them in 'env', like:
         # env:
         #   CIBW_SOME_OPTION: value
 
@@ -234,14 +232,23 @@
 Changelog
 =========
 
 <!-- START bin/update_readme_changelog.py -->
 
 <!-- this section was generated by bin/update_readme_changelog.py -- do not edit manually -->
 
+### v2.9.0
+
+_11 August 2022_
+
+- 🌟 CPython 3.11 wheels are now built by default - without the CIBW_PRERELEASE_PYTHONS flag. It's time to build and upload these wheels to PyPI! This release includes CPython 3.11.0rc1, which is guaranteed to be ABI compatible with the final release. (#1226)
+- ⚠️ Removed support for running cibuildwheel in Python 3.6. Python 3.6 is EOL. However, cibuildwheel continues to build CPython 3.6 wheels for the moment. (#1175)
+- ✨ Improved error messages when misspelling TOML options, suggesting close matches (#1205)
+- 🛠 When running on Apple Silicon (so far, an unsupported mode of operation), cibuildwheel no longer builds universal2 wheels by default - just arm64. See [#1204](https://github.com/pypa/cibuildwheel/issues/1204) for discussion. We hope to release official support for native builds on Apple Silicon soon! (#1217)
+
 ### v2.8.1
 
 _18 July 2022_
 
 - 🐛 Fix a bug when building CPython 3.8 wheels on an Apple Silicon machine where testing would always fail. cibuildwheel will no longer attempt to test the arm64 part of CPython 3.8 wheels because we use the x86_64 installer of CPython 3.8 due to its macOS system version backward-compatibility. See [#1169](https://github.com/pypa/cibuildwheel/pull/1169) for more details. (#1171)
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b4. (#1180)
 - 🛠 The GitHub Action will ensure a compatible version of Python is installed on the runner (#1114)
@@ -271,21 +278,14 @@
 
 ### v2.6.1
 
 _7 June 2022_
 
 - 🛠 Update the prerelease CPython 3.11 to 3.11.0b3
 
-### v2.6.0
-
-_25 May 2022_
-
-- 🌟 Added the ability to test building wheels on CPython 3.11! Because CPython 3.11 is in beta, these wheels should not be distributed, because they might not be compatible with the final release, but it's available to build for testing purposes. Use the flag [`--prerelease-pythons` or `CIBW_PRERELEASE_PYTHONS`](https://cibuildwheel.readthedocs.io/en/stable/options/#prerelease-pythons) to test. This version of cibuildwheel includes CPython 3.11.0b1. (#1109)
-- 📚 Added an interactive diagram showing how cibuildwheel works to the [docs](https://cibuildwheel.readthedocs.io/en/stable/#how-it-works) (#1100)
-
 <!-- END bin/update_readme_changelog.py -->
 
 ---
 
 That's the last few versions.
 
 ℹ️ **Want more changelog? Head over to [the changelog page in the docs](https://cibuildwheel.readthedocs.io/en/stable/changelog/).**
```

### Comparing `cibuildwheel-2.8.1/cibuildwheel.egg-info/SOURCES.txt` & `cibuildwheel-2.9.0/cibuildwheel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cibuildwheel-2.8.1/cibuildwheel.egg-info/requires.txt` & `cibuildwheel-2.9.0/cibuildwheel.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 filelock
 packaging>=20.9
 platformdirs
 
 [:python_version < "3.11"]
 tomli
 
-[:python_version < "3.7"]
-dataclasses
-
 [:python_version < "3.8"]
 typing-extensions>=3.10.0.0
 
 [all]
 mkdocs-include-markdown-plugin==2.8.0
 mkdocs==1.0.4
 jinja2==3.0.3
```

### Comparing `cibuildwheel-2.8.1/pyproject.toml` & `cibuildwheel-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 
 build-backend = "setuptools.build_meta"
 
 
 [tool.black]
 line-length = 100
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310']
 
 
 [tool.isort]
 profile = "black"
 
 
 [tool.pytest.ini_options]
@@ -84,15 +84,15 @@
     "*.yml",
     "CI.md",  # TODO: can change test/test_ssl and remove this
     "requirements-dev.txt",
     "noxfile.py",
 ]
 
 [tool.pylint]
-master.py-version = "3.6"
+master.py-version = "3.7"
 master.jobs = "0"
 master.fail-on = ["E", "F"]
 master.fail-under = "9.8"
 reports.output-format = "colorized"
 messages_control.enable = [
   "useless-suppression",
 ]
```

### Comparing `cibuildwheel-2.8.1/setup.cfg` & `cibuildwheel-2.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cibuildwheel
-version = 2.8.1
+version = 2.9.0
 description = Build Python wheels on CI with minimal configuration.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/cibuildwheel
 author = Joe Rickerby
 author_email = joerick@mac.com
 license = BSD-2-Clause
@@ -12,15 +12,14 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Build Tools
 keywords = ci,wheel,packaging,pypi,travis,appveyor,macos,linux,windows
@@ -33,18 +32,17 @@
 install_requires = 
 	bashlex!=0.13
 	bracex
 	certifi
 	filelock
 	packaging>=20.9
 	platformdirs
-	dataclasses;python_version < '3.7'
 	tomli;python_version < '3.11'
 	typing-extensions>=3.10.0.0;python_version < '3.8'
-python_requires = >=3.6
+python_requires = >=3.7
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = 
 	cibuildwheel
```

### Comparing `cibuildwheel-2.8.1/setup.py` & `cibuildwheel-2.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from setuptools import setup
 
 extras = {
     "docs": [
         "mkdocs-include-markdown-plugin==2.8.0",
         "mkdocs==1.0.4",  # Doesn't support Python 3.10+
         "jinja2==3.0.3",
```

### Comparing `cibuildwheel-2.8.1/test/test_0_basic.py` & `cibuildwheel-2.9.0/test/test_0_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import textwrap
 
 import pytest
 
 from cibuildwheel.logger import Logger
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_abi_variants.py` & `cibuildwheel-2.9.0/test/test_abi_variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import textwrap
 
 from . import test_projects, utils
 
 limited_api_project = test_projects.new_c_project(
     setup_py_add=textwrap.dedent(
         r"""
```

### Comparing `cibuildwheel-2.8.1/test/test_before_all.py` & `cibuildwheel-2.9.0/test/test_before_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_before_build.py` & `cibuildwheel-2.9.0/test/test_before_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_before_test.py` & `cibuildwheel-2.9.0/test/test_before_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from . import test_projects, utils
 
 before_test_project = test_projects.new_c_project()
 before_test_project.files[
     "test/spam_test.py"
 ] = r"""
 import sys
```

### Comparing `cibuildwheel-2.8.1/test/test_build_skip.py` & `cibuildwheel-2.9.0/test/test_build_skip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import textwrap
 
 from . import test_projects, utils
 
 project_with_skip_asserts = test_projects.new_c_project(
     setup_py_add=textwrap.dedent(
         r"""
```

### Comparing `cibuildwheel-2.8.1/test/test_container_images.py` & `cibuildwheel-2.9.0/test/test_container_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import platform
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_cpp_standards.py` & `cibuildwheel-2.9.0/test/test_cpp_standards.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 import jinja2
 import pytest
 
 from . import utils
 from .test_projects import TestProject
```

### Comparing `cibuildwheel-2.8.1/test/test_dependency_versions.py` & `cibuildwheel-2.9.0/test/test_dependency_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 import textwrap
 
 import pytest
 
 import cibuildwheel.util
```

### Comparing `cibuildwheel-2.8.1/test/test_emulation.py` & `cibuildwheel-2.9.0/test/test_emulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 
 import pytest
 
 from . import test_projects, utils
 
 project_with_a_test = test_projects.new_c_project()
```

### Comparing `cibuildwheel-2.8.1/test/test_environment.py` & `cibuildwheel-2.9.0/test/test_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 import os
 import subprocess
+import sys
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
 
 project_with_environment_asserts = test_projects.new_c_project(
@@ -29,25 +32,26 @@
             raise Exception('$PATH should be expanded in PATH. It was "%s"' % PATH)
         """
     )
 )
 
 
 def test(tmp_path):
+    python_echo = f"'{sys.executable}' -c \"import sys; print(*sys.argv[1:])\""
     project_dir = tmp_path / "project"
     project_with_environment_asserts.generate(project_dir)
 
     # write some information into the CIBW_ENVIRONMENT, for expansion and
     # insertion into the environment by cibuildwheel. This is checked
     # in setup.py
     actual_wheels = utils.cibuildwheel_run(
         project_dir,
         add_env={
             "CIBW_ENVIRONMENT": """CIBW_TEST_VAR="a b c" CIBW_TEST_VAR_2=1 CIBW_TEST_VAR_3="$(echo 'test string 3')" PATH=$PATH:/opt/cibw_test_path""",
-            "CIBW_ENVIRONMENT_WINDOWS": '''CIBW_TEST_VAR="a b c" CIBW_TEST_VAR_2=1 CIBW_TEST_VAR_3="$(echo 'test string 3')" PATH="$PATH;/opt/cibw_test_path"''',
+            "CIBW_ENVIRONMENT_WINDOWS": f'''CIBW_TEST_VAR="a b c" CIBW_TEST_VAR_2=1 CIBW_TEST_VAR_3="$({python_echo} 'test string 3')" PATH="$PATH;/opt/cibw_test_path"''',
         },
     )
 
     # also check that we got the right wheels built
     expected_wheels = utils.expected_wheels("spam", "0.1.0")
     assert set(actual_wheels) == set(expected_wheels)
```

### Comparing `cibuildwheel-2.8.1/test/test_from_sdist.py` & `cibuildwheel-2.9.0/test/test_from_sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import subprocess
 import sys
 import textwrap
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from test.test_projects.base import TestProject
```

### Comparing `cibuildwheel-2.8.1/test/test_macos_archs.py` & `cibuildwheel-2.9.0/test/test_macos_archs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
+
 import platform
 import subprocess
-from typing import Tuple
 
 import pytest
 
 from . import test_projects, utils
 
 basic_project = test_projects.new_c_project()
 
 ALL_MACOS_WHEELS = {
     *utils.expected_wheels("spam", "0.1.0", machine_arch="x86_64"),
-    *utils.expected_wheels("spam", "0.1.0", machine_arch="arm64"),
+    *utils.expected_wheels("spam", "0.1.0", machine_arch="arm64", include_universal2=True),
 }
 
 
-def get_xcode_version() -> Tuple[int, int]:
+def get_xcode_version() -> tuple[int, int]:
     output = subprocess.run(
         ["xcodebuild", "-version"],
-        universal_newlines=True,
+        text=True,
         check=True,
         stdout=subprocess.PIPE,
     ).stdout
     lines = output.splitlines()
     _, version_str = lines[0].split()
 
     version_parts = version_str.split(".")
```

### Comparing `cibuildwheel-2.8.1/test/test_manylinuxXXXX_only.py` & `cibuildwheel-2.9.0/test/test_manylinuxXXXX_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import platform
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_pep518.py` & `cibuildwheel-2.9.0/test/test_pep518.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import textwrap
 
 from . import test_projects, utils
 
 basic_project = test_projects.new_c_project(
     setup_py_add=textwrap.dedent(
         """
```

### Comparing `cibuildwheel-2.8.1/test/test_podman.py` & `cibuildwheel-2.9.0/test/test_podman.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from . import test_projects, utils
 
 basic_project = test_projects.new_c_project()
```

### Comparing `cibuildwheel-2.8.1/test/test_pure_wheel.py` & `cibuildwheel-2.9.0/test/test_pure_wheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 from test import test_projects
 
 import pytest
 
 from . import utils
```

### Comparing `cibuildwheel-2.8.1/test/test_same_wheel.py` & `cibuildwheel-2.9.0/test/test_same_wheel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 from test import test_projects
 
 import pytest
 
 from . import utils
```

### Comparing `cibuildwheel-2.8.1/test/test_ssl.py` & `cibuildwheel-2.9.0/test/test_ssl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import textwrap
 
 from . import test_projects, utils
 
 project_with_ssl_tests = test_projects.new_c_project(
     setup_py_add=textwrap.dedent(
         r"""
```

### Comparing `cibuildwheel-2.8.1/test/test_subdir_package.py` & `cibuildwheel-2.9.0/test/test_subdir_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import jinja2
 
 from . import utils
 from .test_projects import TestProject
 from .test_projects.c import SPAM_C_TEMPLATE
```

### Comparing `cibuildwheel-2.8.1/test/test_testing.py` & `cibuildwheel-2.9.0/test/test_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import subprocess
 import textwrap
 
 import pytest
 
 from . import test_projects, utils
```

### Comparing `cibuildwheel-2.8.1/test/test_troubleshooting.py` & `cibuildwheel-2.9.0/test/test_troubleshooting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 
 import pytest
 
 from . import utils
 from .test_projects import TestProject, new_c_project
```

### Comparing `cibuildwheel-2.8.1/test/test_wheel_tag.py` & `cibuildwheel-2.9.0/test/test_wheel_tag.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from . import test_projects, utils
 
 basic_project = test_projects.new_c_project()
```

