# Comparing `tmp/pyrfu-2.4.0.tar.gz` & `tmp/pyrfu-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfu-2.4.0.tar", last modified: Fri Jun  9 16:04:31 2023, max compression
+gzip compressed data, was "pyrfu-2.4.1.tar", last modified: Sat Jun 10 20:06:20 2023, max compression
```

## Comparing `pyrfu-2.4.0.tar` & `pyrfu-2.4.1.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.654573 pyrfu-2.4.0/
--rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.0/.flake8
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.280712 pyrfu-2.4.0/.github/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.534180 pyrfu-2.4.0/.github/workflows/
--rw-r--r--   0 louisr     (501) staff       (20)      570 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.github/workflows/flake8.yml
--rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 louisr     (501) staff       (20)      588 2023-06-09 14:46:12.000000 pyrfu-2.4.0/.github/workflows/pylint.yml
--rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.0/.gitignore
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.538666 pyrfu-2.4.0/.idea/
--rw-r--r--   0 louisr     (501) staff       (20)      294 2023-06-09 13:55:07.000000 pyrfu-2.4.0/.idea/aws.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.539801 pyrfu-2.4.0/.idea/codeStyles/
--rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.541692 pyrfu-2.4.0/.idea/inspectionProfiles/
--rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/vcs.xml
--rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
--rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-06-09 14:43:25.000000 pyrfu-2.4.0/.pre-commit-config.yaml
--rwxr-xr-x   0 louisr     (501) staff       (20)       83 2023-04-20 14:38:38.000000 pyrfu-2.4.0/.readthedocs.yml
--rw-r--r--   0 louisr     (501) staff       (20)     2972 2023-04-20 14:38:38.000000 pyrfu-2.4.0/CONTRIBUTING.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.0/LICENSE.txt
--rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.0/MANIFEST.in
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-09 16:04:31.653862 pyrfu-2.4.0/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     6490 2023-06-09 10:13:58.000000 pyrfu-2.4.0/README.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.544657 pyrfu-2.4.0/docs/
--rw-r--r--   0 louisr     (501) staff       (20)      640 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/Makefile
--rw-r--r--   0 louisr     (501) staff       (20)      341 2023-04-21 12:45:20.000000 pyrfu-2.4.0/docs/environment.yml
--rw-r--r--   0 louisr     (501) staff       (20)      785 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/make.bat
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.550634 pyrfu-2.4.0/docs/source/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.552639 pyrfu-2.4.0/docs/source/_static/
--rw-r--r--   0 louisr     (501) staff       (20)    18615 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/_static/logo-pyrfu.png
--rw-r--r--   0 louisr     (501) staff       (20)     2011 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/_static/logo-pyrfu.svg
--rw-r--r--   0 louisr     (501) staff       (20)     8992 2023-06-09 14:50:39.000000 pyrfu-2.4.0/docs/source/conf.py
--rw-r--r--   0 louisr     (501) staff       (20)      372 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/contributing.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1044 2023-06-09 09:58:31.000000 pyrfu-2.4.0/docs/source/examples.rst
--rw-r--r--   0 louisr     (501) staff       (20)      192 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/getting_started.rst
--rw-r--r--   0 louisr     (501) staff       (20)      618 2023-04-21 13:33:36.000000 pyrfu-2.4.0/docs/source/index.rst
--rw-r--r--   0 louisr     (501) staff       (20)       72 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/modules.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1283 2023-04-20 14:38:38.000000 pyrfu-2.4.0/docs/source/quick-overview.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.283067 pyrfu-2.4.0/examples/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.553561 pyrfu-2.4.0/examples/00_overview/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.555505 pyrfu-2.4.0/examples/00_overview/.ipynb_checkpoints/
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.0/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.0/examples/00_overview/quick-overview.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.588443 pyrfu-2.4.0/examples/01_mms/
--rw-r--r--   0 louisr     (501) staff       (20)   281483 2023-06-08 15:46:40.000000 pyrfu-2.4.0/examples/01_mms/example_mms_b_e_j.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   564517 2023-06-09 09:46:23.000000 pyrfu-2.4.0/examples/01_mms/example_mms_ebfields.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   371521 2023-06-08 15:46:40.000000 pyrfu-2.4.0/examples/01_mms/example_mms_edr_signatures.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   411079 2023-06-08 15:46:40.000000 pyrfu-2.4.0/examples/01_mms/example_mms_eis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   108423 2023-06-08 16:35:41.000000 pyrfu-2.4.0/examples/01_mms/example_mms_electron_psd.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   432503 2023-06-09 14:51:47.000000 pyrfu-2.4.0/examples/01_mms/example_mms_feeps.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   184196 2023-06-08 15:51:52.000000 pyrfu-2.4.0/examples/01_mms/example_mms_hpca.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   279733 2023-06-08 16:35:41.000000 pyrfu-2.4.0/examples/01_mms/example_mms_ohmslaw.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   353737 2023-06-08 16:40:22.000000 pyrfu-2.4.0/examples/01_mms/example_mms_particle_deflux.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   450116 2023-06-09 09:46:14.000000 pyrfu-2.4.0/examples/01_mms/example_mms_particle_distributions.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   634316 2023-06-09 09:42:51.000000 pyrfu-2.4.0/examples/01_mms/example_mms_particle_pad.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   445067 2023-06-08 15:50:47.000000 pyrfu-2.4.0/examples/01_mms/example_mms_polarizationanalysis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   242849 2023-06-09 07:50:56.000000 pyrfu-2.4.0/examples/01_mms/example_mms_reduced_electron_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   424890 2023-06-09 09:16:19.000000 pyrfu-2.4.0/examples/01_mms/example_mms_reduced_ion_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   205591 2023-06-09 11:46:23.000000 pyrfu-2.4.0/examples/01_mms/example_mms_walen_test.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.590485 pyrfu-2.4.0/examples/02_dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)    51819 2023-06-09 11:47:26.000000 pyrfu-2.4.0/examples/02_dispersion/example_dispersion_one_fluid.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)     2969 2023-06-09 16:03:15.000000 pyrfu-2.4.0/pyproject.toml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.293936 pyrfu-2.4.0/pyrfu/
--rw-r--r--   0 louisr     (501) staff       (20)      334 2023-06-09 15:59:43.000000 pyrfu-2.4.0/pyrfu/__init__.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.596956 pyrfu-2.4.0/pyrfu/__pycache__/
--rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.297869 pyrfu-2.4.0/pyrfu/dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/dispersion/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)    10002 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/dispersion/disp_surf_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3488 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/dispersion/one_fluid_dispersion.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.301473 pyrfu-2.4.0/pyrfu/lp/
--rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-05-15 11:18:18.000000 pyrfu-2.4.0/pyrfu/lp/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/lp/photo_current.py
--rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/lp/thermal_current.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.607856 pyrfu-2.4.0/pyrfu/mms/
--rw-r--r--   0 louisr     (501) staff       (20)     6238 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.0/pyrfu/mms/ancillary.json
--rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/calculate_epsilon.py
--rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     2281 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/copy_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     2196 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/copy_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-05-15 20:29:49.000000 pyrfu-2.4.0/pyrfu/mms/correct_edp_probe_timing.py
--rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/db_get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/db_get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     2658 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/def2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1701 2023-04-21 08:58:14.000000 pyrfu-2.4.0/pyrfu/mms/dft_time_shift.py
--rw-r--r--   0 louisr     (501) staff       (20)     5504 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/download_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     7729 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/download_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/dpf2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     3291 2023-04-21 09:02:25.000000 pyrfu-2.4.0/pyrfu/mms/dsl2gse.py
--rw-r--r--   0 louisr     (501) staff       (20)     3158 2023-04-21 09:02:47.000000 pyrfu-2.4.0/pyrfu/mms/dsl2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-05-15 11:04:37.000000 pyrfu-2.4.0/pyrfu/mms/eis_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/eis_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-04-21 20:23:25.000000 pyrfu-2.4.0/pyrfu/mms/eis_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_pad_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_proton_correction.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/eis_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     4747 2023-05-14 17:25:56.000000 pyrfu-2.4.0/pyrfu/mms/eis_skymap_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_spec_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/eis_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/estimate_phase_speed.py
--rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-05-15 20:31:04.000000 pyrfu-2.4.0/pyrfu/mms/feeps_active_eyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.0/pyrfu/mms/feeps_bad_data.json
--rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_correct_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     3354 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_energy_table.py
--rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_flat_field_corrections.py
--rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/feeps_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/feeps_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/feeps_pitch_angles.py
--rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/feeps_remove_bad_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_remove_sun.py
--rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_sector_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/feeps_split_integral_ch.py
--rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-04-21 10:10:19.000000 pyrfu-2.4.0/pyrfu/mms/fft_bandpass.py
--rw-r--r--   0 louisr     (501) staff       (20)    12130 2023-05-16 12:07:24.000000 pyrfu-2.4.0/pyrfu/mms/fk_power_spectrum_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     9383 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     4902 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_eis_allt.py
--rw-r--r--   0 louisr     (501) staff       (20)     4690 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_feeps_alleyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     2525 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6173 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/get_hpca_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     7052 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_pitch_angle_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)    11547 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/hpca_calc_anodes.py
--rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/hpca_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     5854 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/hpca_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1621 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/hpca_spin_sum.py
--rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/lh_wave_analysis.py
--rw-r--r--   0 louisr     (501) staff       (20)     6790 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/list_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     4366 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/list_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2882 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/load_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2861 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/load_brst_segments.py
--rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/make_model_kappa.py
--rw-r--r--   0 louisr     (501) staff       (20)     7023 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/make_model_rq.py
--rw-r--r--   0 louisr     (501) staff       (20)     7030 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/make_model_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)    25074 2023-05-15 20:42:21.000000 pyrfu-2.4.0/pyrfu/mms/mms_keys.json
--rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-04-21 10:35:28.000000 pyrfu-2.4.0/pyrfu/mms/probe_align_times.py
--rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/psd2def.py
--rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/psd2dpf.py
--rw-r--r--   0 louisr     (501) staff       (20)    18467 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/psd_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     3307 2023-04-21 09:53:59.000000 pyrfu-2.4.0/pyrfu/mms/psd_rebin.py
--rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/read_feeps_sector_masks_csv.py
--rw-r--r--   0 louisr     (501) staff       (20)     9191 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     5568 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/remove_edist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     2099 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/remove_idist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     3224 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/remove_imoms_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     7295 2023-04-21 10:35:32.000000 pyrfu-2.4.0/pyrfu/mms/rotate_tensor.py
--rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/scpot2ne.py
--rw-r--r--   0 louisr     (501) staff       (20)      945 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/spectr_to_dataset.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.634082 pyrfu-2.4.0/pyrfu/mms/sun/
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3854 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/tokenize.py
--rw-r--r--   0 louisr     (501) staff       (20)     3363 2023-06-09 09:40:21.000000 pyrfu-2.4.0/pyrfu/mms/vdf_elim.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/mms/vdf_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)    11804 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/vdf_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     8578 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/vdf_reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     2488 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/vdf_to_e64.py
--rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/mms/whistler_b2e.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.635274 pyrfu-2.4.0/pyrfu/models/
--rw-r--r--   0 louisr     (501) staff       (20)      689 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/models/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     2741 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/models/igrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/models/igrf13coeffs.csv
--rw-r--r--   0 louisr     (501) staff       (20)     6278 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/models/magnetopause_normal.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.419317 pyrfu-2.4.0/pyrfu/plot/
--rw-r--r--   0 louisr     (501) staff       (20)     1645 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/add_position.py
--rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/annotate_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)      935 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/plot/colorbar.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.637708 pyrfu-2.4.0/pyrfu/plot/logo/
--rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
--rw-r--r--   0 louisr     (501) staff       (20)     1160 2023-05-16 12:44:48.000000 pyrfu-2.4.0/pyrfu/plot/make_labels.py
--rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/mms_pl_config.py
--rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/pl_scatter_matrix.py
--rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/pl_tx.py
--rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_clines.py
--rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1495 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_line.py
--rw-r--r--   0 louisr     (501) staff       (20)     3809 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_reduced_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)    11634 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_sitl_overview.py
--rw-r--r--   0 louisr     (501) staff       (20)     4628 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_spectr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/plot_surf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/plot/span_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/plot/zoom.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.649770 pyrfu-2.4.0/pyrfu/pyrf/
--rw-r--r--   0 louisr     (501) staff       (20)     5735 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1964 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/autocorr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2743 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/pyrf/average_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1156 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/avg_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/c_4_grad.py
--rw-r--r--   0 louisr     (501) staff       (20)     4189 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/c_4_j.py
--rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/c_4_k.py
--rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/c_4_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2080 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_ag.py
--rw-r--r--   0 louisr     (501) staff       (20)     1422 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_agyro.py
--rw-r--r--   0 louisr     (501) staff       (20)     1850 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_dng.py
--rw-r--r--   0 louisr     (501) staff       (20)      623 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_dt.py
--rw-r--r--   0 louisr     (501) staff       (20)      646 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_fs.py
--rw-r--r--   0 louisr     (501) staff       (20)     1809 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/calc_sqrtq.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/cart2sph.py
--rw-r--r--   0 louisr     (501) staff       (20)     1997 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/cart2sph_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1654 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/cdfepoch2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/compress_cwt.py
--rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/convert_fac.py
--rw-r--r--   0 louisr     (501) staff       (20)     6686 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/corr_deriv.py
--rw-r--r--   0 louisr     (501) staff       (20)    10734 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/cotrans.py
--rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/cross.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/date_str.py
--rw-r--r--   0 louisr     (501) staff       (20)      821 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/datetime2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      842 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/datetime642iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/datetime642ttns.py
--rw-r--r--   0 louisr     (501) staff       (20)      694 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/datetime642unix.py
--rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/dec_par_perp.py
--rw-r--r--   0 louisr     (501) staff       (20)     2992 2023-05-09 14:12:30.000000 pyrfu-2.4.0/pyrfu/pyrf/dist_append.py
--rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/dot.py
--rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/dynamic_press.py
--rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/e_vxb.py
--rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/eb_nrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    37491 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/ebsp.py
--rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/edb.py
--rw-r--r--   0 louisr     (501) staff       (20)      625 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/end.py
--rw-r--r--   0 louisr     (501) staff       (20)     3113 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/estimate.py
--rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/extend_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     3882 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/filt.py
--rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/find_closest.py
--rw-r--r--   0 louisr     (501) staff       (20)     3978 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/get_omni_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/gradient.py
--rw-r--r--   0 louisr     (501) staff       (20)      987 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/gse2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     2402 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/histogram.py
--rw-r--r--   0 louisr     (501) staff       (20)     3160 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/histogram2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/increments.py
--rw-r--r--   0 louisr     (501) staff       (20)    18762 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/int_sph_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     2106 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/integrate.py
--rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/iplasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)      585 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/iso2unix.py
--rw-r--r--   0 louisr     (501) staff       (20)      875 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/iso86012datetime.py
--rw-r--r--   0 louisr     (501) staff       (20)      626 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/iso86012datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/iso86012timevec.py
--rw-r--r--   0 louisr     (501) staff       (20)      999 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/l_shell.py
--rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/lowpass.py
--rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/pyrf/magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/match_phibe_dir.py
--rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/match_phibe_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/mean.py
--rw-r--r--   0 louisr     (501) staff       (20)     2391 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/mean_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/mean_field.py
--rw-r--r--   0 louisr     (501) staff       (20)     2336 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/medfilt.py
--rw-r--r--   0 louisr     (501) staff       (20)     2362 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/median_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1836 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/movmean.py
--rw-r--r--   0 louisr     (501) staff       (20)     4827 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/mva.py
--rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/new_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/norm.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/normalize.py
--rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/optimize_nbins_1d.py
--rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/optimize_nbins_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     3719 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/pid_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/plasma_beta.py
--rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/plasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/poynting_flux.py
--rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/pres_anis.py
--rw-r--r--   0 louisr     (501) staff       (20)     3060 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/pvi.py
--rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/pvi_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1277 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/read_cdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     2094 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/remove_repeated_points.py
--rw-r--r--   0 louisr     (501) staff       (20)     9204 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/resample.py
--rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.0/pyrfu/pyrf/shock_models_parameters.json
--rw-r--r--   0 louisr     (501) staff       (20)    15260 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/shock_normal.py
--rw-r--r--   0 louisr     (501) staff       (20)     9265 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/shock_parameters.py
--rw-r--r--   0 louisr     (501) staff       (20)     1646 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/solid_angle.py
--rw-r--r--   0 louisr     (501) staff       (20)      905 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/sph2cart.py
--rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/st_diff.py
--rw-r--r--   0 louisr     (501) staff       (20)      600 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/start.py
--rw-r--r--   0 louisr     (501) staff       (20)     1936 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/struct_func.py
--rw-r--r--   0 louisr     (501) staff       (20)     1146 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/t_eval.py
--rw-r--r--   0 louisr     (501) staff       (20)     3837 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/pyrf/time_clip.py
--rw-r--r--   0 louisr     (501) staff       (20)     1212 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/timevec2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)     1501 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/trace.py
--rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/transformation_indices.json
--rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_append.py
--rw-r--r--   0 louisr     (501) staff       (20)      956 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_scalar.py
--rw-r--r--   0 louisr     (501) staff       (20)     3150 2023-05-09 14:12:22.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_tensor_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      672 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_time.py
--rw-r--r--   0 louisr     (501) staff       (20)     1022 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ts_vec_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      928 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/ttns2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)      718 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/unix2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/vht.py
--rw-r--r--   0 louisr     (501) staff       (20)     1749 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/wave_fft.py
--rw-r--r--   0 louisr     (501) staff       (20)     6512 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/wavelet.py
--rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/pyrf/wavepolarize_means.py
--rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/pyrf/waverage.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.652278 pyrfu-2.4.0/pyrfu/solo/
--rw-r--r--   0 louisr     (501) staff       (20)      384 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/solo/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.0/pyrfu/solo/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     1148 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/solo/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     4781 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/solo/read_lfr_density.py
--rw-r--r--   0 louisr     (501) staff       (20)     8500 2023-06-09 14:49:17.000000 pyrfu-2.4.0/pyrfu/solo/read_tnr.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.529721 pyrfu-2.4.0/pyrfu/tests/
--rw-r--r--   0 louisr     (501) staff       (20)      206 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/tests/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1553 2023-04-21 10:37:39.000000 pyrfu-2.4.0/pyrfu/tests/test_pyrf.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.595996 pyrfu-2.4.0/pyrfu.egg-info/
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-09 16:04:31.000000 pyrfu-2.4.0/pyrfu.egg-info/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)    16001 2023-06-09 16:04:31.000000 pyrfu-2.4.0/pyrfu.egg-info/SOURCES.txt
--rw-r--r--   0 louisr     (501) staff       (20)        1 2023-06-09 16:04:31.000000 pyrfu-2.4.0/pyrfu.egg-info/dependency_links.txt
--rw-r--r--   0 louisr     (501) staff       (20)      235 2023-06-09 16:04:31.000000 pyrfu-2.4.0/pyrfu.egg-info/requires.txt
--rw-r--r--   0 louisr     (501) staff       (20)       30 2023-06-09 16:04:31.000000 pyrfu-2.4.0/pyrfu.egg-info/top_level.txt
--rw-r--r--   0 louisr     (501) staff       (20)     2691 2023-06-09 14:45:06.000000 pyrfu-2.4.0/requirements.txt
--rw-r--r--   0 louisr     (501) staff       (20)       38 2023-06-09 16:04:31.654690 pyrfu-2.4.0/setup.cfg
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.280263 pyrfu-2.4.0/venv/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-09 16:04:31.530831 pyrfu-2.4.0/venv/bin/
--rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.0/venv/bin/activate_this.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.189452 pyrfu-2.4.1/
+-rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.1/.flake8
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.952866 pyrfu-2.4.1/.github/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.801874 pyrfu-2.4.1/.github/workflows/
+-rw-r--r--   0 louisr     (501) staff       (20)      570 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.github/workflows/flake8.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      588 2023-06-09 14:46:12.000000 pyrfu-2.4.1/.github/workflows/pylint.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.1/.gitignore
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.809442 pyrfu-2.4.1/.idea/
+-rw-r--r--   0 louisr     (501) staff       (20)      294 2023-06-09 19:35:51.000000 pyrfu-2.4.1/.idea/aws.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.812557 pyrfu-2.4.1/.idea/codeStyles/
+-rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.816298 pyrfu-2.4.1/.idea/inspectionProfiles/
+-rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/vcs.xml
+-rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
+-rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-06-09 14:43:25.000000 pyrfu-2.4.1/.pre-commit-config.yaml
+-rwxr-xr-x   0 louisr     (501) staff       (20)       83 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.readthedocs.yml
+-rw-r--r--   0 louisr     (501) staff       (20)     2972 2023-04-20 14:38:38.000000 pyrfu-2.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.1/LICENSE.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.1/MANIFEST.in
+-rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-10 20:06:20.188637 pyrfu-2.4.1/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)     6490 2023-06-09 10:13:58.000000 pyrfu-2.4.1/README.rst
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.821843 pyrfu-2.4.1/docs/
+-rw-r--r--   0 louisr     (501) staff       (20)      640 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/Makefile
+-rw-r--r--   0 louisr     (501) staff       (20)      341 2023-04-21 12:45:20.000000 pyrfu-2.4.1/docs/environment.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      785 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/make.bat
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.855506 pyrfu-2.4.1/docs/source/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.857951 pyrfu-2.4.1/docs/source/_static/
+-rw-r--r--   0 louisr     (501) staff       (20)    18615 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/_static/logo-pyrfu.png
+-rw-r--r--   0 louisr     (501) staff       (20)     2011 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/_static/logo-pyrfu.svg
+-rw-r--r--   0 louisr     (501) staff       (20)     8992 2023-06-09 14:50:39.000000 pyrfu-2.4.1/docs/source/conf.py
+-rw-r--r--   0 louisr     (501) staff       (20)      372 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/contributing.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1044 2023-06-09 09:58:31.000000 pyrfu-2.4.1/docs/source/examples.rst
+-rw-r--r--   0 louisr     (501) staff       (20)      192 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/getting_started.rst
+-rw-r--r--   0 louisr     (501) staff       (20)      618 2023-04-21 13:33:36.000000 pyrfu-2.4.1/docs/source/index.rst
+-rw-r--r--   0 louisr     (501) staff       (20)       72 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/modules.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1283 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/quick-overview.rst
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.955589 pyrfu-2.4.1/examples/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.859208 pyrfu-2.4.1/examples/00_overview/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.864806 pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/
+-rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.1/examples/00_overview/quick-overview.ipynb
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.936951 pyrfu-2.4.1/examples/01_mms/
+-rw-r--r--   0 louisr     (501) staff       (20)   281483 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_b_e_j.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   564517 2023-06-09 09:46:23.000000 pyrfu-2.4.1/examples/01_mms/example_mms_ebfields.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   371521 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_edr_signatures.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   411079 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_eis.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   108423 2023-06-08 16:35:41.000000 pyrfu-2.4.1/examples/01_mms/example_mms_electron_psd.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   432503 2023-06-09 14:51:47.000000 pyrfu-2.4.1/examples/01_mms/example_mms_feeps.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   184196 2023-06-08 15:51:52.000000 pyrfu-2.4.1/examples/01_mms/example_mms_hpca.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   279733 2023-06-08 16:35:41.000000 pyrfu-2.4.1/examples/01_mms/example_mms_ohmslaw.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   353737 2023-06-08 16:40:22.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_deflux.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   450116 2023-06-09 09:46:14.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_distributions.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   634316 2023-06-09 09:42:51.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_pad.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   445067 2023-06-08 15:50:47.000000 pyrfu-2.4.1/examples/01_mms/example_mms_polarizationanalysis.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   242849 2023-06-09 07:50:56.000000 pyrfu-2.4.1/examples/01_mms/example_mms_reduced_electron_dist.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   424890 2023-06-09 09:16:19.000000 pyrfu-2.4.1/examples/01_mms/example_mms_reduced_ion_dist.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   205591 2023-06-09 11:46:23.000000 pyrfu-2.4.1/examples/01_mms/example_mms_walen_test.ipynb
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.004226 pyrfu-2.4.1/examples/02_dispersion/
+-rw-r--r--   0 louisr     (501) staff       (20)    51819 2023-06-09 11:47:26.000000 pyrfu-2.4.1/examples/02_dispersion/example_dispersion_one_fluid.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)     3050 2023-06-10 20:05:29.000000 pyrfu-2.4.1/pyproject.toml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.966591 pyrfu-2.4.1/pyrfu/
+-rw-r--r--   0 louisr     (501) staff       (20)      334 2023-06-10 20:05:29.000000 pyrfu-2.4.1/pyrfu/__init__.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.034939 pyrfu-2.4.1/pyrfu/__pycache__/
+-rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.968998 pyrfu-2.4.1/pyrfu/dispersion/
+-rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/dispersion/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10002 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/dispersion/disp_surf_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3488 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/dispersion/one_fluid_dispersion.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.973018 pyrfu-2.4.1/pyrfu/lp/
+-rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-05-15 11:18:18.000000 pyrfu-2.4.1/pyrfu/lp/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/lp/photo_current.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/lp/thermal_current.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.091387 pyrfu-2.4.1/pyrfu/mms/
+-rw-r--r--   0 louisr     (501) staff       (20)     6238 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.1/pyrfu/mms/ancillary.json
+-rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/calculate_epsilon.py
+-rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2281 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/copy_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2196 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/copy_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-05-15 20:29:49.000000 pyrfu-2.4.1/pyrfu/mms/correct_edp_probe_timing.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2658 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/def2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1701 2023-04-21 08:58:14.000000 pyrfu-2.4.1/pyrfu/mms/dft_time_shift.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5504 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/download_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7729 2023-06-10 20:03:44.000000 pyrfu-2.4.1/pyrfu/mms/download_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/dpf2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3291 2023-04-21 09:02:25.000000 pyrfu-2.4.1/pyrfu/mms/dsl2gse.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3158 2023-04-21 09:02:47.000000 pyrfu-2.4.1/pyrfu/mms/dsl2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-05-15 11:04:37.000000 pyrfu-2.4.1/pyrfu/mms/eis_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-04-21 20:23:25.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_proton_correction.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4747 2023-05-14 17:25:56.000000 pyrfu-2.4.1/pyrfu/mms/eis_skymap_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_spec_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/estimate_phase_speed.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-05-15 20:31:04.000000 pyrfu-2.4.1/pyrfu/mms/feeps_active_eyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.1/pyrfu/mms/feeps_bad_data.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_correct_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3354 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_energy_table.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_flat_field_corrections.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pitch_angles.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_remove_bad_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_remove_sun.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_sector_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_split_integral_ch.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-04-21 10:10:19.000000 pyrfu-2.4.1/pyrfu/mms/fft_bandpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)    12130 2023-05-16 12:07:24.000000 pyrfu-2.4.1/pyrfu/mms/fk_power_spectrum_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9383 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4902 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_eis_allt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4690 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_feeps_alleyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2525 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6173 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/get_hpca_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7052 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_pitch_angle_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11547 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_calc_anodes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5854 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/hpca_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1621 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_spin_sum.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/lh_wave_analysis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6790 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/list_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4366 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/list_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2882 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/load_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2861 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/load_brst_segments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_kappa.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7023 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_rq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7030 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    25074 2023-05-15 20:42:21.000000 pyrfu-2.4.1/pyrfu/mms/mms_keys.json
+-rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-04-21 10:35:28.000000 pyrfu-2.4.1/pyrfu/mms/probe_align_times.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd2def.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd2dpf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18467 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3307 2023-04-21 09:53:59.000000 pyrfu-2.4.1/pyrfu/mms/psd_rebin.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/read_feeps_sector_masks_csv.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9191 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5568 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_edist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2099 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_idist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3224 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_imoms_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7295 2023-04-21 10:35:32.000000 pyrfu-2.4.1/pyrfu/mms/rotate_tensor.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/scpot2ne.py
+-rw-r--r--   0 louisr     (501) staff       (20)      945 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/spectr_to_dataset.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.163973 pyrfu-2.4.1/pyrfu/mms/sun/
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3854 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/tokenize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3363 2023-06-09 09:40:21.000000 pyrfu-2.4.1/pyrfu/mms/vdf_elim.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/vdf_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11804 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8578 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2488 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_to_e64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/whistler_b2e.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.165571 pyrfu-2.4.1/pyrfu/models/
+-rw-r--r--   0 louisr     (501) staff       (20)      689 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2741 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/igrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/models/igrf13coeffs.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     6278 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/magnetopause_normal.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.429523 pyrfu-2.4.1/pyrfu/plot/
+-rw-r--r--   0 louisr     (501) staff       (20)     1645 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/add_position.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/annotate_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)      935 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/colorbar.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.170127 pyrfu-2.4.1/pyrfu/plot/logo/
+-rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
+-rw-r--r--   0 louisr     (501) staff       (20)     1160 2023-05-16 12:44:48.000000 pyrfu-2.4.1/pyrfu/plot/make_labels.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/mms_pl_config.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/pl_scatter_matrix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/pl_tx.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_clines.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1495 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_line.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3809 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_reduced_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11634 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_sitl_overview.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4628 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_spectr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_surf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/span_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/zoom.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.183483 pyrfu-2.4.1/pyrfu/pyrf/
+-rw-r--r--   0 louisr     (501) staff       (20)     5735 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1964 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/autocorr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2743 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/average_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1156 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/avg_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_grad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4189 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_j.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_k.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2080 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_ag.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1422 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_agyro.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1850 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_dng.py
+-rw-r--r--   0 louisr     (501) staff       (20)      623 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_dt.py
+-rw-r--r--   0 louisr     (501) staff       (20)      646 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_fs.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1809 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_sqrtq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cart2sph.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1997 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cart2sph_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1654 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/cdfepoch2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/compress_cwt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/convert_fac.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6686 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/corr_deriv.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10734 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/cotrans.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cross.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/date_str.py
+-rw-r--r--   0 louisr     (501) staff       (20)      821 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      842 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642ttns.py
+-rw-r--r--   0 louisr     (501) staff       (20)      694 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/dec_par_perp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2992 2023-05-09 14:12:30.000000 pyrfu-2.4.1/pyrfu/pyrf/dist_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/dot.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/dynamic_press.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/e_vxb.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/eb_nrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    37491 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/ebsp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/edb.py
+-rw-r--r--   0 louisr     (501) staff       (20)      625 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/end.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3113 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/estimate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/extend_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3882 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/filt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/find_closest.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3978 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/get_omni_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/gradient.py
+-rw-r--r--   0 louisr     (501) staff       (20)      987 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/gse2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2402 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/histogram.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3160 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/histogram2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/increments.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18801 2023-06-10 20:04:38.000000 pyrfu-2.4.1/pyrfu/pyrf/int_sph_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2106 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/integrate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/iplasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)      585 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso2unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)      875 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime.py
+-rw-r--r--   0 louisr     (501) staff       (20)      626 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012timevec.py
+-rw-r--r--   0 louisr     (501) staff       (20)      999 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/l_shell.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/lowpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/match_phibe_dir.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/match_phibe_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/mean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2391 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mean_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mean_field.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2336 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/medfilt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2362 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/median_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1836 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/movmean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4827 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mva.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/new_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/norm.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/normalize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_1d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3719 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pid_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/plasma_beta.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/plasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/poynting_flux.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pres_anis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3060 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/pvi.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pvi_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1277 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/read_cdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2094 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/remove_repeated_points.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9204 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/resample.py
+-rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_models_parameters.json
+-rw-r--r--   0 louisr     (501) staff       (20)    15260 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_normal.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9265 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_parameters.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1646 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/solid_angle.py
+-rw-r--r--   0 louisr     (501) staff       (20)      905 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/sph2cart.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/st_diff.py
+-rw-r--r--   0 louisr     (501) staff       (20)      600 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/start.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1936 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/struct_func.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1146 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/t_eval.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3837 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/time_clip.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1212 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/timevec2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1501 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/trace.py
+-rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/transformation_indices.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)      956 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_scalar.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3150 2023-05-09 14:12:22.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_tensor_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      672 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_time.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1022 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_vec_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      928 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ttns2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)      718 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/unix2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/vht.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1749 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wave_fft.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6512 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wavelet.py
+-rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wavepolarize_means.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/waverage.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.186141 pyrfu-2.4.1/pyrfu/solo/
+-rw-r--r--   0 louisr     (501) staff       (20)      384 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/solo/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1148 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4781 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/read_lfr_density.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8500 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/read_tnr.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.794898 pyrfu-2.4.1/pyrfu/tests/
+-rw-r--r--   0 louisr     (501) staff       (20)      206 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/tests/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1553 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/tests/test_pyrf.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.033744 pyrfu-2.4.1/pyrfu.egg-info/
+-rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)    16027 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/SOURCES.txt
+-rw-r--r--   0 louisr     (501) staff       (20)        1 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/dependency_links.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      235 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/requires.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       36 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/top_level.txt
+-rw-r--r--   0 louisr     (501) staff       (20)     2691 2023-06-09 14:45:06.000000 pyrfu-2.4.1/requirements.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       38 2023-06-10 20:06:20.189599 pyrfu-2.4.1/setup.cfg
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.952182 pyrfu-2.4.1/venv/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.796417 pyrfu-2.4.1/venv/bin/
+-rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.1/venv/bin/activate_this.py
```

### Comparing `pyrfu-2.4.0/.github/workflows/flake8.yml` & `pyrfu-2.4.1/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/.github/workflows/publish-to-pypi.yml` & `pyrfu-2.4.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/.github/workflows/pylint.yml` & `pyrfu-2.4.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/.idea/inspectionProfiles/Project_Default.xml` & `pyrfu-2.4.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml` & `pyrfu-2.4.1/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/.pre-commit-config.yaml` & `pyrfu-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/CONTRIBUTING.rst` & `pyrfu-2.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/LICENSE.txt` & `pyrfu-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/PKG-INFO` & `pyrfu-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
```

### Comparing `pyrfu-2.4.0/README.rst` & `pyrfu-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/Makefile` & `pyrfu-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/make.bat` & `pyrfu-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/_static/logo-pyrfu.png` & `pyrfu-2.4.1/docs/source/_static/logo-pyrfu.png`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/_static/logo-pyrfu.svg` & `pyrfu-2.4.1/docs/source/_static/logo-pyrfu.svg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/conf.py` & `pyrfu-2.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/examples.rst` & `pyrfu-2.4.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/index.rst` & `pyrfu-2.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/docs/source/quick-overview.rst` & `pyrfu-2.4.1/docs/source/quick-overview.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb` & `pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/00_overview/quick-overview.ipynb` & `pyrfu-2.4.1/examples/00_overview/quick-overview.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_b_e_j.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_b_e_j.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_ebfields.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_ebfields.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_edr_signatures.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_edr_signatures.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_eis.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_eis.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_electron_psd.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_electron_psd.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_feeps.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_feeps.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_hpca.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_hpca.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_ohmslaw.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_ohmslaw.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_particle_deflux.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_particle_deflux.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_particle_distributions.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_particle_distributions.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_particle_pad.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_particle_pad.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_polarizationanalysis.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_polarizationanalysis.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_reduced_electron_dist.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_reduced_electron_dist.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_reduced_ion_dist.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_reduced_ion_dist.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/01_mms/example_mms_walen_test.ipynb` & `pyrfu-2.4.1/examples/01_mms/example_mms_walen_test.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/examples/02_dispersion/example_dispersion_one_fluid.ipynb` & `pyrfu-2.4.1/examples/02_dispersion/example_dispersion_one_fluid.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyproject.toml` & `pyrfu-2.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel==0.38.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfu"
-version = "2.4.0"
+version = "2.4.1"
 description = "Python Space Physics (RymdFysik) Utilities"
 readme = "README.rst"
 authors = [{ name = "Louis RICHARD", email = "louir@irfu.se" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Other Environment",
@@ -56,17 +56,22 @@
 [project.urls]
 homepage = "https://pypi.org/project/pyrfu/"
 documentation = "https://pyrfu.readthedocs.io/en/latest/"
 source = "https://github.com/louis-richard/irfu-python"
 
 
 [tool.setuptools]
-package-dir = {"" = "."}
 include-package-data = true
 
+[tool.setuptools.packages.find]
+where = ["."]
+
+[tool.setuptools.package-data]
+"*" = ["*.json", "*.csv"]
+
 [tool.black]
 py36 = true
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
@@ -107,17 +112,17 @@
     igrf13coeffs.csv,
     mms_keys.json,
     transformation_indices.json
 """
 ignored-modules = "scipy,cdflib"
 
 [tool.bumpver]
-current_version = "2.4.0"
+current_version = "2.4.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
-push            = true
+push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "pyrfu/__init__.py" = ["{version}"]
```

### Comparing `pyrfu-2.4.0/pyrfu/__pycache__/__init__.cpython-38.pyc` & `pyrfu-2.4.1/pyrfu/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/dispersion/disp_surf_calc.py` & `pyrfu-2.4.1/pyrfu/dispersion/disp_surf_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/dispersion/one_fluid_dispersion.py` & `pyrfu-2.4.1/pyrfu/dispersion/one_fluid_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/lp/__init__.py` & `pyrfu-2.4.1/pyrfu/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/lp/photo_current.py` & `pyrfu-2.4.1/pyrfu/lp/photo_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/lp/thermal_current.py` & `pyrfu-2.4.1/pyrfu/lp/thermal_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/__init__.py` & `pyrfu-2.4.1/pyrfu/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/ancillary.json` & `pyrfu-2.4.1/pyrfu/mms/ancillary.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/calculate_epsilon.py` & `pyrfu-2.4.1/pyrfu/mms/calculate_epsilon.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/copy_files.py` & `pyrfu-2.4.1/pyrfu/mms/copy_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/copy_files_ancillary.py` & `pyrfu-2.4.1/pyrfu/mms/copy_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/correct_edp_probe_timing.py` & `pyrfu-2.4.1/pyrfu/mms/correct_edp_probe_timing.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/db_get_ts.py` & `pyrfu-2.4.1/pyrfu/mms/db_get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/db_get_variable.py` & `pyrfu-2.4.1/pyrfu/mms/db_get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/db_init.py` & `pyrfu-2.4.1/pyrfu/mms/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/def2psd.py` & `pyrfu-2.4.1/pyrfu/mms/def2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/dft_time_shift.py` & `pyrfu-2.4.1/pyrfu/mms/dft_time_shift.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/download_ancillary.py` & `pyrfu-2.4.1/pyrfu/mms/download_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/download_data.py` & `pyrfu-2.4.1/pyrfu/mms/download_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import numpy as np
 import pkg_resources
 import requests
 import tqdm
 from dateutil.parser import parse
 
 # Local imports
-from pyrfu.mms import tokenize
+from .tokenize import tokenize
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2022"
 __license__ = "MIT"
 __version__ = "2.3.13"
 __status__ = "Prototype"
```

### Comparing `pyrfu-2.4.0/pyrfu/mms/dpf2psd.py` & `pyrfu-2.4.1/pyrfu/mms/dpf2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/dsl2gse.py` & `pyrfu-2.4.1/pyrfu/mms/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/dsl2gsm.py` & `pyrfu-2.4.1/pyrfu/mms/dsl2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_ang_ang.py` & `pyrfu-2.4.1/pyrfu/mms/eis_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_pad.py` & `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_skymap.py` & `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_combine_proton_spec.py` & `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_moments.py` & `pyrfu-2.4.1/pyrfu/mms/eis_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_omni.py` & `pyrfu-2.4.1/pyrfu/mms/eis_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_pad.py` & `pyrfu-2.4.1/pyrfu/mms/eis_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_pad_combine_sc.py` & `pyrfu-2.4.1/pyrfu/mms/eis_pad_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_pad_spinavg.py` & `pyrfu-2.4.1/pyrfu/mms/eis_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_proton_correction.py` & `pyrfu-2.4.1/pyrfu/mms/eis_proton_correction.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_skymap.py` & `pyrfu-2.4.1/pyrfu/mms/eis_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_skymap_combine_sc.py` & `pyrfu-2.4.1/pyrfu/mms/eis_skymap_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_spec_combine_sc.py` & `pyrfu-2.4.1/pyrfu/mms/eis_spec_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/eis_spin_avg.py` & `pyrfu-2.4.1/pyrfu/mms/eis_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/estimate_phase_speed.py` & `pyrfu-2.4.1/pyrfu/mms/estimate_phase_speed.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_active_eyes.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_active_eyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_bad_data.json` & `pyrfu-2.4.1/pyrfu/mms/feeps_bad_data.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_correct_energies.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_correct_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_energy_table.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_energy_table.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_flat_field_corrections.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_flat_field_corrections.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_omni.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_pad.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_pad_spinavg.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_pitch_angles.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_pitch_angles.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_remove_bad_data.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_remove_bad_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_remove_sun.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_remove_sun.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_sector_spec.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_sector_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_spin_avg.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/feeps_split_integral_ch.py` & `pyrfu-2.4.1/pyrfu/mms/feeps_split_integral_ch.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/fft_bandpass.py` & `pyrfu-2.4.1/pyrfu/mms/fft_bandpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/fk_power_spectrum_4sc.py` & `pyrfu-2.4.1/pyrfu/mms/fk_power_spectrum_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_data.py` & `pyrfu-2.4.1/pyrfu/mms/get_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_dist.py` & `pyrfu-2.4.1/pyrfu/mms/get_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_eis_allt.py` & `pyrfu-2.4.1/pyrfu/mms/get_eis_allt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_feeps_alleyes.py` & `pyrfu-2.4.1/pyrfu/mms/get_feeps_alleyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_feeps_omni.py` & `pyrfu-2.4.1/pyrfu/mms/get_feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_hpca_dist.py` & `pyrfu-2.4.1/pyrfu/mms/get_hpca_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_pitch_angle_dist.py` & `pyrfu-2.4.1/pyrfu/mms/get_pitch_angle_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_ts.py` & `pyrfu-2.4.1/pyrfu/mms/get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/get_variable.py` & `pyrfu-2.4.1/pyrfu/mms/get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/hpca_calc_anodes.py` & `pyrfu-2.4.1/pyrfu/mms/hpca_calc_anodes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/hpca_energies.py` & `pyrfu-2.4.1/pyrfu/mms/hpca_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/hpca_pad.py` & `pyrfu-2.4.1/pyrfu/mms/hpca_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/hpca_spin_sum.py` & `pyrfu-2.4.1/pyrfu/mms/hpca_spin_sum.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/lh_wave_analysis.py` & `pyrfu-2.4.1/pyrfu/mms/lh_wave_analysis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/list_files.py` & `pyrfu-2.4.1/pyrfu/mms/list_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/list_files_ancillary.py` & `pyrfu-2.4.1/pyrfu/mms/list_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/load_ancillary.py` & `pyrfu-2.4.1/pyrfu/mms/load_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/load_brst_segments.py` & `pyrfu-2.4.1/pyrfu/mms/load_brst_segments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/make_model_kappa.py` & `pyrfu-2.4.1/pyrfu/mms/make_model_kappa.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/make_model_rq.py` & `pyrfu-2.4.1/pyrfu/mms/make_model_rq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/make_model_vdf.py` & `pyrfu-2.4.1/pyrfu/mms/make_model_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/mms_keys.json` & `pyrfu-2.4.1/pyrfu/mms/mms_keys.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/probe_align_times.py` & `pyrfu-2.4.1/pyrfu/mms/probe_align_times.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/psd2def.py` & `pyrfu-2.4.1/pyrfu/mms/psd2def.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/psd2dpf.py` & `pyrfu-2.4.1/pyrfu/mms/psd2dpf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/psd_moments.py` & `pyrfu-2.4.1/pyrfu/mms/psd_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/psd_rebin.py` & `pyrfu-2.4.1/pyrfu/mms/psd_rebin.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/read_feeps_sector_masks_csv.py` & `pyrfu-2.4.1/pyrfu/mms/read_feeps_sector_masks_csv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/reduce.py` & `pyrfu-2.4.1/pyrfu/mms/reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/remove_edist_background.py` & `pyrfu-2.4.1/pyrfu/mms/remove_edist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/remove_idist_background.py` & `pyrfu-2.4.1/pyrfu/mms/remove_idist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/remove_imoms_background.py` & `pyrfu-2.4.1/pyrfu/mms/remove_imoms_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/rotate_tensor.py` & `pyrfu-2.4.1/pyrfu/mms/rotate_tensor.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/scpot2ne.py` & `pyrfu-2.4.1/pyrfu/mms/scpot2ne.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/spectr_to_dataset.py` & `pyrfu-2.4.1/pyrfu/mms/spectr_to_dataset.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/tokenize.py` & `pyrfu-2.4.1/pyrfu/mms/tokenize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/vdf_elim.py` & `pyrfu-2.4.1/pyrfu/mms/vdf_elim.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/vdf_omni.py` & `pyrfu-2.4.1/pyrfu/mms/vdf_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/vdf_projection.py` & `pyrfu-2.4.1/pyrfu/mms/vdf_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/vdf_reduce.py` & `pyrfu-2.4.1/pyrfu/mms/vdf_reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/vdf_to_e64.py` & `pyrfu-2.4.1/pyrfu/mms/vdf_to_e64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/mms/whistler_b2e.py` & `pyrfu-2.4.1/pyrfu/mms/whistler_b2e.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/models/__init__.py` & `pyrfu-2.4.1/pyrfu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/models/igrf.py` & `pyrfu-2.4.1/pyrfu/models/igrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/models/igrf13coeffs.csv` & `pyrfu-2.4.1/pyrfu/models/igrf13coeffs.csv`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/models/magnetopause_normal.py` & `pyrfu-2.4.1/pyrfu/models/magnetopause_normal.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/__init__.py` & `pyrfu-2.4.1/pyrfu/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/add_position.py` & `pyrfu-2.4.1/pyrfu/plot/add_position.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/annotate_heatmap.py` & `pyrfu-2.4.1/pyrfu/plot/annotate_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/colorbar.py` & `pyrfu-2.4.1/pyrfu/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg` & `pyrfu-2.4.1/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/make_labels.py` & `pyrfu-2.4.1/pyrfu/plot/make_labels.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/mms_pl_config.py` & `pyrfu-2.4.1/pyrfu/plot/mms_pl_config.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/pl_scatter_matrix.py` & `pyrfu-2.4.1/pyrfu/plot/pl_scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/pl_tx.py` & `pyrfu-2.4.1/pyrfu/plot/pl_tx.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_ang_ang.py` & `pyrfu-2.4.1/pyrfu/plot/plot_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_clines.py` & `pyrfu-2.4.1/pyrfu/plot/plot_clines.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_heatmap.py` & `pyrfu-2.4.1/pyrfu/plot/plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_line.py` & `pyrfu-2.4.1/pyrfu/plot/plot_line.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_magnetosphere.py` & `pyrfu-2.4.1/pyrfu/plot/plot_magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_projection.py` & `pyrfu-2.4.1/pyrfu/plot/plot_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_reduced_2d.py` & `pyrfu-2.4.1/pyrfu/plot/plot_reduced_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_sitl_overview.py` & `pyrfu-2.4.1/pyrfu/plot/plot_sitl_overview.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_spectr.py` & `pyrfu-2.4.1/pyrfu/plot/plot_spectr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/plot_surf.py` & `pyrfu-2.4.1/pyrfu/plot/plot_surf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/span_tint.py` & `pyrfu-2.4.1/pyrfu/plot/span_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/plot/zoom.py` & `pyrfu-2.4.1/pyrfu/plot/zoom.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/__init__.py` & `pyrfu-2.4.1/pyrfu/pyrf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/autocorr.py` & `pyrfu-2.4.1/pyrfu/pyrf/autocorr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/average_vdf.py` & `pyrfu-2.4.1/pyrfu/pyrf/average_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/avg_4sc.py` & `pyrfu-2.4.1/pyrfu/pyrf/avg_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/c_4_grad.py` & `pyrfu-2.4.1/pyrfu/pyrf/c_4_grad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/c_4_j.py` & `pyrfu-2.4.1/pyrfu/pyrf/c_4_j.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/c_4_k.py` & `pyrfu-2.4.1/pyrfu/pyrf/c_4_k.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/c_4_v.py` & `pyrfu-2.4.1/pyrfu/pyrf/c_4_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_ag.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_ag.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_agyro.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_agyro.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_dng.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_dng.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_dt.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_dt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_fs.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_fs.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/calc_sqrtq.py` & `pyrfu-2.4.1/pyrfu/pyrf/calc_sqrtq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/cart2sph.py` & `pyrfu-2.4.1/pyrfu/pyrf/cart2sph.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/cart2sph_ts.py` & `pyrfu-2.4.1/pyrfu/pyrf/cart2sph_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/cdfepoch2datetime64.py` & `pyrfu-2.4.1/pyrfu/pyrf/cdfepoch2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/compress_cwt.py` & `pyrfu-2.4.1/pyrfu/pyrf/compress_cwt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/convert_fac.py` & `pyrfu-2.4.1/pyrfu/pyrf/convert_fac.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/corr_deriv.py` & `pyrfu-2.4.1/pyrfu/pyrf/corr_deriv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/cotrans.py` & `pyrfu-2.4.1/pyrfu/pyrf/cotrans.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/cross.py` & `pyrfu-2.4.1/pyrfu/pyrf/cross.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/date_str.py` & `pyrfu-2.4.1/pyrfu/pyrf/date_str.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/datetime2iso8601.py` & `pyrfu-2.4.1/pyrfu/pyrf/datetime2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/datetime642iso8601.py` & `pyrfu-2.4.1/pyrfu/pyrf/datetime642iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/datetime642ttns.py` & `pyrfu-2.4.1/pyrfu/pyrf/datetime642ttns.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/datetime642unix.py` & `pyrfu-2.4.1/pyrfu/pyrf/datetime642unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/dec_par_perp.py` & `pyrfu-2.4.1/pyrfu/pyrf/dec_par_perp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/dist_append.py` & `pyrfu-2.4.1/pyrfu/pyrf/dist_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/dot.py` & `pyrfu-2.4.1/pyrfu/pyrf/dot.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/dynamic_press.py` & `pyrfu-2.4.1/pyrfu/pyrf/dynamic_press.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/e_vxb.py` & `pyrfu-2.4.1/pyrfu/pyrf/e_vxb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/eb_nrf.py` & `pyrfu-2.4.1/pyrfu/pyrf/eb_nrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ebsp.py` & `pyrfu-2.4.1/pyrfu/pyrf/ebsp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/edb.py` & `pyrfu-2.4.1/pyrfu/pyrf/edb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/end.py` & `pyrfu-2.4.1/pyrfu/pyrf/end.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/estimate.py` & `pyrfu-2.4.1/pyrfu/pyrf/estimate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/extend_tint.py` & `pyrfu-2.4.1/pyrfu/pyrf/extend_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/filt.py` & `pyrfu-2.4.1/pyrfu/pyrf/filt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/find_closest.py` & `pyrfu-2.4.1/pyrfu/pyrf/find_closest.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/get_omni_data.py` & `pyrfu-2.4.1/pyrfu/pyrf/get_omni_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/gradient.py` & `pyrfu-2.4.1/pyrfu/pyrf/gradient.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/gse2gsm.py` & `pyrfu-2.4.1/pyrfu/pyrf/gse2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/histogram.py` & `pyrfu-2.4.1/pyrfu/pyrf/histogram.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/histogram2d.py` & `pyrfu-2.4.1/pyrfu/pyrf/histogram2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/increments.py` & `pyrfu-2.4.1/pyrfu/pyrf/increments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/int_sph_dist.py` & `pyrfu-2.4.1/pyrfu/pyrf/int_sph_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 
                     if use_point * (i_vxg < n_vg):
                         f_g[i_vxg] += f_ijk * c_ijk / d_a
 
     return f_g
 
 
-@numba.jit(fastmath=True)
+@numba.jit(cache=True, nogil=True, parallel=True, nopython=True)
 def mc_cart_3d(
     vdf,
     v,
     phi,
     theta,
     d_v,
     d_v_m,
```

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/integrate.py` & `pyrfu-2.4.1/pyrfu/pyrf/integrate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/iplasma_calc.py` & `pyrfu-2.4.1/pyrfu/pyrf/iplasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/iso2unix.py` & `pyrfu-2.4.1/pyrfu/pyrf/iso2unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/iso86012datetime.py` & `pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/iso86012datetime64.py` & `pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/iso86012timevec.py` & `pyrfu-2.4.1/pyrfu/pyrf/iso86012timevec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/l_shell.py` & `pyrfu-2.4.1/pyrfu/pyrf/l_shell.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/lowpass.py` & `pyrfu-2.4.1/pyrfu/pyrf/lowpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/magnetosphere.py` & `pyrfu-2.4.1/pyrfu/pyrf/magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/match_phibe_dir.py` & `pyrfu-2.4.1/pyrfu/pyrf/match_phibe_dir.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/match_phibe_v.py` & `pyrfu-2.4.1/pyrfu/pyrf/match_phibe_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/mean.py` & `pyrfu-2.4.1/pyrfu/pyrf/mean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/mean_bins.py` & `pyrfu-2.4.1/pyrfu/pyrf/mean_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/mean_field.py` & `pyrfu-2.4.1/pyrfu/pyrf/mean_field.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/medfilt.py` & `pyrfu-2.4.1/pyrfu/pyrf/medfilt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/median_bins.py` & `pyrfu-2.4.1/pyrfu/pyrf/median_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/movmean.py` & `pyrfu-2.4.1/pyrfu/pyrf/movmean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/mva.py` & `pyrfu-2.4.1/pyrfu/pyrf/mva.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/new_xyz.py` & `pyrfu-2.4.1/pyrfu/pyrf/new_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/norm.py` & `pyrfu-2.4.1/pyrfu/pyrf/norm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/normalize.py` & `pyrfu-2.4.1/pyrfu/pyrf/normalize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/optimize_nbins_1d.py` & `pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_1d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/optimize_nbins_2d.py` & `pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/pid_4sc.py` & `pyrfu-2.4.1/pyrfu/pyrf/pid_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/plasma_beta.py` & `pyrfu-2.4.1/pyrfu/pyrf/plasma_beta.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/plasma_calc.py` & `pyrfu-2.4.1/pyrfu/pyrf/plasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/poynting_flux.py` & `pyrfu-2.4.1/pyrfu/pyrf/poynting_flux.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/pres_anis.py` & `pyrfu-2.4.1/pyrfu/pyrf/pres_anis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/psd.py` & `pyrfu-2.4.1/pyrfu/pyrf/psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/pvi.py` & `pyrfu-2.4.1/pyrfu/pyrf/pvi.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/pvi_4sc.py` & `pyrfu-2.4.1/pyrfu/pyrf/pvi_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/read_cdf.py` & `pyrfu-2.4.1/pyrfu/pyrf/read_cdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/remove_repeated_points.py` & `pyrfu-2.4.1/pyrfu/pyrf/remove_repeated_points.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/resample.py` & `pyrfu-2.4.1/pyrfu/pyrf/resample.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/shock_models_parameters.json` & `pyrfu-2.4.1/pyrfu/pyrf/shock_models_parameters.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/shock_normal.py` & `pyrfu-2.4.1/pyrfu/pyrf/shock_normal.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/shock_parameters.py` & `pyrfu-2.4.1/pyrfu/pyrf/shock_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/solid_angle.py` & `pyrfu-2.4.1/pyrfu/pyrf/solid_angle.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/sph2cart.py` & `pyrfu-2.4.1/pyrfu/pyrf/sph2cart.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/st_diff.py` & `pyrfu-2.4.1/pyrfu/pyrf/st_diff.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/start.py` & `pyrfu-2.4.1/pyrfu/pyrf/start.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/struct_func.py` & `pyrfu-2.4.1/pyrfu/pyrf/struct_func.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/t_eval.py` & `pyrfu-2.4.1/pyrfu/pyrf/t_eval.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/time_clip.py` & `pyrfu-2.4.1/pyrfu/pyrf/time_clip.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/timevec2iso8601.py` & `pyrfu-2.4.1/pyrfu/pyrf/timevec2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/trace.py` & `pyrfu-2.4.1/pyrfu/pyrf/trace.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/transformation_indices.json` & `pyrfu-2.4.1/pyrfu/pyrf/transformation_indices.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_append.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_scalar.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_scalar.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_skymap.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_tensor_xyz.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_tensor_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_time.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_time.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ts_vec_xyz.py` & `pyrfu-2.4.1/pyrfu/pyrf/ts_vec_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/ttns2datetime64.py` & `pyrfu-2.4.1/pyrfu/pyrf/ttns2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/unix2datetime64.py` & `pyrfu-2.4.1/pyrfu/pyrf/unix2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/vht.py` & `pyrfu-2.4.1/pyrfu/pyrf/vht.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/wave_fft.py` & `pyrfu-2.4.1/pyrfu/pyrf/wave_fft.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/wavelet.py` & `pyrfu-2.4.1/pyrfu/pyrf/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/wavepolarize_means.py` & `pyrfu-2.4.1/pyrfu/pyrf/wavepolarize_means.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/pyrf/waverage.py` & `pyrfu-2.4.1/pyrfu/pyrf/waverage.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/solo/db_init.py` & `pyrfu-2.4.1/pyrfu/solo/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/solo/read_lfr_density.py` & `pyrfu-2.4.1/pyrfu/solo/read_lfr_density.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/solo/read_tnr.py` & `pyrfu-2.4.1/pyrfu/solo/read_tnr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu/tests/test_pyrf.py` & `pyrfu-2.4.1/pyrfu/tests/test_pyrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/pyrfu.egg-info/PKG-INFO` & `pyrfu-2.4.1/pyrfu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
```

### Comparing `pyrfu-2.4.0/pyrfu.egg-info/SOURCES.txt` & `pyrfu-2.4.1/pyrfu.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -538,8 +538,9 @@
 pyrfu/pyrf/waverage.py
 pyrfu/solo/__init__.py
 pyrfu/solo/config.json
 pyrfu/solo/db_init.py
 pyrfu/solo/read_lfr_density.py
 pyrfu/solo/read_tnr.py
 pyrfu/tests/__init__.py
-pyrfu/tests/test_pyrf.py
+pyrfu/tests/test_pyrf.py
+venv/bin/activate_this.py
```

### Comparing `pyrfu-2.4.0/requirements.txt` & `pyrfu-2.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.0/venv/bin/activate_this.py` & `pyrfu-2.4.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

