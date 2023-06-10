# Comparing `tmp/matgl-0.5.1.tar.gz` & `tmp/matgl-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.1.tar", last modified: Fri Jun  9 15:25:44 2023, max compression
+gzip compressed data, was "matgl-0.5.2.tar", last modified: Sat Jun 10 15:11:39 2023, max compression
```

## Comparing `matgl-0.5.1.tar` & `matgl-0.5.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.958579 matgl-0.5.1/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.1/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     8467 2023-06-09 15:25:44.958408 matgl-0.5.1/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     7310 2023-06-09 15:25:13.000000 matgl-0.5.1/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.946812 matgl-0.5.1/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      337 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.947702 matgl-0.5.1/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.1/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4008 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/apps/pes.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948188 matgl-0.5.1/matgl/apps/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/apps/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/apps/tests/test_pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     2029 2023-06-09 14:52:44.000000 matgl-0.5.1/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948563 matgl-0.5.1/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.1/matgl/data/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948914 matgl-0.5.1/matgl/data/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/data/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      724 2023-06-09 03:29:05.000000 matgl-0.5.1/matgl/data/tests/test_transformer.py
--rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.949597 matgl-0.5.1/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.1/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15782 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5318 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.950015 matgl-0.5.1/matgl/ext/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/ext/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/ext/tests/test_ase.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.951002 matgl-0.5.1/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.951703 matgl-0.5.1/matgl/graph/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.1/matgl/graph/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/tests/test_compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/tests/test_converters.py
--rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.1/matgl/graph/tests/test_data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.953256 matgl-0.5.1/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3567 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.954604 matgl-0.5.1/matgl/layers/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/layers/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.1/matgl/layers/tests/test_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_core_and_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.955394 matgl-0.5.1/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    10129 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9181 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     1774 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.955984 matgl-0.5.1/matgl/models/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.1/matgl/models/tests/test_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/test_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/test_wrapper.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.957246 matgl-0.5.1/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)     9495 2023-06-09 14:54:15.000000 matgl-0.5.1/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.958091 matgl-0.5.1/matgl/utils/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/utils/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.1/matgl/utils/tests/test_cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)      686 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/utils/tests/test_io.py
--rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.1/matgl/utils/tests/test_maths.py
--rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.1/matgl/utils/tests/test_training.py
--rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.947492 matgl-0.5.1/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     8467 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2551 2023-06-09 14:09:11.000000 matgl-0.5.1/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-09 15:25:44.958624 matgl-0.5.1/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-09 15:24:51.000000 matgl-0.5.1/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.534804 matgl-0.5.2/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.2/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     9125 2023-06-10 15:11:39.534651 matgl-0.5.2/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     7968 2023-06-09 23:37:39.000000 matgl-0.5.2/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.523256 matgl-0.5.2/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      370 2023-06-10 15:02:25.000000 matgl-0.5.2/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.524138 matgl-0.5.2/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.2/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4057 2023-06-10 04:40:15.000000 matgl-0.5.2/matgl/apps/pes.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.524566 matgl-0.5.2/matgl/apps/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/apps/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/apps/tests/test_pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1666 2023-06-10 04:27:24.000000 matgl-0.5.2/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525073 matgl-0.5.2/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.2/matgl/data/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525274 matgl-0.5.2/matgl/data/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/data/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      724 2023-06-09 03:29:05.000000 matgl-0.5.2/matgl/data/tests/test_transformer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525717 matgl-0.5.2/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.2/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15834 2023-06-10 05:11:25.000000 matgl-0.5.2/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5326 2023-06-09 22:52:38.000000 matgl-0.5.2/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.526208 matgl-0.5.2/matgl/ext/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/ext/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/ext/tests/test_ase.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.527078 matgl-0.5.2/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.528174 matgl-0.5.2/matgl/graph/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.2/matgl/graph/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/tests/test_compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/tests/test_converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.2/matgl/graph/tests/test_data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.529643 matgl-0.5.2/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3567 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.530944 matgl-0.5.2/matgl/layers/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/layers/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.2/matgl/layers/tests/test_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_core_and_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_graph_conv.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.531803 matgl-0.5.2/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10178 2023-06-10 04:39:58.000000 matgl-0.5.2/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9230 2023-06-10 04:39:58.000000 matgl-0.5.2/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2190 2023-06-10 14:43:56.000000 matgl-0.5.2/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.532642 matgl-0.5.2/matgl/models/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.2/matgl/models/tests/test_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/test_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/test_wrapper.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.533599 matgl-0.5.2/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10683 2023-06-10 15:08:18.000000 matgl-0.5.2/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.534379 matgl-0.5.2/matgl/utils/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/utils/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.2/matgl/utils/tests/test_cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1065 2023-06-10 15:02:45.000000 matgl-0.5.2/matgl/utils/tests/test_io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.2/matgl/utils/tests/test_maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.2/matgl/utils/tests/test_training.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.523930 matgl-0.5.2/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     9125 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2551 2023-06-09 14:09:11.000000 matgl-0.5.2/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-10 15:11:39.534842 matgl-0.5.2/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-10 15:10:51.000000 matgl-0.5.2/setup.py
```

### Comparing `matgl-0.5.1/LICENSE` & `matgl-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/PKG-INFO` & `matgl-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.1
+Version: 0.5.2
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -32,72 +32,67 @@
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Docs](#docs)
+- [API Docs](#api-docs)
+- [Developer's Guide](#developers-guide)
 - [References](#references)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
-and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
-The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
-- A more intuitive API and class structure based on the Deep Graph Library.
+In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
+and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
+The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
+over the TF implementations:
+- A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
-This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
-(Santiago Miret, Marcel Nassar, Carmelo Gonzales).
+This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
+Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
-Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+Major milestones are summarized below. Please refer to [change log][changelog] for details.
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
-The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
-learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
-array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
-Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
-(See "Learning properties of ordered and disordered materials from multi-fidelity data").
-
-Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
-attributes are updated using information from each other, generating an output graph.
+The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-[M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
-stresses via auto-differentiation.
-
-As a framework, M3GNet has diverse applications, including:
+stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project](http://materialsproject.org).
+  in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -135,47 +130,60 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-## Example notebooks
+### Jupyter notebooks
+
+We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
+Colab. This will be the primary form of usage documentation.
 
-Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
+## API Docs
 
-## Docs
+The Sphinx-generated API docs are available [here][apidocs].
 
-<http://materialsvirtuallab.github.io/matgl>
+## Developer's Guide
+
+A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
 
 ## References
 
 Please cite the following works:
 
-- MEGNet
+> ### MEGNet
+>
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+
+> ### Multi-fidelity MEGNet
+>
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+
+> ### M3GNet
+>
+> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
+>  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
 
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
-
-- Multi-fidelity MEGNet
-
-    ```txt
-    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
-    ```
-
-- M3GNet
-
-    ```txt
-    Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-    2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
-    ```
 
 ## Acknowledgments
 
-This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
-Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
+This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
+Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
+
+[m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
+[megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
+[dgl]: https://www.dgl.ai "DGL website"
+[mavrl]: http://materialsvirtuallab.org "MAVRL website"
+[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
+[megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
+[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mp]: http://materialsproject.org "Materials Project"
+[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
+[doc]: http://materialsvirtuallab.github.io/matgl
```

### Comparing `matgl-0.5.1/README.md` & `matgl-0.5.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,72 +8,67 @@
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Docs](#docs)
+- [API Docs](#api-docs)
+- [Developer's Guide](#developers-guide)
 - [References](#references)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
-and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
-The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
-- A more intuitive API and class structure based on the Deep Graph Library.
+In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
+and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
+The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
+over the TF implementations:
+- A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
-This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
-(Santiago Miret, Marcel Nassar, Carmelo Gonzales).
+This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
+Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
-Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+Major milestones are summarized below. Please refer to [change log][changelog] for details.
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
-The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
-learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
-array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
-Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
-(See "Learning properties of ordered and disordered materials from multi-fidelity data").
-
-Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
-attributes are updated using information from each other, generating an output graph.
+The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-[M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
-stresses via auto-differentiation.
-
-As a framework, M3GNet has diverse applications, including:
+stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project](http://materialsproject.org).
+  in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -111,47 +106,60 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-## Example notebooks
+### Jupyter notebooks
+
+We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
+Colab. This will be the primary form of usage documentation.
 
-Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
+## API Docs
 
-## Docs
+The Sphinx-generated API docs are available [here][apidocs].
 
-<http://materialsvirtuallab.github.io/matgl>
+## Developer's Guide
+
+A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
 
 ## References
 
 Please cite the following works:
 
-- MEGNet
+> ### MEGNet
+>
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+
+> ### Multi-fidelity MEGNet
+>
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+
+> ### M3GNet
+>
+> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
+>  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
 
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
-
-- Multi-fidelity MEGNet
-
-    ```txt
-    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
-    ```
-
-- M3GNet
-
-    ```txt
-    Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-    2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
-    ```
 
 ## Acknowledgments
 
-This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
-Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
+This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
+Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
+
+[m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
+[megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
+[dgl]: https://www.dgl.ai "DGL website"
+[mavrl]: http://materialsvirtuallab.org "MAVRL website"
+[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
+[megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
+[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mp]: http://materialsproject.org "Materials Project"
+[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
+[doc]: http://materialsvirtuallab.github.io/matgl
```

### Comparing `matgl-0.5.1/matgl/apps/pes.py` & `matgl-0.5.2/matgl/apps/pes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 
 class Potential(nn.Module, IOMixIn):
     """
     A class representing an interatomic potential.
     """
 
+    # Model version number.
+    __version__ = 1
+
     def __init__(
         self,
         model: nn.Module,
         data_mean: torch.tensor | None = None,
         data_std: torch.tensor | None = None,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
```

### Comparing `matgl-0.5.1/matgl/apps/tests/test_pes.py` & `matgl-0.5.2/matgl/apps/tests/test_pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/data/tests/test_transformer.py` & `matgl-0.5.2/matgl/data/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/data/transformer.py` & `matgl-0.5.2/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/ext/ase.py` & `matgl-0.5.2/matgl/ext/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,38 +43,41 @@
     "SciPyFminBFGS": SciPyFminBFGS,
     "BFGSLineSearch": BFGSLineSearch,
 }
 
 
 class Atoms2Graph(GraphConverter):
     """
-    Construct a DGL graph from ASE atoms.
+    Construct a DGL graph from ASE Atoms.
     """
 
     def __init__(
         self,
         element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
         """
-        Parameters
-        ----------
-        element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
-            constructed with the same dimensionality of features.
-        cutoff: Cutoff radius for graph representation
+        Init Atoms2Graph from element types and cutoff radius.
+
+        Args:
+            element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
+                constructed with the same dimensionality of features.
+            cutoff: Cutoff radius for graph representation
         """
         self.element_types = tuple(element_types)
         self.cutoff = cutoff
 
     def get_graph(self, atoms: Atoms) -> tuple[dgl.DGLGraph, list]:
         """
-        Get a DGL graph from an input Structure.
+        Get a DGL graph from an input Atoms.
+
+        Args:
+            atoms: Atoms object.
 
-        :param structure: pymatgen structure object
-        :return:
+        Returns:
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
         Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
@@ -96,15 +99,15 @@
             dst_id[exclude_self],
             images[exclude_self],
             bond_dist[exclude_self],
         )
         u, v = tensor(src_id), tensor(dst_id)
         g = dgl.graph((u, v))
         g.edata["pbc_offset"] = torch.tensor(images)
-        g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
+        g.edata["lattice"] = tensor(np.stack([lattice_matrix for _ in range(g.num_edges())]))
         g.ndata["attr"] = tensor(Z)
         g.ndata["node_type"] = tensor(np.hstack([[element_types.index(i.symbol)] for i in atoms]))
         g.ndata["pos"] = tensor(cart_coords)
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
```

### Comparing `matgl-0.5.1/matgl/ext/pymatgen.py` & `matgl-0.5.2/matgl/ext/pymatgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,14 @@
             dst_id[exclude_self],
             images[exclude_self],
             bond_dist[exclude_self],
         )
         u, v = tensor(src_id), tensor(dst_id)
         g = dgl.graph((u, v))
         g.edata["pbc_offset"] = torch.tensor(images)
-        g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
+        g.edata["lattice"] = tensor(np.stack([lattice_matrix for _ in range(g.num_edges())]))
         g.ndata["attr"] = tensor(Z)
         g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
         g.ndata["pos"] = tensor(cart_coords)
-        g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
+        g.ndata["volume"] = tensor([volume for _ in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
         return g, state_attr
```

### Comparing `matgl-0.5.1/matgl/ext/tests/test_ase.py` & `matgl-0.5.2/matgl/ext/tests/test_ase.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/compute.py` & `matgl-0.5.2/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/converters.py` & `matgl-0.5.2/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/data.py` & `matgl-0.5.2/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/tests/test_compute.py` & `matgl-0.5.2/matgl/graph/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/tests/test_converters.py` & `matgl-0.5.2/matgl/graph/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/graph/tests/test_data.py` & `matgl-0.5.2/matgl/graph/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/__init__.py` & `matgl-0.5.2/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_activations.py` & `matgl-0.5.2/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_atom_ref.py` & `matgl-0.5.2/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_bond.py` & `matgl-0.5.2/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_core.py` & `matgl-0.5.2/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_embedding.py` & `matgl-0.5.2/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_graph_convolution.py` & `matgl-0.5.2/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_readout.py` & `matgl-0.5.2/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/_three_body.py` & `matgl-0.5.2/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_activations.py` & `matgl-0.5.2/matgl/layers/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_atom_ref.py` & `matgl-0.5.2/matgl/layers/tests/test_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_basis.py` & `matgl-0.5.2/matgl/layers/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_bond.py` & `matgl-0.5.2/matgl/layers/tests/test_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_core_and_embedding.py` & `matgl-0.5.2/matgl/layers/tests/test_core_and_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_graph_conv.py` & `matgl-0.5.2/matgl/layers/tests/test_graph_conv.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_readout.py` & `matgl-0.5.2/matgl/layers/tests/test_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/layers/tests/test_three_body.py` & `matgl-0.5.2/matgl/layers/tests/test_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/models/_m3gnet.py` & `matgl-0.5.2/matgl/models/_m3gnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
 
 class M3GNet(nn.Module, IOMixIn):
     """
     The main M3GNet model.
     """
 
+    # Model version number.
+    __version__ = 1
+
     def __init__(
         self,
         element_types: tuple[str],
         dim_node_embedding: int = 64,
         dim_edge_embedding: int = 64,
         dim_state_embedding: int | None = None,
         dim_state_types: int | None = None,
```

### Comparing `matgl-0.5.1/matgl/models/_megnet.py` & `matgl-0.5.2/matgl/models/_megnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 
 class MEGNet(nn.Module, IOMixIn):
     """
     DGL implementation of MEGNet.
     """
 
+    # Model version number.
+    __version__ = 1
+
     def __init__(
         self,
         dim_node_embedding: int = 16,
         dim_edge_embedding: int = 100,
         dim_state_embedding: int = 2,
         ntypes_state: int | None = None,
         nblocks: int = 3,
```

### Comparing `matgl-0.5.1/matgl/models/_wrappers.py` & `matgl-0.5.2/matgl/models/_wrappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 from matgl.data.transformer import Transformer
 from matgl.utils.io import IOMixIn
 
 
 class TransformedTargetModel(nn.Module, IOMixIn):
     """
     A model where the target is first transformed prior to training and the reverse transformation is performed for
-    predictions. This is modelled after scikit-learn's TransformedTargetRegressor.
+    predictions. This is modelled after scikit-learn's TransformedTargetRegressor. It should be noted that this model
+    is almost never used for training since the general idea is to use the transformed target for loss computation.
+    Instead, it is created after a model has been fitted for serialization for end user to call the model to perform
+    predictions without having to worry about what target transformations have been performed.
     """
 
+    # Model version number.
+    __version__ = 1
+
     def __init__(self, model: nn.Module, target_transformer: Transformer):
         """
         Args:
             model: Input model
             target_transformer: Transformer for target.
         """
         super().__init__()
@@ -35,15 +41,15 @@
         Returns:
             Inverse transformed output.
         """
         output = self.model.forward(*args, **kwargs)
         return self.transformer.inverse_transform(output)
 
     def __repr__(self):
-        return f"TransformedTargetModel:\nModel: {self.model.__repr()}\nTransformer: {self.transformer.__repr__()}"
+        return f"TransformedTargetModel:\n\tModel: {self.model.__repr()}\n\tTransformer: {self.transformer.__repr__()}"
 
     def predict_structure(self, *args, **kwargs):
         """
         Pass through to parent model.predict_structure with inverse transform.
 
         Args:
             *args: Pass-through to self.model.predict_structure.
```

### Comparing `matgl-0.5.1/matgl/models/tests/test_m3gnet.py` & `matgl-0.5.2/matgl/models/tests/test_m3gnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/models/tests/test_megnet.py` & `matgl-0.5.2/matgl/models/tests/test_megnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/models/tests/test_wrapper.py` & `matgl-0.5.2/matgl/models/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/cutoff.py` & `matgl-0.5.2/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/io.py` & `matgl-0.5.2/matgl/utils/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 import os
 import warnings
 from pathlib import Path
 
 import requests
 import torch
 
-from matgl.config import MATGL_CACHE, MODEL_VERSION, PRETRAINED_MODELS_BASE_URL
+from matgl.config import MATGL_CACHE, PRETRAINED_MODELS_BASE_URL
 
 logger = logging.getLogger(__file__)
 
 
 class IOMixIn:
     """
-    Mixin class for model saving and loading.
+    Mixin class for model saving and loading. For proper usage, models should subclass nn.Module and IOMix and the
+    `save_args` method should be called immediately after the `super().__init__()` call.
+
+    ```
+    super().__init__()
+    self.save_args(locals(), kwargs)
+    ```
     """
 
     def save_args(self, locals: dict, kwargs: dict | None = None) -> None:
         r"""
         Method to save args into a private _init_args variable. This should be called after super in the __init__
         method, e.g., `self.save_args(locals(), kwargs)`.
 
@@ -39,15 +45,15 @@
 
         # If one of the args is a subclass of IOMixIn, we will serialize that class.
         for k, v in d.items():
             if issubclass(v.__class__, IOMixIn):
                 d[k] = {
                     "@class": v.__class__.__name__,
                     "@module": v.__class__.__module__,
-                    "@model_version": MODEL_VERSION,
+                    "@model_version": getattr(v, "__version__", 0),
                     "init_args": v._init_args,
                 }
         self._init_args = d
 
     def save(self, path: str | Path = ".", metadata: dict | None = None, makedirs: bool = True):
         """
         Save model to a directory. Three files will be saved.
@@ -67,80 +73,67 @@
             os.makedirs(path, exist_ok=True)
 
         torch.save(self._init_args, path / "model.pt")  # type: ignore
         torch.save(self.state_dict(), path / "state.pt")  # type: ignore
         d = {
             "@class": self.__class__.__name__,
             "@module": self.__class__.__module__,
-            "@model_version": MODEL_VERSION,
+            "@model_version": getattr(self, "__version__", 0),
             "metadata": metadata,
             "kwargs": self._init_args,
         }  # type: ignore
         with open(path / "model.json", "w") as f:
             json.dump(d, f, default=lambda o: str(o), indent=4)
 
     @classmethod
-    def load(cls, path: str | Path, include_json=False, **kwargs):
+    def load(cls, path: str | Path | dict, **kwargs):
         """
         Load the model weights from a directory.
 
         Args:
-            path (str|path): Path to saved model or name of pre-trained model. The search order is path, followed by
-                download from PRETRAINED_MODELS_BASE_URL (with caching).
-            include_json (bool): If True, the "model.json" file is also loaded. This file can contain metadata about
-                the model, e.g., if scaling was performed in training the model, this file may contain the mean and
-                standard deviation of the models, which needs to be applied to the final predictions.
+            path (str|path|dict): Path to saved model or name of pre-trained model. If it is a dict, it is assumed to
+                be of the form
+                {
+                    "model.pt": path to model.pt file,
+                    "state.pt": path to state file,
+                    "model.json": path to model.json file
+                }
+                Otherwise, the search order is path, followed by download from PRETRAINED_MODELS_BASE_URL
+                (with caching).
             kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
                 want to update the model.
 
         Returns: model_object if include_json is false. (model_object, dict) if include_json is True.
         """
-        path = Path(path)
+        fpaths = path if isinstance(path, dict) else _get_file_paths(Path(path), **kwargs)
 
-        fnames = ["model.pt", "state.pt"]
-        if include_json:
-            fnames.append("model.json")
+        with open(fpaths["model.json"]) as f:
+            model_data = json.load(f)
 
-        if all((path / fn).exists() for fn in fnames):
-            fpaths = {fn: path / fn for fn in fnames}
-        else:
-            try:
-                fpaths = {
-                    fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames
-                }
-            except BaseException:
-                raise ValueError(
-                    f"No valid model found in {path} or among pre-trained_models at "
-                    f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
-                ) from None
+        _check_ver(cls, model_data)
 
         if not torch.cuda.is_available():
             state = torch.load(fpaths["state.pt"], map_location=torch.device("cpu"))
         else:
             state = torch.load(fpaths["state.pt"])
         d = torch.load(fpaths["model.pt"])
 
         # Deserialize any args that are IOMixIn subclasses.
         for k, v in d.items():
             if isinstance(v, dict) and "@class" in v and "@module" in v:
                 modname = v["@module"]
                 classname = v["@class"]
                 mod = __import__(modname, globals(), locals(), [classname], 0)
                 cls_ = getattr(mod, classname)
+                _check_ver(cls_, v)  # Check version of any subclasses too.
                 d[k] = cls_(**v["init_args"])
         d = {k: v for k, v in d.items() if not k.startswith("@")}
         model = cls(**d)
         model.load_state_dict(state)  # type: ignore
 
-        if include_json:
-            with open(fpaths["model.json"]) as f:
-                model_data = json.load(f)
-
-            return model, model_data
-
         return model
 
 
 class RemoteFile:
     """
     Handling of download of remote files to a local cache.
     """
@@ -206,37 +199,87 @@
             want to update the model.
 
     Returns:
         Returns: model_object if include_json is false. (model_object, dict) if include_json is True.
     """
     path = Path(path)
 
-    fnames = ["model.pt", "state.pt", "model.json"]
+    fpaths = _get_file_paths(path, **kwargs)
+
+    try:
+        with open(fpaths["model.json"]) as f:
+            d = json.load(f)
+            modname = d["@module"]
+            classname = d["@class"]
+
+            mod = __import__(modname, globals(), locals(), [classname], 0)
+            cls_ = getattr(mod, classname)
+            return cls_.load(fpaths, **kwargs)
+    except BaseException:
+        raise ValueError(
+            "Bad serialized model detected. It is possible that you have an older model cached. Please "
+            'clear your cache by running `python -c "import matgl; matgl.clear_cache()"`'
+        ) from None
+
+
+def _get_file_paths(path: Path, **kwargs):
+    """
+    Search path for files.
+
+    Args:
+        path (Path): Path to saved model or name of pre-trained model. The search order is path, followed by
+            download from PRETRAINED_MODELS_BASE_URL (with caching).
+        **kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
+            want to update the model.
+
+    Returns:
+        {
+            "model.pt": path to model.pt file,
+            "state.pt": path to state file,
+            "model.json": path to model.json file
+        }
+    """
+    fnames = ("model.pt", "state.pt", "model.json")
 
     if all((path / fn).exists() for fn in fnames):
-        fpaths = {fn: path / fn for fn in fnames}
-    else:
-        try:
-            fpaths = {fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames}
-        except BaseException:
-            raise ValueError(
-                f"No valid model found in {path} or among pre-trained_models at "
-                f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
-            ) from None
-
-    with open(fpaths["model.json"]) as f:
-        d = json.load(f)
-        modname = d["@module"]
-        classname = d["@class"]
-        model_version = d.get("@model_version", 0)
-        if model_version < MODEL_VERSION:
-            warnings.warn(
-                "Incompatible model version detected! The code will continue to load the model but it is "
-                "recommended that you provide a path to an updated model, increment your @model_version in model.json "
-                "if you are confident that the changes are not problematic, or clear your ~/.matgl cache using "
-                '`python -c "import matgl; matgl.clear_cache()"`',
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        mod = __import__(modname, globals(), locals(), [classname], 0)
-        cls_ = getattr(mod, classname)
-        return cls_.load(path, **kwargs)
+        return {fn: path / fn for fn in fnames}
+
+    try:
+        return {fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames}
+    except BaseException:
+        raise ValueError(
+            f"No valid model found in {path} or among pre-trained_models at "
+            f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
+        ) from None
+
+
+def _check_ver(cls_, d: dict):
+    """
+    Check version of cls_ in current matgl against those noted in a model.json dict.
+
+    Args:
+        cls_: Class object.
+        d: Dict from serialized json.
+
+    Raises:
+        Deprecation warning if the code is
+    """
+    if getattr(cls_, "__version__", 0) > d.get("@model_version", 0):
+        warnings.warn(
+            "Incompatible model version detected! The code will continue to load the model but it is "
+            "recommended that you provide a path to an updated model, increment your @model_version in model.json "
+            "if you are confident that the changes are not problematic, or clear your ~/.matgl cache using "
+            '`python -c "import matgl; matgl.clear_cache()"`',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+
+def get_available_pretrained_models() -> list[str]:
+    """
+    Checks Github for available pretrained_models for download. These can be used with load_model.
+
+    Returns:
+        List of available models.
+    """
+    r = requests.get("https://api.github.com/repos/materialsvirtuallab/matgl/contents/pretrained_models")
+    return [d["name"] for d in json.loads(r.content.decode("utf-8")) if d["type"] == "dir"]
```

### Comparing `matgl-0.5.1/matgl/utils/maths.py` & `matgl-0.5.2/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/sb_roots.npy` & `matgl-0.5.2/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/tests/test_cutoff.py` & `matgl-0.5.2/matgl/utils/tests/test_cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/tests/test_maths.py` & `matgl-0.5.2/matgl/utils/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/tests/test_training.py` & `matgl-0.5.2/matgl/utils/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl/utils/training.py` & `matgl-0.5.2/matgl/utils/training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/matgl.egg-info/PKG-INFO` & `matgl-0.5.2/matgl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.1
+Version: 0.5.2
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -32,72 +32,67 @@
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Docs](#docs)
+- [API Docs](#api-docs)
+- [Developer's Guide](#developers-guide)
 - [References](#references)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
-In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
-and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
-The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
-- A more intuitive API and class structure based on the Deep Graph Library.
+In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
+and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
+The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
+over the TF implementations:
+- A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
-This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
-(Santiago Miret, Marcel Nassar, Carmelo Gonzales).
+This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
+Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
-Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+Major milestones are summarized below. Please refer to [change log][changelog] for details.
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
-The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
-learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
-array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
-Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
-(See "Learning properties of ordered and disordered materials from multi-fidelity data").
-
-Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
-attributes are updated using information from each other, generating an output graph.
+The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-[M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
-stresses via auto-differentiation.
-
-As a framework, M3GNet has diverse applications, including:
+stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project](http://materialsproject.org).
+  in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -135,47 +130,60 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-## Example notebooks
+### Jupyter notebooks
+
+We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
+Colab. This will be the primary form of usage documentation.
 
-Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
+## API Docs
 
-## Docs
+The Sphinx-generated API docs are available [here][apidocs].
 
-<http://materialsvirtuallab.github.io/matgl>
+## Developer's Guide
+
+A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
 
 ## References
 
 Please cite the following works:
 
-- MEGNet
+> ### MEGNet
+>
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+
+> ### Multi-fidelity MEGNet
+>
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+
+> ### M3GNet
+>
+> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
+>  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
 
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
-
-- Multi-fidelity MEGNet
-
-    ```txt
-    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
-    ```
-
-- M3GNet
-
-    ```txt
-    Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-    2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
-    ```
 
 ## Acknowledgments
 
-This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
-Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
+This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
+Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
+
+[m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
+[megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
+[dgl]: https://www.dgl.ai "DGL website"
+[mavrl]: http://materialsvirtuallab.org "MAVRL website"
+[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
+[megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
+[mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
+[m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
+[mp]: http://materialsproject.org "Materials Project"
+[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
+[doc]: http://materialsvirtuallab.github.io/matgl
```

### Comparing `matgl-0.5.1/matgl.egg-info/SOURCES.txt` & `matgl-0.5.2/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/pyproject.toml` & `matgl-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matgl-0.5.1/setup.py` & `matgl-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.5.1",
+    version="0.5.2",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

