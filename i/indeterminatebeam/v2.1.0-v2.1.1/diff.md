# Comparing `tmp/indeterminatebeam-v2.1.0.tar.gz` & `tmp/indeterminatebeam-v2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\indeterminatebeam-v2.1.0.tar", last modified: Wed May 12 22:03:14 2021, max compression
+gzip compressed data, was "dist\indeterminatebeam-v2.1.1.tar", last modified: Sun May 16 01:03:38 2021, max compression
```

## Comparing `indeterminatebeam-v2.1.0.tar` & `indeterminatebeam-v2.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2021-05-12 22:03:14.000000 indeterminatebeam-v2.1.0/
--rw-rw-rw-   0        0        0      768 2021-05-12 22:03:14.000000 indeterminatebeam-v2.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-05-12 22:03:14.000000 indeterminatebeam-v2.1.0/indeterminatebeam/
--rw-rw-rw-   0        0        0      467 2021-05-11 09:44:11.000000 indeterminatebeam-v2.1.0/indeterminatebeam/__init__.py
--rw-rw-rw-   0        0        0     1231 2021-02-23 09:33:39.000000 indeterminatebeam-v2.1.0/indeterminatebeam/data_validation.py
--rw-rw-rw-   0        0        0    73638 2021-05-12 12:02:41.000000 indeterminatebeam-v2.1.0/indeterminatebeam/indeterminatebeam.py
--rw-rw-rw-   0        0        0    17263 2021-05-12 12:26:24.000000 indeterminatebeam-v2.1.0/indeterminatebeam/loading.py
--rw-rw-rw-   0        0        0    37868 2021-05-12 12:40:47.000000 indeterminatebeam-v2.1.0/indeterminatebeam/plotly_drawing_aid.py
--rw-rw-rw-   0        0        0     1868 2021-05-11 11:39:16.000000 indeterminatebeam-v2.1.0/indeterminatebeam/units.py
--rw-rw-rw-   0        0        0       22 2021-05-11 09:43:41.000000 indeterminatebeam-v2.1.0/indeterminatebeam/version.py
--rw-rw-rw-   0        0        0       63 2020-12-13 02:17:03.000000 indeterminatebeam-v2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1921 2021-05-04 09:47:18.000000 indeterminatebeam-v2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-16 01:03:38.338220 indeterminatebeam-v2.1.1/
+-rw-rw-rw-   0        0        0      768 2021-05-16 01:03:38.338220 indeterminatebeam-v2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-05-16 01:03:38.337222 indeterminatebeam-v2.1.1/indeterminatebeam/
+-rw-rw-rw-   0        0        0      614 2021-05-14 23:24:33.059334 indeterminatebeam-v2.1.1/indeterminatebeam/__init__.py
+-rw-rw-rw-   0        0        0     1962 2021-05-14 23:24:05.319106 indeterminatebeam-v2.1.1/indeterminatebeam/data_validation.py
+-rw-rw-rw-   0        0        0    74573 2021-05-15 07:28:59.592794 indeterminatebeam-v2.1.1/indeterminatebeam/indeterminatebeam.py
+-rw-rw-rw-   0        0        0    17263 2021-05-12 12:26:24.000000 indeterminatebeam-v2.1.1/indeterminatebeam/loading.py
+-rw-rw-rw-   0        0        0    37878 2021-05-15 07:21:55.385217 indeterminatebeam-v2.1.1/indeterminatebeam/plotly_drawing_aid.py
+-rw-rw-rw-   0        0        0     1549 2021-05-14 23:54:28.863775 indeterminatebeam-v2.1.1/indeterminatebeam/units.py
+-rw-rw-rw-   0        0        0       22 2021-05-16 01:00:07.679760 indeterminatebeam-v2.1.1/indeterminatebeam/version.py
+-rw-rw-rw-   0        0        0       63 2020-12-13 02:17:03.324406 indeterminatebeam-v2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1921 2021-05-04 09:47:18.000000 indeterminatebeam-v2.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `indeterminatebeam-v2.1.0/PKG-INFO` & `indeterminatebeam-v2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: indeterminatebeam
-Version: v2.1.0
+Version: v2.1.1
 Summary: A solver for 1D indeterminate beams
 Home-page: https://github.com/JesseBonanno/IndeterminateBeam
 Author: Jesse Bonanno
 Author-email: jessebonanno@gmail.com
 License: MIT
-Download-URL: https://github.com/JesseBonanno/IndeterminateBeam/archive/v2.1.0.tar.gz
+Download-URL: https://github.com/JesseBonanno/IndeterminateBeam/archive/v2.1.1.tar.gz
 Description: UNKNOWN
 Keywords: statics,indeterminate,beam,civil,structural,shear-force,bending-moment,deflection
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `indeterminatebeam-v2.1.0/indeterminatebeam/indeterminatebeam.py` & `indeterminatebeam-v2.1.1/indeterminatebeam/indeterminatebeam.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,25 @@
 import numpy as np
 from sympy import (integrate, lambdify, Piecewise, sympify, symbols,
                    linsolve, sin, cos, oo, SingularityFunction)
 from sympy.abc import x
 from plotly.subplots import make_subplots
 import plotly.graph_objects as go
 
-# Local Application Imports
+# Local Application Imports'
+import os, sys
+sys.path.insert(0, os.path.abspath('../'))
+
 from indeterminatebeam.data_validation import (
     assert_number,
     assert_positive_number,
-    assert_strictly_positive_number, assert_length
+    assert_strictly_positive_number,
+    assert_length,
+    assert_list_contents,
+    assert_contents,
 )
 from indeterminatebeam.loading import (
     PointLoad,
     PointLoadV,
     PointLoadH,
     DistributedLoad,
     DistributedLoadV,
@@ -60,15 +66,15 @@
     draw_reaction_hoverlabel,
     draw_support_hoverlabel,
     draw_support_rollers,
     draw_support_spring,
     draw_support
 )
 
-from indeterminatebeam.units import IMPERIAL_UNITS, METRIC_UNITS
+from indeterminatebeam.units import IMPERIAL_UNITS, METRIC_UNITS, UNIT_KEYS, UNIT_VALUES
 
 class Support:
     """
     A class to represent a support.
 
     Attributes:
     -------------
@@ -124,27 +130,18 @@
         # validate support stiffness if assigned
         if kx:
             assert_positive_number(kx, 'kx')
         if ky:
             assert_positive_number(ky, 'ky')
 
         # validate fixed tuple elements
-        for a in fixed:
-            if a not in [0, 1]:
-                raise ValueError(
-                    "The provided fixed parameter, must be a tuple of " +
-                    "booleans of length 3"
-                )
+        assert_list_contents(fixed, (0,1), "fixed")
 
         # validate fixed tuple length
-        if len(fixed) != 3:
-            raise ValueError(
-                "The provided fixed parameter, must be a tuple of " +
-                "booleans of length 3"
-            )
+        assert_length(fixed, 3, "fixed")
 
         # Spring representation, set rigid to infinity instead of 1.
         # Otherwise set to 0
         self._stiffness = [oo if a else 0 for a in fixed]
 
         # If kx or ky has been included override oo or 0 value
         if kx:
@@ -272,15 +269,15 @@
 
         self._DATA_POINTS = 200
         self._units = {
             'length': 'm',
             'force': 'N',
             'moment': 'N.m',
             'distributed': 'N/m',
-            'spring stiffness': 'N/m',
+            'stiffness': 'N/m',
             'A': 'm2',
             "E": 'Pa',
             'I': 'm4',
             'deflection': 'm',
         }
 
         self._analysis_reset()
@@ -300,15 +297,15 @@
         """Change units used for inputs and outputs.
         
         Parameters
         ----------
         key: string, default 'length'
             Identifying property with unit to be changed.
             One of the following: 'length', 'force', 'moment',
-            'distributed', 'spring stiffness', 'A', 'E', 'I',
+            'distributed', 'stiffness', 'A', 'E', 'I',
             'deflection'
         unit: string, default 'm'
             unit to assign should contain a unit balanced representation
             consisting of the following units: 'mm', 'cm', 'm', 'N', 'kN',
             'Pa', 'kPa', 'MPa', 'in', 'ft', 'lbf', 'kip'. 
             Unit combinations are written in the following formats:
             'mm2', 'mm4', 'N/m', 'N.m', 'kip/ft2'.
@@ -317,35 +314,27 @@
             """
         if reset:
             self._units= {
                 'length': 'm',
                 'force': 'N',
                 'moment': 'N.m',
                 'distributed': 'N/m',
-                'spring stiffness': 'N/m',
+                'stiffness': 'N/m',
                 'A': 'm2',
                 "E": 'Pa',
                 'I': 'm4',
                 'deflection': 'm',
             }
             self._analysis_reset()
         else:  
-            keys = [k for k in self._units.keys()]
-            if key not in keys:
-                _ = ", ".join(keys)
-                raise ValueError(f'key should be on of the following: {_}')
-            else:
-                units = [u for u in METRIC_UNITS[key].keys()]
-                units += [u for u in IMPERIAL_UNITS[key].keys()]
-                if unit not in units:
-                    _ = ", ".join(units)
-                    raise ValueError(f'unit for "{key}" should be on of the following: {_}')
-                else:
-                    self._units[key] = unit
-                    self._analysis_reset()
+            assert_contents(key,UNIT_KEYS,"key")
+            assert_contents(unit, UNIT_VALUES[key], "unit")
+
+            self._units[key] = unit
+            self._analysis_reset()
 
     def add_loads(self, *loads):
         """Associate load objects with the beam object.
 
         Parameters
         ----------
         *loads : iterable
@@ -524,15 +513,18 @@
         # to seperate all load types so that appropriate unit conversion factors
         # could be applied.
 
         # create a dictionary that associates units with the unit conversion value,
         # i.e. the number that the input should be multiplied by to change to SI
         units = {}
         for key, val in self._units.items():
-            units[key] = METRIC_UNITS[key][val]
+            if val in METRIC_UNITS[key].keys():
+                units[key] = METRIC_UNITS[key][val]
+            else:
+                units[key] = IMPERIAL_UNITS[key][val]
         
         x1 = self._x1
 
         # initialised with position and stiffness.
         self._supports = sorted(
             self._supports,
             key=lambda item: item._position
@@ -706,15 +698,15 @@
         # F/k, where k is the spring stiffness which is a real number for a
         # spring and infinity for conventional fixed support.)
         # all units are in N and m, deflection is in m.
         for reaction in unknowns['y']:
             equations_ym.append(
                 v_EI.subs(x, reaction['position'])
                 / (self._E * units['E'] * self._I * units['I'])
-                + reaction['variable'] / (reaction['stiffness'] * units['spring stiffness'])
+                + reaction['variable'] / (reaction['stiffness'] * units['stiffness'])
             )
 
         # equation for normal forces
         equations_xx = [F_Rx]
 
         # the extension of the beam will be equal to the spring
         # displacement on right minus spring displacment on left.
@@ -736,17 +728,17 @@
                 # axial deformation between start and end =
                 #   (NV_EA(end) - NV_EA(start)) / (EA)
                 equations_xx.append(
                     (
                         Nv_EA.subs(x, end['position']) -
                         Nv_EA.subs(x, start['position'])
                     ) / (self._E * units['E'] * self._A * units['A'])
-                    + start['variable'] / (start['stiffness'] * units['spring stiffness'])
+                    + start['variable'] / (start['stiffness'] * units['stiffness'])
                     # represents elongation displacment on right
-                    - end['variable'] / (end['stiffness'] * units['spring stiffness'])
+                    - end['variable'] / (end['stiffness'] * units['stiffness'])
                 )
 
         # compute analysis with linsolve
         solutions_ym = list(linsolve(equations_ym, unknowns_ym))[0]
         solutions_xx = list(linsolve(equations_xx, unknowns_xx))[0]
 
         # Create solution dictionary
@@ -784,15 +776,15 @@
                 else:
                     i = 2
 
                 # assign reaction to self._reactions using support position
                 # as key, and using i for correct position in list.
                 # Note list for each supports reaction forces is of form
                 # [x,y,m].
-                self._reactions[position][i] = float(round(ans/units['force'], 5))
+                self._reactions[position][i] = float(round(ans/units['force'], 10))
 
         # set calculated beam equations on beam changing all singularity
         # functions to piecewise functions (see sympy_expr_to_piecewise
         # for more details.)
         self._normal_forces = (self.sympy_expr_to_piecewise(N_i_1) + N_i_2) / units['force']
         self._shear_forces = (self.sympy_expr_to_piecewise(F_i_1) + F_i_2) / units['force']
         self._bending_moments = (self.sympy_expr_to_piecewise(M_i_1) + M_i_2) / units['moment']
@@ -909,17 +901,16 @@
 
         directions = ['x', 'y', 'm']
 
         # if a direction has been passed will be returning a single value
         # for the reaction force in that direction
         if direction:
             # check direction valid
-            if direction not in directions:
-                raise ValueError(
-                    "direction should be the value 'x', 'y' or 'm'")
+            assert_contents(direction, directions, "direction")
+
             # if direction valid return appropriate reaction fore
             return self._reactions[x_coord][directions.index(direction)]
 
         # if no direction is specified return a list of all the reaction
         # forces.
         return self._reactions[x_coord]
 
@@ -983,35 +974,35 @@
             # being at a singularity value the values from each side
             # are inspected and the absmax case is returned.)
             x_ = []
             for p in x_coord:
                 l = p - 0.0000001
                 r = p + 0.0000001
 
-                a = round(float(y_lam(l)), 3)
-                b = round(float(y_lam(r)), 3)
+                a = round(float(y_lam(l)), 10)
+                b = round(float(y_lam(r)), 10)
 
                 c = max([a,b], key = abs)
                 x_.append(c)
 
             # make a list of one only return one value to match
             # data type return from previous versions.
             if len(x_) == 1:
                 return x_[0]
             return x_
 
         min_ = float(y_vec.min())
         max_ = float(y_vec.max())
 
         if return_max:
-            return round(max_, 3)
+            return round(max_, 10)
         elif return_min:
-            return round(min_, 3)
+            return round(min_, 10)
         else:
-            return round(max(abs(min_), max_), 3)
+            return round(max(abs(min_), max_), 10)
 
     def get_bending_moment(self, *x_coord, return_max=False,
                            return_min=False, return_absmax=False):
         """Find the bending moment(s) on the beam object.
 
         Parameters
         ----------
@@ -1471,17 +1462,17 @@
             fig.update_xaxes(title_text=xt)
 
         # visible false means y axis doesnt show, fixing range means
         # wont zoom in y direction
             fig.update_yaxes(visible=False, range=[-3, 3], fixedrange=True)
 
         for position, values in self._reactions.items():
-            x_ = round(values[0], 3)
-            y_ = round(values[1], 3)
-            m_ = round(values[2], 3)
+            x_ = round(values[0], 10)
+            y_ = round(values[1], 10)
+            m_ = round(values[2], 10)
 
             # if there are reaction forces
             if abs(x_) > 0 or abs(y_) > 0 or abs(m_) > 0:
                 # subplot case
                 if row and col:
                     fig = draw_reaction_hoverlabel(
                         fig,
@@ -1842,26 +1833,26 @@
             else:
                 ay = -40
 
             if switch_axes:
 
                 annotation = dict(
                     x=q_res, y=q_val,
-                    text=f"{str(q_val)} {xunits}<br>{str(q_res)} {yunits}",
+                    text=f"{q_val:.3f} {xunits}<br>{q_res:.3f} {yunits}",
                     showarrow=True,
                     arrowhead=1,
                     xref='x',
                     yref='y',
                     ax=ay,
                     ay=0,
                 )
             else:
                 annotation = dict(
                     x=q_val, y=q_res,
-                    text=f"{str(q_val)} {xunits}<br>{str(q_res)} {yunits}",
+                    text=f"{q_val:.3f} {xunits}<br>{q_res:.3f} {yunits}",
                     showarrow=True,
                     arrowhead=1,
                     xref='x',
                     yref='y',
                     ax=0,
                     ay=ay
                 )
@@ -1953,24 +1944,59 @@
             return func
 
 
 if __name__ == "__main__":
     # if want to run directly from this file add the following
     # two lines at the start of this script:
 
-    beam = Beam(3)
-
-    a = Support(0,(1,1,1))
-    b = Support(3,(0,1,0))
-
-    load_1 = PointLoadV(-8000,1.5)
-    load_2 = UDLV(-6000, (0,3))
 
-    beam.add_supports(a,b)
-    beam.add_loads(load_1,load_2)
+    # Lets define every possible degree of freedom combination for
+    # supports below, and view them on a plot:
+    support_0 = Support(0, (1,1,1))     # conventional fixed support
+    support_1 = Support(1, (1,1,0))     # conventional pin support
+    support_2 = Support(2, (1,0,1))     
+    support_3 = Support(3, (0,1,1))
+    support_4 = Support(4, (0,0,1))
+    support_5 = Support(5, (0,1,0))     # conventional roller support
+    support_6 = Support(6, (1,0,0))
+
+    # Note we could also explicitly define parameters as follows:
+    support_0 = Support(coord=0, fixed=(1,1,1))
+
+    # Now lets define some spring supports
+    support_7 = Support(7, (0,0,0), kx = 10)    #spring in x direction only
+    support_8 = Support(8, (0,0,0), ky = 5)     # spring in y direction only
+    support_9 = Support(9, (0,0,0), kx = 100, ky = 100)     # spring in x and y direction
+
+    # Now lets define a support which is fixed in one degree of freedom
+    # but has a spring stiffness in another degree of freedom
+    support_10 = Support(10, (0,1,0), kx = 10) #spring in x direction, fixed in y direction
+    support_11 = Support(11, (0,1,1), kx = 10) #spring in x direction, fixed in y and m direction
+
+    # Note we could also do the following for the same result since the spring
+    # stiffness overides the fixed boolean in respective directions
+    support_10 = Support(10, (1,1,0), kx =10)
+
+    # Now lets plot all the supports we have created
+    beam = Beam(11)
+
+    beam.add_supports(
+        support_0,
+        support_1,
+        support_2,
+        support_3,
+        support_4,
+        support_5,
+        support_6,
+        support_7,
+        support_8,
+        support_9,
+        support_10,
+        support_11,
+    )
 
     beam.analyse()
 
     fig1 = beam.plot_beam_internal()
     fig1.show()
 
     fig2 = beam.plot_beam_external()
```

### Comparing `indeterminatebeam-v2.1.0/indeterminatebeam/loading.py` & `indeterminatebeam-v2.1.1/indeterminatebeam/loading.py`

 * *Files identical despite different names*

### Comparing `indeterminatebeam-v2.1.0/indeterminatebeam/plotly_drawing_aid.py` & `indeterminatebeam-v2.1.1/indeterminatebeam/plotly_drawing_aid.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
         annotation = dict(
             xref="x", yref="y",
             x=x0,
             y=y0,
             xshift=x1,
             yshift=y1,
-            text=str(force)+" "+units,
+            text=f"{force:.3f} {units}",
             font_color=color,
             showarrow=False,
         )
 
         # Append shape to plot or subplot
         if row and col:
             fig.add_annotation(annotation, row=row, col=col)
@@ -449,15 +449,15 @@
     if show_values:
 
         annotation = dict(
             xref="x", yref="y",
             x=x_sup,
             y=0,
             yshift=-20,
-            text=str(moment)+" "+units,
+            text=f"{moment:.3f} {units}",
             font_color=color,
             showarrow=False,
         )
 
         # Append shape to plot or subplot
         if row and col:
             fig.add_annotation(annotation, row=row, col=col)
@@ -534,15 +534,15 @@
         if isinstance(load, DistributedLoad):
             name = 'Distributed<br>Load'
             x0, x1 = load.span
             expr = load.expr
             # numpy array for x positions closely spaced (allow for graphing)
             x_vec = np.linspace(x0, x1, int(min((x1 - x0) * 100 + 1, 1e3)))
             y_lam = lambdify(x, expr, 'numpy')
-            y_vec = np.array([round(float(y_lam(t)), 3) for t in x_vec])
+            y_vec = np.array([round(float(y_lam(t)), 10) for t in x_vec])
 
         elif isinstance(load, UDL):
             name = 'UDL'
             x_vec = np.array(load.span)
             y_vec = np.array([load.force, load.force])
         else:
             name = 'Trapezoidal<br>Load'
@@ -621,20 +621,20 @@
     if isinstance(load, (PointLoad, PointTorque)):
         x_sup = load.position
         color = 'red'
         meta = [load.force, load.position, units['length'], units['force'], units['moment']]  # load, position
 
         if isinstance(load, PointTorque):
             color = 'magenta'
-            hovertemplate = 'x: %{meta[1]} %{meta[2]}<br>Moment: %{meta[0]} %{meta[4]}'
+            hovertemplate = 'x: %{meta[1]:.3f} %{meta[2]}<br>Moment: %{meta[0]:.3f} %{meta[4]}'
             name = 'Point<br>Torque'
         elif isinstance(load, PointLoad):
             meta.append(load.angle)
-            hovertemplate = 'x: %{meta[1]} %{meta[2]}<br>Force: %{meta[0]} %{meta[3]}\
-            <br>Angle: %{meta[5]} deg'
+            hovertemplate = 'x: %{meta[1]:.3f} %{meta[2]}<br>Force: %{meta[0]:.3f} %{meta[3]}\
+            <br>Angle: %{meta[5]:.3f} deg'
             name = 'Point<br>Load'
 
         # Define hoverlabel as a marker with 0 opacity and a hovertemplate that
         # relies on meta data field
         trace = go.Scatter(
             x=[x_sup], y=[y_sup],
             showlegend=False, mode="markers",
@@ -667,32 +667,32 @@
         x0, x1 = load.span
         angle = load.angle
         name = 'Distributed<br>Load'
 
         if isinstance(load, DistributedLoad):
             expr = load.expr
             meta = [
-                (x0, round(float(expr.subs(x, x0)), 3), angle),
-                (x1, round(float(expr.subs(x, x1)), 3), angle)
+                (x0, round(float(expr.subs(x, x0)), 10), angle),
+                (x1, round(float(expr.subs(x, x1)), 10), angle)
             ]
 
         elif isinstance(load, UDL):
             meta = [
                 (x0, load.force, angle),
                 (x1, load.force, angle)
             ]
         else:
             meta = [
                 (x0, load.force[0], angle),
                 (x1, load.force[1], angle)
             ]
         
         
-        hovertemplate = 'x: %{meta[0]} %{meta[3]}<br>Force: %{meta[1]} %{meta[4]}\
-        <br>Angle: %{meta[2]} deg'
+        hovertemplate = 'x: %{meta[0]:.3f} %{meta[3]}<br>Force: %{meta[1]:.3f} %{meta[4]}\
+        <br>Angle: %{meta[2]:.3f} deg'
 
         for x_, y_, a_ in meta:
             trace = go.Scatter(
                 x=[x_], y=[0],
                 showlegend=False, mode="markers",
                 name=name,
                 meta=[x_, y_, a_, units['length'], units['distributed']],
@@ -737,21 +737,21 @@
     plotly figure
         plotly figure to append hoverlabel representation to.
     """
     # reactions should be [x,y,m]
     x_, y_, m_ = reactions
 
     # Write hovertemplate depending on support restraints
-    hovertemplate = "Reactions<br>x coord: %{x} %{meta[3]}"
+    hovertemplate = "Reactions<br>x coord: %{x:.3f} %{meta[3]}"
     if x_:
-        hovertemplate += "<br>x: %{meta[0]} %{meta[4]}"
+        hovertemplate += "<br>x: %{meta[0]:.3f} %{meta[4]}"
     if y_:
-        hovertemplate += "<br>y: %{meta[1]} %{meta[4]}"
+        hovertemplate += "<br>y: %{meta[1]:.3f} %{meta[4]}"
     if m_:
-        hovertemplate += "<br>m: %{meta[2]} %{meta[5]}"
+        hovertemplate += "<br>m: %{meta[2]:.3f} %{meta[5]}"
 
     # Create scatter object with opacity 0 for hovertemplate
     trace = go.Scatter(
         x=[x_sup], y=[0],
         showlegend=False, mode="markers",
         name="Reaction",
         meta=[x_, y_, m_, units['length'], units['force'], units['moment']],
@@ -766,36 +766,36 @@
         fig.add_trace(trace, row=row, col=col)
     else:
         fig.add_trace(trace)
 
     return fig
 
 
-def draw_support_hoverlabel(fig, support, kx=0, ky=0, row=None, col=None, units={'length':'m','spring stiffness':"N/m"}):
+def draw_support_hoverlabel(fig, support, kx=0, ky=0, row=None, col=None, units={'length':'m','stiffness':"N/m"}):
     """Draw a reaction hoverlabel on a plotly figure
 
     Parameters
     ----------
     fig : plotly figure
         plotly figure to append force representation to.
     support : Support instance
         support to be represented on figure
     kx : int, optional
-        The spring stiffness of the support in the x direction, default 0
+        The stiffness of the support in the x direction, default 0
     ky : int, optional
-        The spring stiffness of the support in the y direction, default 0
+        The stiffness of the support in the y direction, default 0
     row : int or None,
         Row of subplot to draw line on. If None specified assumes a full plot,
         by default None.
     col : int or None,
         Column of subplot to draw line on. If None specified assumes a full
         plot, by default None.
     units : dict,
         unit dictionary associating the units with different properties of the beam.
-        default is {'length':'m','spring stiffness':"N/m"}.
+        default is {'length':'m','stiffness':"N/m"}.
 
     Returns
     -------
     plotly figure
         plotly figure with hoverlabel appended to it.
     """
     # This could be implemented better (hovertemplates in general could be)
@@ -811,26 +811,26 @@
     x_sup = support._position
 
     # Spring
     if kx or ky:
         name = "Spring"
         color = 'orange'
         meta = [kx, ky, units['length'], units['distributed']]
-        hovertemplate = "x: %{x} %{meta[2]}"
+        hovertemplate = "x: %{x:.3f} %{meta[2]}"
         if kx:
-            hovertemplate += "<br>kx: %{meta[0]} %{meta[3]}"
+            hovertemplate += "<br>kx: %{meta[0]:.3f} %{meta[3]}"
         if ky:
-            hovertemplate += "<br>ky: %{meta[1]} %{meta[3]}"
+            hovertemplate += "<br>ky: %{meta[1]:.3f} %{meta[3]}"
 
     # Support
     else:
         name = "Support"
         color = 'blue'
         meta = [str(fixed), units['length']]
-        hovertemplate = "x: %{x} %{meta[1]}<br>Fixed: %{meta[0]}"
+        hovertemplate = "x: %{x:.3f} %{meta[1]}<br>Fixed: %{meta[0]}"
 
     # necessary for hover information, opacicity 0 so not visible otherwise
     # symbol is arbritrary since invisible
     trace = go.Scatter(
         x=[x_sup], y=[0],
         showlegend=False, mode="markers",
         name=name,
@@ -944,15 +944,15 @@
     row : int or None,
         Row of subplot to draw line on. If None specified assumes a full plot,
         by default None.
     col : int or None,
         Column of subplot to draw line on. If None specified assumes a full
         plot, by default None.
     units: str,
-        The units suffix drawn with the spring stiffness value. Default is 'N/m'.
+        The units suffix drawn with the stiffness value. Default is 'N/m'.
 
     Returns
     -------
     plotly figure
         Returns the plotly figure passed into function with the spring shape
         appended to it."""
 
@@ -1008,29 +1008,29 @@
 
             annotation = dict(
                 xref="x", yref="y",
                 x=x_sup,
                 y=0,
                 yshift=y0 * 1.5,
                 xshift=x0 * 2,
-                text=str(stiffness)+" "+units,
+                text=f"{stiffness:.3f} {units}",
                 font_color=color,
                 showarrow=False,
             )
 
             # Append shape to plot or subplot
             if row and col:
                 fig.add_annotation(annotation, row=row, col=col)
             else:
                 fig.add_annotation(annotation)
 
     return fig
 
 
-def draw_support(fig, support, row=None, col=None, units = {'length':'m', 'spring stiffness':'N/m'}):
+def draw_support(fig, support, row=None, col=None, units = {'length':'m', 'stiffness':'N/m'}):
     """Draw a support on a plotly figure.
 
     Parameters
     ----------
     fig : plotly figure
         plotly figure to append roller shape to.
     support : Support instance
@@ -1039,15 +1039,15 @@
         Row of subplot to draw line on. If None specified assumes a full plot,
         by default None.
     col : int or None,
         Column of subplot to draw line on. If None specified assumes a full
         plot, by default None.
     units : dict,
         unit dictionary associating the units with different properties of the beam.
-        default is {'length':'m', 'spring stiffness':'N/m'}.
+        default is {'length':'m', 'stiffness':'N/m'}.
 
     Returns
     -------
     plotly figure
         Returns the plotly figure passed into function with a support drawn."""
 
     # grab values from support instance
@@ -1163,26 +1163,26 @@
     if springx:
         fig = draw_support_spring(
             fig,
             support,
             orientation="right",
             row=row,
             col=col,
-            units=units['spring stiffness']
+            units=units['stiffness']
         )
 
     # if springy then draw a spring with up orientation
     if springy:
         fig = draw_support_spring(
             fig,
             support,
             orientation="up",
             row=row,
             col=col,
-            units=units['spring stiffness']
+            units=units['stiffness']
         )
 
     # draw hover label for springs
     if springx or springy:
         fig = draw_support_hoverlabel(
             fig,
             support,
```

### Comparing `indeterminatebeam-v2.1.0/indeterminatebeam/units.py` & `indeterminatebeam-v2.1.1/indeterminatebeam/units.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,32 +6,20 @@
 mm = 0.001
 cm = 0.01
 m = 1
 
 N = 1
 kN = 1000
 
-# METRIC_UNITS = {
-# 'length': {'mm':0.001, 'cm':0.01, 'm':1},
-# 'force': {'N':1, 'kN':1000},
-# 'moment': {'N.mm':0.001, 'kN.mm':1, 'N.m':1, 'kN.m':1000},
-# 'distributed': {'N/mm':0.001, 'kN/mm': 1, 'N/m':1, 'kN/m':1000},
-# 'spring stiffness': {'N/mm':0.001, 'kN/mm': 1, 'N/m':1, 'kN/m':1000},
-# 'A': {'mm2':(10**-3)**2, 'cm2':(10**-2)**2, 'm2':1},
-# "E": {'Pa':1, 'kPa':1000, 'MPa':1000000},
-# 'I': {'mm4':(10**-3)**4, 'cm4':(10**-2)**4, 'm4':1},
-# 'deflection': {'mm':0.001, 'cm':0.01, 'm':1},
-# }
-
 METRIC_UNITS = {
 'length': {'mm':mm, 'cm':cm, 'm':m},
 'force': {'N':N, 'kN':kN},
 'moment': {'N.mm':N*mm, 'kN.mm':kN*mm, 'N.m':N*m, 'kN.m':kN*m},
 'distributed': {'N/mm':N/mm, 'kN/mm': kN/mm, 'N/m':N/m, 'kN/m':kN/m},
-'spring stiffness': {'N/mm':N/mm, 'kN/mm': kN/mm, 'N/m':N/m, 'kN/m':kN/m},
+'stiffness': {'N/mm':N/mm, 'kN/mm': kN/mm, 'N/m':N/m, 'kN/m':kN/m},
 'A': {'mm2':mm**2, 'cm2':cm**2, 'm2':m**2},
 "E": {'Pa':N/(m**2), 'kPa':kN/(m**2), 'MPa':N/(mm**2)},
 'I': {'mm4':mm**4, 'cm4':cm**4, 'm4':m**4},
 'deflection': {'mm':mm, 'cm':cm, 'm':m},
 }
 
 inch = 0.0254
@@ -40,13 +28,20 @@
 kip = 4448.2216
 
 IMPERIAL_UNITS = {
 'length': {'in':inch,'ft':ft},
 'force': {'lbf':lbf,'kip':kip},
 'moment': {'lbf.ft':lbf*ft, 'kip.ft':kip*ft, 'lbf.in':lbf*inch, 'kip.in':kip*inch},
 'distributed': {'kip/ft':kip/ft, 'kip/in': kip/inch, 'lbf/ft':lbf/ft, 'lbf/in':lbf/inch},
-'spring stiffness': {'kip/ft':kip/ft, 'kip/in': kip/inch, 'lbf/ft':lbf/ft, 'lbf/in':lbf/inch},
+'stiffness': {'kip/ft':kip/ft, 'kip/in': kip/inch, 'lbf/ft':lbf/ft, 'lbf/in':lbf/inch},
 'A': {'in2':inch**2, 'ft2':ft**2},
 "E": {'kip/in2':kip/(inch**2), 'kip/ft2':kip/(ft**2), 'lbf/in2':lbf/(inch**2),'lbf/ft2':lbf/(ft**2)},
 'I': {'in4':(inch**4), 'ft4':(ft**4)},
 'deflection': {'in':inch, 'ft':ft},
-}
+}
+
+UNIT_KEYS = [k for k in METRIC_UNITS.keys()]
+UNIT_VALUES = {}
+
+for a in UNIT_KEYS:
+    UNIT_VALUES[a] = [u for u in METRIC_UNITS[a].keys()]
+    UNIT_VALUES[a] += [u for u in IMPERIAL_UNITS[a].keys()]
```

### Comparing `indeterminatebeam-v2.1.0/setup.py` & `indeterminatebeam-v2.1.1/setup.py`

 * *Files identical despite different names*

