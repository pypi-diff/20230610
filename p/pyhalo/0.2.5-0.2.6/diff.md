# Comparing `tmp/pyhalo-0.2.5.tar.gz` & `tmp/pyhalo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.5.tar", last modified: Tue Jun  6 21:41:38 2023, max compression
+gzip compressed data, was "pyhalo-0.2.6.tar", last modified: Fri Jun  9 22:35:03 2023, max compression
```

## Comparing `pyhalo-0.2.5.tar` & `pyhalo-0.2.6.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.579511 pyhalo-0.2.5/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.5/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.5/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.5/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.5/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-06 21:41:38.579196 pyhalo-0.2.5/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.5/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.509370 pyhalo-0.2.5/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.5/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.519891 pyhalo-0.2.5/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.525630 pyhalo-0.2.5/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.5/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.530139 pyhalo-0.2.5/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.535945 pyhalo-0.2.5/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.5/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.5/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-06 20:13:42.000000 pyhalo-0.2.5/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.539246 pyhalo-0.2.5/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.544076 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.548330 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.5/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.5/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.5/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6721 2023-06-06 21:18:38.000000 pyhalo-0.2.5/pyHalo/plotting_routines.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    46449 2023-06-06 21:16:50.000000 pyhalo-0.2.5/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.5/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1302 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.5/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.522590 pyhalo-0.2.5/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     3944 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.5/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-06 21:40:17.000000 pyhalo-0.2.5/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-06 21:41:38.579618 pyhalo-0.2.5/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.5/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.556727 pyhalo-0.2.5/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.5/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.560780 pyhalo-0.2.5/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.5/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.570082 pyhalo-0.2.5/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.5/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.5/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.5/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.5/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.5/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      928 2023-06-06 21:02:20.000000 pyhalo-0.2.5/tests/test_plotting.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3223 2023-06-06 21:04:45.000000 pyhalo-0.2.5/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.572062 pyhalo-0.2.5/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.5/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.575866 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.578466 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.5/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.958711 pyhalo-0.2.6/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.6/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.6/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.6/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.6/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-09 22:35:03.957948 pyhalo-0.2.6/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.6/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.826415 pyhalo-0.2.6/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.6/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.6/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.839040 pyhalo-0.2.6/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.845242 pyhalo-0.2.6/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.6/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.849377 pyhalo-0.2.6/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.860430 pyhalo-0.2.6/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.6/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.6/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.6/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-06 20:13:42.000000 pyhalo-0.2.6/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.871354 pyhalo-0.2.6/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.879001 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.887724 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.6/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.6/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.6/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.6/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.6/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3640 2023-06-09 20:44:13.000000 pyhalo-0.2.6/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6721 2023-06-06 21:18:38.000000 pyhalo-0.2.6/pyHalo/plotting_routines.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    46449 2023-06-06 21:16:50.000000 pyhalo-0.2.6/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.6/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.6/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.6/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.6/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.843557 pyhalo-0.2.6/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.6/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-09 22:35:03.000000 pyhalo-0.2.6/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-09 21:08:15.000000 pyhalo-0.2.6/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-09 22:35:03.958935 pyhalo-0.2.6/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.6/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.900228 pyhalo-0.2.6/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.6/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1898 2023-06-09 22:30:00.000000 pyhalo-0.2.6/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.905500 pyhalo-0.2.6/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.6/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.931258 pyhalo-0.2.6/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.6/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.6/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.6/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.6/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.6/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      928 2023-06-06 21:02:20.000000 pyhalo-0.2.6/tests/test_plotting.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3223 2023-06-06 21:04:45.000000 pyhalo-0.2.6/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.945527 pyhalo-0.2.6/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.6/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.953187 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-09 22:35:03.956369 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.6/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.6/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.6/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.5/CONTRIBUTING.rst` & `pyhalo-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/LICENSE` & `pyhalo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/PKG-INFO` & `pyhalo-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.5/README.rst` & `pyhalo-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/docs/Makefile` & `pyhalo-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/docs/conf.py` & `pyhalo-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/docs/installation.rst` & `pyhalo-0.2.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/docs/make.bat` & `pyhalo-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.6/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.6/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.6/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/concentration.py` & `pyhalo-0.2.6/pyHalo/Halos/concentration.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.6/pyHalo/Halos/halo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.6/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.6/pyHalo/Halos/tidal_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Halos/util.py` & `pyhalo-0.2.6/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.6/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.6/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.6/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.6/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.6/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.6/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.6/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.6/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/concentration_models.py` & `pyhalo-0.2.6/pyHalo/concentration_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyHalo.Halos.concentration import *
 from copy import deepcopy
-
+import numpy as np
 
 def preset_concentration_models(model_name, kwargs_model=None):
     """
     This function loads the concentration models, and implements some specific models from the literature
     :param model_name: the name of the concentration model (a string)
     :param kwargs_model: keyword arguments for the model class
     :return: the concentration model
@@ -36,14 +36,23 @@
         # calibrated for ultra-light dark matter
         kwargs_model_return['concentration_cdm_class'] = ConcentrationDiemerJoyce
         kwargs_model_return['kwargs_cdm'] = {}
         kwargs_model_return['c_scale'] = 21.42
         kwargs_model_return['c_power'] = -0.42
         kwargs_model_return['c_power_inner'] = 1.62
         return ConcentrationWDMPolynomial, kwargs_model_return
+    elif model_name == 'FROM_FORMATION_HISTORY':
+        norm, slope = 0.75, 0.4
+        a = norm * (0.7 / kwargs_model['dlogT_dlogk']) ** slope
+        norm, slope, shift = 0.94, 0.7, 0.6
+        b = norm * abs(np.log(1.76 + shift) / np.log(kwargs_model['dlogT_dlogk'] + shift)) ** slope
+        kwargs_model_return['a'] = a
+        kwargs_model_return['b'] = b
+        del kwargs_model_return['dlogT_dlogk']
+        return ConcentrationWDMHyperbolic, kwargs_model_return
     elif model_name == 'CUSTOM':
         if not hasattr(kwargs_model_return['custom_class'], 'nfw_concentration'):
             raise Exception('a custom concentration-mass relation class must have a method nfw_concentration that'
                             'takes as input (halo mass, redshift) and returns the concentration')
         custom_mc_relation_class = kwargs_model_return['custom_class']
         del kwargs_model_return['custom_class']
         return custom_mc_relation_class, kwargs_model_return
```

### Comparing `pyhalo-0.2.5/pyHalo/defaults.py` & `pyhalo-0.2.6/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/mass_function_models.py` & `pyhalo-0.2.6/pyHalo/mass_function_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,80 @@
 from pyHalo.Rendering.MassFunctions.mass_function_base import *
 from pyHalo.Rendering.MassFunctions.density_peaks import *
+from copy import deepcopy
 
-def preset_mass_function_models(model_name):
+
+def preset_mass_function_models(model_name, kwargs_model={}):
     """
     This function loads the concentration models, and implements some specific models from the literature
     :param model_name: the name of the concentration model (a string)
     :param kwargs_model: keyword arguments for the model class
     :return: the concentration model
     """
-    kwargs_model = {}
+    kwargs_model_out = deepcopy(kwargs_model)
     if model_name == 'SHMF_LOVELL2020':
         # calibrated for subhalos
         # from https://arxiv.org/pdf/2003.01125.pdf
-        kwargs_model['a_wdm'] = 4.2
-        kwargs_model['b_wdm'] = 2.5
-        kwargs_model['c_wdm'] = -0.2
-        return WDMPowerLaw, kwargs_model
+        kwargs_model_out['a_wdm'] = 4.2
+        kwargs_model_out['b_wdm'] = 2.5
+        kwargs_model_out['c_wdm'] = -0.2
+        return WDMPowerLaw, kwargs_model_out
     elif model_name == 'LOVELL2020':
         # calibrated for field halos
         # from https://arxiv.org/pdf/2003.01125.pdf
-        kwargs_model['a_wdm'] = 2.3
-        kwargs_model['b_wdm'] = 0.8
-        kwargs_model['c_wdm'] = -1.0
-        return ShethTormenTurnover, kwargs_model
+        kwargs_model_out['a_wdm'] = 2.3
+        kwargs_model_out['b_wdm'] = 0.8
+        kwargs_model_out['c_wdm'] = -1.0
+        return ShethTormenTurnover, kwargs_model_out
     elif model_name == 'SHMF_LOVELL2014':
-        kwargs_model['a_wdm'] = 1.0
-        kwargs_model['b_wdm'] = 1.0
-        kwargs_model['c_wdm'] = -1.3
-        return WDMPowerLaw, kwargs_model
+        kwargs_model_out['a_wdm'] = 1.0
+        kwargs_model_out['b_wdm'] = 1.0
+        kwargs_model_out['c_wdm'] = -1.3
+        return WDMPowerLaw, kwargs_model_out
     elif model_name == 'LOVELL2014':
-        kwargs_model['a_wdm'] = 1.0
-        kwargs_model['b_wdm'] = 1.0
-        kwargs_model['c_wdm'] = -1.3
-        return ShethTormenTurnover, kwargs_model
+        kwargs_model_out['a_wdm'] = 1.0
+        kwargs_model_out['b_wdm'] = 1.0
+        kwargs_model_out['c_wdm'] = -1.3
+        return ShethTormenTurnover, kwargs_model_out
     elif model_name == 'SCHIVE2016':
         # https://arxiv.org/pdf/1508.04621.pdf
         # calibrated for ultra-light dark matter
-        kwargs_model['a_wdm'] = 1.0
-        kwargs_model['b_wdm'] = 1.1
-        kwargs_model['c_wdm'] = -2.2
-        return ShethTormenTurnover, kwargs_model
+        kwargs_model_out['a_wdm'] = 1.0
+        kwargs_model_out['b_wdm'] = 1.1
+        kwargs_model_out['c_wdm'] = -2.2
+        return ShethTormenTurnover, kwargs_model_out
     elif model_name == 'SHMF_SCHIVE2016':
         # https://arxiv.org/pdf/1508.04621.pdf
         # calibrated for ultra-light dark matter
-        kwargs_model['a_wdm'] = 1.0
-        kwargs_model['b_wdm'] = 1.1
-        kwargs_model['c_wdm'] = -2.2
-        return WDMPowerLaw, kwargs_model
+        kwargs_model_out['a_wdm'] = 1.0
+        kwargs_model_out['b_wdm'] = 1.1
+        kwargs_model_out['c_wdm'] = -2.2
+        return WDMPowerLaw, kwargs_model_out
     elif model_name == 'POWER_LAW':
-        return CDMPowerLaw, kwargs_model
+        return CDMPowerLaw, kwargs_model_out
     elif model_name == 'POWER_LAW_TURNOVER':
-        return WDMPowerLaw, kwargs_model
+        return WDMPowerLaw, kwargs_model_out
     elif model_name == 'SHMF_MIXED_WDM_TURNOVER':
-        return MixedWDMPowerLaw, kwargs_model
+        return MixedWDMPowerLaw, kwargs_model_out
     elif model_name == 'MIXED_WDM_TURNOVER':
-        return ShethTormenMixedWDM, kwargs_model
+        return ShethTormenMixedWDM, kwargs_model_out
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
+        return WDMPowerLaw, kwargs_model_out
     else:
         raise Exception('model name '+str(model_name)+' not recognized')
```

### Comparing `pyhalo-0.2.5/pyHalo/plotting_routines.py` & `pyhalo-0.2.6/pyHalo/plotting_routines.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/preset_models.py` & `pyhalo-0.2.6/pyHalo/preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/pyhalo.py` & `pyhalo-0.2.6/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/realization_extensions.py` & `pyhalo-0.2.6/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/single_realization.py` & `pyhalo-0.2.6/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo/utilities.py` & `pyhalo-0.2.6/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.6/pyHalo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.5/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.6/pyHalo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 pyHalo/Rendering/rendering_class_base.py
 pyHalo/Rendering/subhalos.py
 pyHalo/Rendering/two_halo.py
 pyHalo/Rendering/MassFunctions/__init__.py
 pyHalo/Rendering/MassFunctions/delta_function.py
 pyHalo/Rendering/MassFunctions/density_peaks.py
 pyHalo/Rendering/MassFunctions/mass_function_base.py
+pyHalo/Rendering/MassFunctions/stucker.py
 pyHalo/Rendering/MassFunctions/util.py
 pyHalo/Rendering/SpatialDistributions/__init__.py
 pyHalo/Rendering/SpatialDistributions/base.py
 pyHalo/Rendering/SpatialDistributions/correlated.py
 pyHalo/Rendering/SpatialDistributions/nfw.py
 pyHalo/Rendering/SpatialDistributions/uniform.py
 pyhalo/__init__.py
@@ -113,11 +114,12 @@
 tests/test_rendering/test_los.py
 tests/test_rendering/test_population.py
 tests/test_rendering/test_subhalos.py
 tests/test_rendering/test_mass_functions/__init__.py
 tests/test_rendering/test_mass_functions/test_base_functions.py
 tests/test_rendering/test_mass_functions/test_delta_function.py
 tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+tests/test_rendering/test_mass_functions/test_stucker.py
 tests/test_rendering/test_spatial_distribution/__init__.py
 tests/test_rendering/test_spatial_distribution/test_correlated.py
 tests/test_rendering/test_spatial_distribution/test_nfw.py
 tests/test_rendering/test_spatial_distribution/test_uniform.py
```

### Comparing `pyhalo-0.2.5/pyproject.toml` & `pyhalo-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.5/setup.py` & `pyhalo-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_concentration_models.py` & `pyhalo-0.2.6/tests/test_concentration_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,9 +41,15 @@
         c = concentration_model.nfw_concentration(10 ** 7.5, 0.5)
         npt.assert_almost_equal(c, kwargs_model['a'] * (10 ** 7.5 / 10 ** 8) ** kwargs_model['b'] / 1.5)
 
         kwargs_model = {'custom_class': _CustomMCInvalid}
         args = ('CUSTOM', kwargs_model)
         npt.assert_raises(Exception, preset_concentration_models, args)
 
+    def test_formation_history(self):
+
+        kwargs_model = {'dlogT_dlogk': 2.0}
+        mod, kw = preset_concentration_models('FROM_FORMATION_HISTORY', kwargs_model)
+        concentration_model = mod(**kw)
+
 if __name__ == '__main__':
      pytest.main()
```

### Comparing `pyhalo-0.2.5/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.6/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.6/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.6/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.6/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.6/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.6/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.6/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.6/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.6/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.6/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.6/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.6/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.6/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_truncation.py` & `pyhalo-0.2.6/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_uldm.py` & `pyhalo-0.2.6/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_halos/test_util.py` & `pyhalo-0.2.6/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_mass_function_models.py` & `pyhalo-0.2.6/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_plotting.py` & `pyhalo-0.2.6/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_preset_models.py` & `pyhalo-0.2.6/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_pyhalo_base.py` & `pyhalo-0.2.6/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_realization_extensions.py` & `pyhalo-0.2.6/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.6/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_los.py` & `pyhalo-0.2.6/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.6/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 import numpy as np
 from pyHalo.Cosmology.cosmology import Cosmology
 from pyHalo.Cosmology.geometry import Geometry
 import numpy.testing as npt
 from pyHalo.Rendering.MassFunctions.density_peaks import ShethTormen, ShethTormenTurnover, ShethTormenMixedWDM
 from pyHalo.Rendering.MassFunctions.mass_function_base import CDMPowerLaw, WDMPowerLaw, MixedWDMPowerLaw
 from colossus.lss.mass_function import massFunction
-from pyHalo.Rendering.SpatialDistributions.uniform import LensConeUniform
-from pyHalo.pyhalo import pyHalo
-from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche
-from pyHalo.Halos.concentration import ConcentrationDiemerJoyce
 
 class TestShethTormen(object):
 
     def setup_method(self):
 
         z = 0.5
         delta_z = 0.02
```

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_population.py` & `pyhalo-0.2.6/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.6/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.6/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_single_realization.py` & `pyhalo-0.2.6/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.5/tests/test_utilities.py` & `pyhalo-0.2.6/tests/test_utilities.py`

 * *Files identical despite different names*

