# Comparing `tmp/omniplate-0.9.85.tar.gz` & `tmp/omniplate-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.85.tar", max compression
+gzip compressed data, was "omniplate-0.9.9.tar", max compression
```

## Comparing `omniplate-0.9.85.tar` & `omniplate-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.85/README.md
--rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.85/om_code/__init__.py
--rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.85/om_code/admin.py
--rw-r--r--   0        0        0     2577 2023-04-24 14:56:03.906492 omniplate-0.9.85/om_code/analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-01-30 16:21:37.981212 omniplate-0.9.85/om_code/analyseSunrise.py
--rw-r--r--   0        0        0     2609 2023-04-24 14:56:03.906801 omniplate-0.9.85/om_code/analyseTecan.py
--rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.85/om_code/clogger.py
--rw-r--r--   0        0        0    24412 2023-05-16 09:18:38.726986 omniplate-0.9.85/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.85/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.85/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     6965 2023-04-24 14:56:03.907876 omniplate-0.9.85/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3666 2023-01-30 16:21:38.140112 omniplate-0.9.85/om_code/loadplatedata.py
--rw-r--r--   0        0        0     3905 2023-05-09 11:28:17.000000 omniplate-0.9.85/om_code/midlog.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.85/om_code/omerrors.py
--rw-r--r--   0        0        0    17865 2023-05-12 16:40:15.463890 omniplate-0.9.85/om_code/omfitderiv.py
--rw-r--r--   0        0        0     4179 2023-05-09 11:28:17.000000 omniplate-0.9.85/om_code/omgenutils.py
--rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.85/om_code/omplot.py
--rw-r--r--   0        0        0     6473 2023-05-09 11:28:17.000000 omniplate-0.9.85/om_code/omstats.py
--rw-r--r--   0        0        0     6211 2023-05-16 09:18:38.727419 omniplate-0.9.85/om_code/sunder.py
--rw-r--r--   0        0        0    95799 2023-05-16 09:18:38.728218 omniplate-0.9.85/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.85/omniplate/__init__.py
--rw-r--r--   0        0        0     1116 2023-05-16 09:18:38.728614 omniplate-0.9.85/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 omniplate-0.9.85/setup.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.85/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.9/om_code/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.9/om_code/admin.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.9/om_code/clogger.py
+-rw-r--r--   0        0        0    23910 2023-06-10 14:52:08.047214 omniplate-0.9.9/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.9/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.9/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.058039 omniplate-0.9.9/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3470 2023-05-26 11:17:09.852745 omniplate-0.9.9/om_code/loaddata.py
+-rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.069421 omniplate-0.9.9/om_code/midlog.py
+-rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.866642 omniplate-0.9.9/om_code/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.866955 omniplate-0.9.9/om_code/old_analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.867263 omniplate-0.9.9/om_code/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.9/om_code/omerrors.py
+-rw-r--r--   0        0        0    11866 2023-06-10 14:52:08.126153 omniplate-0.9.9/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.317129 omniplate-0.9.9/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.9/om_code/omplot.py
+-rw-r--r--   0        0        0     6781 2023-06-10 14:52:08.375378 omniplate-0.9.9/om_code/omstats.py
+-rw-r--r--   0        0        0     4256 2023-06-10 14:52:08.413530 omniplate-0.9.9/om_code/parseplate.py
+-rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.481613 omniplate-0.9.9/om_code/runfitderiv.py
+-rw-r--r--   0        0        0     6211 2023-05-16 09:18:38.727419 omniplate-0.9.9/om_code/sunder.py
+-rw-r--r--   0        0        0    93614 2023-06-10 14:52:08.661990 omniplate-0.9.9/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.9/omniplate/__init__.py
+-rw-r--r--   0        0        0     1115 2023-06-10 14:52:08.693966 omniplate-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 omniplate-0.9.9/setup.py
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 omniplate-0.9.9/PKG-INFO
```

### Comparing `omniplate-0.9.85/om_code/admin.py` & `omniplate-0.9.9/om_code/admin.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/analyseOldTecan.py` & `omniplate-0.9.9/om_code/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/analyseSunrise.py` & `omniplate-0.9.9/om_code/old_analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/analyseTecan.py` & `omniplate-0.9.9/om_code/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/clogger.py` & `omniplate-0.9.9/om_code/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/corrections.py` & `omniplate-0.9.9/om_code/corrections.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from scipy.interpolate import interp1d
 from scipy.optimize import minimize_scalar
 from statsmodels.nonparametric.smoothers_lowess import lowess
 
 import om_code.omerrors as errors
 import om_code.omgenutils as gu
 import om_code.sunder as sunder
-from om_code.omfitderiv import fitderiv
+from om_code.runfitderiv import runfitderiv
 
 
 def _read_dilution_data(fname):
     d = import_files.read_text("om_code", fname)
     res = np.array(re.split(r"\n|\t", d)[:-1]).astype(float)
     if fname == "dilution_data_xiao.tsv":
         od, dilfac = res[::2], res[1::2]
@@ -45,17 +45,18 @@
     """
     print("Fitting dilution data for OD correction for non-linearities.")
     if ODfname is not None:
         try:
             od_df = pd.read_csv(
                 str(wdirpath / ODfname), sep=None, engine="python", header=None
             )
-            print(f"Using {ODfname}.")
+            print(f"Using {ODfname}. \nAssuming three replicates.\n")
             od_data = od_df.to_numpy()
-            od, dilfac = od_data[:, 0], od_data[:, 1]
+            od = od_data[:, 0].reshape(int(od_data.shape[0] / 3), 3)
+            dilfac = od_data[:, 1].reshape(int(od_data.shape[0] / 3), 3)
         except (FileNotFoundError, OSError):
             raise errors.FileNotFound(str(wdirpath / ODfname))
     else:
         print("Using default data.")
         fname = "dilution_data_xiao.tsv"
         od, dilfac = _read_dilution_data(fname)
     # run nunchaku
@@ -219,90 +220,86 @@
                 self,
                 strains,
                 strainincludes,
                 strainexcludes,
                 "strain",
                 nonull=True,
             ):
-                if not self.sc[
-                    (self.sc.experiment == e)
-                    & (self.sc.condition == c)
-                    & (self.sc.strain == s)
-                ][f[0] + "_corrected_for_autofluorescence"].any():
-                    od, rawfl = sunder.extractwells(
-                        self.r, self.s, e, c, s, ["OD", f[0]]
+                od, rawfl = sunder.extractwells(
+                    self.r, self.s, e, c, s, ["OD", f[0]]
+                )
+                # no data
+                if od.size == 0 or rawfl.size == 0:
+                    print(f"\n-> No data found for {e}: {s} in {c}.\n")
+                    continue
+                # correct autofluorescence for each replicate
+                fl = np.transpose(
+                    [
+                        rawfl[:, i] - refstrfn(od[:, i])
+                        for i in range(od.shape[1])
+                    ]
+                )
+                fl[fl < 0] = np.nan
+                if useGPs:
+                    # get time
+                    t = self.s.query(
+                        "experiment == @e and condition == @c and strain == @s"
+                    )["time"].to_numpy()
+                    flperod = samplewithGPs(
+                        self,
+                        f,
+                        t,
+                        fl,
+                        od,
+                        flcvfn,
+                        bd,
+                        nosamples,
+                        e,
+                        c,
+                        s,
+                        figs,
+                        **kwargs,
                     )
-                    # no data
-                    if od.size == 0 or rawfl.size == 0:
-                        print(f"\n-> No data found for {e}: {s} in {c}.\n")
-                        continue
-                    # correct autofluorescence for each replicate
-                    fl = np.transpose(
-                        [
-                            rawfl[:, i] - refstrfn(od[:, i])
-                            for i in range(od.shape[1])
-                        ]
+                else:
+                    # use only the replicates
+                    flperod = np.transpose(
+                        [fl[:, i] / od[:, i] for i in range(od.shape[1])]
                     )
-                    fl[fl < 0] = np.nan
-                    if useGPs:
-                        # get time
-                        t = self.s.query(
-                            "experiment == @e and condition == @c and strain == @s"
-                        )["time"].to_numpy()
-                        flperod = samplewithGPs(
-                            self,
-                            t,
-                            fl,
-                            od,
-                            flcvfn,
-                            bd,
-                            nosamples,
-                            e,
-                            c,
-                            s,
-                            figs,
-                            **kwargs,
+                    flperod[flperod < 0] = np.nan
+                # check number of NaN
+                nonans = np.count_nonzero(np.isnan(fl))
+                if np.any(nonans):
+                    if nonans == fl.size:
+                        print(
+                            f"\n-> Corrected fluorescence is all NaN for {e}: {s} in {c}.\n"
                         )
                     else:
-                        # use only the replicates
-                        flperod = np.transpose(
-                            [fl[:, i] / od[:, i] for i in range(od.shape[1])]
+                        print(
+                            f"Warning - {e}: {s} in {c}\n"
+                            f"{nonans} corrected data points are"
+                            " NaN because the corrected fluorescence"
+                            " was negative.",
                         )
-                        flperod[flperod < 0] = np.nan
-                    # check number of NaN
-                    nonans = np.count_nonzero(np.isnan(fl))
-                    if np.any(nonans):
-                        if nonans == fl.size:
-                            print(
-                                f"\n-> Corrected fluorescence is all NaN for {e}: {s} in {c}.\n"
-                            )
-                        else:
-                            print(
-                                f"Warning - {e}: {s} in {c}\n"
-                                f"{nonans} corrected data points are"
-                                " NaN because the corrected fluorescence"
-                                " was negative.",
-                            )
-                    # store results
-                    bname = "c-" + f[0]
-                    autofdict = {
-                        "experiment": e,
-                        "condition": c,
-                        "strain": s,
-                        "time": self.s.query(
-                            "experiment == @e and condition == @c "
-                            "and strain == @s"
-                        )["time"].to_numpy(),
-                        bname: np.nanmean(fl, 1),
-                        bname + "_err": nanstdzeros2nan(fl, 1),
-                        bname + "perOD": np.nanmean(flperod, 1),
-                        bname + "perOD_err": nanstdzeros2nan(flperod, 1),
-                    }
-                    addtodataframes(self, autofdict, bname)
-                    addrecord(self, f[0], e, c, s)
+                # store results
+                bname = "c-" + f[0]
+                autofdict = {
+                    "experiment": e,
+                    "condition": c,
+                    "strain": s,
+                    "time": self.s.query(
+                        "experiment == @e and condition == @c "
+                        "and strain == @s"
+                    )["time"].to_numpy(),
+                    bname: np.nanmean(fl, 1),
+                    bname + "_err": nanstdzeros2nan(fl, 1),
+                    bname + "perOD": np.nanmean(flperod, 1),
+                    bname + "perOD_err": nanstdzeros2nan(flperod, 1),
+                }
+                addtodataframes(self, autofdict, bname)
+                addrecord(self, f[0], e, c, s)
 
 
 def processref1(self, f, refstrain, figs, experiment, condition):
     """
     Process reference strain for data with one fluorescence measurement.
 
     Use lowess to smooth the fluorescence of the reference
@@ -424,38 +421,32 @@
                 self,
                 strains,
                 strainincludes,
                 strainexcludes,
                 "strain",
                 nonull=True,
             ):
-                if s != refstrain and not (
-                    self.sc[
-                        (self.sc.experiment == e)
-                        & (self.sc.condition == c)
-                        & (self.sc.strain == s)
-                    ][f[0] + "_corrected_for_autofluorescence"].any()
-                ):
-                    f0, f1, od = sunder.extractwells(
+                if s != refstrain:
+                    fl_0, fl_1, od = sunder.extractwells(
                         self.r, self.s, e, c, s, f.copy() + ["OD"]
                     )
-                    if f0.size == 0 or f1.size == 0:
+                    if fl_0.size == 0 or fl_1.size == 0:
                         print(f"Warning: No data found for {e}: {s} in {c} !!")
                         continue
-                    nodata, nr = f0.shape
+                    nodata, nr = fl_0.shape
                     # set negative values to NaNs
-                    f0[f0 < 0] = np.nan
-                    f1[f1 < 0] = np.nan
+                    fl_0[fl_0 < 0] = np.nan
+                    fl_1[fl_1 < 0] = np.nan
                     # use mean OD for correction
                     odmean = self.s.query(
                         "experiment == @e and condition == @c and strain == @s"
                     )["OD_mean"].to_numpy()
                     # correct autofluorescence
                     ra = refqrfn(odmean)
-                    fl = applyautoflcorrection(self, ra, f0, f1)
+                    fl = applyautoflcorrection(self, ra, fl_0, fl_1)
                     fl[fl < 0] = np.nan
                     # get time
                     t = self.s.query(
                         "experiment == @e and condition == @c and strain == @s"
                     )["time"].to_numpy()
                     # store corrected fluorescence
                     bname = "c-" + f[0]
@@ -466,14 +457,15 @@
                         "time": t,
                         bname: np.nanmean(fl, 1),
                         bname + " err": nanstdzeros2nan(fl, 1),
                     }
                     if useGPs:
                         flperod = samplewithGPs(
                             self,
+                            f[0],
                             t,
                             fl,
                             od,
                             flcvfn,
                             bd,
                             nosamples,
                             e,
@@ -652,67 +644,70 @@
         (self.sc.experiment == exp)
         & (self.sc.condition == con)
         & (self.sc.strain == s)
     ]
     try:
         cvfn = sdf["gp_for_gr"].values[0]
         hypers = [
-            sdf[col].values[0] for col in sorted(sdf.columns) if "hyper" in col
+            sdf[col].values[0]
+            for col in sorted(sdf.columns)
+            if ("hyper" in col and "gr" in col)
         ]
         if np.any(np.isnan(hypers)):
             return None, None
         else:
             return hypers, cvfn
     except KeyError:
         return None, None
 
 
+def instantiateGP(hypers, cvfn, x, y):
+    """Instantiate a Gaussian process."""
+    x1 = np.tile(x, y.shape[1])
+    y1 = np.reshape(y, y.size, order="F")
+    y1 = y1[np.argsort(x1)]
+    x1 = np.sort(x1)
+    # bounds are irrelevant because parameters are optimal
+    go = getattr(gp, cvfn + "GP")({0: (-5, 5), 1: (-4, 4), 2: (-5, 2)}, x1, y1)
+    go.lth_opt = hypers
+    # make predictions so that samples can be generated
+    go.predict(x, derivs=2)
+    return go
+
+
 def samplewithGPs(
-    self, t, fl, od, flcvfn, bd, nosamples, e, c, s, figs, **kwargs
+    self, flname, t, fl, od, flcvfn, bd, nosamples, e, c, s, figs, **kwargs
 ):
     """Generate extra samples of flperod using Gaussian processes."""
     hypers, cvfn = gethypers(self, e, c, s)
     if hypers is None or cvfn is None:
         raise SystemExit(
             f"\nYou first must run getstats for {s} in {c} for {e}."
         )
     # initialise GP for log ODs
-    t1 = np.tile(t, od.shape[1])
-    od1 = np.reshape(od, od.size, order="F")
-    od1 = od1[np.argsort(t1)]
-    t1 = np.sort(t1)
-    # bounds are irrelevant because parameters are optimal
-    go = getattr(gp, cvfn + "GP")(
-        {0: (-5, 5), 1: (-4, 4), 2: (-5, 2)},
-        t1,
-        np.log(od1),
-    )
-    go.lth_opt = hypers
-    go.predict(t)
+    go = instantiateGP(hypers, cvfn, t, np.log(od))
     # run GP for log fluorescence
-    print(f"Fitting fluorescence for {e}: {s} in {c}")
-    ff = fitderiv(
+    fitvar = f"log_{flname}"
+    derivname = f"d/dt_{fitvar}"
+    ff, _ = runfitderiv(
+        self,
         t,
         fl,
-        cvfn=flcvfn,
+        fitvar,
+        derivname,
+        e,
+        c,
+        s,
         bd=bd,
+        cvfn=flcvfn,
         logs=True,
-        stats=False,
+        figs=figs,
         **kwargs,
     )
-    if ff.success:
-        print()
-        if figs:
-            plt.figure()
-            ff.plotfit(
-                ylabel="log fluorescence",
-                figtitle=f"{e}: {s} in {c}",
-            )
-            plt.show(block=False)
-    else:
+    if not ff.success:
         print(f"\n-> Fitting fluorescence failed for {e}: {s} in {c}.\n")
         return np.nan * np.ones(fl.shape)
     # sample
     lod_samples = go.sample(nosamples)
     lfl_samples = ff.fitderivsample(nosamples)[0]
     flperod = np.exp(lfl_samples - lod_samples)
     return flperod
```

### Comparing `omniplate-0.9.85/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.9/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.9/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/getfitnesspenalty.py` & `omniplate-0.9.9/om_code/getfitnesspenalty.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,130 +1,153 @@
+import matplotlib.pylab as plt
 import numpy as np
 from scipy import integrate
 from scipy.interpolate import interp1d
-import matplotlib.pylab as plt
-import om_code.omerrors as errors
-from om_code.stats import statserr
+
+import om_code.sunder as sunder
+from om_code.corrections import gethypers, instantiateGP
+from om_code.omstats import statserr
 
 
-def getfitnesspenalty(
-    self, ref, com, y="gr", abs=False, figs=True, nosamples=100, norm=False
+def getfp(
+    self,
+    ref,
+    com,
+    yvar="gr",
+    figs=True,
+    nosamples=100,
+    abs=False,
+    norm=False,
 ):
     """
     Estimate the difference in fitness between two strains.
 
     Calculate the area between typically two growth rate versus OD
     curves, normalised by the length along the OD-axis where they overlap.
 
     Parameters
     -----------
+    self: omniplate.platereader instance
+        An instance of platereader with data loaded.
     ref: list of strings
         For only a single experiment, a list of two strings. The first string
         specifies the condition and the second specifies the strain to be used
         for the reference to which fitness is to be calculated.
         With multiple experiments, a list of three strings. The first string
         specifies the experiment, the second specifies the condition, and the
         third specifies the strain.
     com: list of strings
         For only a single experiment, a list of two strings. The first string
         specifies the condition and the second specifies the strain to be
         compared with the reference.
         With multiple experiments, a list of three strings. The first string
         specifies the experiment, the second specifies the condition, and the
         third specifies the strain.
-    y: string, optional
+    yvar: string, optional
         The variable to be compared.
     figs: boolean, optional
         If True, a plot of the area between the two growth rate versus OD
         curves is shown.
     nosamples: integer
         The number bootstraps used to estimate the error.
+    abs: boolean
+        If True, integrate the absolute difference between the two curves.
     norm: boolean
         If True, returns the mean and variance of the area under the reference
         strain for normalisation.
 
     Returns
     -------
     fp: float
         The area between the two curves.
     err: float
         An estimate of the error in the calculated error, found by
         bootstrapping.
     reffp: float, optional
         The area beneath the reference strain.
     referr: float, optional
-        An estimate of the erroe in the calculated area for the reference
+        An estimate of the error in the calculated area for the reference
         strain.
 
     Example
     -------
-    >>> p.getfitnesspenalty(['1% raf 0.0µg/ml cyclohex', 'WT'],
-    ...                     ['1% raf 0.5µg/ml cyclohex', 'WT'])
+    >>> import omniplate as om
+    >>> from om_code.getfitnesspenalty import getfp
+    >>> p = om.platereader("ExampleData.xlsx", "ExampleDataContents.xlsx", wdir="data")
+    >>> p.getstats(strains="WT", conditions = ["2% Mal", "WT"], ["2% Raf", "WT"])
+    >>> fp, err = getfp(p, ["2% Mal", "WT"], ["2% Raf", "WT"])
     """
-    if len(self.allexperiments) == 1:
+    if len(ref) == 2 & len(com) == 2:
+        # add experiment
         ref.insert(0, self.allexperiments[0])
         com.insert(0, self.allexperiments[0])
-    # get and sample from Gaussian processes
-    if nosamples and y == "gr":
-        # estimate errors
-        try:
-            # sample from Gaussian process
-            f0s, g0s, h0s = self.progress["getstatsGP"][ref[0]][ref[1]][
-                ref[2]
-            ].fitderivsample(nosamples)
-            f1s, g1s, h1s = self.progress["getstatsGP"][com[0]][com[1]][
-                com[2]
-            ].fitderivsample(nosamples)
-            xsref, ysref = np.exp(f0s), g0s
-            xscom, yscom = np.exp(f1s), g1s
-        except KeyError:
-            raise errors.GetFitnessPenalty(
-                "getstats('OD') needs to be run for these strains to "
-                "estimate errors or else set nosamples= 0"
-            )
+    # get and sample from GPs
+    if nosamples and yvar == "gr":
+        # instantiate GPS to estimate errors
+        for ecs in [ref, com]:
+            e, c, s = ecs
+            hypers, cvfn = gethypers(self, e, c, s, yvar)
+            if hypers is None or cvfn is None:
+                raise SystemExit(
+                    "\nYou must first run getstats or set nosamples= 0."
+                )
+            od = sunder.extractwells(self.r, self.s, e, c, s, ["OD"])
+            t = self.s.query(
+                "experiment == @e and condition == @c and strain == @s"
+            )["time"].to_numpy()
+            if ecs == ref:
+                g_ref = instantiateGP(hypers, cvfn, t, od)
+            else:
+                g_com = instantiateGP(hypers, cvfn, t, od)
+        # sample from GPs
+        f0s, g0s = g_ref.sample(nosamples, derivs=1)
+        f1s, g1s = g_com.sample(nosamples, derivs=1)
+        xsref, ysref = np.exp(f0s), g0s
+        xscom, yscom = np.exp(f1s), g1s
+
     else:
         # no estimates of errors
         if nosamples:
             print(
                 "Cannot estimate errors - require y= 'gr' and a recently "
                 "run getstats"
             )
         xsref = self.s.query(
             "experiment == @ref[0] and condition == @ref[1] and "
             "strain == @ref[2]"
         )["OD mean"][:, None]
         ysref = self.s.query(
             "experiment == @ref[0] and condition == @ref[1] and "
             "strain == @ref[2]"
-        )[y].to_numpy()[:, None]
+        )[yvar].to_numpy()[:, None]
         xscom = self.s.query(
             "experiment == @com[0] and condition == @com[1] and "
             "strain == @com[2]"
         )["OD mean"].to_numpy()[:, None]
         yscom = self.s.query(
             "experiment == @com[0] and condition == @com[1] and "
             "strain == @com[2]"
-        )[y].to_numpy()[:, None]
+        )[yvar].to_numpy()[:, None]
         if xsref.size == 0 or ysref.size == 0:
-            print(ref[0] + ": Data missing for", ref[2], "in", ref[1])
+            print(f"{ref[0]}: Data missing for {ref[2]} in {ref[1]}")
             return np.nan, np.nan
         elif xscom.size == 0 or yscom.size == 0:
-            print(com[0] + ": Data missing for", com[2], "in", com[1])
+            print(f"{com[0]}: Data missing for {com[2]} in {com[1]}")
             return np.nan, np.nan
     fps = np.zeros(xsref.shape[1])
     nrm = np.zeros(xsref.shape[1])
     samples = zip(
         np.transpose(xsref),
         np.transpose(ysref),
         np.transpose(xscom),
         np.transpose(yscom),
     )
     # process samples
     for j, (xref, yref, xcom, ycom) in enumerate(samples):
-        # remove any double values in OD because of OD plateau'ing
+        # remove any double values in OD because of OD plateauing
         uxref, uiref = np.unique(xref, return_inverse=True)
         uyref = np.array(
             [
                 np.median(yref[np.nonzero(uiref == i)[0]])
                 for i in range(len(uxref))
             ]
         )
@@ -137,15 +160,15 @@
         )
         # interpolate data
         iref = interp1d(uxref, uyref, fill_value="extrapolate", kind="slinear")
         icom = interp1d(uxcom, uycom, fill_value="extrapolate", kind="slinear")
         # find common range of x
         uxi = np.max([uxref[0], uxcom[0]])
         uxf = np.min([uxref[-1], uxcom[-1]])
-        # perform integration to find normalized area between curves
+        # perform integration to find normalised area between curves
         if abs:
 
             def igrand(x):
                 return np.abs(iref(x) - icom(x))
 
         else:
 
@@ -166,19 +189,19 @@
         # an example figure
         if figs and j == 0:
             plt.figure()
             plt.plot(uxref, uyref, "k-", uxcom, uycom, "b-")
             x = np.linspace(uxi, uxf, np.max([len(uxref), len(uxcom)]))
             plt.fill_between(x, iref(x), icom(x), facecolor="red", alpha=0.5)
             plt.xlabel("OD")
-            plt.ylabel(y)
+            plt.ylabel(yvar)
             plt.legend(
                 [
-                    ref[0] + ": " + ref[2] + " in " + ref[1],
-                    com[0] + ": " + com[2] + " in " + com[1],
+                    f"{ref[0]}: {ref[2]} in {ref[1]}",
+                    f"{com[0]}: {com[2]} in {com[1]}",
                 ],
                 loc="upper left",
                 bbox_to_anchor=(-0.05, 1.15),
             )
             plt.show(block=False)
     if norm:
         return (
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `omniplate-0.9.85/om_code/omfitderiv.py` & `omniplate-0.9.9/om_code/omfitderiv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-import numpy as np
+import copy
 import warnings
+
+import gaussianprocessderivatives as gp
 import matplotlib.pylab as plt
+import numpy as np
 from scipy.interpolate import interp1d
-import copy
-import gaussianprocessderivatives as gp
+
 import om_code.omgenutils as gu
-import om_code.omstats as omstats
 
 
 class fitderiv:
     """
     Smooth and estimate the time derivative of the data via Gaussian processes.
 
-    Summary statistics - the maximal time derivative, the time at which the
-    maximal time derivative occurs, the timescale found from inverting the
-    maximal time derivative, the maximal value of the smoothed data, and the
-    lag time (the time when the tangent from the point with the maximal time
-    derivative crosses a line parallel to the time-axis that passes through the
-    first data point) - are found and their errors estimated using
-    bootstrapping. All statistics can be postfixed by ' err' to find this
-    error.
-
-    A summary statistic is given as the median of a distribution of the
-    statistic calculated from time series sampled from the optimal Gaussian
-    process. Its error is estimated as the interquartile range of this
-    distribution.
-
     After a successful optimisation, the following attributes are generated:
 
     t: array
         The times specified as input.
     d: array
         The data specified as input.
     f: array
@@ -41,16 +28,14 @@
         The inferred first time-derivative.
     dfvar: array
         The inferred variance of the first time-derivative.
     ddf: array
         The inferred second time-derivative.
     ddfvar: array
         The inferred variance of the second time-derivative.
-    ds: dictionary
-        The summary statistics and their estimated errors.
 
     Examples
     --------
     A typical work flow is:
 
     >>> from fitderiv import fitderiv
     >>> q= fitderiv(t, od, figs= True)
@@ -77,19 +62,14 @@
         logs=True,
         noruns=5,
         noinits=100,
         exitearly=False,
         bd=False,
         empirical_errors=False,
         optmethod="L-BFGS-B",
-        nosamples=100,
-        stats=True,
-        statnames=False,
-        printstats=True,
-        showstaterrors=True,
         warn=False,
         linalgmax=3,
         iskip=False,
     ):
         """
         Smooth data and estimate time derivatives with a Gaussian process.
 
@@ -128,38 +108,14 @@
             variance across replicates at each time point.
             If False, the variance of the measurement error is assumed to be
             the same for all time points and its magnitude is a hyperparameter
             that is optimised.
         optmethod: string, optional
             The algorithm used to optimise the hyperparameters, either
             'l_bfgs_b' or 'tnc'.
-        nosamples: integer, optional
-            The number of bootstrap samples taken to estimate errors in
-            statistics.
-        stats: boolean, optional
-            If True, calculate summary statistics for both the smoothed data and
-            the inferred time- derivative.
-        statnames: list of strings
-            To customise the names of the statistics.
-            The default names are:
-            'max df' for the maximal time derivative;
-            'time of max df' for the time at which the maximal time
-            derivative occurs;
-            'inverse max df' for the timescale found from inverting the
-            maximal time
-            derivative;
-            'max f' for the maximal value of the smoothed data;
-            'lag time' for the lag time defined as the time when the
-            tangent from the point with the maximal time derivative
-            crosses a line parallel to the time-axis that passes
-            through the first data point.
-        printstats: boolean, optional
-            If True, print the summary statistics calculated.
-        showstaterrors: boolean, optional
-            If True, display estimated errors for the statistics when printing.
         warn: boolean, optional
             If False, warnings created by covariance matrices that are not
             positive semi-definite are suppressed.
         linalgmax: integer, optional
             The number of times errors generated by underlying linear algebra
             modules during the optimisation by poor choices of the
             hyperparameters should be ignored.
@@ -262,36 +218,26 @@
                 ta,
                 da,
                 ma,
                 noruns,
                 noinits,
                 exitearly,
                 optmethod,
-                stats,
-                nosamples,
-                statnames,
-                showstaterrors,
-                printstats,
             )
 
     def run(
         self,
         cvfn,
         ta,
         da,
         ma,
         noruns,
         noinits,
         exitearly,
         optmethod,
-        stats,
-        nosamples,
-        statnames,
-        showstaterrors,
-        printstats,
     ):
         """Instantiate and run a Gaussian process."""
         try:
             # instantiate GP
             g = getattr(gp, cvfn + "GP")(self.bds, ta, da, merrors=ma)
             print("Using a " + g.description + ".")
             g.info
@@ -322,18 +268,14 @@
         self.lth = g.lth_opt
         self.f = g.f
         self.df = g.df
         self.ddf = g.ddf
         self.fvar = g.fvar
         self.dfvar = g.dfvar
         self.ddfvar = g.ddfvar
-        if stats:
-            self.calculatestats(
-                nosamples, statnames, showstaterrors, printstats
-            )
 
     def fitderivsample(self, nosamples, newt=None):
         """
         Generate samples from the latent function.
 
         Both values for the latent function and its first two
         derivatives are returned, as a tuple.
@@ -363,119 +305,14 @@
             gps = copy.deepcopy(self.g)
             gps.predict(newt, derivs=2, addnoise=True)
         else:
             gps = self.g
         samples = gps.sample(nosamples, derivs=2)
         return samples
 
-    def calculatestats(self, nosamples, statnames, showerrors, printstats):
-        """
-        Calculate statistics from the smoothed data.
-
-        The default names are 'max df', 'time of max df', 'inverse max grad',
-        'max f', and 'lag time'.
-
-        Parameters
-        ----------
-        nosamples: integer
-            The number of bootstrap samples used to estimate errors.
-        statnames: list of strings, optional
-            A list of alternative names for the statistics.
-        showerrors: boolean, optional
-            If True, display the estimated errors.
-        printstats: boolean, optional
-            If True, print the summary stats calculated.
-        """
-        print(f"\nCalculating statistics with {nosamples} samples.")
-        if statnames:
-            self.stats = statnames
-        else:
-            self.stats = [
-                "min_f",
-                "max_f",
-                "max_df",
-                "time_of_max_df",
-                "doubling_time_from_max_df",
-                "lag_time",
-            ]
-        t = self.t
-        fs, gs, hs = self.fitderivsample(nosamples)
-        # min f
-        min_od = fs[np.argmin(fs, 0), np.arange(nosamples)]
-        if self.logs:
-            min_od = np.exp(min_od)
-        # max f
-        max_od = fs[np.argmax(fs, 0), np.arange(nosamples)]
-        if self.logs:
-            max_od = np.exp(max_od)
-        # calculate df stats
-        im = np.argmax(gs, 0)
-        # max df
-        mgr = gs[im, np.arange(nosamples)]
-        # time of max df
-        tmgr = np.array([t[i] for i in im])
-        # inverse max df
-        dt = np.log(2) / mgr
-        # lag time
-        lagtime = (
-            tmgr
-            + (fs[0, np.arange(nosamples)] - fs[im, np.arange(nosamples)])
-            / mgr
-        )
-        # store stats
-        ds = {}
-        for stname, st in zip(
-            self.stats, [min_od, max_od, mgr, tmgr, dt, lagtime]
-        ):
-            ds[stname] = np.median(st)
-            ds[stname + "_err"] = omstats.statserr(st) / 2
-        self.ds = ds
-        self.nosamples = nosamples
-        self.stats2dict(showerrors, printstats)
-
-    def stats2dict(self, showerrors, printstats):
-        """
-        Create and print a dictionary of statistics.
-
-        The statistics are calculated from the smoothed data and its
-        inferred time-derivatives.
-
-        Parameters
-        ----------
-        showerrors: boolean, optional
-            If True, display the errors.
-        printstats: boolean optional
-            If True, display the statistics.
-
-        Returns
-        -------
-        statd: dictionary
-            The statistics and their errors.
-        """
-        if showerrors and printstats:
-            print("\t(displaying median +/- half interquartile range)\n")
-        ds = self.ds
-        statd = {}
-        lenstr = np.max([len(s) for s in self.stats])
-        for s in self.stats:
-            statd[s] = ds[s]
-            statd[s + "_err"] = ds[s + "_err"]
-            if printstats:
-                stname = s.rjust(lenstr + 1)
-                if showerrors:
-                    print(
-                        "{:s}= {:6e} +/- {:6e}".format(
-                            stname, statd[s], ds[s + "_err"]
-                        )
-                    )
-                else:
-                    print("{:s}= {:6e}".format(stname, statd[s]))
-        print()
-        return statd
-
     def plotfit(
         self, char="f", errorfac=1, xlabel="time", ylabel=False, figtitle=False
     ):
         """
         Plot the results of the fitting.
 
         Either the data and the mean of the optimal Gaussian process or
```

### Comparing `omniplate-0.9.85/om_code/omgenutils.py` & `omniplate-0.9.9/om_code/omgenutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,26 +133,14 @@
     ell: list
     """
     if isinstance(ell, list):  # Is a list
         return all(map(islistempty, ell))
     return False  # Not a list
 
 
-# to be deleted - use scipy instead
-# def findiqr(d):
-#     """
-#     Find the interquartile range of data in an array.
-
-#     Parameters
-#     --
-#     d: a one-dimensional array of data
-#     """
-#     return np.subtract(*np.percentile(d, [75, 25]))
-
-
 def makelist(c):
     """
     Ensure that a variable is a list.
 
     Parameters
     --
     c: variable to be made into a list
```

### Comparing `omniplate-0.9.85/om_code/omplot.py` & `omniplate-0.9.9/om_code/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/om_code/omstats.py` & `omniplate-0.9.9/om_code/omstats.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,141 +4,135 @@
 from scipy import integrate
 from scipy.interpolate import interp1d
 from scipy.signal import find_peaks
 from scipy.stats import iqr
 
 
 def statserr(d, **kwargs):
-    """
-    Use the half the interquartile range as an error.
-
-    For errors in statistics calculated from samples from a
-    Gaussian process to be consistent with fitderiv.
-    """
-    return iqr(d)
-
-
-def cleansc(self):
-    """Ensure that NaNs do not change numeric variables from being floats."""
-    floatvars = [
-        "log2_OD_ratio",
-        "log2_OD_ratio_err",
-        "local_max_gr",
-        "local_max_gr_err",
-        "time_of_local_max_gr",
-        "time_of_local_max_gr_err",
-        "area_under_gr_vs_OD",
-        "area_under_gr_vs_OD_err",
-        "normalised_area_under_gr_vs_OD",
-        "normalised_area_under_gr_vs_OD_err",
-        "area_under_OD",
-        "area_under_OD_err",
-        "normalised_area_under_OD",
-        "normalised_area_under_OD_err",
-        "OD_logmaxlike",
-        "max_gr",
-        "max_gr_err",
-        "time_of_max_gr",
-        "time_of_max_gr_err",
-        "doubling_time",
-        "doubling_time_err",
-        "max_OD",
-        "max_OD_err",
-        "lag_time",
-        "lag_time_err",
-    ]
-    for var in floatvars:
-        if var in self.sc.columns:
-            self.sc[var] = self.sc[var].astype(float)
+    """Use the half the interquartile range as an error."""
+    return iqr(d) / 2
 
 
 def findsummarystats(
-    dtype,
+    fitvar,
     derivname,
-    logs,
+    statnames,
     nosamples,
     f,
     t,
     e,
     c,
     s,
     findareas,
     figs,
     plotlocalmax,
     axgr,
     showpeakproperties,
     **kwargs,
 ):
-    """Find summary statistics from GP fit to time series of dtype."""
-    warning = None
-    odtype = "log(" + dtype + ")" if logs else dtype
-    outdf = pd.DataFrame(
+    """
+    Find summary statistics from GP fit to time series of fitvar.
+
+    Find summary statistics with bootstrapped errors including:
+        - the maximal time derivative
+        - the time at which the maximal time derivative occurs
+        - the timescale found from inverting the maximal time derivative
+        - the extreme values and range of the smoothed data
+        - the lag time (the time when the tangent from the point with the
+            maximal time derivative crosses a line parallel to the time-axis
+            that passes through the first data point
+
+    A summary statistic is given as the median of a distribution of the
+    statistic calculated from time series sampled from the optimal Gaussian
+    process.
+
+    Its error is estimated as the interquartile range of this
+    distribution.
+    """
+    # check derivative has been sensibly defined
+    if (
+        np.max(np.abs(f.df)) < 1.0e-20
+        and np.max(np.abs(np.diff(f.dfvar))) < 1.0e-20
+    ):
+        warning = f"\nWarning: getstats may have failed for {e}: {s} in {c}."
+    else:
+        warning = None
+    # time-series for s dataframe
+    df_for_s = pd.DataFrame(
         {
             "experiment": e,
             "condition": c,
             "strain": s,
             "time": t,
-            "f" + odtype: f.f,
-            "f" + odtype + "_err": np.sqrt(f.fvar),
+            f"smoothed_{fitvar}": f.f,
+            f"smoothed_{fitvar}_err": np.sqrt(f.fvar),
             derivname: f.df,
             derivname + "_err": np.sqrt(f.dfvar),
-            "d/dt_" + derivname: f.ddf,
-            "d/dt_" + derivname + "_err": np.sqrt(f.ddfvar),
+            f"d/dt_{derivname}": f.ddf,
+            f"d/dt_{derivname}_err": np.sqrt(f.ddfvar),
         }
     )
-    # check derivative has been sensibly defined
-    if (
-        np.max(np.abs(f.df)) < 1.0e-20
-        and np.max(np.abs(np.diff(f.dfvar))) < 1.0e-20
-    ):
-        warning = (
-            "\nWarning: getstats may have failed for "
-            + e
-            + ": "
-            + s
-            + " in "
-            + c
-        )
-    # find summary statistics
+    # stats for sc dataframe
+    # sample from GP
     fs, gs, hs = f.fitderivsample(nosamples)
+    # min f
+    min_f = fs[np.argmin(fs, 0), np.arange(nosamples)]
+    # max f
+    max_f = fs[np.argmax(fs, 0), np.arange(nosamples)]
+    # range
+    range_f = fs[np.argmax(fs, 0), :] - fs[np.argmin(fs, 0), :]
+    # calculate df stats
+    im = np.argmax(gs, 0)
+    # max df
+    max_df = gs[im, np.arange(nosamples)]
+    # time of max df
+    t_max_df = np.array([t[i] for i in im])
+    # inverse max df
+    dt = np.log(2) / max_df
+    # lag time
+    lagtime = (
+        t_max_df
+        + (fs[0, np.arange(nosamples)] - fs[im, np.arange(nosamples)]) / max_df
+    )
     # find local maximal derivative
     da, dt = findlocalmaxderiv(
         f, gs, axgr, figs, plotlocalmax, showpeakproperties, **kwargs
     )
-    # find area under df vs f and area under f vs t
+    # find area under df/dt vs f and area under f vs t
     if findareas:
-        adff, andff, aft, anft = findareasunder(t, fs, gs, logs)
+        adff, andff, aft, anft = findareasunder(t, fs, gs)
     else:
         adff, andff, aft, anft = np.nan, np.nan, np.nan, np.nan
     # store results
-    statsdict = {
+    dict_for_sc = {
         "experiment": e,
         "condition": c,
         "strain": s,
-        "local_max_" + derivname: np.median(da),
-        "local_max_" + derivname + "_err": statserr(da),
-        "time_of_local_max_" + derivname: np.median(dt),
-        "time_of_local_max_" + derivname + "_err": statserr(dt),
-        "area_under_" + derivname + "_vs_" + dtype: np.median(adff),
-        "area_under_" + derivname + "_vs_" + dtype + "_err": statserr(adff),
-        "normalised_area_under_"
-        + derivname
-        + "_vs_"
-        + dtype: np.median(andff),
-        "normalised_area_under_"
-        + derivname
-        + "_vs_"
-        + dtype
-        + "_err": statserr(andff),
-        "area_under_" + dtype: np.median(aft),
-        "area_under_" + dtype + "_err": statserr(aft),
-        "normalised_area_under_" + dtype: np.median(anft),
-        "normalised_area_under_" + dtype + "_err": statserr(anft),
+        f"local_max_{derivname}": np.median(da),
+        f"local_max_{derivname}_err": statserr(da),
+        f"time_of_local_max_{derivname}": np.median(dt),
+        f"time_of_local_max_{derivname}_err": statserr(dt),
+        # area under df/dt vs f
+        f"area_under_{derivname}_vs_{fitvar}": np.median(adff),
+        f"area_under_{derivname}_vs_{fitvar}_err": statserr(adff),
+        f"normalised_area_under_{derivname}_vs_{fitvar}": np.median(andff),
+        f"normalised_area_under_{derivname}_vs_{fitvar}_err": statserr(andff),
+        # area under f vs t
+        f"area_under_{fitvar}": np.median(aft),
+        f"area_under_{fitvar}_err": statserr(aft),
+        f"normalised_area_under_{fitvar}": np.median(anft),
+        f"normalised_area_under_{fitvar}_err": statserr(anft),
     }
-    return outdf, statsdict, warning
+    # add statnames stats
+    for stname, st in zip(
+        statnames, [min_f, max_f, range_f, max_df, t_max_df, dt, lagtime]
+    ):
+        dict_for_sc[stname] = np.median(st)
+        dict_for_sc[stname + "_err"] = statserr(st)
+    return df_for_s, dict_for_sc, warning
 
 
 def findlocalmaxderiv(
     f, gs, axgr, figs, plotlocalmax, showpeakproperties, **kwargs
 ):
     """
     Find the greatest local maxima in the derivative.
@@ -176,38 +170,40 @@
             )
         return da, dt
     else:
         # mean df has no peaks
         return np.nan, np.nan
 
 
-def findareasunder(t, fs, gs, logs):
+def findareasunder(t, fs, gs):
     """
     Find areas.
 
     Given samples of f, as arguments fs, and of df, as arguments gs,
-    either find the area under df/dt vs f and the area under f vs t
-    or if logs find the area under d/dt log(f) vs f and the area
-    under f vs t.
+    find the area under df/dt vs f and the area under f vs t.
     """
     adff, andff, aft, anft = [], [], [], []
     for fsample, gsample in zip(np.transpose(fs), np.transpose(gs)):
-        sf = np.exp(fsample) if logs else fsample
         # area under df vs f: integrand has f as x and df as y
         def integrand(x):
-            return interp1d(sf, gsample)(x)
+            return interp1d(fsample, gsample)(x)
 
         iresult = integrate.quad(
-            integrand, np.min(sf), np.max(sf), limit=100, full_output=1
+            integrand,
+            np.min(fsample),
+            np.max(fsample),
+            limit=100,
+            full_output=1,
         )[0]
         adff.append(iresult)
-        andff.append(iresult / (np.max(sf) - np.min(sf)))
+        andff.append(iresult / (np.max(fsample) - np.min(fsample)))
+
         # area under f vs t: integrand has t as x and f as y
         def integrand(x):
-            return interp1d(t, sf)(x)
+            return interp1d(t, fsample)(x)
 
         iresult = integrate.quad(
             integrand, np.min(t), np.max(t), limit=100, full_output=1
         )[0]
         aft.append(iresult)
         anft.append(iresult / (np.max(t) - np.min(t)))
     return adff, andff, aft, anft
```

### Comparing `omniplate-0.9.85/om_code/sunder.py` & `omniplate-0.9.9/om_code/sunder.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.85/omniplate/Omniplate.py` & `omniplate-0.9.9/omniplate/Omniplate.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 
 import gaussianprocessderivatives as gp
 import matplotlib.pyplot as plt
 import numpy as np
 import om_code.admin as admin
 import om_code.clogger as clogger
 import om_code.corrections as corrections
-import om_code.loadplatedata as loadplatedata
+import om_code.loaddata as loaddata
+import om_code.midlog as midlog
 import om_code.omerrors as errors
 import om_code.omgenutils as gu
 import om_code.omplot as omplot
-import om_code.omstats as omstats
 import om_code.sunder as sunder
-import om_code.midlog as midlog
 import pandas as pd
 import seaborn as sns
-from om_code.omfitderiv import fitderiv
+from om_code.runfitderiv import runfitderiv
 
-version = "0.9.85"
+version = "0.9.9"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
@@ -124,16 +123,17 @@
         anames: string or list of strings, optional
             The name of file containing the corresponding annotation or a list
             of file names.
         wdir: string, optional
             The working directory where the data files are stored and where
             output will be saved.
         platereadertype: string
-            The type of plate reader, currently either 'Tecan' or 'Sunrise' or
-            'old Tecan'.
+            The type of plate reader, currently either "Tecan" or "tidy" for
+            data parsed into a tsv file of columns, with headings "time",
+            "well", "OD", "GFP", and any other measurements taken.
         dsheetnumbers: integer or list of integers, optional
             The relevant sheets of the Excel files storing the data.
         asheetnumbers: integer or list of integers, optional
             The relevant sheets of the corresponding Excel files for the
             annotation.
         info: boolean
             If True (default), display summary information on the data once
@@ -278,16 +278,15 @@
         dnames: string or list of strings, optional
             The name of the file containing the data from the plate reader
             or a list of file names.
         anames: string or list of strings, optional
             The name of file containing the corresponding annotation or a list
             of file names.
         platereadertype: string
-            The type of plate reader, currently either 'Tecan' or 'Sunrise' or
-            'old Tecan'.
+            The type of plate reader, currently either 'Tecan' or 'tidy'.
         dsheetnumbers: integer or list of integers, optional
             The relevant sheets of the Excel files storing the data.
         asheetnumbers: integer or list of integers, optional
             The relevant sheets of the corresponding Excel files for the
             annotation.
         info: boolean
             If True (default), display summary information on the data once
@@ -316,15 +315,15 @@
             (
                 rdf,
                 allconditionssingle,
                 allstrainssingle,
                 alldatasingle,
                 experiment,
                 datatypes,
-            ) = loadplatedata.loadfromplate(
+            ) = loaddata.loaddatafiles(
                 platereadertype,
                 self.wdirpath,
                 dname,
                 dsheetnumbers[i],
                 anames[i],
                 asheetnumbers[i],
             )
@@ -339,15 +338,14 @@
                 else rdf
             )
             # update progress dictionary
             admin.initialiseprogress(self, experiment)
 
         # dataframe for summary stats and corrections
         alldfs = []
-        # for exp in self.allexperiments:
         for exp in alldata:
             strs, cons = [], []
             for cs in alldata[exp]:
                 strs.append(cs.split(" in ")[0])
                 cons.append(cs.split(" in ")[1])
             corrdict = {
                 "experiment": exp,
@@ -815,14 +813,15 @@
     def addcommonvar(
         self,
         var="time",
         dvar=None,
         varmin=None,
         varmax=None,
         figs=True,
+        silent=False,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
         conditions="all",
         conditionincludes=False,
         conditionexcludes=False,
         strains="all",
@@ -870,14 +869,16 @@
         varmin: float, optional
             The minimum of the common variable.
         varmax: float, optional
             The maximum of the common variable.
         figs: boolean
             If True, generate plot to check if the variable and the common
             variable generated from it are sufficiently close in value.
+        silent: boolean
+            If True, stop all text output.
         experiments: string or list of strings
             The experiments to include.
         conditions: string or list of strings
             The conditions to include.
         strains: string or list of strings
             The strains to include.
         experimentincludes: string, optional
@@ -915,47 +916,46 @@
             conditionincludes,
             conditionexcludes,
             strains,
             strainincludes,
             strainexcludes,
             nonull=True,
         )
-        print(f"Finding common {var}.")
+        if not silent:
+            print(f"Finding common {var}.")
         for df in [self.r, self.s]:
             if var in df:
                 loc = (
                     df.experiment.isin(exps)
                     & df.condition.isin(cons)
                     & df.strain.isin(strs)
                 )
-                print("r dataframe") if df.equals(self.r) else print(
-                    "s dataframe"
-                )
+                if not silent:
+                    print("r dataframe") if df.equals(self.r) else print(
+                        "s dataframe"
+                    )
                 if dvar is None:
                     # calculated for tidy printing
                     elen = np.max([len(e) for e in exps]) + 5
                     # find median increment in var
-                    for e in exps:
-                        evar = df[loc][var].to_numpy()
-                        print(
-                            " {:{}} {}_min= {:.2e} ; d{}= {:.2e}".format(
-                                e,
-                                elen,
-                                var,
-                                np.min(evar),
-                                var,
-                                np.median(np.diff(evar)),
+                    if not silent:
+                        for e in df[loc].experiment.unique():
+                            evar = df[loc][var].to_numpy()
+                            print(
+                                f" {e:{elen}} {var}_min = {np.min(evar):2e}"
+                                f" ; d{var} = {np.median(np.diff(evar)):2e}"
                             )
-                        )
                     ldvar = np.median(np.diff(df[loc][var].to_numpy()))
                 else:
                     ldvar = dvar
-                print(f" Using d{var}= {ldvar:.2e}")
+                if not silent:
+                    print(f" Using d{var}= {ldvar:.2e}")
                 lvarmin = df[loc][var].min() if varmin is None else varmin
-                print(f" Using {var}_min= {lvarmin:.2e}\n")
+                if not silent:
+                    print(f" Using {var}_min= {lvarmin:.2e}\n")
                 lvarmax = df[loc][var].max() if varmax is None else varmax
                 # define common var
                 cvar = np.arange(lvarmin, lvarmax, ldvar)
                 df.loc[loc, "common" + var] = df[loc][var].apply(
                     lambda x: cvar[np.argmin((x - cvar) ** 2)]
                 )
                 if figs:
@@ -1838,16 +1838,14 @@
         empirical_errors=False,
         noruns=10,
         exitearly=True,
         noinits=100,
         nosamples=100,
         logs=True,
         iskip=False,
-        stats=True,
-        printstats=False,
         figs=True,
         findareas=False,
         plotlocalmax=True,
         showpeakproperties=False,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
@@ -1856,21 +1854,21 @@
         conditionexcludes=False,
         strains="all",
         strainincludes=False,
         strainexcludes=False,
         **kwargs,
     ):
         """
-        Estimate first and second time derivatives.
+        Smooth data, find its derivatives, and calculate summary statistics.
 
-        The derivatives are found, typically of OD, using a Gaussian process
-        (Swain et al., 2016), as well as corresponding summary statistics.
+        The first and second time derivatives are found, typically of OD,
+        using a Gaussian process (Swain et al., 2016).
 
-        The derivatives are stored in the .s dataframe; summary statistics are
-        stored in the .sc dataframe.
+        The derivatives are stored in the .s dataframe;
+        summary statistics are stored in the .sc dataframe.
 
         Parameters
         ----------
         dtype: string, optional
             The type of data - 'OD', 'GFP', 'c-GFPperOD', or 'c-GFP' - for
             which the derivatives are to be found. The data must exist in the
             .r or .s dataframes.
@@ -1906,18 +1904,14 @@
             The number of samples used to calculate errors in statistics by
             bootstrapping.
         logs: boolean, optional
             If True, find the derivative of the log of the data and should be
             True to determine the specific growth rate when dtype= 'OD'.
         iskip: integer, optional
             Use only every iskip'th data point to increase speed.
-        stats: boolean, optional
-            If True, calculate summary statistics.
-        printstats: boolean, optional
-            If True, print summary statistics.
         figs: boolean, optional
             If True, plot both the fits and inferred derivative.
         findareas: boolean, optional
             If True, find the area under the plot of gr vs OD and the area
             under the plot of OD vs time. Setting to True can make getstats
             slow.
         plotlocalmax: boolean, optional
@@ -1970,36 +1964,24 @@
         ----------
         PS Swain, K Stevenson, A Leary, LF Montano-Gutierrez, IB Clark,
         J Vogel, T Pilizota. (2016). Inferring time derivatives including cell
         growth rates using Gaussian processes. Nat Commun, 7, 1-8.
         """
         linalgmax = 5
         warnings = ""
-        if dtype == "OD" and logs:
-            derivname = "gr"
-        else:
-            derivname = "d/dt_" + dtype
-        snames = [
-            "min_" + dtype,
-            "max_" + dtype,
-            "max_" + derivname,
-            "time_of_max_" + derivname,
-        ]
-        if dtype == "OD" and logs:
-            # special names with estimating specific growth rate
-            snames += ["doubling_time", "lag_time"]
-        else:
-            snames += [
-                "doubling_time_from-" + derivname,
-                "lag_time_from_" + derivname,
-            ]
+        # variable to be fit
         if logs:
-            ylabels = ["log(" + dtype + ")", derivname]
+            fitvar = f"log_{dtype}"
+        else:
+            fitvar = dtype
+        # name of derivative of fit variable
+        if fitvar == "log_OD":
+            derivname = "gr"
         else:
-            ylabels = [dtype, derivname]
+            derivname = f"d/dt_{fitvar}"
         # extract data
         exps, cons, strs = sunder.getall(
             self,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
@@ -2009,15 +1991,15 @@
             strainincludes,
             strainexcludes,
         )
         # find growth rate and stats
         for e in exps:
             for c in cons:
                 for s in strs:
-                    figtitle = e + ": " + s + " in " + c
+                    esc_name = f"{e}: {s} in {c}"
                     if dtype in self.r.columns:
                         # raw data
                         d = sunder.extractwells(self.r, self.s, e, c, s, dtype)
                         t = self.s.query(
                             "experiment == @e and condition == @c and "
                             "strain == @s"
                         )["time"].to_numpy()
@@ -2037,102 +2019,51 @@
                         # convert to array for fitderiv
                         d = piv_df.values
                         t = piv_df.index.to_numpy()
                         numberofnans = np.count_nonzero(np.isnan(d))
                         if np.any(numberofnans):
                             print(f"\nWarning: {numberofnans} NaNs in data")
                     else:
-                        print(f"\n-> {dtype} not recognised for {figtitle}.\n")
+                        print(f"\n-> {dtype} not recognised for {esc_name}.\n")
                         return
                     # checks
                     if d.size == 0:
                         # no data
                         print(
-                            f"\n-> No data found for {dtype} for {figtitle}.\m"
+                            f"\n-> No data found for {dtype} for {esc_name}.\m"
                         )
                         continue
-                    if logs:
-                        print(f"\nFitting log({dtype}) for {figtitle}.")
-                    else:
-                        print(f"\nFitting {dtype} for {figtitle}.")
-                    # call fitderiv
-                    f = fitderiv(
+                    # run fit
+                    _, warning = runfitderiv(
+                        self,
                         t,
                         d,
-                        cvfn=cvfn,
-                        logs=logs,
-                        bd=bd,
-                        empirical_errors=empirical_errors,
-                        statnames=snames,
-                        printstats=printstats,
-                        noruns=noruns,
-                        noinits=noinits,
-                        exitearly=exitearly,
-                        linalgmax=linalgmax,
-                        nosamples=nosamples,
-                        iskip=iskip,
+                        fitvar,
+                        derivname,
+                        e,
+                        c,
+                        s,
+                        bd,
+                        cvfn,
+                        empirical_errors,
+                        noruns,
+                        exitearly,
+                        noinits,
+                        nosamples,
+                        logs,
+                        iskip,
+                        figs,
+                        findareas,
+                        plotlocalmax,
+                        showpeakproperties,
+                        linalgmax,
+                        **kwargs,
                     )
-                    if f.success:
-                        if figs:
-                            plt.figure()
-                            plt.subplot(2, 1, 1)
-                            f.plotfit(
-                                "f", ylabel=ylabels[0], figtitle=figtitle
-                            )
-                            axgr = plt.subplot(2, 1, 2)
-                            f.plotfit("df", ylabel=ylabels[1])
-                            plt.tight_layout()
-                        else:
-                            axgr = None
-                        # find summary statistics
-                        outdf, statsdict, warning = omstats.findsummarystats(
-                            dtype,
-                            derivname,
-                            logs,
-                            nosamples,
-                            f,
-                            t,
-                            e,
-                            c,
-                            s,
-                            findareas,
-                            figs,
-                            plotlocalmax,
-                            axgr,
-                            showpeakproperties,
-                            **kwargs,
-                        )
-                        if warning:
-                            warnings += warning
-                        # store results in the dataframes
-                        statsdict[
-                            "logmaxlikehood_for_" + derivname
-                        ] = f.logmaxlike
-                        statsdict["gp_for_" + derivname] = cvfn
-                        for j, val in enumerate(f.lth):
-                            statsdict[
-                                "log_hyperparameter_"
-                                + str(j)
-                                + "_for_"
-                                + derivname
-                            ] = val
-                        # add time series to s dataframe
-                        admin.add_to_s(self, derivname, outdf)
-                        if stats:
-                            # add stats calculated by omfitderiv
-                            for sname in f.ds.keys():
-                                statsdict[sname] = f.ds[sname]
-                        # create or add summary stats to sc dataframe
-                        statsdf = pd.DataFrame(
-                            statsdict, index=pd.RangeIndex(0, 1, 1)
-                        )
-                        admin.add_to_sc(self, statsdf)
-                        if figs:
-                            plt.show(block=False)
-        omstats.cleansc(self)
+                    if warning:
+                        warnings += warning
         if warnings:
             print(warnings)
 
     @clogger.log
     def averageoverexpts(
         self,
         condition,
@@ -2217,15 +2148,15 @@
         self,
         f=["GFP", "AutoFL"],
         refstrain="WT",
         figs=True,
         useGPs=True,
         flcvfn="matern",
         bd=None,
-        nosamples=500,
+        nosamples=1000,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
         conditions="all",
         conditionincludes=False,
         conditionexcludes=False,
         strains="all",
@@ -2463,54 +2394,57 @@
         else:
             fnamepath = self.wdirpath / ("".join(self.allexperiments) + ".log")
         with fnamepath.open("w") as f:
             f.write(self.logstream.getvalue())
         print("Exported successfully.")
 
     @clogger.log
-    def exportdf(self, commonname=False, type="tsv"):
+    def exportdf(self, fname=False, type="tsv", ldirec=False):
         """
         Export the dataframes.
 
         The exported data may either be tab-delimited or csv or json files.
         Dataframes for the (processed) raw data, for summary data, and for
         summary statistics and corrections, as well as a log file, are
         exported.
 
         Parameters
         ----------
-        commonname: string, optional
+        fname: string, optional
             The name used for the output files.
             If unspecified, the experiment or experiments is used.
         type: string
             The type of file for export, either 'json' or 'csv' or 'tsv'.
+        ldirec: string, optional
+            The directory to write. If False, the working directory is used.
 
         Examples
         --------
         >>> p.exportdf()
         >>> p.exportdf('processed', type= 'json')
         """
-        if commonname:
-            fullcommonname = str(self.wdirpath / commonname)
+        if not fname:
+            fname = "".join(self.allexperiments)
+        if ldirec:
+            ldirec = Path(ldirec)
+            fullfname = str(ldirec / fname)
         else:
-            fullcommonname = str(self.wdirpath / "".join(self.allexperiments))
+            fullfname = str(self.wdirpath / fname)
         # export data
         if type == "json":
-            self.r.to_json(fullcommonname + "_r.json", orient="split")
-            self.s.to_json(fullcommonname + "_s.json", orient="split")
-            self.sc.to_json(fullcommonname + "_sc.json", orient="split")
+            self.r.to_json(fullfname + "_r.json", orient="split")
+            self.s.to_json(fullfname + "_s.json", orient="split")
+            self.sc.to_json(fullfname + "_sc.json", orient="split")
         else:
             sep = "\t" if type == "tsv" else ","
-            self.r.to_csv(fullcommonname + "_r." + type, sep=sep, index=False)
-            self.s.to_csv(fullcommonname + "_s." + type, sep=sep, index=False)
-            self.sc.to_csv(
-                fullcommonname + "_sc." + type, sep=sep, index=False
-            )
+            self.r.to_csv(fullfname + "_r." + type, sep=sep, index=False)
+            self.s.to_csv(fullfname + "_s." + type, sep=sep, index=False)
+            self.sc.to_csv(fullfname + "_sc." + type, sep=sep, index=False)
         # export log to file
-        self.savelog(commonname)
+        self.savelog(fname)
 
     @clogger.log
     def importdf(self, commonnames, info=True, sep="\t"):
         """
         Import dataframes saved as either json or csv or tsv files.
 
         Parameters
@@ -2612,16 +2546,19 @@
                 "\nLikely ERROR: data with the same experiment, condition, "
                 "strain, and time now appears twice!!"
             )
 
     @clogger.log
     def getmidlog(
         self,
-        stat="mean",
+        stats=["mean", "median", "min", "max"],
         min_duration=1,
+        max_num=4,
+        prior=[-5, 5],
+        use_smoothed=False,
         figs=True,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
         conditions="all",
         conditionincludes=False,
         conditionexcludes=False,
@@ -2636,25 +2573,34 @@
         Find the region of mid-log growth using nunchakue and calculate a
         statistic for each variable in the s dataframe in this region only.
 
         The results are added to the sc dataframe.
 
         Parameters
         ----------
-        stat: str
-            The name of the statistic to be calculated (using pandas).
-        min_duration: float
+        stats: str, optional
+            A list of statistics to be calculated (using pandas).
+        min_duration: float, optional
             The expected minimal duration of the midlog phase in units of time.
-        figs: boolean
-            If True, show nunchaku's results with the mid-log region marked by black squares.
-        experiments: string or list of strings
+        max_num: int, optional
+            The maximum number of segments of a growth curve.
+        prior: list of two floats, optional
+            Prior for nunchaku giving the lower and upper bounds on the gradients of the line segments.
+        use_smoothed: boolean, optional
+            If True, use the smoothed OD found by getstats and its estimated
+            errors.
+            If False, use the OD of the replicates in different wells.
+        figs: boolean, optional
+            If True, show nunchaku's results with the mid-log region marked by
+            black squares.
+        experiments: string or list of strings, optional
             The experiments to include.
-        conditions: string or list of strings
+        conditions: string or list of strings, optional
             The conditions to include.
-        strains: string or list of strings
+        strains: string or list of strings, optional
             The strains to include.
         experimentincludes: string, optional
             Selects only experiments that include the specified string in
             their name.
         experimentexcludes: string, optional
             Ignores experiments that include the specified string in their
             name.
@@ -2682,15 +2628,25 @@
             strainincludes,
             strainexcludes,
             nonull=True,
             nomedia=True,
         )
         # run Nunchaku to find midlog and take the mean of summary stats
         midlog.find_midlog_stats(
-            self, stat, min_duration, figs, exps, cons, strs
+            self,
+            stats,
+            min_duration,
+            max_num,
+            prior,
+            use_smoothed,
+            figs,
+            exps,
+            cons,
+            strs,
+            **kwargs,
         )
 
     @property
     def cols_to_underscore(self):
         """Replace spaces in column names of all dataframes with underscores."""
         for df in [self.r, self.s, self.sc]:
             df.columns = df.columns.str.replace(" ", "_")
```

### Comparing `omniplate-0.9.85/pyproject.toml` & `omniplate-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.85"
+version = "0.9.9"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-0.9.85/setup.py` & `omniplate-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pandas>=1.5.1',
  'scipy>=1.10.1,<2.0.0',
  'seaborn>=0.11.2',
  'statsmodels>=0.13.1']
 
 setup_kwargs = {
     'name': 'omniplate',
-    'version': '0.9.85',
+    'version': '0.9.9',
     'description': 'For analysing and meta-analysing plate-reader data',
     'long_description': 'A Python package for analysing data from plate-reader studies of growing biological cells. Users can correct for autofluorescence, determine growth rates and the amount of fluorescence per cell, and simultaneously analyse multiple experiments.\n',
     'author': 'Peter Swain',
     'author_email': 'peter.swain@ed.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://swainlab.bio.ed.ac.uk/software/omniplate',
```

### Comparing `omniplate-0.9.85/PKG-INFO` & `omniplate-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.85
+Version: 0.9.9
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```

