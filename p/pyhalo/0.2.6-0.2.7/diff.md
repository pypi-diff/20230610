# Comparing `tmp/pyhalo-0.2.6.tar.gz` & `tmp/pyhalo-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.6.tar", last modified: Fri Jun  9 22:35:03 2023, max compression
+gzip compressed data, was "pyhalo-0.2.7.tar", last modified: Sat Jun 10 17:52:09 2023, max compression
```

## Comparing `pyhalo-0.2.6.tar` & `pyhalo-0.2.7.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.958711 pyhalo-0.2.6/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.6/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.6/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.6/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.6/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-09 22:35:03.957948 pyhalo-0.2.6/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.6/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.826415 pyhalo-0.2.6/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.6/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.839040 pyhalo-0.2.6/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.845242 pyhalo-0.2.6/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.6/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.849377 pyhalo-0.2.6/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.860430 pyhalo-0.2.6/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.6/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.6/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-06 20:13:42.000000 pyhalo-0.2.6/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.871354 pyhalo-0.2.6/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.879001 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.887724 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.6/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.6/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.6/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.6/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3640 2023-06-09 20:44:13.000000 pyhalo-0.2.6/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6721 2023-06-06 21:18:38.000000 pyhalo-0.2.6/pyHalo/plotting_routines.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    46449 2023-06-06 21:16:50.000000 pyhalo-0.2.6/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.6/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.6/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.6/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.843557 pyhalo-0.2.6/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.6/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-09 21:08:15.000000 pyhalo-0.2.6/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-09 22:35:03.958935 pyhalo-0.2.6/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.6/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.900228 pyhalo-0.2.6/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.6/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1898 2023-06-09 22:30:00.000000 pyhalo-0.2.6/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.905500 pyhalo-0.2.6/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.6/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.931258 pyhalo-0.2.6/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.6/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.6/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.6/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.6/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.6/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      928 2023-06-06 21:02:20.000000 pyhalo-0.2.6/tests/test_plotting.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3223 2023-06-06 21:04:45.000000 pyhalo-0.2.6/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.945527 pyhalo-0.2.6/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.6/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.953187 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.956369 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.6/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.671340 pyhalo-0.2.7/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.7/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.7/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.7/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.7/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-10 17:52:09.670659 pyhalo-0.2.7/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.7/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.565345 pyhalo-0.2.7/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.7/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.577395 pyhalo-0.2.7/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.584871 pyhalo-0.2.7/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.7/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.589746 pyhalo-0.2.7/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.599882 pyhalo-0.2.7/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.7/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-06-10 17:05:16.000000 pyhalo-0.2.7/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.7/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-10 01:21:15.000000 pyhalo-0.2.7/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.610087 pyhalo-0.2.7/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.617359 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-06-10 17:27:13.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.623072 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.7/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.7/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.7/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.7/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4769 2023-06-10 17:07:58.000000 pyhalo-0.2.7/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8338 2023-06-10 16:58:29.000000 pyhalo-0.2.7/pyHalo/plotting_routines.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    52889 2023-06-10 17:09:44.000000 pyhalo-0.2.7/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.7/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.7/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.7/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.582986 pyhalo-0.2.7/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.7/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-10 17:51:37.000000 pyhalo-0.2.7/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-10 17:52:09.671532 pyhalo-0.2.7/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.7/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.636345 pyhalo-0.2.7/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.7/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1858 2023-06-10 01:03:10.000000 pyhalo-0.2.7/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.640788 pyhalo-0.2.7/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.7/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.653923 pyhalo-0.2.7/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.7/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.7/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.7/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.7/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.7/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      917 2023-06-10 17:50:52.000000 pyhalo-0.2.7/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1153 2023-06-10 17:27:13.000000 pyhalo-0.2.7/tests/test_plotting.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3384 2023-06-10 01:27:42.000000 pyhalo-0.2.7/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.659579 pyhalo-0.2.7/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.7/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.665346 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.669292 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.7/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.6/CONTRIBUTING.rst` & `pyhalo-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/LICENSE` & `pyhalo-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/PKG-INFO` & `pyhalo-0.2.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.6
+Version: 0.2.7
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.6/README.rst` & `pyhalo-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/docs/Makefile` & `pyhalo-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/docs/conf.py` & `pyhalo-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/docs/installation.rst` & `pyhalo-0.2.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/docs/make.bat` & `pyhalo-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.7/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.7/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.7/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/concentration.py` & `pyhalo-0.2.7/pyHalo/Halos/concentration.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.7/pyHalo/Halos/halo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.7/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.7/pyHalo/Halos/tidal_truncation.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         log10c = min(self._max_c, log10c)
         log10mass_loss_fraction = max(-1.5, log10mass_loss_fraction)
         log10mass_loss_fraction = min(-0.01, log10mass_loss_fraction)
         return (log10c, log10mass_loss_fraction)
 
 class TruncateMeanDensity(object):
 
-    def __init__(self, lens_cosmo, median_rt_over_rs=1.0, c_power=3.0):
+    def __init__(self, lens_cosmo, median_rt_over_rs=2.0, c_power=3.0):
         """
 
         :param lens_cosmo:
         :param median_rt_over_rs:
         :param c_power:
         """
```

### Comparing `pyhalo-0.2.6/pyHalo/Halos/util.py` & `pyhalo-0.2.7/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/stucker.py` & `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.7/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.7/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.7/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.7/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.7/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.7/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/concentration_models.py` & `pyhalo-0.2.7/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/defaults.py` & `pyhalo-0.2.7/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/mass_function_models.py` & `pyhalo-0.2.7/pyHalo/mass_function_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,21 +47,23 @@
         # calibrated for ultra-light dark matter
         kwargs_model_out['a_wdm'] = 1.0
         kwargs_model_out['b_wdm'] = 1.1
         kwargs_model_out['c_wdm'] = -2.2
         return WDMPowerLaw, kwargs_model_out
     elif model_name == 'POWER_LAW':
         return CDMPowerLaw, kwargs_model_out
-    elif model_name == 'POWER_LAW_TURNOVER':
+    elif model_name == 'POWER_LAW_TURNOVER_SHMF':
         return WDMPowerLaw, kwargs_model_out
+    elif model_name == 'POWER_LAW_TURNOVER':
+        return ShethTormenTurnover, kwargs_model_out
     elif model_name == 'SHMF_MIXED_WDM_TURNOVER':
         return MixedWDMPowerLaw, kwargs_model_out
     elif model_name == 'MIXED_WDM_TURNOVER':
         return ShethTormenMixedWDM, kwargs_model_out
-    elif model_name == 'STUCKER':
+    elif model_name == 'STUCKER_SHMF':
         if 'dlogT_dlogk' not in kwargs_model.keys():
             raise Exception('Must specify |dlogT_dlogk| (absolute value of the ' \
             'logarithmic derivative of the transfer function) when using the STUCKER model.)')
         if 'a_wdm' in kwargs_model.keys():
             raise Exception('Cannot specify a_wdm with the Stucker model.')
         if 'b_wdm' in kwargs_model.keys():
             raise Exception('Cannot specify b_wdm with the Stucker model.')
@@ -70,11 +72,28 @@
         from pyHalo.Rendering.MassFunctions.stucker import stucker_suppression_params
         a_wdm, b_wdm, c_wdm = stucker_suppression_params(kwargs_model_out['dlogT_dlogk'])
         kwargs_model_out['a_wdm'] = a_wdm
         kwargs_model_out['b_wdm'] = b_wdm
         kwargs_model_out['c_wdm'] = c_wdm
         del kwargs_model_out['dlogT_dlogk']
         return WDMPowerLaw, kwargs_model_out
+    elif model_name == 'STUCKER':
+        if 'dlogT_dlogk' not in kwargs_model.keys():
+            raise Exception('Must specify |dlogT_dlogk| (absolute value of the ' \
+            'logarithmic derivative of the transfer function) when using the STUCKER model.)')
+        if 'a_wdm' in kwargs_model.keys():
+            raise Exception('Cannot specify a_wdm with the Stucker model.')
+        if 'b_wdm' in kwargs_model.keys():
+            raise Exception('Cannot specify b_wdm with the Stucker model.')
+        if 'c_wdm' in kwargs_model.keys():
+            raise Exception('Cannot specify c_wdm with the Stucker model.')
+        from pyHalo.Rendering.MassFunctions.stucker import stucker_suppression_params
+        a_wdm, b_wdm, c_wdm = stucker_suppression_params(kwargs_model_out['dlogT_dlogk'])
+        kwargs_model_out['a_wdm'] = a_wdm
+        kwargs_model_out['b_wdm'] = b_wdm
+        kwargs_model_out['c_wdm'] = c_wdm
+        del kwargs_model_out['dlogT_dlogk']
+        return ShethTormenTurnover, kwargs_model_out
     else:
         raise Exception('model name '+str(model_name)+' not recognized')
```

### Comparing `pyhalo-0.2.6/pyHalo/plotting_routines.py` & `pyhalo-0.2.7/pyHalo/plotting_routines.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,68 @@
 import matplotlib.pyplot as plt
 import numpy as np
+from pyHalo.single_realization import realization_at_z
 
 plt.rcParams['axes.linewidth'] = 2.5
 plt.rcParams['xtick.major.width'] = 3.5
 plt.rcParams['xtick.major.size'] = 10
 plt.rcParams['xtick.minor.size'] = 6
 plt.rcParams['ytick.minor.size'] = 6
 plt.rcParams['ytick.major.width'] = 3.5
 plt.rcParams['ytick.major.size'] = 10
 plt.rcParams['ytick.labelsize'] = 20
 plt.rcParams['xtick.labelsize'] = 20
 plt.rcParams['font.family']
 
 
+def plot_halo_mass_function(realization, z_eval=None, ax=None, color='k', kwargs_plot={},
+                                     log_mlow=6.0, log_mhigh=10.0, nbins=25):
+
+    """
+    Makes a log-log plot of the halo mass function for a given realization.
+
+    :param realization:
+    :param z_eval:
+    :param ax:
+    :param color:
+    :param kwargs_plot:
+    :param log_mlow:
+    :param log_mhigh:
+    :param nbins:
+    :param show_errorbars:
+    :return:
+    """
+    if ax is None:
+        fig = plt.figure()
+        ax = plt.subplot(111)
+
+    xlabel = 'halo mass '+r'$\left[M_{\odot}\right]$'
+    ylabel = r'$n\left(m\right)$'
+    if z_eval is None:
+        masses = realization.masses
+    elif isinstance(z_eval, float) or isinstance(z_eval, int):
+        real = realization_at_z(realization, z_eval)[0]
+        masses = real.masses
+    elif isinstance(z_eval, list):
+        masses = []
+        for halo in realization.halos:
+            if halo.is_subhalo:
+                continue
+            if halo.z >= z_eval[0] and halo.z < z_eval[1]:
+                masses.append(halo.mass)
+    else:
+        raise Exception('z_eval must be one of: a specific redshift (i.e. a floating point number), or an'
+                        'interval z_eval = [z_min, z_max]')
+    h, m = np.histogram(masses, bins=np.logspace(log_mlow, log_mhigh, nbins))
+    ax.plot(m[0:-1], h, color=color, **kwargs_plot)
+    ax.set_xlabel(xlabel, fontsize=14)
+    ax.set_ylabel(ylabel, fontsize=14)
+    ax.set_xscale('log')
+    ax.set_yscale('log')
+
 def plot_concentration_mass_relation(realization, z_eval, ax=None, color='k', kwargs_plot={},
                                      log_mlow=6.0, log_mhigh=10.0, nbins=20, show_errorbars=False):
 
     """
     Makes a log-log plot of the concentration-mass relation for a given realization.
 
     :param realization: an instance of the Realization class
@@ -33,61 +79,65 @@
     """
     if ax is None:
         fig = plt.figure()
         ax = plt.subplot(111)
 
     if z_eval == 'z_lens':
         xlabel = 'infall halo mass ' + r'$\left[M_{\odot}\right]$'
+        ylabel = r'$c\left(m\right)$'
         halo_mass_list = []
         halo_concentration_list = []
         for halo in realization.halos:
             if halo.is_subhalo:
                 halo_mass_list.append(halo.mass)
                 halo_concentration_list.append(halo.c)
     elif isinstance(z_eval, float) or isinstance(z_eval, int):
-        xlabel = 'halo mass at z=' +str(z_eval)
+        xlabel = 'halo mass ' + r'$\left[M_{\odot}\right]$'
+        ylabel = r'$c\left(m\right)$'
         halo_mass_list = []
         halo_concentration_list = []
         for halo in realization.halos:
             if halo.is_subhalo and halo.z == z_eval:
                 halo_mass_list.append(halo.mass)
                 halo_concentration_list.append(halo.c)
     elif isinstance(z_eval, list):
-        xlabel = 'halo mass (' + str(z_eval[0])+' < z < '+str(z_eval[1])+')'
+        xlabel = 'halo mass ' + r'$\left[M_{\odot}\right]$'
+        ylabel = r'$c\left(m\right)$'
         halo_mass_list = []
         halo_concentration_list = []
         for halo in realization.halos:
-            if halo.is_subhalo:
-                if halo.z >= z_eval[0] and halo.z < z_eval[1]:
-                    halo_mass_list.append(halo.mass)
-                    halo_concentration_list.append(halo.c)
+            if halo.z >= z_eval[0] and halo.z < z_eval[1]:
+                halo_mass_list.append(halo.mass)
+                halo_concentration_list.append(halo.c)
     else:
         raise Exception('z_eval must be one of: z_lens, a specific redshift (i.e. a floating point number), or an'
                         'interval z_eval = [z_min, z_max]')
 
     halo_masses = np.array(halo_mass_list)
     halo_concentrations = np.array(halo_concentration_list)
 
     x = np.logspace(log_mlow, log_mhigh, nbins + 1)
     c = []
     c_error = []
     for i in range(0, len(x) - 1):
         cond1 = halo_masses >= x[i]
         cond2 = halo_masses < x[i + 1]
         inds = np.where(np.logical_and(cond1, cond2))[0]
-        log10c_median = np.median(np.log10(halo_concentrations[inds]))
-        log10c_std = np.std(np.log10(halo_concentrations[inds]))
-        c.append(log10c_median)
-        c_error.append(log10c_std)
-    log10m = np.log10(x)[0:-1]
+        c_median = np.median(halo_concentrations[inds])
+        c_std = np.std(halo_concentrations[inds])
+        c.append(c_median)
+        c_error.append(c_std)
+
     if show_errorbars:
-        ax.errorbar(log10m, c, yerr=c_error, fmt='none', color=color)
-    ax.plot(log10m, c, color=color, **kwargs_plot)
+        ax.errorbar(x[0:-1], c, yerr=c_error, fmt='none', color=color)
+    ax.plot(x[0:-1], c, color=color, **kwargs_plot)
     ax.set_xlabel(xlabel, fontsize=15)
-    ax.set_ylabel(r'$\log_{10} c$', fontsize=15)
+    ax.set_ylabel(ylabel, fontsize=15)
+    ax.set_xscale('log')
+    ax.set_yscale('linear')
 
 
 def plot_subhalo_bound_mass(realization, ax=None, color='k', kwargs_plot={},
                             log_mlow=6.0, log_mhigh=10.0):
     """
     Plots the bound mass of subhalos defined as the mass inside the infall virial radius of a truncated
     profile. Note: the halo mass definition must have a truncation radius specified for this method
```

### Comparing `pyhalo-0.2.6/pyHalo/preset_models.py` & `pyhalo-0.2.7/pyHalo/preset_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pyHalo.single_realization import Realization
 from copy import copy
 import numpy as np
 from pyHalo.realization_extensions import RealizationExtensions
 from pyHalo.utilities import de_broglie_wavelength, MinHaloMassULDM
 
 __all__ = ['preset_model_from_name', 'CDM', 'WDM', 'ULDM', 'SIDM_core_collapse', 'WDM_mixed',
-           'CDMFromEmulator']
+           'CDMFromEmulator', 'WDMGeneral']
 
 def preset_model_from_name(name):
     """
     Retruns a preset_model function from a string
     :param name: the name of the preset model, should be the name of a function in this file
     :return: the function
     """
@@ -37,14 +37,16 @@
         return SIDM_core_collapse
     elif name == 'ULDM':
         return ULDM
     elif name == 'CDMEmulator':
         return CDMFromEmulator
     elif name == 'WDM_mixed':
         return WDM_mixed
+    elif name == 'WDMGeneral':
+        return WDMGeneral
     else:
         raise Exception('preset model '+ str(name)+' not recognized!')
 
 def CDM(z_lens, z_source, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         concentration_model_subhalos='DIEMERJOYCE19', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='DIEMERJOYCE19', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
@@ -232,21 +234,21 @@
 
     # SET THE SPATIAL DISTRIBUTION MODELS FOR SUBHALOS AND FIELD HALOS:
     subhalo_spatial_distribution = ProjectedNFW
     fieldhalo_spatial_distribution = LensConeUniform
 
     # SET THE MASS FUNCTION MODELS FOR SUBHALOS AND FIELD HALOS
     # NOTE: MASS FUNCTIONS SHOULD NOT BE INSTANTIATED HERE
-    mass_function_model_subhalos, kwargs_mfunc_subs = preset_mass_function_models(mass_function_model_subhalos)
-    kwargs_mfunc_subs.update(kwargs_mass_function_subhalos)
-    kwargs_mfunc_subs['log_mc'] = log_mc
-
-    mass_function_model_fieldhalos, kwargs_mfunc_field = preset_mass_function_models(mass_function_model_fieldhalos)
-    kwargs_mfunc_field.update(kwargs_mass_function_fieldhalos)
-    kwargs_mfunc_field['log_mc'] = log_mc
+    mass_function_model_subhalos, kwargs_mass_function_subhalos = preset_mass_function_models(mass_function_model_subhalos,
+                                                                                              kwargs_mass_function_subhalos)
+    kwargs_mass_function_subhalos['log_mc'] = log_mc
+
+    mass_function_model_fieldhalos, kwargs_mass_function_fieldhalos = preset_mass_function_models(mass_function_model_fieldhalos,
+                                                                                                  kwargs_mass_function_fieldhalos)
+    kwargs_mass_function_fieldhalos['log_mc'] = log_mc
 
     # SET THE CONCENTRATION-MASS RELATION FOR SUBHALOS AND FIELD HALOS
     kwargs_concentration_model_subhalos['cosmo'] = pyhalo.astropy_cosmo
     kwargs_concentration_model_subhalos['log_mc'] = log_mc
     kwargs_concentration_model_fieldhalos['cosmo'] = pyhalo.astropy_cosmo
     kwargs_concentration_model_fieldhalos['log_mc'] = log_mc
 
@@ -280,28 +282,28 @@
 
     # NOW THAT THE CLASSES ARE SPECIFIED, WE SORT THE KEYWORD ARGUMENTS AND CLASSES INTO LISTS
     population_model_list = ['SUBHALOS', 'LINE_OF_SIGHT', 'TWO_HALO']
 
     mass_function_class_list = [mass_function_model_subhalos,
                                 mass_function_model_fieldhalos,
                                 mass_function_model_fieldhalos]
-    kwargs_mfunc_subs.update({'log_mlow': log_mlow,
+    kwargs_mass_function_subhalos.update({'log_mlow': log_mlow,
                        'log_mhigh': log_mhigh,
                        'm_pivot': 10 ** 8,
                        'power_law_index': shmf_log_slope,
                        'log_m_host': log_m_host,
                        'sigma_sub': sigma_sub,
                        'delta_power_law_index': 0.0})
-    kwargs_mfunc_field.update({'log_mlow': log_mlow,
+    kwargs_mass_function_fieldhalos.update({'log_mlow': log_mlow,
                   'log_mhigh': log_mhigh,
                   'LOS_normalization': LOS_normalization,
                   'm_pivot': 10 ** 8,
                   'log_m_host': log_m_host,
                   'delta_power_law_index': 0.0})
-    kwargs_mass_function_list = [kwargs_mfunc_subs, kwargs_mfunc_field, kwargs_mfunc_field]
+    kwargs_mass_function_list = [kwargs_mass_function_subhalos, kwargs_mass_function_fieldhalos, kwargs_mass_function_fieldhalos]
     spatial_distribution_class_list = [subhalo_spatial_distribution, fieldhalo_spatial_distribution, fieldhalo_spatial_distribution]
     kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens,
                                'rmax2d_arcsec': cone_opening_angle_arcsec / 2, 'r_core_units_rs': r_tidal,
                                'lens_cosmo': pyhalo.lens_cosmo}
     kwargs_los_spatial = {'cone_opening_angle': cone_opening_angle_arcsec, 'geometry': geometry}
     kwargs_spatial_distribution_list = [kwargs_subhalos_spatial, kwargs_los_spatial, kwargs_los_spatial]
 
@@ -669,14 +671,123 @@
                   'shmf_log_slope': shmf_log_slope, 'cone_opening_angle_arcsec': cone_opening_angle_arcsec,
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'kwargs_density_profile': kwargs_density_profile
                   }
     return WDM(**kwargs_wdm)
 
+def WDMGeneral(z_lens, z_source, log_mc, dlogT_dlogk, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
+        shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
+        LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
+        mdef_subhalos='TNFW', mdef_field_halos='TNFW', kwargs_density_profile={}):
+
+    """
+
+    :param z_lens: the lens redshift
+    :param z_source:
+    :param log_mc:
+    :param dlogT_dlogk:
+    :param sigma_sub:
+    :param log_mlow:
+    :param log_mhigh:
+    :param shmf_log_slope:
+    :param cone_opening_angle_arcsec:
+    :param log_m_host:
+    :param r_tidal:
+    :param LOS_normalization:
+    :param geometry_type:
+    :param kwargs_cosmo:
+    :param mdef_subhalos:
+    :param mdef_field_halos:
+    :param kwargs_density_profile:
+    :return:
+    """
+    # FIRST WE CREATE AN INSTANCE OF PYHALO, WHICH SETS THE COSMOLOGY
+    pyhalo = pyHalo(z_lens, z_source, kwargs_cosmo)
+    # WE ALSO SPECIFY THE GEOMETRY OF THE RENDERING VOLUME
+    geometry = Geometry(pyhalo.cosmology, z_lens, z_source,
+                        cone_opening_angle_arcsec, geometry_type)
+
+    # SET THE SPATIAL DISTRIBUTION MODELS FOR SUBHALOS AND FIELD HALOS:
+    subhalo_spatial_distribution = ProjectedNFW
+    fieldhalo_spatial_distribution = LensConeUniform
+
+    kwargs_model_dlogT_dlogk = {'dlogT_dlogk': dlogT_dlogk}
+    mass_function_model_subhalos, kwargs_mfunc_subs = preset_mass_function_models('STUCKER_SHMF', kwargs_model_dlogT_dlogk)
+    mass_function_model_fieldhalos, kwargs_mfunc_field = preset_mass_function_models('STUCKER', kwargs_model_dlogT_dlogk)
+
+    # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
+    truncation_model_subhalos = 'TRUNCATION_MEAN_DENSITY'
+    truncation_model_fieldhalos = 'SPLASHBACK'
+
+    model_subhalos, kwargs_truncation_model_subhalos = truncation_models(truncation_model_subhalos)
+    kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    truncation_model_subhalos = model_subhalos(**kwargs_truncation_model_subhalos)
+
+    model_fieldhalos, kwargs_truncation_model_fieldhalos = truncation_models(truncation_model_fieldhalos)
+    kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    truncation_model_fieldhalos = model_fieldhalos(**kwargs_truncation_model_fieldhalos)
+
+    # SET THE CONCENTRATION-MASS RELATION FOR SUBHALOS AND FIELD HALOS
+    concentration_model = 'FROM_FORMATION_HISTORY'
+    model_subhalos, kwargs_concentration_model_subhalos = preset_concentration_models(concentration_model,
+                                                                                      kwargs_model_dlogT_dlogk)
+    concentration_model_CDM = preset_concentration_models('DIEMERJOYCE19')[0]
+    kwargs_concentration_model_subhalos['concentration_cdm_class'] = concentration_model_CDM
+    kwargs_concentration_model_subhalos['cosmo'] = pyhalo.astropy_cosmo
+    kwargs_concentration_model_subhalos['log_mc'] = log_mc
+    concentration_model_subhalos = model_subhalos(**kwargs_concentration_model_subhalos)
+
+    model_fieldhalos, kwargs_concentration_model_fieldhalos = preset_concentration_models(concentration_model,
+                                                                                          kwargs_model_dlogT_dlogk)
+    kwargs_concentration_model_fieldhalos['concentration_cdm_class'] = concentration_model_CDM
+    kwargs_concentration_model_fieldhalos['cosmo'] = pyhalo.astropy_cosmo
+    kwargs_concentration_model_fieldhalos['log_mc'] = log_mc
+    concentration_model_fieldhalos = model_fieldhalos(**kwargs_concentration_model_fieldhalos)
+
+    # NOW THAT THE CLASSES ARE SPECIFIED, WE SORT THE KEYWORD ARGUMENTS AND CLASSES INTO LISTS
+    population_model_list = ['SUBHALOS', 'LINE_OF_SIGHT', 'TWO_HALO']
+
+    mass_function_class_list = [mass_function_model_subhalos,
+                                mass_function_model_fieldhalos,
+                                mass_function_model_fieldhalos]
+    kwargs_mfunc_subs.update({'log_mlow': log_mlow,
+                       'log_mhigh': log_mhigh,
+                       'm_pivot': 10 ** 8,
+                       'power_law_index': shmf_log_slope,
+                       'log_m_host': log_m_host,
+                       'sigma_sub': sigma_sub,
+                       'delta_power_law_index': 0.0,
+                        'log_mc': log_mc})
+    kwargs_mfunc_field.update({'log_mlow': log_mlow,
+                  'log_mhigh': log_mhigh,
+                  'LOS_normalization': LOS_normalization,
+                  'm_pivot': 10 ** 8,
+                  'log_m_host': log_m_host,
+                  'delta_power_law_index': 0.0,
+                  'log_mc': log_mc})
+    kwargs_mass_function_list = [kwargs_mfunc_subs, kwargs_mfunc_field, kwargs_mfunc_field]
+    spatial_distribution_class_list = [subhalo_spatial_distribution, fieldhalo_spatial_distribution, fieldhalo_spatial_distribution]
+    kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens,
+                               'rmax2d_arcsec': cone_opening_angle_arcsec / 2, 'r_core_units_rs': r_tidal,
+                               'lens_cosmo': pyhalo.lens_cosmo}
+    kwargs_los_spatial = {'cone_opening_angle': cone_opening_angle_arcsec, 'geometry': geometry}
+    kwargs_spatial_distribution_list = [kwargs_subhalos_spatial, kwargs_los_spatial, kwargs_los_spatial]
+
+    kwargs_halo_model = {'truncation_model_subhalos': truncation_model_subhalos,
+                         'concentration_model_subhalos': concentration_model_subhalos,
+                         'truncation_model_field_halos': truncation_model_fieldhalos,
+                         'concentration_model_field_halos': concentration_model_fieldhalos,
+                         'kwargs_density_profile': kwargs_density_profile}
+
+    realization_list = pyhalo.render(population_model_list, mass_function_class_list, kwargs_mass_function_list,
+                                     spatial_distribution_class_list, kwargs_spatial_distribution_list,
+                                     geometry, mdef_subhalos, mdef_field_halos, kwargs_halo_model, nrealizations=1)
+    return realization_list[0]
+
 def CDMFromEmulator(z_lens, z_source, emulator_input, kwargs_cdm):
     """
     This generates a realization of subhalos using an emulator of the semi-analytic modeling code Galacticus, and
      generates line-of-sight halos from a mass function parameterized as Sheth-Tormen.
 
     :param z_lens: main deflector redshift
     :param z_source: sourcee redshift
```

### Comparing `pyhalo-0.2.6/pyHalo/pyhalo.py` & `pyhalo-0.2.7/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/realization_extensions.py` & `pyhalo-0.2.7/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/single_realization.py` & `pyhalo-0.2.7/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/truncation_models.py` & `pyhalo-0.2.7/pyHalo/truncation_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo/utilities.py` & `pyhalo-0.2.7/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.7/pyHalo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.6
+Version: 0.2.7
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.6/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.7/pyHalo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/pyproject.toml` & `pyhalo-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.6/setup.py` & `pyhalo-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_concentration_models.py` & `pyhalo-0.2.7/tests/test_concentration_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,11 +45,10 @@
         args = ('CUSTOM', kwargs_model)
         npt.assert_raises(Exception, preset_concentration_models, args)
 
     def test_formation_history(self):
 
         kwargs_model = {'dlogT_dlogk': 2.0}
         mod, kw = preset_concentration_models('FROM_FORMATION_HISTORY', kwargs_model)
-        concentration_model = mod(**kw)
 
 if __name__ == '__main__':
      pytest.main()
```

### Comparing `pyhalo-0.2.6/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.7/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.7/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.7/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.7/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.7/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.7/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.7/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.7/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.7/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.7/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.7/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.7/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.7/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_truncation.py` & `pyhalo-0.2.7/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_uldm.py` & `pyhalo-0.2.7/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_halos/test_util.py` & `pyhalo-0.2.7/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_mass_function_models.py` & `pyhalo-0.2.7/tests/test_mass_function_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pyHalo.mass_function_models import preset_mass_function_models
 
 class TestMassFunctionModels(object):
 
     def setup_method(self):
         self.model_list = ['SHMF_LOVELL2020', 'LOVELL2020', 'SHMF_LOVELL2014',
                            'LOVELL2014', 'SCHIVE2016', 'SHMF_SCHIVE2016', 'POWER_LAW',
-                           'POWER_LAW_TURNOVER']
+                           'POWER_LAW_TURNOVER', 'POWER_LAW_TURNOVER_SHMF']
         self.model_names = ['WDM_POWER_LAW', 'SHETH_TORMEN', 'WDM_POWER_LAW',
                             'SHETH_TORMEN', 'SHETH_TORMEN', 'WDM_POWER_LAW', 'CDM_POWER_LAW',
-                            'WDM_POWER_LAW']
+                            'SHETH_TORMEN', 'WDM_POWER_LAW']
 
     def test_models(self):
 
         for model, model_name in zip(self.model_list, self.model_names):
             mod, kw = preset_mass_function_models(model)
             npt.assert_string_equal(model_name, mod.name)
```

### Comparing `pyhalo-0.2.6/tests/test_plotting.py` & `pyhalo-0.2.7/tests/test_plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import numpy.testing as npt
 import pytest
 from pyHalo.preset_models import CDM
-from pyHalo.plotting_routines import plot_subhalo_bound_mass, plot_subhalo_mass_functon, plot_concentration_mass_relation
+from pyHalo.plotting_routines import plot_subhalo_bound_mass, \
+    plot_subhalo_mass_functon, plot_concentration_mass_relation, plot_halo_mass_function
 
 class TestPlottingRoutines(object):
 
     def setup_method(self):
         self.realization = CDM(0.5, 1.5, sigma_sub=0.025, LOS_normalization=0.0)
 
     def test_mass_function_plot(self):
 
         plot_subhalo_mass_functon(self.realization)
         plot_subhalo_mass_functon(self.realization, bound_mass_function=True)
+        plot_halo_mass_function(self.realization, z_eval=0.5)
+        plot_halo_mass_function(self.realization, z_eval=None)
+        plot_halo_mass_function(self.realization, z_eval=[0.5, 0.6])
 
     def test_bound_mass_function_plot(self):
 
         plot_subhalo_bound_mass(self.realization)
 
     def test_plot_mc_relation(self):
```

### Comparing `pyhalo-0.2.6/tests/test_preset_models.py` & `pyhalo-0.2.7/tests/test_preset_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,19 @@
         _ = preset_model_from_name('SIDM_core_collapse')
 
     def test_WDM_mixed(self):
         wdm_mixed = WDM_mixed(0.5, 1.5, 8.0, 0.5)
         _ = wdm_mixed.lensing_quantities()
         _ = preset_model_from_name('WDM_mixed')
 
+    def test_WDM_general(self):
+        func = preset_model_from_name('WDMGeneral')
+        wdm = func(0.5, 1.5, 7.7, 2.0)
+        _ = wdm.lensing_quantities()
+
     def test_CDM_emulator(self):
 
         def emulator_input_callable(*args, **kwargs):
             subhalo_infall_masses = np.array([10**7,10**8])
             subhalo_x_kpc = np.array([1.0, 1.0])
             subhalo_y_kpc = np.array([1.0, 1.0])
             subhalo_final_bound_masses = subhalo_infall_masses / 2
```

### Comparing `pyhalo-0.2.6/tests/test_pyhalo_base.py` & `pyhalo-0.2.7/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_realization_extensions.py` & `pyhalo-0.2.7/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.7/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_los.py` & `pyhalo-0.2.7/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_stucker.py` & `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_population.py` & `pyhalo-0.2.7/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.7/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_single_realization.py` & `pyhalo-0.2.7/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.6/tests/test_utilities.py` & `pyhalo-0.2.7/tests/test_utilities.py`

 * *Files identical despite different names*

