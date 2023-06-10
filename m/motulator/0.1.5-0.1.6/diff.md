# Comparing `tmp/motulator-0.1.5.tar.gz` & `tmp/motulator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motulator-0.1.5.tar", last modified: Sun May 28 14:12:23 2023, max compression
+gzip compressed data, was "motulator-0.1.6.tar", last modified: Sat Jun 10 11:59:40 2023, max compression
```

## Comparing `motulator-0.1.5.tar` & `motulator-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.505939 motulator-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-28 14:12:07.000000 motulator-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:23.505939 motulator-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-28 14:12:07.000000 motulator-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator/control/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/control/im/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_obs_vhz.py
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_vhz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/control/sm/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_flux_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_obs_vhz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_signal_inj.py
--rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/model/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/model/im/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/im/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/im/_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.505939 motulator-0.1.5/motulator/model/sm/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/_flux_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-28 14:12:07.000000 motulator-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-28 14:12:23.505939 motulator-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.432807 motulator-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-10 11:59:19.000000 motulator-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-10 11:59:40.432807 motulator-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-10 11:59:19.000000 motulator-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.424807 motulator-0.1.6/motulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/control/im/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/im/_obs_vhz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/im/_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/im/_vhz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/control/sm/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/_flux_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/_obs_vhz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/_signal_inj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/_torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/control/sm/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/model/im/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/im/_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.428807 motulator-0.1.6/motulator/model/sm/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/sm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/sm/_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-10 11:59:19.000000 motulator-0.1.6/motulator/model/sm/_flux_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:59:40.424807 motulator-0.1.6/motulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-10 11:59:40.000000 motulator-0.1.6/motulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-10 11:59:40.000000 motulator-0.1.6/motulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:59:40.000000 motulator-0.1.6/motulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 11:59:40.000000 motulator-0.1.6/motulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-10 11:59:19.000000 motulator-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-10 11:59:40.432807 motulator-0.1.6/setup.cfg
```

### Comparing `motulator-0.1.5/LICENSE` & `motulator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/PKG-INFO` & `motulator-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motulator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Motor Drive Simulator in Python
 Home-page: https://github.com/Aalto-Electric-Drives/motulator
 Author: Marko Hinkkanen
 Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: motulator Version: 0.1.5 Summary: Motor Drive
+Metadata-Version: 2.1 Name: motulator Version: 0.1.6 Summary: Motor Drive
 Simulator in Python Home-page: https://github.com/Aalto-Electric-Drives/
 motulator Author: Marko Hinkkanen Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # *motulator:* Motor Drive Simulator in Python [![Build Status](https:/
```

### Comparing `motulator-0.1.5/README.md` & `motulator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/__init__.py` & `motulator-0.1.6/motulator/__init__.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/_helpers.py` & `motulator-0.1.6/motulator/_helpers.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/_plots.py` & `motulator-0.1.6/motulator/_plots.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from cycler import cycler
 from motulator._helpers import complex2abc
 from motulator._utils import Bunch
 
 # Plotting parameters
-plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
-plt.rcParams['lines.linewidth'] = 1.
-plt.rcParams['axes.grid'] = True
+plt.rcParams["axes.prop_cycle"] = cycler(color="brgcmyk")
+plt.rcParams["lines.linewidth"] = 1.
+plt.rcParams["axes.grid"] = True
 plt.rcParams.update({"text.usetex": False})
 
 
 # %%
 # pylint: disable=too-many-branches
 def plot(sim, base=None, t_span=None):
     """
@@ -47,110 +47,110 @@
         base = Bunch(w=1, u=1, i=1, psi=1, tau=1)  # Unity base values
     else:
         pu_vals = True
 
     # Recognize the motor type by checking if the rotor flux data exist
     try:
         if mdl.psi_Rs is not None:
-            motor_type = 'im'
+            motor_type = "im"
     except AttributeError:
-        motor_type = 'sm'
+        motor_type = "sm"
 
     fig, (ax1, ax2, ax3, ax4, ax5) = plt.subplots(5, 1, figsize=(8, 10))
 
     # Subplot 1: angular speeds
-    ax1.step(ctrl.t, ctrl.w_m_ref/base.w, '--', where='post')
+    ax1.step(ctrl.t, ctrl.w_m_ref/base.w, "--", where="post")
     ax1.plot(mdl.t, mdl.w_m/base.w)
     try:
-        ax1.step(ctrl.t, ctrl.w_m/base.w, where='post')
+        ax1.step(ctrl.t, ctrl.w_m/base.w, where="post")
     except AttributeError:
         pass
     ax1.legend([
-        r'$\omega_\mathrm{m,ref}$',
-        r'$\omega_\mathrm{m}$',
-        r'$\hat \omega_\mathrm{m}$',
+        r"$\omega_\mathrm{m,ref}$",
+        r"$\omega_\mathrm{m}$",
+        r"$\hat \omega_\mathrm{m}$",
     ])
     ax1.set_xlim(t_span)
     ax1.set_xticklabels([])
 
     # Subplot 2: torques
-    ax2.plot(mdl.t, mdl.tau_L/base.tau, '--')
+    ax2.plot(mdl.t, mdl.tau_L/base.tau, "--")
     ax2.plot(mdl.t, mdl.tau_M/base.tau)
     try:
         ax2.step(ctrl.t, ctrl.tau_M_ref_lim/base.tau)  # Limited torque ref
     except AttributeError:
         pass
     ax2.legend([
-        r'$\tau_\mathrm{L}$',
-        r'$\tau_\mathrm{M}$',
-        r'$\tau_\mathrm{M,ref}$',
+        r"$\tau_\mathrm{L}$",
+        r"$\tau_\mathrm{M}$",
+        r"$\tau_\mathrm{M,ref}$",
     ])
     ax2.set_xlim(t_span)
     ax2.set_xticklabels([])
 
     # Subplot 3: currents
-    ax3.step(ctrl.t, ctrl.i_s.real/base.i, where='post')
-    ax3.step(ctrl.t, ctrl.i_s.imag/base.i, where='post')
+    ax3.step(ctrl.t, ctrl.i_s.real/base.i, where="post")
+    ax3.step(ctrl.t, ctrl.i_s.imag/base.i, where="post")
     try:
-        ax3.step(ctrl.t, ctrl.i_s_ref.real/base.i, '--', where='post')
-        ax3.step(ctrl.t, ctrl.i_s_ref.imag/base.i, '--', where='post')
+        ax3.step(ctrl.t, ctrl.i_s_ref.real/base.i, "--", where="post")
+        ax3.step(ctrl.t, ctrl.i_s_ref.imag/base.i, "--", where="post")
     except AttributeError:
         pass
     ax3.legend([
-        r'$i_\mathrm{sd}$',
-        r'$i_\mathrm{sq}$',
-        r'$i_\mathrm{sd,ref}$',
-        r'$i_\mathrm{sq,ref}$',
+        r"$i_\mathrm{sd}$",
+        r"$i_\mathrm{sq}$",
+        r"$i_\mathrm{sd,ref}$",
+        r"$i_\mathrm{sq,ref}$",
     ])
     ax3.set_xlim(t_span)
     ax3.set_xticklabels([])
 
     # Subplot 4: voltages
-    ax4.step(ctrl.t, np.abs(ctrl.u_s)/base.u, where='post')
-    ax4.step(ctrl.t, ctrl.u_dc/np.sqrt(3)/base.u, '--', where='post')
-    ax4.legend([r'$u_\mathrm{s}$', r'$u_\mathrm{dc}/\sqrt{3}$'])
+    ax4.step(ctrl.t, np.abs(ctrl.u_s)/base.u, where="post")
+    ax4.step(ctrl.t, ctrl.u_dc/np.sqrt(3)/base.u, "--", where="post")
+    ax4.legend([r"$u_\mathrm{s}$", r"$u_\mathrm{dc}/\sqrt{3}$"])
     ax4.set_xlim(t_span)
     ax4.set_xticklabels([])
 
     # Subplot 5: flux linkages
-    if motor_type == 'sm':
+    if motor_type == "sm":
         ax5.plot(mdl.t, np.abs(mdl.psi_s)/base.psi)
         try:
-            ax5.step(ctrl.t, np.abs(ctrl.psi_s)/base.psi, where='post')
+            ax5.step(ctrl.t, np.abs(ctrl.psi_s)/base.psi, where="post")
         except AttributeError:
             pass
-        ax5.legend([r'$\psi_\mathrm{s}$', r'$\hat\psi_\mathrm{s}$'])
+        ax5.legend([r"$\psi_\mathrm{s}$", r"$\hat\psi_\mathrm{s}$"])
     else:
         ax5.plot(mdl.t, np.abs(mdl.psi_ss)/base.psi)
         ax5.plot(mdl.t, np.abs(mdl.psi_Rs)/base.psi)
         try:
             ax5.plot(ctrl.t, np.abs(ctrl.psi_s)/base.psi)
         except AttributeError:
             pass
         ax5.legend([
-            r'$\psi_\mathrm{s}$',
-            r'$\psi_\mathrm{R}$',
-            r'$\hat \psi_\mathrm{s}$',
+            r"$\psi_\mathrm{s}$",
+            r"$\psi_\mathrm{R}$",
+            r"$\hat \psi_\mathrm{s}$",
         ])
     ax5.set_xlim(t_span)
 
     # Add axis labels
     if pu_vals:
-        ax1.set_ylabel('Speed (p.u.)')
-        ax2.set_ylabel('Torque (p.u.)')
-        ax3.set_ylabel('Current (p.u.)')
-        ax4.set_ylabel('Voltage (p.u.)')
-        ax5.set_ylabel('Flux linkage (p.u.)')
+        ax1.set_ylabel("Speed (p.u.)")
+        ax2.set_ylabel("Torque (p.u.)")
+        ax3.set_ylabel("Current (p.u.)")
+        ax4.set_ylabel("Voltage (p.u.)")
+        ax5.set_ylabel("Flux linkage (p.u.)")
     else:
-        ax1.set_ylabel('Speed (rad/s)')
-        ax2.set_ylabel('Torque (Nm)')
-        ax3.set_ylabel('Current (A)')
-        ax4.set_ylabel('Voltage (V)')
-        ax5.set_ylabel('Flux linkage (Vs)')
-    ax5.set_xlabel('Time (s)')
+        ax1.set_ylabel("Speed (rad/s)")
+        ax2.set_ylabel("Torque (Nm)")
+        ax3.set_ylabel("Current (A)")
+        ax4.set_ylabel("Voltage (V)")
+        ax5.set_ylabel("Flux linkage (Vs)")
+    ax5.set_xlabel("Time (s)")
     fig.align_ylabels()
 
     plt.tight_layout()
     plt.show()
 
 
 # %%
@@ -189,31 +189,31 @@
 
     fig1, (ax1, ax2) = plt.subplots(2, 1)
 
     # Subplot 1: voltages
     ax1.plot(mdl.t, mdl.u_ss.real/base.u)
     ax1.plot(ctrl.t, ctrl.u_ss.real/base.u)
     ax1.set_xlim(t_span)
-    ax1.legend([r'$u_\mathrm{sa}$', r'$\hat u_\mathrm{sa}$'])
+    ax1.legend([r"$u_\mathrm{sa}$", r"$\hat u_\mathrm{sa}$"])
     ax1.set_xticklabels([])
 
     # Subplot 2: currents
     ax2.plot(mdl.t, complex2abc(mdl.i_ss).T/base.i)
-    ax2.step(ctrl.t, ctrl.i_ss.real/base.i, where='post')
+    ax2.step(ctrl.t, ctrl.i_ss.real/base.i, where="post")
     ax2.set_xlim(t_span)
-    ax2.legend([r'$i_\mathrm{sa}$', r'$i_\mathrm{sb}$', r'$i_\mathrm{sc}$'])
+    ax2.legend([r"$i_\mathrm{sa}$", r"$i_\mathrm{sb}$", r"$i_\mathrm{sc}$"])
 
     # Add axis labels
     if pu_vals:
-        ax1.set_ylabel('Voltage (p.u.)')
-        ax2.set_ylabel('Current (p.u.)')
+        ax1.set_ylabel("Voltage (p.u.)")
+        ax2.set_ylabel("Current (p.u.)")
     else:
-        ax1.set_ylabel('Voltage (V)')
-        ax2.set_ylabel('Current (A)')
-    ax2.set_xlabel('Time (s)')
+        ax1.set_ylabel("Voltage (V)")
+        ax2.set_ylabel("Current (A)")
+    ax2.set_xlabel("Time (s)")
     fig1.align_ylabels()
 
     # Plots the DC bus and grid-side variables (if exist)
     try:
         mdl.i_L
     except AttributeError:
         mdl.i_L = None
@@ -223,33 +223,33 @@
         fig2, (ax1, ax2) = plt.subplots(2, 1)
 
         # Subplot 1: voltages
         ax1.plot(mdl.t, mdl.u_di/base.u)
         ax1.plot(mdl.t, mdl.u_dc/base.u)
         ax1.plot(mdl.t, complex2abc(mdl.u_g).T/base.u)
         ax1.legend(
-            [r'$u_\mathrm{di}$', r'$u_\mathrm{dc}$', r'$u_\mathrm{ga}$'])
+            [r"$u_\mathrm{di}$", r"$u_\mathrm{dc}$", r"$u_\mathrm{ga}$"])
         ax1.set_xlim(t_span)
         ax1.set_xticklabels([])
 
         # Subplot 2: currents
         ax2.plot(mdl.t, mdl.i_L/base.i)
         ax2.plot(mdl.t, mdl.i_dc/base.i)
         ax2.plot(mdl.t, mdl.i_g.real/base.i)
-        ax2.legend([r'$i_\mathrm{L}$', r'$i_\mathrm{dc}$', r'$i_\mathrm{ga}$'])
+        ax2.legend([r"$i_\mathrm{L}$", r"$i_\mathrm{dc}$", r"$i_\mathrm{ga}$"])
         ax2.set_xlim(t_span)
 
     # Add axis labels
     if pu_vals:
-        ax1.set_ylabel('Voltage (p.u.)')
-        ax2.set_ylabel('Current (p.u.)')
+        ax1.set_ylabel("Voltage (p.u.)")
+        ax2.set_ylabel("Current (p.u.)")
     else:
-        ax1.set_ylabel('Voltage (V)')
-        ax2.set_ylabel('Current (A)')
-    ax2.set_xlabel('Time (s)')
+        ax1.set_ylabel("Voltage (V)")
+        ax2.set_ylabel("Current (A)")
+    ax2.set_xlabel("Time (s)")
 
     try:
         fig2.align_ylabels()
     except UnboundLocalError:
         pass
 
     plt.tight_layout()
@@ -266,8 +266,8 @@
 
     Parameters
     ----------
     name : string
         Name for the figure
 
     """
-    plt.savefig(name + '.pdf')
+    plt.savefig(name + ".pdf")
```

### Comparing `motulator-0.1.5/motulator/_utils.py` & `motulator-0.1.6/motulator/_utils.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/_common.py` & `motulator-0.1.6/motulator/control/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     ----------
     realized_voltage : complex
         Realized voltage (V) in synchronous coordinates.
 
     References
     ----------
     .. [#Bae2003] Bae, Sul, "A compensation method for time delay of 
-       full-digital synchronous frame current regulator of PWM AC drives," IEEE Trans. Ind. Appl., 2003, https://doi.org/10.1109/TIA.2003.810660
+       full-digital synchronous frame current regulator of PWM AC drives," IEEE
+       Trans. Ind. Appl., 2003, https://doi.org/10.1109/TIA.2003.810660
     
     """
 
     def __init__(self, six_step=False):
         self.six_step = six_step
         self.realized_voltage = 0
         self._u_ref_lim_old = 0
@@ -222,15 +223,15 @@
     """
 
     def __init__(self, k_p, k_i, k_t=None, u_max=np.inf):
         self.u_max = u_max
         # Gains
         self.k_p = k_p
         self.k_t = k_t if k_t is not None else k_p
-        self.alpha_i = k_i/k_t  # Inverse of the integration time T_i
+        self.alpha_i = k_i/self.k_t  # Inverse of the integration time T_i
         # States
         self.v, self.u_i = 0, 0
 
     def output(self, y_ref, y):
         """
         Compute the controller output.
 
@@ -346,15 +347,15 @@
 
     """
 
     def __init__(self, k_p, k_i, k_t=None):
         # Gains
         self.k_p = k_p
         self.k_t = k_t if k_t is not None else k_p
-        self.alpha_i = k_i/k_t  # Inverse of the integration time T_i
+        self.alpha_i = k_i/self.k_t  # Inverse of the integration time T_i
         # States
         self.v, self.u_i = 0, 0
 
     def output(self, i_ref, i):
         """
         Compute the controller output.
 
@@ -401,15 +402,15 @@
 class RateLimiter:
     """
     Rate limiter.
 
     Parameters
     ----------
     rate_limit : float, optional
-        Rate limit. The default is `inf`.
+        Rate limit. The default is inf.
 
     """
 
     def __init__(self, rate_limit=np.inf):
         self.rate_limit = rate_limit
         self._y_old = 0
```

### Comparing `motulator-0.1.5/motulator/control/im/_obs_vhz.py` & `motulator-0.1.6/motulator/control/im/_obs_vhz.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/im/_vector.py` & `motulator-0.1.6/motulator/control/im/_vector.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/im/_vhz.py` & `motulator-0.1.6/motulator/control/im/_vhz.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/sm/__init__.py` & `motulator-0.1.6/motulator/control/sm/__init__.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/sm/_flux_vector.py` & `motulator-0.1.6/motulator/control/sm/_flux_vector.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/sm/_obs_vhz.py` & `motulator-0.1.6/motulator/control/sm/_obs_vhz.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/sm/_signal_inj.py` & `motulator-0.1.6/motulator/control/sm/_signal_inj.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/control/sm/_torque.py` & `motulator-0.1.6/motulator/control/sm/_torque.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from sys import float_info
 import numpy as np
 from scipy.interpolate import interp1d
 import matplotlib.pyplot as plt
 from cycler import cycler
 from motulator._utils import Bunch
 
-plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
-plt.rcParams['lines.linewidth'] = 1.
+plt.rcParams["axes.prop_cycle"] = cycler(color="brgcmyk")
+plt.rcParams["lines.linewidth"] = 1.
 plt.rcParams.update({"text.usetex": False})  # Disable LaTeX in plots
 
 
 # %%
 class TorqueCharacteristics:
     """
     Compute MTPA and MTPV loci based on the machine parameters.
@@ -432,15 +432,15 @@
 
         # Create an interpolant that can be used as a look-up table
         tau_M_vs_abs_psi_s = interp1d(
             np.abs(psi_s),
             tau_M,
             bounds_error=False,
             fill_value=(tau_M[0], tau_M[-1]))
-        i_sd_vs_tau_M = interp1d(tau_M, i_sd, fill_value='extrapolate')
+        i_sd_vs_tau_M = interp1d(tau_M, i_sd, fill_value="extrapolate")
 
         # Return the result as a bunch object
         return Bunch(
             tau_M_vs_abs_psi_s=tau_M_vs_abs_psi_s, i_sd_vs_tau_M=i_sd_vs_tau_M)
 
     def plot_flux_loci(self, i_s_max, base, N=20):
         """
@@ -466,32 +466,32 @@
             N=N,
             gamma1=np.angle(mtpv.i_s[-1]),
             gamma2=np.angle(mtpa.i_s[-1]))
 
         # Plot the i_sd--i_sq current plane
         _, ax = plt.subplots()
         ax.plot(
-            mtpa.psi_s.real/base.psi, mtpa.psi_s.imag/base.psi, label='MTPA')
+            mtpa.psi_s.real/base.psi, mtpa.psi_s.imag/base.psi, label="MTPA")
         try:
             ax.plot(
                 mtpv.psi_s.real/base.psi,
                 mtpv.psi_s.imag/base.psi,
-                label='MTPV')
+                label="MTPV")
         except AttributeError:
             pass
         ax.plot(
             clim.psi_s.real/base.psi,
             clim.psi_s.imag/base.psi,
-            label='Const current')
+            label="Const current")
 
         ax.legend()
-        ax.set_xlabel(r'$\psi_\mathrm{sd}$ (p.u.)')
-        ax.set_ylabel(r'$\psi_\mathrm{sq}$ (p.u.)')
+        ax.set_xlabel(r"$\psi_\mathrm{sd}$ (p.u.)")
+        ax.set_ylabel(r"$\psi_\mathrm{sq}$ (p.u.)")
         ax.set_ylim(0, None)
-        ax.set_aspect('equal')
+        ax.set_aspect("equal")
 
     def plot_current_loci(self, i_s_max, base, N=20):
         """
         Plot the current loci.
 
         Per-unit quantities are used.
 
@@ -512,32 +512,32 @@
             i_s_max=i_s_max,
             N=N,
             gamma1=np.angle(mtpv.i_s[-1]),
             gamma2=np.angle(mtpa.i_s[-1]))
 
         # Plot the i_sd--i_sq current plane
         _, ax = plt.subplots()
-        ax.plot(mtpa.i_s.real/base.i, mtpa.i_s.imag/base.i, label='MTPA')
+        ax.plot(mtpa.i_s.real/base.i, mtpa.i_s.imag/base.i, label="MTPA")
         try:
-            ax.plot(mtpv.i_s.real/base.i, mtpv.i_s.imag/base.i, label='MTPV')
+            ax.plot(mtpv.i_s.real/base.i, mtpv.i_s.imag/base.i, label="MTPV")
         except AttributeError:
             pass
         ax.plot(
-            clim.i_s.real/base.i, clim.i_s.imag/base.i, label='Const current')
+            clim.i_s.real/base.i, clim.i_s.imag/base.i, label="Const current")
 
-        ax.set_xlabel(r'$i_\mathrm{sd}$ (p.u.)')
-        ax.set_ylabel(r'$i_\mathrm{sq}$ (p.u.)')
+        ax.set_xlabel(r"$i_\mathrm{sd}$ (p.u.)")
+        ax.set_ylabel(r"$i_\mathrm{sq}$ (p.u.)")
         ax.legend()
         if self.psi_f == 0:
             ax.axis([0, i_s_max/base.i, 0, i_s_max/base.i])
         elif self.L_q > self.L_d:
             ax.axis([-i_s_max/base.i, 0, 0, i_s_max/base.i])
         else:
             ax.axis([-i_s_max/base.i, i_s_max/base.i, 0, i_s_max/base.i])
-        ax.set_aspect('equal')
+        ax.set_aspect("equal")
 
     def plot_torque_current(self, i_s_max, base, N=20):
         """
         Plot torque vs. current characteristics.
 
         Per-unit quantities are used.
 
@@ -570,30 +570,30 @@
         ax1.plot(clim.tau_M/base.tau, clim.i_s.real/base.i)
 
         ax1.set_xlim(0, i_s_max/base.i)
         if self.psi_f == 0:
             ax1.set_ylim(0, None)
         elif self.L_q > self.L_d:
             ax1.set_ylim(None, 0)
-        ax1.legend(['MTPA', 'MTPV', 'Const current'])
-        ax1.set_ylabel(r'$i_\mathrm{sd}$ (p.u.)')
+        ax1.legend(["MTPA", "MTPV", "Const current"])
+        ax1.set_ylabel(r"$i_\mathrm{sd}$ (p.u.)")
 
         # Plot i_sq vs. tau_M
         ax2.plot(mtpa.tau_M/base.tau, mtpa.i_s.imag/base.i)
         try:
             ax2.plot(mtpv.tau_M/base.tau, mtpv.i_s.imag/base.i)
         except TypeError:
             pass
         ax2.plot(clim.tau_M/base.tau, clim.i_s.imag/base.i)
 
         ax2.set_xlim(0, i_s_max/base.i)
         ax2.set_ylim(0, None)
-        ax2.legend(['MTPA', 'MTPV', 'Const current'])
-        ax2.set_ylabel(r'$i_\mathrm{sq}$ (p.u.)')
-        ax2.set_xlabel(r'$\tau_\mathrm{M}$ (p.u.)')
+        ax2.legend(["MTPA", "MTPV", "Const current"])
+        ax2.set_ylabel(r"$i_\mathrm{sq}$ (p.u.)")
+        ax2.set_xlabel(r"$\tau_\mathrm{M}$ (p.u.)")
 
     def plot_torque_flux(self, i_s_max, base, N=20):
         """
         Plot torque vs. flux magnitude characteristics.
 
         Per-unit quantities are used.
 
@@ -621,10 +621,10 @@
         ax.plot(np.abs(mtpa.psi_s)/base.psi, mtpa.tau_M/base.tau)
         try:
             ax.plot(np.abs(mtpv.psi_s)/base.psi, mtpv.tau_M/base.tau)
         except AttributeError:
             pass
         ax.plot(np.abs(clim.psi_s)/base.psi, clim.tau_M/base.tau)
 
-        ax.legend(['MTPA', 'MTPV', 'Const current'])
-        ax.set_xlabel(r'$\psi_\mathrm{s}$ (p.u.)')
-        ax.set_ylabel(r'$\tau_\mathrm{m}$ (p.u.)')
+        ax.legend(["MTPA", "MTPV", "Const current"])
+        ax.set_xlabel(r"$\psi_\mathrm{s}$ (p.u.)")
+        ax.set_ylabel(r"$\tau_\mathrm{m}$ (p.u.)")
```

### Comparing `motulator-0.1.5/motulator/control/sm/_vector.py` & `motulator-0.1.6/motulator/control/sm/_vector.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/model/_converter.py` & `motulator-0.1.6/motulator/model/_converter.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/model/_mechanics.py` & `motulator-0.1.6/motulator/model/_mechanics.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/model/_simulation.py` & `motulator-0.1.6/motulator/model/_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,31 +214,31 @@
         Solve the continuous-time model and call the discrete-time controller.
 
         Parameters
         ----------
         t_stop : float, optional
             Simulation stop time. The default is 1.
         max_step : float, optional
-            Max step size of the solver. The default is `inf`.
+            Max step size of the solver. The default is inf.
 
         Notes
         -----
         Other options of `solve_ivp` could be easily changed if needed, but, for
         simplicity, only `max_step` is included as an option of this method.
 
         """
         try:
             self._simulation_loop(t_stop, max_step)
         except FloatingPointError:
-            print(f'Invalid value encountered at {self.mdl.t0:.2f} seconds.')
+            print(f"Invalid value encountered at {self.mdl.t0:.2f} seconds.")
         # Call the post-processing functions
         self.mdl.post_process()
         self.ctrl.post_process()
 
-    @np.errstate(invalid='raise')
+    @np.errstate(invalid="raise")
     def _simulation_loop(self, t_stop, max_step):
         """Run the main simulation loop."""
         while self.mdl.t0 <= t_stop:
 
             # Run the digital controller
             T_s, d_abc_ref = self.ctrl(self.mdl)
 
@@ -266,19 +266,19 @@
                     t0_new, x0_new = t_span[-1], sol.y[:, -1]
                     self.mdl.set_initial_values(t0_new, x0_new)
 
                     # Save the solution
                     sol.q = len(sol.t)*[self.mdl.converter.q]
                     self.mdl.save(sol)
 
-    def save_mat(self, name='sim'):
+    def save_mat(self, name="sim"):
         """
         Save the simulation data into MATLAB .mat files.
 
         Parameters
         ----------
         name : str, optional
-            Name for the simulation instance. The default is 'sim'.
+            Name for the simulation instance. The default is `sim`.
 
         """
-        savemat(name + '_mdl_data' + '.mat', self.mdl.data)
-        savemat(name + '_ctrl_data' + '.mat', self.ctrl.data)
+        savemat(name + "_mdl_data" + ".mat", self.mdl.data)
+        savemat(name + "_ctrl_data" + ".mat", self.ctrl.data)
```

### Comparing `motulator-0.1.5/motulator/model/im/_drive.py` & `motulator-0.1.6/motulator/model/im/_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 
 # %%
 class InductionMachine:
     """
     Γ-equivalent model of an induction machine.
 
-    An induction machine is modeled using the Γ-equivalent model [Sle1989]_. The 
-    model is implemented in stator coordinates. The flux linkages are used as 
-    state variables.
+    An induction machine is modeled using the Γ-equivalent model [#Sle1989]_. 
+    The model is implemented in stator coordinates. The flux linkages are used 
+    as state variables.
 
     Parameters
     ----------
     n_p : int
         Number of pole pairs.
     R_s : float
         Stator resistance (Ω).
@@ -33,19 +33,19 @@
         Stator inductance (H).
 
     Notes
     -----
     The Γ model is chosen here since it can be extended with the magnetic
     saturation model in a staightforward manner. If the magnetic saturation is
     omitted, the Γ model is mathematically identical to the inverse-Γ and T
-    models [Sle1989]_.
+    models [#Sle1989]_.
 
     References
     ----------
-    .. [Sle1989] Slemon, "Modelling of induction machines for electric drives," 
+    .. [#Sle1989] Slemon, "Modelling of induction machines for electric drives," 
        IEEE Trans. Ind. Appl., 1989, https://doi.org/10.1109/28.44251.
 
     """
 
     def __init__(self, n_p, R_s, R_r, L_ell, L_s):
         # pylint: disable=too-many-arguments
         self.n_p = n_p
```

### Comparing `motulator-0.1.5/motulator/model/sm/_drive.py` & `motulator-0.1.6/motulator/model/sm/_drive.py`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/motulator/model/sm/_flux_maps.py` & `motulator-0.1.6/motulator/model/sm/_flux_maps.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 import matplotlib.pyplot as plt
 from cycler import cycler
 from scipy.io import loadmat
 from scipy.interpolate import griddata
 from motulator._utils import Bunch
 
 # Plotting parameters
-plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
-plt.rcParams['lines.linewidth'] = 1.
-plt.rcParams['axes.grid'] = True
-plt.rcParams.update({'text.usetex': False})
+plt.rcParams["axes.prop_cycle"] = cycler(color="brgcmyk")
+plt.rcParams["lines.linewidth"] = 1.
+plt.rcParams["axes.grid"] = True
+plt.rcParams.update({"text.usetex": False})
 
 
 # %%
-def import_syre_data(fname='THOR.mat', add_negative_q_axis=True):
+def import_syre_data(fname, add_negative_q_axis=True):
     """
     Import a flux map from the MATLAB data file in the SyR-e format.
 
     For more information on the SyR-e project and the MATLAB file format,
     please visit:
 
         https://github.com/SyR-e/syre_public
 
     The imported data is converted to the PMSM coordinate convention, in which
     the PM flux is along the d axis.
 
     Parameters
     ----------
-    fname : str, optional
-        MATLAB file name. The default is 'THOR.mat'.
+    fname : str
+        MATLAB file name.
     add_negative_q_axis : bool, optional
         Adds the negative q-axis data based on the symmetry.
 
     Returns
     -------
     Bunch object with the following fields defined:
     i_s : complex ndarray
@@ -52,23 +52,23 @@
 
     """
     # Read the data from mat-file
     mat = loadmat(fname)
 
     # Use the PMSM convention in coordinates. Rotate the matrices by -90 deg
     # to get monotonically increasing grid data.
-    i_d = -np.rot90(mat['motorModel'][0, 0]['FluxMap_dq'][0, 0]['Iq'], -1)
-    i_q = np.rot90(mat['motorModel'][0, 0]['FluxMap_dq'][0, 0]['Id'], -1)
-    psi_d = -np.rot90(mat['motorModel'][0, 0]['FluxMap_dq'][0, 0]['Fq'], -1)
-    psi_q = np.rot90(mat['motorModel'][0, 0]['FluxMap_dq'][0, 0]['Fd'], -1)
-    tau_M = np.rot90(mat['motorModel'][0, 0]['FluxMap_dq'][0, 0]['T'], -1)
+    i_d = -np.rot90(mat["motorModel"][0, 0]["FluxMap_dq"][0, 0]["Iq"], -1)
+    i_q = np.rot90(mat["motorModel"][0, 0]["FluxMap_dq"][0, 0]["Id"], -1)
+    psi_d = -np.rot90(mat["motorModel"][0, 0]["FluxMap_dq"][0, 0]["Fq"], -1)
+    psi_q = np.rot90(mat["motorModel"][0, 0]["FluxMap_dq"][0, 0]["Fd"], -1)
+    tau_M = np.rot90(mat["motorModel"][0, 0]["FluxMap_dq"][0, 0]["T"], -1)
 
     # Clip the negative q-axis values
-    np.clip(i_q, 0, np.inf, out=i_q)
-    np.clip(psi_q, 0, np.inf, out=psi_q)
+    i_q = np.clip(i_q, 0, np.inf)
+    psi_q = np.clip(psi_q, 0, np.inf)
 
     if add_negative_q_axis:
         # Add the negative q-axis data, flipped based on the symmetry
         i_d = np.concatenate((np.flipud(i_d), i_d))
         i_q = np.concatenate((-np.flipud(i_q), i_q))
         psi_d = np.concatenate((np.flipud(psi_d), psi_d))
         psi_q = np.concatenate((-np.flipud(psi_q), psi_q))
@@ -89,43 +89,43 @@
     Parameters
     ----------
     data : Bunch
         Flux map data.
 
     """
     fig = plt.figure(figsize=(10, 5))
-    ax1 = fig.add_subplot(1, 2, 1, projection='3d')
-    ax2 = fig.add_subplot(1, 2, 2, projection='3d')
+    ax1 = fig.add_subplot(1, 2, 1, projection="3d")
+    ax2 = fig.add_subplot(1, 2, 2, projection="3d")
     ax1.plot_surface(data.i_s.real, data.i_s.imag, data.psi_s.real)
     ax2.plot_surface(data.i_s.real, data.i_s.imag, data.psi_s.imag)
-    ax1.set_xlabel(r'$i_\mathrm{d}$ (A)')
-    ax1.set_ylabel(r'$i_\mathrm{q}$ (A)')
-    ax1.set_zlabel(r'$\psi_\mathrm{d}$ (Vs)')
-    ax2.set_xlabel(r'$i_\mathrm{d}$ (A)')
-    ax2.set_ylabel(r'$i_\mathrm{q}$ (A)')
-    ax2.set_zlabel(r'$\psi_\mathrm{q}$ (Vs)')
+    ax1.set_xlabel(r"$i_\mathrm{d}$ (A)")
+    ax1.set_ylabel(r"$i_\mathrm{q}$ (A)")
+    ax1.set_zlabel(r"$\psi_\mathrm{d}$ (Vs)")
+    ax2.set_xlabel(r"$i_\mathrm{d}$ (A)")
+    ax2.set_ylabel(r"$i_\mathrm{q}$ (A)")
+    ax2.set_zlabel(r"$\psi_\mathrm{q}$ (Vs)")
 
 
 # %%
 def plot_torque_map(data):
     """
     Plot the torque as function of the current.
 
     Parameters
     ----------
     data : Bunch
         Flux map data.
 
     """
     fig = plt.figure()
-    ax = fig.add_subplot(projection='3d')
+    ax = fig.add_subplot(projection="3d")
     ax.plot_surface(data.i_s.real, data.i_s.imag, data.tau_M)
-    ax.set_xlabel(r'$i_\mathrm{d}$ (A)')
-    ax.set_ylabel(r'$i_\mathrm{q}$ (A)')
-    ax.set_zlabel(r'$\tau_\mathrm{M}$ (Nm)')
+    ax.set_xlabel(r"$i_\mathrm{d}$ (A)")
+    ax.set_ylabel(r"$i_\mathrm{q}$ (A)")
+    ax.set_zlabel(r"$\tau_\mathrm{M}$ (Nm)")
 
 
 # %%
 def plot_flux_vs_current(data):
     """
     Plot the flux vs. current characteristics.
 
@@ -143,44 +143,44 @@
     ind_d_max = np.argmax(data.i_s.real[0, :])
 
     fig = plt.figure()
     ax = fig.add_subplot()
     ax.plot(
         data.i_s.real[ind_q_0, :],
         data.psi_s.real[ind_q_0, :],
-        color='r',
-        linestyle='-',
-        label=r'$\psi_\mathrm{d}(i_\mathrm{d}, 0)$')
+        color="r",
+        linestyle="-",
+        label=r"$\psi_\mathrm{d}(i_\mathrm{d}, 0)$")
     ax.plot(
         data.i_s.real[-1, :],
         data.psi_s.real[-1, :],
-        color='r',
-        linestyle='--',
-        label=r'$\psi_\mathrm{d}(i_\mathrm{d}, i_\mathrm{q,max})$')
+        color="r",
+        linestyle="--",
+        label=r"$\psi_\mathrm{d}(i_\mathrm{d}, i_\mathrm{q,max})$")
     ax.plot(
         data.i_s.imag[:, ind_d_0],
         data.psi_s.imag[:, ind_d_0],
-        color='b',
-        linestyle='-',
-        label=r'$\psi_\mathrm{q}(0, i_\mathrm{q})$')
+        color="b",
+        linestyle="-",
+        label=r"$\psi_\mathrm{q}(0, i_\mathrm{q})$")
     ax.plot(
         data.i_s.imag[:, ind_d_min],
         data.psi_s.imag[:, ind_d_min],
-        color='b',
-        linestyle=':',
-        label=r'$\psi_\mathrm{q}(i_\mathrm{d,min}, i_\mathrm{q})$')
+        color="b",
+        linestyle=":",
+        label=r"$\psi_\mathrm{q}(i_\mathrm{d,min}, i_\mathrm{q})$")
     ax.plot(
         data.i_s.imag[:, ind_d_max],
         data.psi_s.imag[:, ind_d_max],
-        color='b',
-        linestyle='--',
-        label=r'$\psi_\mathrm{q}(i_\mathrm{d,max}, i_\mathrm{q})$')
+        color="b",
+        linestyle="--",
+        label=r"$\psi_\mathrm{q}(i_\mathrm{d,max}, i_\mathrm{q})$")
 
-    ax.set_xlabel(r'$i_\mathrm{d}$, $i_\mathrm{q}$ (A)')
-    ax.set_ylabel(r'$\psi_\mathrm{d}$, $\psi_\mathrm{q}$ (Vs)')
+    ax.set_xlabel(r"$i_\mathrm{d}$, $i_\mathrm{q}$ (A)")
+    ax.set_ylabel(r"$\psi_\mathrm{d}$, $\psi_\mathrm{q}$ (Vs)")
     ax.legend()
 
 
 # %%
 def downsample_flux_map(data, N_d=32, N_q=32):
     """
     Downsample the flux map by means of linear interpolation.
@@ -208,16 +208,16 @@
     # Points at which to interpolate data
     i_d = np.linspace(np.min(data.i_s.real), np.max(data.i_s.real), N_d)
     i_q = np.linspace(np.min(data.i_s.imag), np.max(data.i_s.imag), N_q)
     i_d, i_q = np.meshgrid(i_d, i_q)
 
     # Interpolate data
     points = (np.ravel(data.i_s.real), np.ravel(data.i_s.imag))
-    psi_s = griddata(points, np.ravel(data.psi_s), (i_d, i_q), method='linear')
-    tau_M = griddata(points, np.ravel(data.tau_M), (i_d, i_q), method='linear')
+    psi_s = griddata(points, np.ravel(data.psi_s), (i_d, i_q), method="linear")
+    tau_M = griddata(points, np.ravel(data.tau_M), (i_d, i_q), method="linear")
     i_s = i_d + 1j*i_q
 
     return Bunch(i_s=i_s, psi_s=psi_s, tau_M=tau_M)
 
 
 # %%
 def invert_flux_map(data, N_d=32, N_q=32):
@@ -253,13 +253,13 @@
     # Points at which to interpolate data
     psi_d = np.linspace(psi_d_min, psi_d_max, N_d)
     psi_q = np.linspace(psi_q_min, psi_q_max, N_q)
     psi_d, psi_q = np.meshgrid(psi_d, psi_q)
 
     # Interpolate data
     points = (np.ravel(data.psi_s.real), np.ravel(data.psi_s.imag))
-    i_s = griddata(points, np.ravel(data.i_s), (psi_d, psi_q), method='linear')
+    i_s = griddata(points, np.ravel(data.i_s), (psi_d, psi_q), method="linear")
     tau_M = griddata(
-        points, np.ravel(data.tau_M), (psi_d, psi_q), method='linear')
+        points, np.ravel(data.tau_M), (psi_d, psi_q), method="linear")
     psi_s = psi_d + 1j*psi_q
 
     return Bunch(psi_s=psi_s, i_s=i_s, tau_M=tau_M)
```

### Comparing `motulator-0.1.5/motulator.egg-info/PKG-INFO` & `motulator-0.1.6/motulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motulator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Motor Drive Simulator in Python
 Home-page: https://github.com/Aalto-Electric-Drives/motulator
 Author: Marko Hinkkanen
 Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: motulator Version: 0.1.5 Summary: Motor Drive
+Metadata-Version: 2.1 Name: motulator Version: 0.1.6 Summary: Motor Drive
 Simulator in Python Home-page: https://github.com/Aalto-Electric-Drives/
 motulator Author: Marko Hinkkanen Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # *motulator:* Motor Drive Simulator in Python [![Build Status](https:/
```

### Comparing `motulator-0.1.5/motulator.egg-info/SOURCES.txt` & `motulator-0.1.6/motulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `motulator-0.1.5/setup.cfg` & `motulator-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = motulator
-version = 0.1.5
+version = 0.1.6
 author = Marko Hinkkanen
 author_email = marko.hinkkanen@aalto.fi
 description = Motor Drive Simulator in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Aalto-Electric-Drives/motulator
 project_urls =
```

