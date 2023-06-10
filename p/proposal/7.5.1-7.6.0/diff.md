# Comparing `tmp/proposal-7.5.1.tar.gz` & `tmp/proposal-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proposal-7.5.1.tar", last modified: Thu Mar  9 07:38:06 2023, max compression
+gzip compressed data, was "proposal-7.6.0.tar", last modified: Sat Jun 10 19:36:48 2023, max compression
```

## Comparing `proposal-7.5.1.tar` & `proposal-7.6.0.tar`

### file list

```diff
@@ -1,447 +1,446 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.763184 proposal-7.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-09 07:37:34.000000 proposal-7.5.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-09 07:37:34.000000 proposal-7.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-09 07:37:34.000000 proposal-7.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-03-09 07:38:06.763184 proposal-7.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-03-09 07:37:34.000000 proposal-7.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-09 07:37:34.000000 proposal-7.5.1/conanfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.687184 proposal-7.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-09 07:37:34.000000 proposal-7.5.1/docs/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.691184 proposal-7.5.1/proposal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-03-09 07:38:06.000000 proposal-7.5.1/proposal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21480 2023-03-09 07:38:06.000000 proposal-7.5.1/proposal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 07:38:06.000000 proposal-7.5.1/proposal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 07:38:06.000000 proposal-7.5.1/proposal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-09 07:38:06.000000 proposal-7.5.1/proposal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-09 07:37:34.000000 proposal-7.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-09 07:38:06.763184 proposal-7.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-09 07:37:34.000000 proposal-7.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.691184 proposal-7.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-09 07:37:34.000000 proposal-7.5.1/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.691184 proposal-7.5.1/src/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/Config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.691184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/Constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/DefaultFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/Logging.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/PROPOSAL.h
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/Propagator.h
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/Secondaries.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.695184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.695184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.695184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.695184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.699184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/AnnihilationFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/ComptonFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/IonizationFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/MupairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoeffectFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoproductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/WeakInteractionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.703184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.703184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/DecayTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/StableChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.703184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.707184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Box.h
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Geometry.h
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Sphere.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.707184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Function.h
--rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Integral.h
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/MathMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Spherical3D.h
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Spline.h
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/TableWriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Vector3D.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.707184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/Components.h
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/Medium.h
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/methods.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.707184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/particle/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/particle/Particle.h
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.711184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Time.h
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.711184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/Scattering.h
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/Bremsstrahlung.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.715184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.719184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/PROPOSAL/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/detail/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Constants.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Logging.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    24313 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.723184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.727184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.727184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.727184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.735184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    23803 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)  1205025 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.735184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.735184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.739184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.739184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    66888 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    54597 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.739184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/methods.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.739184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/particle/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.743184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Displacment.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Time.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.683184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.743184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.683184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.743184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.743184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.743184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.687184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-09 07:37:34.000000 proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.747184 proposal-7.5.1/src/pyPROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.751184 proposal-7.5.1/src/pyPROPOSAL/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/components.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/crosssection.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/decay.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/density_distribution.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/math.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/medium.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    48088 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/parametrization.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    34074 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/particle.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/pybindings.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/scattering.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/detail/secondaries.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.751184 proposal-7.5.1/src/pyPROPOSAL/pyPROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-09 07:37:34.000000 proposal-7.5.1/src/pyPROPOSAL/pyPROPOSAL/pyBindings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.759184 proposal-7.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Annihilation_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Bremsstrahlung_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Compton_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/ContinuousRandomization_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/CrossSection_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/DecayChannel_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/DecayTable_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Decay_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Density_distribution_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Displacement_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/EnergyCutSettings_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Epairproduction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    42070 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Geometry_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Integral_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Interaction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Interpolant_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Ionization_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/MathMethods_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Medium_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Mupairproduction_TEST.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.759184 proposal-7.5.1/tests/PROPOSALTestUtilities/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/PROPOSALTestUtilities/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/PROPOSALTestUtilities/TestFilesHandling.h
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/ParticleDef_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Particle_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/PhotoMuPair_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/PhotoPair_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Photoeffect_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    23832 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Photonuclear_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Propagator_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Scattering_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Secondaries_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/SecondaryProduction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Sector_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Spline_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Time_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/UtilityIntegral_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/UtilityInterpolant_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Utility_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/Vector3D_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/WeakInteraction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/conanfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.763184 proposal-7.5.1/tests/gen_testfiles_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/annihilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/bremsstrahlung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/compton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/continous_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/epairproduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/ionization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/mupairproduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/photomupair.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/photonuclear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/photopair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/gen_testfiles_scripts/weak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:38:06.763184 proposal-7.5.1/tests/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-09 07:37:34.000000 proposal-7.5.1/tests/python/test_continuous_loss_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-10 19:36:26.000000 proposal-7.6.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-10 19:36:26.000000 proposal-7.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-10 19:36:26.000000 proposal-7.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-10 19:36:48.200896 proposal-7.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-10 19:36:26.000000 proposal-7.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-10 19:36:26.000000 proposal-7.6.0/conanfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-10 19:36:26.000000 proposal-7.6.0/docs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/proposal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:36:47.000000 proposal-7.6.0/proposal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 19:36:26.000000 proposal-7.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-10 19:36:48.200896 proposal-7.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-10 19:36:26.000000 proposal-7.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 19:36:26.000000 proposal-7.6.0/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/src/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.148895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/DefaultFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/PROPOSAL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Propagator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Secondaries.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.152895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.152895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/AnnihilationFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/ComptonFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/IonizationFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/MupairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoeffectFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoproductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/WeakInteractionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/StableChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Box.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Geometry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Sphere.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Function.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Integral.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/MathMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spherical3D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/TableWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Vector3D.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Components.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Medium.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/methods.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/Particle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Time.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/Scattering.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/Bremsstrahlung.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Constants.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Logging.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    24313 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    23803 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)  1205025 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    66888 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    54597 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/methods.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Displacment.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Time.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.132895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.136895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.136895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/pyPROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.192896 proposal-7.6.0/src/pyPROPOSAL/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/components.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/crosssection.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/decay.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/density_distribution.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/math.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/medium.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/parametrization.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    34074 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/particle.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/pybindings.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/scattering.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/secondaries.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.192896 proposal-7.6.0/src/pyPROPOSAL/pyPROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/pyPROPOSAL/pyBindings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.196896 proposal-7.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Annihilation_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Bremsstrahlung_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Compton_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/ContinuousRandomization_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/CrossSection_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/DecayChannel_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/DecayTable_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Decay_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Density_distribution_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Displacement_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/EnergyCutSettings_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Epairproduction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    42070 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Geometry_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Integral_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Interaction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Interpolant_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Ionization_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/MathMethods_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Medium_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Mupairproduction_TEST.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.196896 proposal-7.6.0/tests/PROPOSALTestUtilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PROPOSALTestUtilities/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PROPOSALTestUtilities/TestFilesHandling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/ParticleDef_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Particle_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PhotoMuPair_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PhotoPair_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Photoeffect_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    23832 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Photonuclear_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Propagator_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Scattering_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Secondaries_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/SecondaryProduction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Sector_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Spline_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Time_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/UtilityIntegral_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/UtilityInterpolant_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Utility_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Vector3D_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/WeakInteraction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/conanfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/tests/gen_testfiles_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/annihilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/bremsstrahlung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/compton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/continous_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/epairproduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/ionization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/mupairproduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photomupair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photonuclear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photopair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/weak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/python/test_continuous_loss_output.py
```

### Comparing `proposal-7.5.1/CMakeLists.txt` & `proposal-7.6.0/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 cmake_minimum_required(VERSION 3.9)
 
 set(PROPOSAL_VERSION_MAJOR 7)
-set(PROPOSAL_VERSION_MINOR 5)
-set(PROPOSAL_VERSION_PATCH 1)
+set(PROPOSAL_VERSION_MINOR 6)
+set(PROPOSAL_VERSION_PATCH 0)
 set(PROPOSAL_VERSION ${PROPOSAL_VERSION_MAJOR}.${PROPOSAL_VERSION_MINOR}.${PROPOSAL_VERSION_PATCH})
 
 project(PROPOSAL
     VERSION ${PROPOSAL_VERSION}
     LANGUAGES CXX
     DESCRIPTION "The very best photon and lepton propagator."
     )
 
-if (EXISTS ${CMAKE_BINARY_DIR}/conan_paths.cmake)
-    include(${CMAKE_BINARY_DIR}/conan_paths.cmake)
-endif()
-
 if(NOT CMAKE_BUILD_TYPE)
   message(STATUS "No build type has been specified. Using default system build type. You may want to change this to"
   	"'Release' if you are using PROPOSAL for production purposes.")
 else()
 	if(CMAKE_BUILD_TYPE STREQUAL "Debug" OR CMAKE_BUILD_TYPE STREQUAL "DEBUG")
   		message(WARNING "Build type set to ${CMAKE_BUILD_TYPE}. This build type should only be used for development "
   			"and debugging purposes and not for production since the runtime of PROPOSAL with be significantly higher!")
```

### Comparing `proposal-7.5.1/LICENSE.md` & `proposal-7.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/PKG-INFO` & `proposal-7.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proposal
-Version: 7.5.1
+Version: 7.6.0
 Summary: Monte Carlo simulation library to propagate leptons and gamma rays
 Home-page: https://github.com/tudo-astroparticlephysics/PROPOSAL
 Author: PROPOSAL Development Team
 Author-email: jean-marco.alameddine@tu-dortmund.de
 License: LGPLv3
 Platform: unix
 Classifier: Intended Audience :: Science/Research
```

### Comparing `proposal-7.5.1/README.md` & `proposal-7.6.0/README.md`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/proposal.egg-info/PKG-INFO` & `proposal-7.6.0/proposal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proposal
-Version: 7.5.1
+Version: 7.6.0
 Summary: Monte Carlo simulation library to propagate leptons and gamma rays
 Home-page: https://github.com/tudo-astroparticlephysics/PROPOSAL
 Author: PROPOSAL Development Team
 Author-email: jean-marco.alameddine@tu-dortmund.de
 License: LGPLv3
 Platform: unix
 Classifier: Intended Audience :: Science/Research
```

### Comparing `proposal-7.5.1/proposal.egg-info/SOURCES.txt` & `proposal-7.6.0/proposal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h
+src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h
 src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h
 src/PROPOSAL/detail/CMakeLists.txt
 src/PROPOSAL/detail/PROPOSAL/Constants.cxx
 src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx
 src/PROPOSAL/detail/PROPOSAL/Logging.cxx
@@ -279,15 +280,14 @@
 src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx
-src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx
 src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx
 src/pyPROPOSAL/CMakeLists.txt
```

### Comparing `proposal-7.5.1/setup.cfg` & `proposal-7.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/CMakeLists.txt` & `proposal-7.6.0/src/PROPOSAL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/Config.cmake.in` & `proposal-7.6.0/src/PROPOSAL/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/Constants.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Constants.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/DefaultFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/DefaultFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/Logging.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Logging.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/PROPOSAL.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/PROPOSAL.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/Propagator.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Propagator.h`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     std::vector<std::shared_ptr<CrossSectionBase>> CreateCrossSectionList(
         const ParticleDef& p_def, const Medium& medium,
         std::shared_ptr<const EnergyCutSettings> cuts, bool interpolate,
         double density_correction, const nlohmann::json& config);
 
     ParticleDef p_def;
     enum Type : int {
-        MinimalE = 0,
-        Decay = 1,
+        Decay = 0,
+        MinimalE = 1,
         Stochastic = 2,
     };
     enum AdvancementType : int {
         InvalidStep = 0,
         ReachedInteraction = 1,
         ReachedMaxDistance = 2,
         ReachedBorder = 3
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/Secondaries.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Secondaries.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -106,26 +106,26 @@
 
 template<>
 template <typename CrossVec, typename P, typename M>
 void DefaultCrossSections<EMinusDef>::Append(CrossVec& cross_vec, P p, M m,std::shared_ptr<const EnergyCutSettings> cut, bool interpolate)
 {
     auto brems = std::make_tuple(crosssection::BremsElectronScreening{ false }, p, m, cut, interpolate);
     auto epair = std::make_tuple(crosssection::EpairForElectronPositron{ false }, p, m, cut, interpolate);
-    auto ioniz = std::make_tuple(crosssection::IonizBergerSeltzerBhabha{ EnergyCutSettings(*cut) }, p, m, cut, interpolate);
+    auto ioniz = std::make_tuple(crosssection::IonizBergerSeltzerMoller{ EnergyCutSettings(*cut) }, p, m, cut, interpolate);
     auto photo = std::make_tuple(crosssection::PhotoAbramowiczLevinLevyMaor97 { make_unique<crosssection::ShadowButkevichMikheyev>() }, p, m, cut, interpolate);
     append_cross(cross_vec, brems, epair, ioniz, photo);
 }
 
 template<>
 template <typename CrossVec, typename P, typename M>
 void DefaultCrossSections<EPlusDef>::Append(CrossVec& cross_vec, P p, M m,std::shared_ptr<const EnergyCutSettings> cut, bool interpolate)
 {
     auto brems = std::make_tuple(crosssection::BremsElectronScreening{ false }, p, m, cut, interpolate);
     auto epair = std::make_tuple(crosssection::EpairForElectronPositron{ false }, p, m, cut, interpolate);
-    auto ioniz = std::make_tuple(crosssection::IonizBergerSeltzerMoller{ EnergyCutSettings(*cut) }, p, m, cut, interpolate);
+    auto ioniz = std::make_tuple(crosssection::IonizBergerSeltzerBhabha{ EnergyCutSettings(*cut) }, p, m, cut, interpolate);
     auto photo = std::make_tuple(crosssection::PhotoAbramowiczLevinLevyMaor97 { make_unique<crosssection::ShadowButkevichMikheyev>() }, p, m, cut, interpolate);
     auto annih = std::make_tuple(crosssection::AnnihilationHeitler{}, p, m, nullptr, interpolate);
     append_cross(cross_vec, brems, epair, ioniz, photo, annih);
 }
 
 
 template<>
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h`

 * *Files 18% similar despite different names*

```diff
@@ -95,10 +95,40 @@
             std::unique_ptr<ParametrizationDirect> clone() const override;
             double PhotonNucleonCrossSection(double, const Component&) override;
         };
 
         template <> struct ParametrizationName<PhotoproductionRhode> {
             static constexpr auto value = "Rhode";
         };
+
+        class PhotoproductionHeck : virtual public Photoproduction {
+            double sigma_bw(double s, double E, double M, double Gamma, double Sigma0);
+            double Q(double E, double E_th, double w);
+            const std::array<double, 3> resonances_M;
+            const std::array<double, 3> resonances_Gamma;
+            const std::array<double, 3> resonances_Sigma0;
+            const std::array<double, 3> resonances_w;
+
+        public:
+            PhotoproductionHeck();
+            std::unique_ptr<ParametrizationDirect> clone() const override;
+            double PhotonNucleonCrossSection(double, const Component&) override;
+        };
+
+        template <> struct ParametrizationName<PhotoproductionHeck> {
+            static constexpr auto value = "Heck";
+        };
+
+        class PhotoproductionHeckC7Shadowing : virtual public PhotoproductionHeck {
+        public:
+            PhotoproductionHeckC7Shadowing();
+            double PhotonAtomCrossSection(double energy, const Component& comp) override;
+            std::unique_ptr<ParametrizationDirect> clone() const override;
+        };
+
+        template <> struct ParametrizationName<PhotoproductionHeckC7Shadowing> {
+            static constexpr auto value = "HeckC7Shadowing";
+        };
+
     }
 }
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/DecayTable.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayTable.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/StableChannel.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/StableChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Box.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Box.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Geometry.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Geometry.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/geometry/Sphere.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Sphere.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Function.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Function.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Integral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Integral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Interpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Interpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/MathMethods.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/MathMethods.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Spherical3D.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spherical3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Spline.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spline.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/TableWriter.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/TableWriter.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/math/Vector3D.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Vector3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/Components.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Components.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/Medium.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Medium.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/methods.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/methods.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/particle/Particle.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/Particle.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/Scattering.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/Scattering.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h`

 * *Files 16% similar despite different names*

```diff
@@ -23,70 +23,51 @@
  *         GitHub webpage                                                     *
  *                                                                            *
  *         "https://github.com/tudo-astroparticlephysics/PROPOSAL"            *
  *                                                                            *
  ******************************************************************************/
 
 #pragma once
-
-#include <array>
-#include <vector>
-
-#include "PROPOSAL/medium/Medium.h"
-#include "PROPOSAL/scattering/multiple_scattering/Parametrization.h"
+#include "PROPOSAL/math/Vector3D.h"
+#include <memory>
+#include <utility>
 
 namespace PROPOSAL {
-struct ParticleDef;
-
 namespace multiple_scattering {
+    struct ScatteringOffset {
+        ScatteringOffset() : sx(0.), sy(0.), tx(0.), ty(0.) {};
+        friend std::ostream& operator<<(std::ostream& os, const ScatteringOffset& offset) {
+            os << "sx: " << offset.sx << ", sy: " << offset.sy << ", tx: " << offset.tx << ", ty: " << offset.ty  << '\n';
+            return os;
+        };
+        double sx;
+        double sy;
+        double tx;
+        double ty;
+    };
 
-    class Moliere : public Parametrization {
-        bool compare(const Parametrization&) const override;
-        void print(std::ostream&) const override;
-
-        std::unique_ptr<Parametrization> clone() const final
-        {
-            return std::make_unique<Moliere>(*this);
-        }
-
-        int numComp_; // number of components in medium
-        double ZSq_A_average_;
-        std::vector<double> Zi_; // nuclear charge of different components
-        std::vector<double>
-            weight_ZZ_;        // mass weights of different components time Z^2
-        double weight_ZZ_sum_; // inverse of sum of mass weights of different
-                               // components time Z^2
-        int max_weight_index_; // index of the maximium of mass weights of
-                               // different components
-
-        // scattering parameters
-        double chiCSq_; // characteristic angle² in rad²
-        std::vector<double> B_;
-
-        double f1M(double x);
-        double f2M(double x);
+    std::pair<Cartesian3D, Cartesian3D> ScatterInitialDirection(
+            const Vector3D&, const ScatteringOffset&);
 
-        double f(double theta);
+    class Parametrization {
+    protected:
+        double mass;
 
-        double F1M(double x);
-        double F2M(double x);
+    public:
+        Parametrization() = default;
+        Parametrization(double mass);
+        virtual ~Parametrization() = default;
 
-        double F(double theta);
+        virtual std::unique_ptr<Parametrization> clone() const = 0;
 
-        double GetRandom(double pre_factor, double rnd);
+        virtual bool compare(const Parametrization&) const = 0;
+        virtual void print(std::ostream&) const = 0;
 
-    public:
-        // constructor
-        Moliere(const ParticleDef&, Medium const&);
+        virtual ScatteringOffset CalculateRandomAngle(double grammage,
+            double ei, double ef, const std::array<double, 4>& rnd)
+            = 0;
 
-        ScatteringOffset CalculateRandomAngle(double grammage, double ei,
-            double ef, const std::array<double, 4>& rnd) override;
+        virtual bool operator==(const Parametrization& scattering) const;
+        friend std::ostream& operator<<(std::ostream&, Parametrization const&);
     };
 } // namespace multiple_scattering
-
-template <typename... Args> inline auto make_moliere(Args... args)
-{
-    return std::unique_ptr<multiple_scattering::Parametrization>(
-        new multiple_scattering::Moliere(std::forward<Args>(args)...));
-}
-
 } // namespace PROPOSAL
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h`

 * *Files 14% similar despite different names*

```diff
@@ -47,31 +47,35 @@
 
 namespace PROPOSAL {
 
 enum class MultipleScatteringType : int {
     NoScattering,
     Moliere,
     Highland,
-    HighlandIntegral
+    HighlandIntegral,
+    MoliereInterpol
 };
 
 static const std::unordered_map<std::string, MultipleScatteringType>
     MultipleScatteringTable = { { "moliere", MultipleScatteringType::Moliere },
         { "highland", MultipleScatteringType::Highland },
         { "highlandintegral", MultipleScatteringType::HighlandIntegral },
-        { "noscattering", MultipleScatteringType::NoScattering } };
+        { "noscattering", MultipleScatteringType::NoScattering },
+        { "moliereinterpol", MultipleScatteringType::MoliereInterpol }};
 
 inline auto make_multiple_scattering(
     MultipleScatteringType t, ParticleDef const& p, Medium const& m)
 {
     switch (t) {
     case MultipleScatteringType::Highland:
         return make_highland(p, m);
     case MultipleScatteringType::Moliere:
         return make_moliere(p, m);
+    case MultipleScatteringType::MoliereInterpol:
+         return make_moliereinterpol(p, m);
     case MultipleScatteringType::NoScattering:
         return std::unique_ptr<multiple_scattering::Parametrization>(nullptr);
     default:
         throw std::out_of_range("This constructor is not provided.");
     }
 }
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 #pragma once
 
-#include "PROPOSAL/crosssection/parametrization/EpairProduction.h"
+#include "PROPOSAL/crosssection/parametrization/MupairProduction.h"
 #include "PROPOSAL/math/Integral.h"
 #include "PROPOSAL/medium/Medium.h"
-#include "PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h"
+#include "PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h"
 
 namespace PROPOSAL {
 namespace secondaries {
-    class KelnerKokoulinPetrukhinEpairProduction
-        : public secondaries::EpairProduction,
-          public DefaultSecondaries<KelnerKokoulinPetrukhinEpairProduction> {
+    class KelnerKokoulinPetrukhinMupairProduction
+        : public secondaries::MupairProduction,
+          public DefaultSecondaries<KelnerKokoulinPetrukhinMupairProduction> {
 
-        crosssection::EpairKelnerKokoulinPetrukhin param;
+        crosssection::MupairKelnerKokoulinPetrukhin param;
         Integral integral;
         ParticleDef p_def;
-        static constexpr int n_rnd = 3;
 
-        std::tuple<Cartesian3D, Cartesian3D> CalculateDirections(
-            const Vector3D&, double, double, double);
-        std::tuple<double, double> CalculateEnergy(double, double);
+        static constexpr int n_rnd = 3;
 
     public:
-        KelnerKokoulinPetrukhinEpairProduction(
+        KelnerKokoulinPetrukhinMupairProduction(
             const ParticleDef& p, const Medium&)
-            : param(false)
-            , p_def(p)
+            : p_def(p)
         {
         }
-        // TODO: set lpm to true when possible
 
-        double CalculateRho(double, double, const Component&, double, double);
+        double CalculateRho(double, double, const Component&, double, double) final;
+        std::tuple<Cartesian3D, Cartesian3D> CalculateDirections(
+            const Vector3D&, double, double, double) final;
+        std::tuple<double, double> CalculateEnergy(double, double) final;
 
         size_t RequiredRandomNumbers() const noexcept final { return n_rnd; }
         std::vector<ParticleState> CalculateSecondaries(
-            StochasticLoss, const Component&, std::vector<double>&) final;
+                StochasticLoss, const Component&, std::vector<double>&) final;
     };
 } // namespace secondaries
 } // namespace PROPOSAL
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #pragma once
 
 #include "PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h"
 #include "PROPOSAL/crosssection/parametrization/PhotoPairProduction.h"
 #include "PROPOSAL/math/Integral.h"
+#include "PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h"
 
 namespace PROPOSAL {
 namespace secondaries {
     class PhotoPairProductionTsaiForwardPeaked : public PhotoPairProductionInterpolant<crosssection::PhotoPairTsai> {
 
     public:
         PhotoPairProductionTsaiForwardPeaked() = default;
@@ -26,9 +27,27 @@
         PhotoPairProductionTsai(ParticleDef p, Medium m)
             : PhotoPairProductionTsaiForwardPeaked(p, m) {}
 
         std::tuple<Cartesian3D, Cartesian3D> CalculateDirections(
                 const Vector3D&, double, double, const Component&,
                 double, double, double) override;
     };
+
+    class PhotoPairProductionTsaiSauter : public PhotoPairProductionTsaiForwardPeaked, public SauterSampling {
+    public:
+        PhotoPairProductionTsaiSauter() = default;
+        PhotoPairProductionTsaiSauter(ParticleDef p, Medium m)
+            : PhotoPairProductionTsaiForwardPeaked(p, m)
+        {}
+
+        std::tuple<Cartesian3D, Cartesian3D> CalculateDirections(
+                const Vector3D& dir, double energy, double rho,
+                const Component& comp, double rnd1, double rnd2, double rnd3) override {
+            auto energies = CalculateEnergy(energy, rho);
+            double E_electron = std::get<0>(energies);
+            double E_positron = std::get<1>(energies);
+            return SauterSampling::CalculateDirections(dir, comp, rnd1, rnd2, rnd3, E_electron, E_positron);
+        };
+    };
+
 } // namespace secondaries
 } // namespace PROPOSAL
```

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h` & `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Constants.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Constants.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 auto init_param = std::make_pair(std::string(crosssection::ParametrizationName<Param>::value), create_photoproduction<Param>);
 
 std::map<std::string, photo_func_ptr, Helper::case_insensitive_comp> photoproduction_map = {
         init_param<crosssection::PhotoproductionZeus>,
         init_param<crosssection::PhotoproductionBezrukovBugaev>,
         init_param<crosssection::PhotoproductionCaldwell>,
         init_param<crosssection::PhotoproductionKokoulin>,
-        init_param<crosssection::PhotoproductionRhode>
+        init_param<crosssection::PhotoproductionRhode>,
+        init_param<crosssection::PhotoproductionHeck>,
+        init_param<crosssection::PhotoproductionHeckC7Shadowing>
 };
 
 namespace PROPOSAL {
     cross_ptr make_photoproduction(const ParticleDef &p_def, const Medium &medium,
                                    const nlohmann::json &config) {
         if (!config.contains("parametrization"))
             throw std::logic_error("No parametrization passed for photoproduction");
```

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx`

 * *Files 12% similar despite different names*

```diff
@@ -205,8 +205,86 @@
     if (nu <= 0.1) {
         return 0.; // do not extrapolate
     } else if (nu <= 200.) {
         return std::max(interpolant_->InterpolateArray(nu), 0.);
     } else {
         return PhotoproductionCaldwell::PhotonNucleonCrossSection(energy, comp);
     }
-}
+}
+
+// Heck
+crosssection::PhotoproductionHeck::PhotoproductionHeck() : resonances_M{{1.231, 1.515, 1.680}},
+                                                           resonances_Gamma{{0.11, 0.11, 0.125}},
+                                                           resonances_Sigma0{{31.125, 25.567, 17.508}},
+                                                           resonances_w{{0.17, 0.38, 0.38}} {
+    hash_combine(hash, std::string(crosssection::ParametrizationName<PhotoproductionHeck>::value));
+};
+
+std::unique_ptr<crosssection::ParametrizationDirect> crosssection::PhotoproductionHeck::clone() const {
+    using param_t = std::remove_cv_t<std::remove_pointer_t<decltype(this)>>;
+    return std::make_unique<param_t>(*this);
+}
+
+// ------------------------------------------------------------------------- //
+// Formulae of continuum are from https://web.iap.kit.edu/heck/publications/kit-swp-6_vectormeson.pdf
+// The resonances are implemented according to https://arxiv.org/pdf/astro-ph/9903478.pdf using the
+// Delta(1232), N(1520) and N(1680) resonance.
+// To describe shadowing, the parametrization by BezrukovBugaev is used
+// ------------------------------------------------------------------------- //
+double crosssection::PhotoproductionHeck::PhotonNucleonCrossSection(double energy, const Component& comp) {
+    if (energy < GetCutOff(comp))
+        return 0.;
+    energy *= 1e-3; // energy in GeV
+    double m_n = comp.GetAverageNucleonWeight() * 1e-3; // in GeV
+    double s = m_n * m_n + 2 * m_n * energy; // calculate squared center of mass energy in GeV^2
+    double s0 = std::pow(1.0761, 2); // pion production threshold
+
+    double total_cross;
+
+    // calculate continuum of crosssection
+    if (std::sqrt(s) < 19.39)
+        total_cross = (73.7 * std::pow(s, 0.073) + 191.7 * std::pow(s, -0.602)) * std::sqrt(1 - s0/s); // in µb
+    else
+        total_cross = 59.3 * std::pow(s, 0.093) + 120.2 * std::pow(s, -0.358); // in µb
+
+    // add resonances
+    for (unsigned int i = 0; i<resonances_M.size(); i++) {
+        total_cross += sigma_bw(s, energy, resonances_M.at(i), resonances_Gamma.at(i), resonances_Sigma0.at(i))
+                * Q(energy, 0.152, resonances_w.at(i));
+    }
+
+    return total_cross;
+}
+
+double crosssection::PhotoproductionHeck::sigma_bw(double s, double E, double M, double Gamma, double Sigma0) {
+        return s / (E * E) * Sigma0 * Gamma * Gamma * s / (std::pow(s - M*M, 2) + Gamma * Gamma * s);
+}
+
+double crosssection::PhotoproductionHeck::Q(double E, double E_th, double w) {
+    if (E < E_th)
+        return 0;
+    if (E >= w + E_th)
+        return 1;
+    return (E - E_th) / w;
+}
+
+
+// HeckC7Shadowing
+crosssection::PhotoproductionHeckC7Shadowing::PhotoproductionHeckC7Shadowing() {
+    hash_combine(hash, std::string(crosssection::ParametrizationName<PhotoproductionHeckC7Shadowing>::value));
+};
+
+std::unique_ptr<crosssection::ParametrizationDirect> crosssection::PhotoproductionHeckC7Shadowing::clone() const {
+    using param_t = std::remove_cv_t<std::remove_pointer_t<decltype(this)>>;
+    return std::make_unique<param_t>(*this);
+}
+
+// ------------------------------------------------------------------------- //
+// Use simplified shadowing method according to https://web.iap.kit.edu/heck/publications/kit-swp-6_vectormeson.pdf
+// or Phys. Rev. D 32 (1985) 1244 (https://journals.aps.org/prd/pdf/10.1103/PhysRevD.32.1244)
+// ------------------------------------------------------------------------- //
+double crosssection::PhotoproductionHeckC7Shadowing::PhotonAtomCrossSection(double energy, const Component& comp) {
+    auto cross_photon_nucleon = PhotonNucleonCrossSection(energy, comp);
+    if (cross_photon_nucleon == 0.)
+        return 0.;
+    return cross_photon_nucleon * std::pow(comp.GetAtomicNum(), 0.91);
+};
```

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/methods.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/methods.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 #include "PROPOSAL/Constants.h"
 #include "PROPOSAL/math/MathMethods.h"
 #include "PROPOSAL/medium/Medium.h"
 #include "PROPOSAL/particle/ParticleDef.h"
 #include "PROPOSAL/scattering/multiple_scattering/Coefficients.h"
 #include "PROPOSAL/scattering/multiple_scattering/Moliere.h"
+#include <CubicInterpolation/Axis.h>
+#include "PROPOSAL/Logging.h"
 
 using namespace PROPOSAL::multiple_scattering;
 
 ScatteringOffset Moliere::CalculateRandomAngle(
     double grammage, double ei, double ef, const std::array<double, 4>& rnd)
 {
     (void)ef;
@@ -358,15 +360,75 @@
     // only regarding the component with maximum weight
     double theta_np1 = pre_factor * normalppf(rnd) / SQRT2;
 
     // rnd element of ]-0.5,0.5]
     rnd = rnd - 0.5;
 
     // iterating until the number of correct digits is greater than 4
+    unsigned int i = 0;
     do {
+        i++;
         theta_n = theta_np1;
         theta_np1 = theta_n - (F(theta_n) - rnd) / f(theta_n);
-
+        if (i == 100) {
+            Logging::Get("proposal.scattering")->warn(
+                    "Iteration in Moliere::GetRandom did not converge after 100 iterations. "
+                    "Return current value theta = {} (previous iteration: theta = {}", theta_np1, theta_n);
+            return theta_np1;
+        }
     } while (std::abs((theta_n - theta_np1) / theta_np1) > 1e-4);
 
     return theta_np1;
 }
+
+MoliereInterpol::MoliereInterpol(const ParticleDef& p_def, const Medium& medium) : Moliere(p_def, medium) {
+    // initialize interpolation tables
+    Logging::Get("proposal.scattering")->debug("Initialize interpooation tables for MoliereInterpol.");
+
+    auto def_f1M = cubic_splines::CubicSplines<double>::Definition();
+    def_f1M.f = [&](double x) {return Moliere::f1M(x);};
+    def_f1M.axis = std::make_unique<cubic_splines::LinAxis<double>>(0.f, 20, size_t(100));
+    f1M_interpolant_ = std::make_shared<interpolant_t>(std::move(def_f1M));
+
+    auto def_f2M = cubic_splines::CubicSplines<double>::Definition();
+    def_f2M.f = [&](double x) {return Moliere::f2M(x);};
+    def_f2M.axis = std::make_unique<cubic_splines::LinAxis<double>>(0.f, 20, size_t(100));
+    f2M_interpolant_ = std::make_shared<interpolant_t>(std::move(def_f2M));
+
+    auto def_F1M = cubic_splines::CubicSplines<double>::Definition();
+    def_F1M.f = [&](double x) {return Moliere::F1M(x);};
+    def_F1M.axis = std::make_unique<cubic_splines::LinAxis<double>>(0.f, 20, size_t(100));
+    F1M_interpolant_ = std::make_shared<interpolant_t>(std::move(def_F1M));
+
+    auto def_F2M = cubic_splines::CubicSplines<double>::Definition();
+    def_F2M.f = [&](double x) {return Moliere::F2M(x);};
+    def_F2M.axis = std::make_unique<cubic_splines::LinAxis<double>>(0.f, 20, size_t(100));
+    F2M_interpolant_ = std::make_shared<interpolant_t>(std::move(def_F2M));
+}
+
+double MoliereInterpol::f1M(double x)
+{
+    if (x > 20.)
+        return Moliere::f1M(x); // use analytical evaluation outside range of interpolation tables
+    return f1M_interpolant_->evaluate(x);
+}
+
+double MoliereInterpol::f2M(double x)
+{
+    if (x > 20)
+        return Moliere::f2M(x);  // use analytical evaluation outside range of interpolation tables
+    return f2M_interpolant_->evaluate(x);
+}
+
+double MoliereInterpol::F1M(double x)
+{
+    if (x > 20.)
+        return Moliere::F1M(x); // use analytical evaluation outside range of interpolation tables
+    return F1M_interpolant_->evaluate(x);
+}
+
+double MoliereInterpol::F2M(double x)
+{
+    if (x > 20)
+        return Moliere::F2M(x); // use analytical evaluation outside range of interpolation tables
+    return F2M_interpolant_->evaluate(x);
+}
```

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,79 @@
 
-#include "PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h"
+#include "PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h"
 #include "PROPOSAL/Constants.h"
 #include "PROPOSAL/particle/Particle.h"
 
 #include <cmath>
-#include <sstream>
+#include <iostream>
+#include <stdexcept>
 
 using std::fmod;
 using std::get;
 using std::make_tuple;
+using std::tuple;
+using std::vector;
 using std::sqrt;
 
 using namespace PROPOSAL;
 
-double secondaries::KelnerKokoulinPetrukhinEpairProduction::CalculateRho(
+
+double secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateRho(
     double energy, double v, const Component& comp, double rnd1, double rnd2)
 {
-
-    auto aux = 1 - (4 * ME) / (energy * v);
-    auto aux2 = 1 - (6 * p_def.mass * p_def.mass) / (energy * energy * (1 - v));
-
-    double rho_max = std::sqrt(aux) * aux2;
-
-    if (rho_max < 0) {
-        std::stringstream ss;
-        ss << "Rho should never be smaller than zero. Something with aux: "
-           << aux << ", aux2: " << aux2 << " got wrong.";
-        throw std::logic_error(ss.str());
+    auto rho_max = 1 - 2 * MMU / (v * energy);
+    if (rho_max < 0)
+        return 0;
+    integral.IntegrateWithRandomRatio(0, rho_max,
+        [&](double rho) {
+            return param.FunctionToIntegral(p_def, comp, energy, v, rho);
+        },
+        3, rnd1);
+    auto rho_tmp = integral.GetUpperLimit();
+    if (rnd2 < 0.5) {
+        return -rho_tmp;
+    } else {
+        return rho_tmp;
     }
-
-    auto integrand = [&](double rho) {
-        return param.FunctionToIntegral(p_def, comp, energy, v, rho);
-    };
-
-    auto rho = 0.;
-    if (integral.IntegrateWithRandomRatio(0, rho_max, integrand, 3, rnd1) > 0)
-        rho = integral.GetUpperLimit();
-
-    if (rnd2 < 0.5)
-        rho *= -1.;
-
-    return rho;
 }
 
-std::tuple<Cartesian3D, Cartesian3D>
-secondaries::KelnerKokoulinPetrukhinEpairProduction::CalculateDirections(
+tuple<Cartesian3D, Cartesian3D>
+secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateDirections(
     const Vector3D& primary_dir, double, double, double)
 {
     return make_tuple(Cartesian3D(primary_dir), Cartesian3D(primary_dir));
 }
 
-std::tuple<double, double>
-secondaries::KelnerKokoulinPetrukhinEpairProduction::CalculateEnergy(
+tuple<double, double>
+secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateEnergy(
     double energy, double rho)
 {
     auto energy_1 = 0.5 * energy * (1 + rho);
     auto energy_2 = 0.5 * energy * (1 - rho);
     return make_tuple(energy_1, energy_2);
 }
 
-std::vector<ParticleState>
-secondaries::KelnerKokoulinPetrukhinEpairProduction::CalculateSecondaries(
-    StochasticLoss loss, const Component& comp, std::vector<double>& rnd)
+vector<ParticleState>
+secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateSecondaries(
+    StochasticLoss loss, const Component& comp, vector<double> &rnd)
 {
     auto v = loss.energy / loss.parent_particle_energy;
-    auto rho
-        = CalculateRho(loss.parent_particle_energy, v, comp, rnd[0], rnd[1]);
+    auto rho = CalculateRho(loss.parent_particle_energy, v, comp, rnd[0], rnd[1]);
     auto secondary_energies = CalculateEnergy(loss.energy, rho);
-    auto secondary_dir
-        = CalculateDirections(loss.direction, loss.energy, rho, rnd[2]);
+    auto secondary_dir = CalculateDirections(
+        loss.direction, loss.energy, rho, rnd[2]);
 
     auto sec = std::vector<ParticleState>();
+
     sec.emplace_back(static_cast<ParticleType>(p_def.particle_type),
-        loss.position, loss.direction,
-        loss.parent_particle_energy - loss.energy, loss.time,
-        loss.propagated_distance);
+                     loss.position, loss.direction,
+                     loss.parent_particle_energy - loss.energy,
+                     loss.time, loss.propagated_distance);
 
-    sec.emplace_back(ParticleType::EMinus, loss.position, get<0>(secondary_dir),
-        get<0>(secondary_energies), loss.time, 0.);
+    sec.emplace_back(ParticleType::MuMinus, loss.position, get<0>(secondary_dir),
+                     get<0>(secondary_energies), loss.time, 0.);
 
-    sec.emplace_back(ParticleType::EPlus, loss.position, get<1>(secondary_dir),
-        get<1>(secondary_energies), loss.time, 0.);
+    sec.emplace_back(ParticleType::MuPlus, loss.position, get<1>(secondary_dir),
+                     get<1>(secondary_energies), loss.time, 0.);
 
     return sec;
 }
```

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,51 @@
-
-#include "PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h"
+#include "PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h"
 #include "PROPOSAL/Constants.h"
 #include "PROPOSAL/particle/Particle.h"
 
 #include <cmath>
-#include <iostream>
 #include <stdexcept>
 
-using std::fmod;
-using std::get;
-using std::make_tuple;
-using std::tuple;
-using std::vector;
-using std::sqrt;
-
 using namespace PROPOSAL;
 
-
-double secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateRho(
-    double energy, double v, const Component& comp, double rnd1, double rnd2)
-{
-    auto rho_max = 1 - 2 * MMU / (v * energy);
-    if (rho_max < 0)
-        return 0;
-    integral.IntegrateWithRandomRatio(0, rho_max,
-        [&](double rho) {
-            return param.FunctionToIntegral(p_def, comp, energy, v, rho);
-        },
-        3, rnd1);
-    auto rho_tmp = integral.GetUpperLimit();
-    if (rnd2 < 0.5) {
-        return -rho_tmp;
-    } else {
-        return rho_tmp;
-    }
-}
-
-tuple<Cartesian3D, Cartesian3D>
-secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateDirections(
-    const Vector3D& primary_dir, double, double, double)
-{
-    return make_tuple(Cartesian3D(primary_dir), Cartesian3D(primary_dir));
+size_t secondaries::WeakCooperSarkarMertsch::generate_hash(const ParticleDef& p,
+                                                           const Medium& m) {
+    size_t hash = 0;
+    hash_combine(hash, p.GetHash(), m.GetHash(), "secondaries_coopersarkarmertsch");
+    return hash;
 }
 
-tuple<double, double>
-secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateEnergy(
-    double energy, double rho)
-{
-    auto energy_1 = 0.5 * energy * (1 + rho);
-    auto energy_2 = 0.5 * energy * (1 - rho);
-    return make_tuple(energy_1, energy_2);
+double secondaries::WeakCooperSarkarMertsch::CalculateRelativeLoss(
+        double energy, double rnd, const Component& c) {
+    if (!dndx)
+        throw std::logic_error("dndx Interpolant for WeakInteraction not defined.");
+    for (auto& it : *dndx) {
+        if (c.GetHash() == it.first) {
+            auto& calc = *std::get<1>(it.second);
+            auto rate = rnd * calc.Calculate(energy);
+            auto v = calc.GetUpperLimit(energy, rate);
+            return v;
+        }
+    }
+    std::ostringstream s;
+    s << "Component (" << c.GetName()
+    << ") can not be found in the precalculated weak interaction tables.";
+    throw std::out_of_range(s.str());
 }
 
-vector<ParticleState>
-secondaries::KelnerKokoulinPetrukhinMupairProduction::CalculateSecondaries(
-    StochasticLoss loss, const Component& comp, vector<double> &rnd)
+std::vector<ParticleState>
+secondaries::WeakCooperSarkarMertsch::CalculateSecondaries(StochasticLoss loss,
+                                                       const Component& c,
+                                                       std::vector<double>& rnd)
 {
-    auto v = loss.energy / loss.parent_particle_energy;
-    auto rho = CalculateRho(loss.parent_particle_energy, v, comp, rnd[0], rnd[1]);
-    auto secondary_energies = CalculateEnergy(loss.energy, rho);
-    auto secondary_dir = CalculateDirections(
-        loss.direction, loss.energy, rho, rnd[2]);
+    // v corresponds to the energy lost to the hadron
+    auto v = CalculateRelativeLoss(loss.parent_particle_energy, rnd[0], c);
 
     auto sec = std::vector<ParticleState>();
-
-    sec.emplace_back(static_cast<ParticleType>(p_def.particle_type),
-                     loss.position, loss.direction,
-                     loss.parent_particle_energy - loss.energy,
-                     loss.time, loss.propagated_distance);
-
-    sec.emplace_back(ParticleType::MuMinus, loss.position, get<0>(secondary_dir),
-                     get<0>(secondary_energies), loss.time, 0.);
-
-    sec.emplace_back(ParticleType::MuPlus, loss.position, get<1>(secondary_dir),
-                     get<1>(secondary_energies), loss.time, 0.);
-
+    sec.emplace_back(static_cast<ParticleType>(weak_partner_type),
+                     loss.position, loss.direction, (1. - v) * loss.energy,
+                     loss.time, 0.);
+    sec.emplace_back(ParticleType::Hadron,
+                     loss.position, loss.direction, v * loss.energy,
+                     loss.time, 0.);
     return sec;
 }
```

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx` & `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/CMakeLists.txt` & `proposal-7.6.0/src/pyPROPOSAL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/components.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/components.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/crosssection.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/crosssection.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,16 @@
     build_crosssection<crosssection::PhotoMuPairBurkhardtKelnerKokoulin>(m_sub);
 
     build_crosssection<crosssection::PhotoproductionZeus>(m_sub);
     build_crosssection<crosssection::PhotoproductionBezrukovBugaev>(m_sub);
     build_crosssection<crosssection::PhotoproductionCaldwell>(m_sub);
     build_crosssection<crosssection::PhotoproductionKokoulin>(m_sub);
     build_crosssection<crosssection::PhotoproductionRhode>(m_sub);
+    build_crosssection<crosssection::PhotoproductionHeck>(m_sub);
+    build_crosssection<crosssection::PhotoproductionHeckC7Shadowing>(m_sub);
 
     build_crosssection<crosssection::PhotoeffectSauter>(m_sub);
 
     build_crosssection<crosssection::PhotoAbramowiczLevinLevyMaor91>(m_sub);
     build_crosssection<crosssection::PhotoAbramowiczLevinLevyMaor97>(m_sub);
     build_crosssection<crosssection::PhotoButkevichMikheyev>(m_sub);
     build_crosssection<crosssection::PhotoRenoSarcevicSu>(m_sub);
```

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/decay.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/decay.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/density_distribution.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/density_distribution.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/geometry.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/geometry.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/math.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/math.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/medium.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/medium.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/parametrization.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/parametrization.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -709,14 +709,27 @@
     std::shared_ptr<crosssection::PhotoproductionKokoulin>,
     crosssection::Photoproduction>(m_sub_photoproduction, "Kokoulin", py::multiple_inheritance())
         .def(py::init<>());
 
     py::class_<crosssection::PhotoproductionRhode,
     std::shared_ptr<crosssection::PhotoproductionRhode>,
     crosssection::Photoproduction>(m_sub_photoproduction, "Rhode", py::multiple_inheritance())
+        .def(py::init<>())
+        .def("PhotonNucleonCrossSection",
+         &crosssection::PhotoproductionRhode::PhotonNucleonCrossSection,
+         py::arg("energy"), py::arg("component"));
+
+    py::class_<crosssection::PhotoproductionHeck,
+    std::shared_ptr<crosssection::PhotoproductionHeck>,
+    crosssection::Photoproduction>(m_sub_photoproduction, "Heck", py::multiple_inheritance())
+        .def(py::init<>());
+
+    py::class_<crosssection::PhotoproductionHeckC7Shadowing,
+        std::shared_ptr<crosssection::PhotoproductionHeckC7Shadowing>,
+        crosssection::Photoproduction>(m_sub_photoproduction, "HeckC7Shadowing", py::multiple_inheritance())
         .def(py::init<>());
 
     // --------------------------------------------------------------------- //
     // Photoeffect
     // --------------------------------------------------------------------- //
 
     py::module m_sub_photoeffect = m_sub.def_submodule("photoeffect");
```

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/particle.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/particle.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/pybindings.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/pybindings.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/scattering.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/scattering.cxx`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
                     grammage(double): displacement of particle
                     e_i(double): initial energy
                     e_f(double): final energy
             )pbdoc");
 
     py::class_<multiple_scattering::Highland, multiple_scattering::Parametrization,
         std::shared_ptr<multiple_scattering::Highland>>(m_sub, "Highland")
+        .def(py::init<const ParticleDef&, const Medium&>(),
+             py::arg("particle_def"), py::arg("medium"))
         .def("CalculateTheta0", &multiple_scattering::Highland::CalculateTheta0,
              py::arg("grammage"), py::arg("e_i"), py::arg("e_f"),
              R"pbdoc(
                 Calculate the average scattering angle for Highland
                 parametrizations.
 
                 Args:
@@ -45,19 +47,30 @@
                     e_i(double): initial energy
                     e_f(double): final energy
             )pbdoc");
 
     py::class_<multiple_scattering::HighlandIntegral, multiple_scattering::Highland,
             std::shared_ptr<multiple_scattering::HighlandIntegral>>(m_sub, "HighlandIntegral");
 
+    py::class_<multiple_scattering::Moliere, multiple_scattering::Parametrization,
+            std::shared_ptr<multiple_scattering::Moliere>>(m_sub, "Moliere")
+            .def(py::init<const ParticleDef&, const Medium&>(),
+                 py::arg("particle_def"), py::arg("medium"));
+
+    py::class_<multiple_scattering::MoliereInterpol, multiple_scattering::Parametrization,
+            std::shared_ptr<multiple_scattering::MoliereInterpol>>(m_sub, "MoliereInterpol")
+            .def(py::init<const ParticleDef&, const Medium&>(),
+                 py::arg("particle_def"), py::arg("medium"));
+
     py::class_<multiple_scattering::ScatteringOffset>(m_sub, "scattering_offset")
             .def_readwrite("sx", &multiple_scattering::ScatteringOffset::sx)
             .def_readwrite("sy", &multiple_scattering::ScatteringOffset::sy)
             .def_readwrite("tx", &multiple_scattering::ScatteringOffset::tx)
-            .def_readwrite("ty", &multiple_scattering::ScatteringOffset::ty);
+            .def_readwrite("ty", &multiple_scattering::ScatteringOffset::ty)
+            .def("__str__", &py_print<multiple_scattering::ScatteringOffset>);
 
     m_sub.def("scatter_initial_direction", &multiple_scattering::ScatterInitialDirection);
 
     auto scattering_doc
         = R"pbdoc(Factory method for a MultipleScattering object.
 
                 Args:
```

### Comparing `proposal-7.5.1/src/pyPROPOSAL/detail/secondaries.cxx` & `proposal-7.6.0/src/pyPROPOSAL/detail/secondaries.cxx`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,17 @@
 
     SecondariesBuilder<secondaries::NaivCompton, secondaries::Compton> {}
         .decl_param(m_sub, "NaivCompton");
 
     SecondariesBuilder<secondaries::KelnerKokoulinPetrukhinEpairProduction,
         secondaries::EpairProduction> {}
         .decl_rho_param(m_sub, "KelnerKokoulinPetrukhinEpairProduction");
+    SecondariesBuilder<secondaries::ForElectronPositronEpairProduction,
+        secondaries::EpairProduction> {}
+        .decl_rho_param(m_sub, "ForElectronPositronEpairProduction");
     SecondariesBuilder<secondaries::NaivEpairProduction,
         secondaries::EpairProduction> {}
         .decl_param(m_sub, "NaivEpairProduction");
 
     SecondariesBuilder<secondaries::NaivIonization, secondaries::Ionization> {}
         .decl_param(m_sub, "NaivIonization");
 
@@ -144,17 +147,23 @@
 
     SecondariesBuilder<secondaries::PhotoPairProductionTsai,
         secondaries::PhotoPairProduction> {}
         .decl_rho_param(m_sub, "PhotoTsai");
     SecondariesBuilder<secondaries::PhotoPairProductionTsaiForwardPeaked,
         secondaries::PhotoPairProduction> {}
         .decl_rho_param(m_sub, "PhotoTsaiForwardPeaked");
+    SecondariesBuilder<secondaries::PhotoPairProductionTsaiSauter,
+        secondaries::PhotoPairProduction> {}
+        .decl_rho_param(m_sub, "PhotoTsaiSauter");
     SecondariesBuilder<secondaries::PhotoPairProductionKochMotzForwardPeaked,
         secondaries::PhotoPairProduction> {}
         .decl_rho_param(m_sub, "PhotoKochMotzForwardPeaked");
+    SecondariesBuilder<secondaries::PhotoPairProductionKochMotzSauter,
+        secondaries::PhotoPairProduction> {}
+        .decl_rho_param(m_sub, "PhotoKochMotzSauter");
 
     SecondariesBuilder<secondaries::PhotoeffectNoDeflection, secondaries::Photoeffect> {}
         .decl_param(m_sub, "PhotoeffectNoDeflection");
 
     py::class_<secondaries::WeakCooperSarkarMertsch, secondaries::WeakInteraction,
         std::shared_ptr<secondaries::WeakCooperSarkarMertsch>>(m_sub,
                 "WeakCooperSarkarMertsch")
```

### Comparing `proposal-7.5.1/tests/Annihilation_TEST.cxx` & `proposal-7.6.0/tests/Annihilation_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Bremsstrahlung_TEST.cxx` & `proposal-7.6.0/tests/Bremsstrahlung_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/CMakeLists.txt` & `proposal-7.6.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Compton_TEST.cxx` & `proposal-7.6.0/tests/Compton_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/ContinuousRandomization_TEST.cxx` & `proposal-7.6.0/tests/ContinuousRandomization_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/CrossSection_TEST.cxx` & `proposal-7.6.0/tests/CrossSection_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/DecayChannel_TEST.cxx` & `proposal-7.6.0/tests/DecayChannel_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/DecayTable_TEST.cxx` & `proposal-7.6.0/tests/DecayTable_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Decay_TEST.cxx` & `proposal-7.6.0/tests/Decay_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Density_distribution_TEST.cxx` & `proposal-7.6.0/tests/Density_distribution_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Displacement_TEST.cxx` & `proposal-7.6.0/tests/Displacement_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/EnergyCutSettings_TEST.cxx` & `proposal-7.6.0/tests/EnergyCutSettings_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Epairproduction_TEST.cxx` & `proposal-7.6.0/tests/Epairproduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Geometry_TEST.cxx` & `proposal-7.6.0/tests/Geometry_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Integral_TEST.cxx` & `proposal-7.6.0/tests/Integral_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Interaction_TEST.cxx` & `proposal-7.6.0/tests/Interaction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Interpolant_TEST.cxx` & `proposal-7.6.0/tests/Interpolant_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Ionization_TEST.cxx` & `proposal-7.6.0/tests/Ionization_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/MathMethods_TEST.cxx` & `proposal-7.6.0/tests/MathMethods_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Medium_TEST.cxx` & `proposal-7.6.0/tests/Medium_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Mupairproduction_TEST.cxx` & `proposal-7.6.0/tests/Mupairproduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/PROPOSALTestUtilities/TestFilesHandling.h` & `proposal-7.6.0/tests/PROPOSALTestUtilities/TestFilesHandling.h`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/ParticleDef_TEST.cxx` & `proposal-7.6.0/tests/ParticleDef_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Particle_TEST.cxx` & `proposal-7.6.0/tests/Particle_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/PhotoMuPair_TEST.cxx` & `proposal-7.6.0/tests/PhotoMuPair_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/PhotoPair_TEST.cxx` & `proposal-7.6.0/tests/PhotoPair_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Photoeffect_TEST.cxx` & `proposal-7.6.0/tests/Photoeffect_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Photonuclear_TEST.cxx` & `proposal-7.6.0/tests/Photonuclear_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Propagator_TEST.cxx` & `proposal-7.6.0/tests/Propagator_TEST.cxx`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #include "gtest/gtest.h"
 #include "PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h"
 #include "PROPOSAL/Propagator.h"
 #include "PROPOSAL/propagation_utility/TimeBuilder.h"
 #include "PROPOSAL/propagation_utility/InteractionBuilder.h"
 #include "PROPOSAL/propagation_utility/ContRandBuilder.h"
+#include "PROPOSAL/propagation_utility/DecayBuilder.h"
 #include "PROPOSAL/density_distr/density_homogeneous.h"
 #include "PROPOSAL/scattering/ScatteringFactory.h"
 #include "PROPOSAL/geometry/Sphere.h"
 #include "PROPOSAL/particle/Particle.h"
 
 using namespace PROPOSAL;
 
@@ -53,12 +54,52 @@
         if (final_energy < min_energy)
             EXPECT_NE(sec.GetTrackTypes().back(), InteractionType::ContinuousEnergyLoss);
         else
             EXPECT_EQ(sec.GetTrackTypes().back(), InteractionType::ContinuousEnergyLoss);
     }
 }
 
+TEST(Propagator, RestMassDecay)
+{
+    // make sure that all muons decay at the end of their propagation, even if they have reached their rest mass
+    // (see issue https://github.com/tudo-astroparticlephysics/PROPOSAL/issues/323)
+    auto p_def = MuMinusDef();
+    auto medium = Ice();
+    auto cuts = std::make_shared<EnergyCutSettings>(INF, 0.05, true);
+    auto cross = GetStdCrossSections(p_def, medium, cuts, true);
+
+    auto collection = PropagationUtility::Collection();
+    collection.interaction_calc = make_interaction(cross, true);
+    collection.displacement_calc = make_displacement(cross, true);
+    collection.time_calc = make_time(cross, p_def, true);
+    collection.cont_rand = make_contrand(cross, true);
+    collection.scattering = make_scattering(MultipleScatteringType::Highland, {}, p_def, medium);
+    collection.decay_calc = make_decay(cross, p_def, true);
+
+    auto prop_utility = PropagationUtility(collection);
+
+    auto density_distr = std::make_shared<Density_homogeneous>(medium);
+    auto world = std::make_shared<Sphere>(Cartesian3D(0, 0, 0), 1e20);
+
+    auto sector = std::make_tuple(world, prop_utility, density_distr);
+    std::vector<Sector> sec_vec = {sector};
+
+    auto prop = Propagator(p_def, sec_vec);
+
+    auto init_state = ParticleState();
+    init_state.energy = 150;
+    init_state.position = Cartesian3D(0, 0, 0);
+    init_state.direction = Cartesian3D(0, 0, 1);
+
+    for (size_t i=0; i<1000; i++) {
+        auto sec = prop.Propagate(init_state);
+        EXPECT_FALSE(sec.GetDecayProducts().empty()); // check that decay products are produced
+    }
+
+}
+
+
 int main(int argc, char** argv)
 {
     ::testing::InitGoogleTest(&argc, argv);
     return RUN_ALL_TESTS();
 }
```

### Comparing `proposal-7.5.1/tests/Scattering_TEST.cxx` & `proposal-7.6.0/tests/Scattering_TEST.cxx`

 * *Files 4% similar despite different names*

```diff
@@ -211,17 +211,18 @@
 
 TEST(Scattering, ZeroDisplacement){
     // No displacement should mean no scattering
     auto medium = StandardRock();
     auto cuts = std::make_shared<EnergyCutSettings>(INF, 1, false);
     auto cross = GetCrossSections(MuMinusDef(), medium, cuts, true);
 
-    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 3> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
+    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 4> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
                                                                                          make_multiple_scattering("highland", MuMinusDef(), medium),
-                                                                                         make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross)};
+                                                                                         make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross),
+                                                                                         make_multiple_scattering("moliereinterpol", MuMinusDef(), medium)};
 
     for(auto const& scatter: scatter_list){
         auto offset = scatter->CalculateRandomAngle(0, 1e5, 1e5, {0.1, 0.2, 0.3, 0.4});
         EXPECT_EQ(offset.sx, 0);
         EXPECT_EQ(offset.sy, 0);
         EXPECT_EQ(offset.tx, 0);
         EXPECT_EQ(offset.ty, 0);
@@ -234,17 +235,18 @@
     auto position_init  = Cartesian3D(0, 0, 0);
     auto direction_init = Cartesian3D(0, 0, 1);
     auto cuts = std::make_shared<EnergyCutSettings>(INF, 1, false);
 
     int statistics = 1e3;
     auto cross = GetCrossSections(MuMinusDef(), medium, cuts, true);
 
-    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 3> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
+    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 4> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
                                                                make_multiple_scattering("highland", MuMinusDef(), medium),
-                                                               make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross)};
+                                                               make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross),
+                                                               make_multiple_scattering("moliereinterpol", MuMinusDef(), medium),};
     Cartesian3D scatter_sum;
     Cartesian3D offset_sum;
 
     for(auto const& scatter: scatter_list){
         scatter_sum.SetCoordinates({0., 0., 0.});
         offset_sum.SetCoordinates({0., 0., 0.});
 
@@ -273,23 +275,24 @@
 TEST(Scattering, SecondMomentum){
     RandomGenerator::Get().SetSeed(24601);
     auto medium = StandardRock();
     auto position_init  = Cartesian3D(0, 0, 0);
     auto direction_init = Cartesian3D(0, 0, 1);
     auto cuts = std::make_shared<EnergyCutSettings>(INF, 1, false);
 
-    int statistics = 1e3;
+    int statistics = 1e5;
 
     double E_i = 1e14;
     std::array<double, 6> final_energies = {1e13, 1e11, 1e9, 1e7, 1e5, 1e3};
     auto cross = GetCrossSections(MuMinusDef(), medium, cuts, true);
 
-    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 3> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
+    std::array<std::unique_ptr<multiple_scattering::Parametrization>, 4> scatter_list = {make_multiple_scattering("moliere", MuMinusDef(), medium),
                                                                make_multiple_scattering("highland", MuMinusDef(), medium),
-                                                               make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross)};
+                                                               make_multiple_scattering("highlandintegral", MuMinusDef(), medium, cross),
+                                                               make_multiple_scattering("moliereinterpol", MuMinusDef(), medium, cross)};
     double scatter_sum;
     double offset_sum;
     double displacement;
     double old_displacement;
     auto displacement_calculator = DisplacementBuilder(cross, std::false_type());
     std::array<double, 2> variances = {0,0};
     std::array<double, 2> old_variances;
@@ -493,12 +496,62 @@
     };
     auto new_dir = utility.DirectionsScatter(1e2, 1e6, 1e5, init_dir, rnd_lambda);
 
     EXPECT_EQ(std::get<0>(new_dir), init_dir);
     EXPECT_EQ(std::get<1>(new_dir), init_dir);
 }
 
+TEST(MoliereInterpol, ComparionToMoliere) {
+    // MoliereInterpol is based on Moliere, using interpolation tables to speed up the evaluation.
+    // Therefore, we expect results to be similar
+
+    RandomGenerator::Get().SetSeed(24601);
+    auto medium = StandardRock();
+    auto position_init  = Cartesian3D(0, 0, 0);
+    auto direction_init = Cartesian3D(0, 0, 1);
+
+    auto cuts = std::make_shared<EnergyCutSettings>(INF, 1, false);
+
+    std::vector<ParticleDef> particles = {EMinusDef(), MuMinusDef()};
+
+    for (auto p : particles) {
+        //displacement calculator
+        auto cross = GetCrossSections(p, medium, cuts, false);
+        auto displacement = DisplacementBuilder(cross, std::false_type());
+
+        auto moliere = make_multiple_scattering("moliere", p, medium);
+        auto moliere_interpol = make_multiple_scattering("moliereinterpol", p, medium);
+        double E_f = 1e5;
+        auto energies = std::array<double, 6>{2e5, 1e6, 1e7, 1e8, 1e9, 1e10};
+        for (auto E_i : energies) {
+            double grammage = displacement.SolveTrackIntegral(E_i, E_f);
+            auto rnd = std::array<double, 4>{RandomGenerator::Get().RandomDouble(),
+                                             RandomGenerator::Get().RandomDouble(),
+                                             RandomGenerator::Get().RandomDouble(),
+                                             RandomGenerator::Get().RandomDouble()};
+            auto coords = moliere->CalculateRandomAngle(grammage, E_i, E_f, rnd);
+            auto coords_interpol = moliere_interpol->CalculateRandomAngle(grammage, E_i, E_f, rnd);
+            auto vec = multiple_scattering::ScatterInitialDirection(
+                    direction_init, coords);
+            auto vec_interpol = multiple_scattering::ScatterInitialDirection(
+                    direction_init, coords_interpol);
+            EXPECT_NEAR(std::get<0>(vec).GetX(), std::get<0>(vec_interpol).GetX(),
+                        std::abs(std::get<0>(vec).GetX() * 1e-2));
+            EXPECT_NEAR(std::get<0>(vec).GetY(), std::get<0>(vec_interpol).GetY(),
+                        std::abs(std::get<0>(vec).GetY() * 1e-2));
+            EXPECT_NEAR(std::get<0>(vec).GetZ(), std::get<0>(vec_interpol).GetZ(),
+                        std::abs(std::get<0>(vec).GetZ() * 1e-2));
+            EXPECT_NEAR(std::get<1>(vec).GetX(), std::get<1>(vec_interpol).GetX(),
+                        std::abs(std::get<1>(vec).GetX() * 1e-2));
+            EXPECT_NEAR(std::get<1>(vec).GetY(), std::get<1>(vec_interpol).GetY(),
+                        std::abs(std::get<1>(vec).GetY() * 1e-2));
+            EXPECT_NEAR(std::get<1>(vec).GetZ(), std::get<1>(vec_interpol).GetZ(),
+                        std::abs(std::get<1>(vec).GetZ() * 1e-2));
+        }
+    }
+}
+
 int main(int argc, char** argv)
 {
     ::testing::InitGoogleTest(&argc, argv);
     return RUN_ALL_TESTS();
 }
```

### Comparing `proposal-7.5.1/tests/Secondaries_TEST.cxx` & `proposal-7.6.0/tests/Secondaries_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/SecondaryProduction_TEST.cxx` & `proposal-7.6.0/tests/SecondaryProduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Sector_TEST.cxx` & `proposal-7.6.0/tests/Sector_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Spline_TEST.cxx` & `proposal-7.6.0/tests/Spline_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Time_TEST.cxx` & `proposal-7.6.0/tests/Time_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/UtilityIntegral_TEST.cxx` & `proposal-7.6.0/tests/UtilityIntegral_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/UtilityInterpolant_TEST.cxx` & `proposal-7.6.0/tests/UtilityInterpolant_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Utility_TEST.cxx` & `proposal-7.6.0/tests/Utility_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/Vector3D_TEST.cxx` & `proposal-7.6.0/tests/Vector3D_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/WeakInteraction_TEST.cxx` & `proposal-7.6.0/tests/WeakInteraction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/conanfile.py` & `proposal-7.6.0/tests/conanfile.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/__init__.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/annihilation.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/annihilation.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/bremsstrahlung.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/bremsstrahlung.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/compton.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/compton.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/continous_randomization.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/continous_randomization.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/decay.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/decay.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/epairproduction.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/epairproduction.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/ionization.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/ionization.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/mupairproduction.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/mupairproduction.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/photomupair.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/photomupair.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/photonuclear.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/photonuclear.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/photopair.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/photopair.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/propagation.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/propagation.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/scattering.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/scattering.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/sector.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/sector.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/gen_testfiles_scripts/weak.py` & `proposal-7.6.0/tests/gen_testfiles_scripts/weak.py`

 * *Files identical despite different names*

### Comparing `proposal-7.5.1/tests/python/test_continuous_loss_output.py` & `proposal-7.6.0/tests/python/test_continuous_loss_output.py`

 * *Files identical despite different names*

