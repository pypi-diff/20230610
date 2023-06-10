# Comparing `tmp/scipion-em-aretomo-3.6.5.tar.gz` & `tmp/scipion-em-aretomo-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-aretomo-3.6.5.tar", last modified: Thu May 11 11:19:38 2023, max compression
+gzip compressed data, was "scipion-em-aretomo-3.7.tar", last modified: Sat Jun 10 11:31:36 2023, max compression
```

## Comparing `scipion-em-aretomo-3.6.5.tar` & `scipion-em-aretomo-3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols/protocol_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/tests/test_protocols_aretomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.457180 scipion-em-aretomo-3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols/protocol_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/tests/test_protocols_aretomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 11:31:36.457180 scipion-em-aretomo-3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/setup.py
```

### Comparing `scipion-em-aretomo-3.6.5/CHANGES.txt` & `scipion-em-aretomo-3.7/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.7: initial streaming support (@albertmena)
 3.6.5: allow unsorted tilt series
 3.6.4: adding type hints
 3.6.3: reduce number of Set[item] calls
 3.6.2:
  - fix applyTransform in the convert step
  - add interpolated flag
 3.6.1:
```

### Comparing `scipion-em-aretomo-3.6.5/LICENSE` & `scipion-em-aretomo-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/PKG-INFO` & `scipion-em-aretomo-3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.5
+Version: 3.7
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.5/README.rst` & `scipion-em-aretomo-3.7/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/__init__.py` & `scipion-em-aretomo-3.7/aretomo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.6.5'
+__version__ = '3.7'
 _logo = "aretomo_logo.png"
 _references = ['Zheng2022']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = ARETOMO_HOME
     _pathVars = [ARETOMO_HOME, ARETOMO_CUDA_LIB]
```

### Comparing `scipion-em-aretomo-3.6.5/aretomo/bibtex.py` & `scipion-em-aretomo-3.7/aretomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/constants.py` & `scipion-em-aretomo-3.7/aretomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/convert.py` & `scipion-em-aretomo-3.7/aretomo/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/protocols/__init__.py` & `scipion-em-aretomo-3.7/aretomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/protocols/protocol_aretomo.py` & `scipion-em-aretomo-3.7/aretomo/protocols/protocol_aretomo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # **************************************************************************
 # *
 # * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk) [1]
 # *              Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [2]
+# *              Alberto Garcia Mena (alberto.garcia@cnb.csic.es [2]
 # *
 # * [1] MRC Laboratory of Molecular Biology (MRC-LMB)
 # * [2] Centro Nacional de Biotecnologia, CSIC, Spain
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
@@ -25,47 +26,53 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 from glob import glob
 import numpy as np
+import time
 from typing import List, Literal, Tuple, Union, Optional
 
-import pyworkflow.protocol.params as params
+from pyworkflow.protocol import params, STEPS_PARALLEL
 from pyworkflow.constants import BETA
 from pyworkflow.object import Set
+from pyworkflow.protocol import ProtStreamingBase
 import pyworkflow.utils as pwutils
 from pwem.protocols import EMProtocol
 from pwem.objects import Transform
 from pwem.emlib.image import ImageHandler
-
 from tomo.protocols import ProtTomoBase
 from tomo.objects import (Tomogram, TiltSeries, TiltImage,
                           SetOfTomograms, SetOfTiltSeries)
 
 from .. import Plugin
 from ..convert import getTransformationMatrix, readAlnFile
 from ..constants import *
 
-
 OUT_TS = "outputSetOfTiltSeries"
 OUT_TS_ALN = "outputInterpolatedSetOfTiltSeries"
 OUT_TOMO = "outputSetOfTomograms"
 
 
-class ProtAreTomoAlignRecon(EMProtocol, ProtTomoBase):
-    """ Protocol for fiducial-free alignment and reconstruction for tomography. """
+class ProtAreTomoAlignRecon(EMProtocol, ProtTomoBase, ProtStreamingBase):
+    """ Protocol for fiducial-free alignment and reconstruction for tomography available in streaming. """
     _label = 'tilt-series align and reconstruct'
     _devStatus = BETA
     _possibleOutputs = {OUT_TS: SetOfTiltSeries,
                         OUT_TS_ALN: SetOfTiltSeries,
                         OUT_TOMO: SetOfTomograms}
 
-    # --------------------------- DEFINE param functions ----------------------
+    def __init__(self, **args):
+        EMProtocol.__init__(self, **args)
+        self.stepsExecutionMode = STEPS_PARALLEL
+        self.TS_read = []
+        self.outputSOTSList_objID = []
+
+        # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         # Keep this for compatibility with older plugin versions
         form.addHidden('tiltAxisAngle', params.FloatParam,
                        default=0., label='Tilt axis angle',
                        help='Note that the orientation of tilt axis is '
                             'relative to the y-axis (vertical axis of '
                             'tilt image) and rotates counter-clockwise.\n'
@@ -110,15 +117,16 @@
                            "All other input alignment parameters will be ignored.")
 
         form.addParam('binFactor', params.IntParam,
                       default=2, label='Binning', important=True,
                       help='Binning for aligned output tilt-series / volume.')
 
         form.addParam('alignZ', params.IntParam, default=800,
-                      condition='not skipAlign and not useInputProt', important=True,
+                      condition='not skipAlign and not useInputProt',
+                      important=True,
                       label='Volume height for alignment (voxels)',
                       help='Specifies Z height (*unbinned*) of the temporary volume '
                            'reconstructed for projection matching as part '
                            'of the alignment process. This value plays '
                            'an important role in alignment accuracy. This '
                            'Z height should be always smaller than tomogram '
                            'thickness and should be close to the sample '
@@ -152,15 +160,15 @@
                                'Refine and calculate tilt axis at each tilt angle'],
                       display=params.EnumParam.DISPLAY_COMBO,
                       label="Refine tilt axis angle?", default=1,
                       help="Tilt axis determination is a two-step processing in AreTomo. "
                            "A single tilt axis is first calculated followed by the determination "
                            "of how tilt axis varies over the entire tilt range. The initial "
                            "value lets users enter their estimate and AreTomo refines the "
-                           "estimate in [-3°, 3°] range.")
+                           "estimate in [-3º, 3º] range.")
 
         form.addSection(label='Extra options')
         form.addParam('doDW', params.BooleanParam, default=False,
                       label="Do dose-weighting?")
         form.addParam('reconMethod', params.EnumParam,
                       choices=['SART', 'WBP'],
                       display=params.EnumParam.DISPLAY_HLIST,
@@ -188,47 +196,48 @@
                            "making a tilt-series. This way the output orientation "
                            "will be similar to IMOD.")
 
         form.addParam('roiArea', params.StringParam, default='',
                       condition="not useInputProt",
                       label="ROI for focused alignment",
                       help="By default AreTomo assumes the region of interest "
-                           "at the center of 0° projection image. A circular "
+                           "at the center of 0º projection image. A circular "
                            "mask is employed to down-weight the area outside "
                            "ROI during the alignment. When the structures of "
                            "interest are far away from the tilt axis, the "
                            "angular error in the determination of tilt axis "
                            "will significantly amplify the translational error. "
                            "ROI function can effectively improve the alignment "
                            "accuracy for the distant structures.\nHere you can "
                            "provide *a pair of x and y coordinates*, representing "
                            "the center of the region of interest.\n"
-                           "The region of interest should be selected from 0° "
+                           "The region of interest should be selected from 0º "
                            "projection image with the origin at the lower left "
                            "corner. IMOD's Pixel View is a good tool to select "
                            "the center of region of interest.")
 
         group = form.addGroup('Local motion correction')
         group.addParam('sampleType', params.EnumParam,
                        condition="not useInputProt",
-                       choices=['Disable local correction', 'Isolated', 'Well distributed'],
+                       choices=['Disable local correction', 'Isolated',
+                                'Well distributed'],
                        display=params.EnumParam.DISPLAY_COMBO,
                        label="Sample type", default=0,
                        help="AreTomo provides two means to correct the local "
                             "motion, one for isolated sample and the other "
                             "for well distributed across the field of view.")
 
         group.addParam('coordsFn', params.FileParam, default='',
                        label='Coordinate file',
                        condition='not useInputProt and sampleType==%d' % LOCAL_MOTION_COORDS,
                        help="A list of x and y coordinates should be put "
                             "into a two-column text file, one column for x "
                             "and the other for y. Each pair defines a region "
                             "of interest (ROI). The origin of the coordinate "
-                            "system is at the image’s lower left corner.")
+                            "system is at the image's lower left corner.")
 
         line = group.addLine("Patches",
                              condition='not useInputProt and sampleType==%d' % LOCAL_MOTION_PATCHES)
         line.addParam('patchX', params.IntParam, default=5,
                       label='X')
         line.addParam('patchY', params.IntParam, default=5,
                       label='Y')
@@ -244,26 +253,56 @@
                       expertLevel=params.LEVEL_ADVANCED,
                       label='Additional parameters',
                       help="Extra command line parameters. See AreTomo help.")
 
         form.addHidden(params.GPU_LIST, params.StringParam,
                        default='0', label="Choose GPU IDs")
 
+        form.addParallelSection(threads=3, mpi=1)
+
     # --------------------------- INSERT steps functions ----------------------
-    def _insertAllSteps(self):
-        for ts in self.inputSetOfTiltSeries.get():
-            args = (ts.getObjId(), ts.getTsId(),
-                    ts.getFirstItem().getFileName())
-            self._insertFunctionStep(self.convertInputStep, *args)
-            self._insertFunctionStep(self.runAreTomoStep, *args)
-            self._insertFunctionStep(self.createOutputStep, *args)
-        self._insertFunctionStep(self.closeOutputSetsStep)
+    def stepsGeneratorStep(self) -> None:
+        """
+        This step should be implemented by any streaming protocol.
+        It should check its input and when ready conditions are met
+        call the self._insertFunctionStep method.
+        """
+        self.readingOutput()
+        while True:
+            listTSInput = list(self._getSetOfTiltSeries().getIdSet())
+            if not self._getSetOfTiltSeries().isStreamOpen() and self.TS_read == listTSInput:
+                self.info('Input set closed, all items processed\n')
+                break
+            for ts in self._getSetOfTiltSeries():
+                if ts.getObjId() not in self.TS_read:
+                    self.info(f"TS_ID input: {listTSInput}\n"
+                              f"TS_ID reading... {ts.getObjId()}\n"
+                              f"TS_ID read: {self.TS_read}\n")
+                    self.TS_read.append(ts.getObjId())
+                    try:
+                        args = (ts.getObjId(), ts.getTsId(),
+                                ts.getFirstItem().getFileName())
+                        convertInput = self._insertFunctionStep(
+                            self.convertInputStep, *args, prerequisites=[])
+                        runAreTomo = self._insertFunctionStep(
+                            self.runAreTomoStep, *args,
+                            prerequisites=[convertInput])
+                        createOutputS = self._insertFunctionStep(self.createOutputStep, *args,
+                                                                 prerequisites=[runAreTomo])
+                        self._insertFunctionStep(self.closeOutputSetsStep,
+                                                 prerequisites=[createOutputS])
+                    except Exception as e:
+                        self.error(f'Error reading TS info: {e}')
+                        self.error(f'ts.getFirstItem(): {ts.getFirstItem()}')
+                time.sleep(10)
 
     # --------------------------- STEPS functions -----------------------------
     def convertInputStep(self, tsObjId: int, tsId: str, tsFn: str):
+        self.info(f'------- convertInputStep ts_id: {tsObjId}')
+
         ts = self._getSetOfTiltSeries()[tsObjId]
 
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
         pwutils.makePath(tmpPrefix)
         pwutils.makePath(extraPrefix)
 
@@ -276,25 +315,28 @@
         # Generate angle file
         angleFilePath = self.getFilePath(tsFn, tmpPrefix, ".tlt")
         self._generateTltFile(ts, angleFilePath)
 
         if self.useInputProt:
             # Find and copy aln file
             protExtra = self.inputProt.get()._getExtraPath(tsId)
-            protAlnBase = self.getFilePath(tsFn, protExtra, ".aln").replace("_even", "*").replace("_odd", "*")
+            protAlnBase = self.getFilePath(tsFn, protExtra, ".aln").replace(
+                "_even", "*").replace("_odd", "*")
             protAln = glob(protAlnBase)
             if protAln:
                 pwutils.copyFile(protAln[0],
                                  self.getFilePath(tsFn, extraPrefix, ".aln"))
                 self.info(f"Using input alignment: {protAln[0]}")
             else:
                 raise FileNotFoundError("Missing input aln file ", protAlnBase)
 
     def runAreTomoStep(self, tsObjId: int, tsId: str, tsFn: str):
         """ Call AreTomo with the appropriate parameters. """
+        self.info(f'------- runAreTomoStep ts_id: {tsObjId}')
+
         tsSet = self._getSetOfTiltSeries()
         ts = tsSet[tsObjId]
 
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
 
         args = {
@@ -346,20 +388,23 @@
         param = ' '.join([f'{k} {str(v)}' for k, v in args.items()])
         param += ' ' + self.extraParams.get()
         program = Plugin.getProgram()
 
         self.runJob(program, param, env=Plugin.getEnviron())
 
     def createOutputStep(self, tsObjId: int, tsId: str, tsFn: str):
+        self.info(f'------- createOutputStep ts_id: {tsObjId}')
+
         ts = self._getSetOfTiltSeries()[tsObjId]
         extraPrefix = self._getExtraPath(tsId)
 
         if not (self.makeTomo and self.skipAlign):
-            AretomoAln = readAlnFile(self.getFilePath(tsFn, extraPrefix, ".aln"),
-                                     newVersion=Plugin.versionGE("1.3.0"))
+            AretomoAln = readAlnFile(
+                self.getFilePath(tsFn, extraPrefix, ".aln"),
+                newVersion=Plugin.versionGE("1.3.0"))
             alignmentMatrix = getTransformationMatrix(AretomoAln.imod_matrix)
 
         if self.makeTomo:
             outputSetOfTomograms = self.getOutputSetOfTomograms()
             newTomogram = Tomogram()
             newTomogram.setLocation(self.getFilePath(tsFn, extraPrefix, ".mrc"))
 
@@ -444,16 +489,17 @@
                     acq = tiltImage.getAcquisition()
                     acq.setTiltAxisAngle(AretomoAln.tilt_axes[secIndex])
                     newTi.setAcquisition(acq)
                     newTi.setTiltAngle(AretomoAln.tilt_angles[secIndex])
 
                     # set Transform
                     m = alignmentMatrix[:, :, secIndex]
-                    self.debug(f"Section {secNum}: {AretomoAln.tilt_axes[secIndex]}, "
-                               f"{AretomoAln.tilt_angles[secIndex]}")
+                    self.debug(
+                        f"Section {secNum}: {AretomoAln.tilt_axes[secIndex]}, "
+                        f"{AretomoAln.tilt_angles[secIndex]}")
                     transform.setMatrix(m)
 
                 newTi.setTransform(transform)
                 newTi.setSamplingRate(self._getInputSampling())
                 newTs.append(newTi)
 
             # update tilt axis angle for TS with the first value only
@@ -496,39 +542,53 @@
 
         return summary
 
     def _methods(self) -> List[str]:
         methods = []
 
         return methods
-    
+
     def _validate(self) -> List[str]:
         errors = []
+        self._validateThreads(errors)
 
         if self.useInputProt:
             if not self.inputProt.hasValue():
                 errors.append("Provide input AreTomo protocol for alignment.")
             if not Plugin.versionGE(V1_1_1):
                 errors.append("Input alignment can be used only with AreTomo v1.1.1+")
         else:
-            if (not self.skipAlign) and self.makeTomo and (self.alignZ >= self.tomoThickness):
+            if (not self.skipAlign) and self.makeTomo and (
+                    self.alignZ >= self.tomoThickness):
                 errors.append("Z volume height for alignment should be always "
                               "smaller than tomogram thickness.")
 
         if self.skipAlign and not self.makeTomo:
             errors.append("You cannot switch off both alignment and "
                           "reconstruction.")
 
-        if self._getSetOfTiltSeries().hasAlignment() and not self.skipAlign:
-            errors.append("Input tilt-series already have alignment "
-                          "information. You probably want to skip alignment step.")
+        if self._getSetOfTiltSeries():
+            if self._getSetOfTiltSeries().hasAlignment() and not self.skipAlign:
+                errors.append("Input tilt-series already have alignment "
+                              "information. You probably want to skip alignment step.")
 
         return errors
-    
+
     # --------------------------- UTILS functions -----------------------------
+    def readingOutput(self) -> None:
+        try:
+            if self.outputSetOfTiltSeries:
+                for ts in self.outputSetOfTiltSeries:
+                    self.TS_read.append(ts.getObjId())
+            self.info(f'Tomograms calculated for this TS_ID : {self.TS_read}')
+            self.outputSOTSList_objID = self.TS_read
+
+        except AttributeError:  # There is no outputSetOfTiltSeries
+            pass
+
     def getFilePath(self,
                     tsFn: Union[str, os.PathLike],
                     prefix: str,
                     ext: Optional[str] = None) -> Union[str, os.PathLike]:
         fileName, fileExtension = os.path.splitext(os.path.basename(tsFn))
         if ext is not None:
             fileExtension = ext
```

### Comparing `scipion-em-aretomo-3.6.5/aretomo/protocols.conf` & `scipion-em-aretomo-3.7/aretomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/tests/__init__.py` & `scipion-em-aretomo-3.7/aretomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/aretomo/tests/test_protocols_aretomo.py` & `scipion-em-aretomo-3.7/aretomo/tests/test_protocols_aretomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/PKG-INFO` & `scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.5
+Version: 3.7
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/SOURCES.txt` & `scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.5/setup.py` & `scipion-em-aretomo-3.7/setup.py`

 * *Files identical despite different names*

