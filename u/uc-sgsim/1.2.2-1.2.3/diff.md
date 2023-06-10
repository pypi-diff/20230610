# Comparing `tmp/uc_sgsim-1.2.2.tar.gz` & `tmp/uc_sgsim-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_sgsim-1.2.2.tar", last modified: Thu Jun  1 11:23:58 2023, max compression
+gzip compressed data, was "uc_sgsim-1.2.3.tar", last modified: Sat Jun 10 03:08:25 2023, max compression
```

## Comparing `uc_sgsim-1.2.2.tar` & `uc_sgsim-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 11:23:58.067155 uc_sgsim-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/c_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84819 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    37032 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/cov_model/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/krige/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/random_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/sgsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:57.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim/c_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/c_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/c_core/uc_sgsim.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36944 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/c_core/uc_sgsim.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim/cov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/cov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/cov_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/cov_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim/krige/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/krige/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/krige/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/random_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/sgsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-10 03:08:15.000000 uc_sgsim-1.2.3/uc_sgsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:08:25.157746 uc_sgsim-1.2.3/uc_sgsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-06-10 03:08:25.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-10 03:08:25.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:08:25.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:08:24.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 03:08:25.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-10 03:08:25.000000 uc_sgsim-1.2.3/uc_sgsim.egg-info/top_level.txt
```

### Comparing `uc_sgsim-1.2.2/LICENSE.md` & `uc_sgsim-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/PKG-INFO` & `uc_sgsim-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: uc_sgsim
-Version: 1.2.2
+Version: 1.2.3
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
@@ -124,28 +128,28 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
-    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
+    sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
     sgsim_c.mean_plot('ALL')  # Plot mean
     sgsim_c.variance_plot()  # Plot variance
     sgsim_c.cdf_plot(x_location=10)  # CDF
     sgsim_c.hist_plot(x_location=10)  # Hist
     sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim_c.vario_plot()
+    sgsim.variogram_plot()
     # Save random_field and variogram
     sgsim_c.save_random_field('randomfields.csv', save_single=True)
     sgsim_c.save_variogram('variograms.csv', save_single=True)
 
     # show figure
     plt.show()
 ```
```

### Comparing `uc_sgsim-1.2.2/README.md` & `uc_sgsim-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,28 +107,28 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
-    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
+    sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
     sgsim_c.mean_plot('ALL')  # Plot mean
     sgsim_c.variance_plot()  # Plot variance
     sgsim_c.cdf_plot(x_location=10)  # CDF
     sgsim_c.hist_plot(x_location=10)  # Hist
     sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim_c.vario_plot()
+    sgsim.variogram_plot()
     # Save random_field and variogram
     sgsim_c.save_random_field('randomfields.csv', save_single=True)
     sgsim_c.save_variogram('variograms.csv', save_single=True)
 
     # show figure
     plt.show()
 ```
```

### Comparing `uc_sgsim-1.2.2/setup.cfg` & `uc_sgsim-1.2.3/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [metadata]
 name = uc_sgsim
-version = 1.2.2
+version = 1.2.3
 description = Random Field Generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Zncl2222/Stochastic_UC_SGSIM
 author = Zncl2222
 author_email = 3002shinning@gmail.com
 license = MIT
 license_file = LICENSE.md
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
+	Programming Language :: C
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 packages = 
 	uc_sgsim
 	uc_sgsim/cov_model
 	uc_sgsim/krige
```

### Comparing `uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.dll` & `uc_sgsim-1.2.3/uc_sgsim/c_core/uc_sgsim.dll`

 * *Files 2% similar despite different names*

#### objdump

```diff
@@ -5,20 +5,20 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Tue May 30 11:42:46 2023
+Time/Date		Tue Jun  6 11:53:43 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
-SizeOfCode		0000000000006c00
-SizeOfInitializedData	0000000000009a00
+SizeOfCode		0000000000006e00
+SizeOfInitializedData	0000000000009c00
 SizeOfUninitializedData	0000000000000c00
 AddressOfEntryPoint	0000000000001330
 BaseOfCode		0000000000001000
 ImageBase		00000000646c0000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	4
@@ -26,29 +26,29 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00019000
 SizeOfHeaders		00000600
-CheckSum		000231ee
+CheckSum		0002423e
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
-Entry 0 000000000000d000 00000674 Export Directory [.edata (or where ever we found it)]
+Entry 0 000000000000d000 0000068c Export Directory [.edata (or where ever we found it)]
 Entry 1 000000000000e000 00000720 Import Directory [parts of .idata]
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
-Entry 3 000000000000a000 000005b8 Exception Directory [.pdata]
+Entry 3 000000000000a000 000005c4 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 0000000000011000 00000064 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 00000000000091a0 00000028 Thread Storage Directory [.tls]
 Entry a 0000000000000000 00000000 Load Configuration Directory
@@ -124,25 +124,25 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x646cd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		6475e136
+Time/Date stamp 		647f1e47
 Major/Minor 			0/0
-Name 				000000000000d28a uc_sgsim.dll
+Name 				000000000000d294 uc_sgsim.dll
 Ordinal Base 			1
 Number in:
-	Export Address Table 		0000003d
-	[Name Pointer/Ordinal] Table	0000003d
+	Export Address Table 		0000003e
+	[Name Pointer/Ordinal] Table	0000003e
 Table Addresses
 	Export Address Table 		000000000000d028
-	Name Pointer Table 		000000000000d11c
-	Ordinal Table 			000000000000d210
+	Name Pointer Table 		000000000000d120
+	Ordinal Table 			000000000000d218
 
 Export Address Table -- Ordinal Base 1
 	[   0] +base[   1] 4329 Export RVA
 	[   1] +base[   2] 18e2 Export RVA
 	[   2] +base[   3] 1704 Export RVA
 	[   3] +base[   4] 13b0 Export RVA
 	[   4] +base[   5] 1543 Export RVA
@@ -170,42 +170,43 @@
 	[  26] +base[  27] 296e Export RVA
 	[  27] +base[  28] 292e Export RVA
 	[  28] +base[  29] 294c Export RVA
 	[  29] +base[  30] 2f24 Export RVA
 	[  30] +base[  31] 302e Export RVA
 	[  31] +base[  32] 2ec0 Export RVA
 	[  32] +base[  33] 4381 Export RVA
-	[  33] +base[  34] 38c7 Export RVA
-	[  34] +base[  35] 3a7b Export RVA
+	[  33] +base[  34] 38d0 Export RVA
+	[  34] +base[  35] 3a84 Export RVA
 	[  35] +base[  36] 325d Export RVA
 	[  36] +base[  37] 3f98 Export RVA
 	[  37] +base[  38] 3c1a Export RVA
 	[  38] +base[  39] 4490 Export RVA
 	[  39] +base[  40] 2aae Export RVA
 	[  40] +base[  41] 2d5e Export RVA
 	[  41] +base[  42] 2db2 Export RVA
 	[  42] +base[  43] 2caa Export RVA
 	[  43] +base[  44] 2cf4 Export RVA
 	[  44] +base[  45] 2c6d Export RVA
 	[  45] +base[  46] 2a30 Export RVA
 	[  46] +base[  47] 2e27 Export RVA
 	[  47] +base[  48] 4d0e Export RVA
 	[  48] +base[  49] 43dd Export RVA
-	[  49] +base[  50] 4dd5 Export RVA
-	[  50] +base[  51] 46d0 Export RVA
-	[  51] +base[  52] 3180 Export RVA
-	[  52] +base[  53] 3231 Export RVA
-	[  53] +base[  54] 451f Export RVA
-	[  54] +base[  55] 4780 Export RVA
-	[  55] +base[  56] 47e6 Export RVA
-	[  56] +base[  57] 4c0a Export RVA
-	[  57] +base[  58] 34b9 Export RVA
-	[  58] +base[  59] 4c90 Export RVA
-	[  59] +base[  60] 50b6 Export RVA
-	[  60] +base[  61] 4e40 Export RVA
+	[  49] +base[  50] 4e39 Export RVA
+	[  50] +base[  51] 4dd5 Export RVA
+	[  51] +base[  52] 46d0 Export RVA
+	[  52] +base[  53] 3180 Export RVA
+	[  53] +base[  54] 3231 Export RVA
+	[  54] +base[  55] 451f Export RVA
+	[  55] +base[  56] 4780 Export RVA
+	[  56] +base[  57] 47e6 Export RVA
+	[  57] +base[  58] 4c0a Export RVA
+	[  58] +base[  59] 34b9 Export RVA
+	[  59] +base[  60] 4c90 Export RVA
+	[  60] +base[  61] 5146 Export RVA
+	[  61] +base[  62] 4ed0 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] arange
 	[   1] c_array_max_double
 	[   2] c_array_max_float
 	[   3] c_array_max_int
 	[   4] c_array_max_long_long
@@ -249,26 +250,27 @@
 	[  42] mt19937_get_float
 	[  43] mt19937_get_float_range
 	[  44] mt19937_get_int32_range
 	[  45] mt19937_init
 	[  46] mt19937_random_normal
 	[  47] partition2d
 	[  48] pdist
-	[  49] quicksort2d
-	[  50] randompath
-	[  51] sampling_state_init
-	[  52] sampling_state_update
-	[  53] save_1darray
-	[  54] sgsim_init
-	[  55] sgsim_run
-	[  56] sgsim_t_free
-	[  57] simple_kriging
-	[  58] swaprows
-	[  59] variance
-	[  60] variogram
+	[  49] quickselect2d
+	[  50] quicksort2d
+	[  51] randompath
+	[  52] sampling_state_init
+	[  53] sampling_state_update
+	[  54] save_1darray
+	[  55] sgsim_init
+	[  56] sgsim_run
+	[  57] sgsim_t_free
+	[  58] simple_kriging
+	[  59] swaprows
+	[  60] variance
+	[  61] variogram
 
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
  00000000646ca000:	00000000646c1000 00000000646c100c 00000000646cb000
  00000000646ca00c:	00000000646c1010 00000000646c11ff 00000000646cb004
  00000000646ca018:	00000000646c1200 00000000646c132b 00000000646cb018
  00000000646ca024:	00000000646c1330 00000000646c137f 00000000646cb028
@@ -313,17 +315,17 @@
  00000000646ca1f8:	00000000646c2e27 00000000646c2eba 00000000646cb1d8
  00000000646ca204:	00000000646c2ec0 00000000646c2f24 00000000646cb1e8
  00000000646ca210:	00000000646c2f24 00000000646c302e 00000000646cb1f0
  00000000646ca21c:	00000000646c302e 00000000646c317d 00000000646cb1fc
  00000000646ca228:	00000000646c3180 00000000646c3231 00000000646cb208
  00000000646ca234:	00000000646c3231 00000000646c325d 00000000646cb214
  00000000646ca240:	00000000646c325d 00000000646c34b9 00000000646cb21c
- 00000000646ca24c:	00000000646c34b9 00000000646c38c7 00000000646cb228
- 00000000646ca258:	00000000646c38c7 00000000646c3a7b 00000000646cb238
- 00000000646ca264:	00000000646c3a7b 00000000646c3bc5 00000000646cb244
+ 00000000646ca24c:	00000000646c34b9 00000000646c38d0 00000000646cb228
+ 00000000646ca258:	00000000646c38d0 00000000646c3a84 00000000646cb238
+ 00000000646ca264:	00000000646c3a84 00000000646c3bce 00000000646cb244
  00000000646ca270:	00000000646c3bd0 00000000646c3c1a 00000000646cb250
  00000000646ca27c:	00000000646c3c1a 00000000646c3f98 00000000646cb25c
  00000000646ca288:	00000000646c3f98 00000000646c4329 00000000646cb26c
  00000000646ca294:	00000000646c4329 00000000646c4381 00000000646cb278
  00000000646ca2a0:	00000000646c4381 00000000646c43dd 00000000646cb284
  00000000646ca2ac:	00000000646c43dd 00000000646c4490 00000000646cb290
  00000000646ca2b8:	00000000646c4490 00000000646c451f 00000000646cb29c
@@ -332,68 +334,69 @@
  00000000646ca2dc:	00000000646c4780 00000000646c47e6 00000000646cb2c0
  00000000646ca2e8:	00000000646c47e6 00000000646c4c0a 00000000646cb2cc
  00000000646ca2f4:	00000000646c4c0a 00000000646c4c2d 00000000646cb2d8
  00000000646ca300:	00000000646c4c2d 00000000646c4c87 00000000646cb2e4
  00000000646ca30c:	00000000646c4c90 00000000646c4d0e 00000000646cb2f0
  00000000646ca318:	00000000646c4d0e 00000000646c4dd5 00000000646cb2fc
  00000000646ca324:	00000000646c4dd5 00000000646c4e39 00000000646cb308
- 00000000646ca330:	00000000646c4e40 00000000646c50b6 00000000646cb314
- 00000000646ca33c:	00000000646c50b6 00000000646c519e 00000000646cb324
- 00000000646ca348:	00000000646c51b0 00000000646c51e5 00000000646cb330
- 00000000646ca354:	00000000646c51f0 00000000646c5256 00000000646cb338
- 00000000646ca360:	00000000646c5260 00000000646c527f 00000000646cb344
- 00000000646ca36c:	00000000646c5280 00000000646c5356 00000000646cb348
- 00000000646ca378:	00000000646c5360 00000000646c5458 00000000646cb358
- 00000000646ca384:	00000000646c5460 00000000646c548f 00000000646cb368
- 00000000646ca390:	00000000646c5490 00000000646c5503 00000000646cb370
- 00000000646ca39c:	00000000646c5510 00000000646c5513 00000000646cb37c
- 00000000646ca3a8:	00000000646c5520 00000000646c5524 00000000646cb380
- 00000000646ca3b4:	00000000646c5530 00000000646c5534 00000000646cb384
- 00000000646ca3c0:	00000000646c5540 00000000646c570d 00000000646cb394
- 00000000646ca3cc:	00000000646c5710 00000000646c59cb 00000000646cb3a4
- 00000000646ca3d8:	00000000646c59d0 00000000646c5b70 00000000646cb3bc
- 00000000646ca3e4:	00000000646c5b70 00000000646c5c5c 00000000646cb3c4
- 00000000646ca3f0:	00000000646c5c60 00000000646c5e47 00000000646cb3d4
- 00000000646ca3fc:	00000000646c5e50 00000000646c5eba 00000000646cb3dc
- 00000000646ca408:	00000000646c5ec0 00000000646c5f3f 00000000646cb3ec
- 00000000646ca414:	00000000646c5f40 00000000646c5fe0 00000000646cb3fc
- 00000000646ca420:	00000000646c5fe0 00000000646c60ba 00000000646cb404
- 00000000646ca42c:	00000000646c60c0 00000000646c60de 00000000646cb40c
- 00000000646ca438:	00000000646c60e0 00000000646c60f2 00000000646cb410
- 00000000646ca444:	00000000646c6100 00000000646c6144 00000000646cb414
- 00000000646ca450:	00000000646c6150 00000000646c61dd 00000000646cb418
- 00000000646ca45c:	00000000646c61e0 00000000646c6254 00000000646cb424
- 00000000646ca468:	00000000646c6260 00000000646c629e 00000000646cb42c
- 00000000646ca474:	00000000646c62a0 00000000646c630f 00000000646cb434
- 00000000646ca480:	00000000646c6310 00000000646c6347 00000000646cb43c
- 00000000646ca48c:	00000000646c6350 00000000646c63e1 00000000646cb444
- 00000000646ca498:	00000000646c63f0 00000000646c6496 00000000646cb44c
- 00000000646ca4a4:	00000000646c64a0 00000000646c64a3 00000000646cb454
- 00000000646ca4b0:	00000000646c64f0 00000000646c64f6 00000000646cb458
- 00000000646ca4bc:	00000000646c6500 00000000646c6506 00000000646cb45c
- 00000000646ca4c8:	00000000646c6510 00000000646c6564 00000000646cb460
- 00000000646ca4d4:	00000000646c6570 00000000646c6696 00000000646cb464
- 00000000646ca4e0:	00000000646c66a0 00000000646c66a5 00000000646cb470
- 00000000646ca4ec:	00000000646c66b0 00000000646c6787 00000000646cb474
- 00000000646ca4f8:	00000000646c6790 00000000646c6884 00000000646cb478
- 00000000646ca504:	00000000646c68c0 00000000646c6aa4 00000000646cb484
- 00000000646ca510:	00000000646c6ab0 00000000646c6bd0 00000000646cb490
- 00000000646ca51c:	00000000646c6bd0 00000000646c6c66 00000000646cb49c
- 00000000646ca528:	00000000646c6c70 00000000646c71c7 00000000646cb4a4
- 00000000646ca534:	00000000646c71d0 00000000646c744e 00000000646cb4c0
- 00000000646ca540:	00000000646c7520 00000000646c75de 00000000646cb4cc
- 00000000646ca54c:	00000000646c7700 00000000646c7725 00000000646cb4d4
- 00000000646ca558:	00000000646c7730 00000000646c77f8 00000000646cb4d8
- 00000000646ca564:	00000000646c7800 00000000646c786f 00000000646cb4e8
- 00000000646ca570:	00000000646c7870 00000000646c788f 00000000646cb4f4
- 00000000646ca57c:	00000000646c7960 00000000646c79a1 00000000646cb4fc
- 00000000646ca588:	00000000646c79b0 00000000646c79bc 00000000646cb504
- 00000000646ca594:	00000000646c79c0 00000000646c7abc 00000000646cb508
- 00000000646ca5a0:	00000000646c7ad0 00000000646c7b39 00000000646cb388
- 00000000646ca5ac:	00000000646c7b40 00000000646c7b45 00000000646cb520
+ 00000000646ca330:	00000000646c4e39 00000000646c4ec4 00000000646cb314
+ 00000000646ca33c:	00000000646c4ed0 00000000646c5146 00000000646cb320
+ 00000000646ca348:	00000000646c5146 00000000646c522e 00000000646cb330
+ 00000000646ca354:	00000000646c5240 00000000646c5275 00000000646cb33c
+ 00000000646ca360:	00000000646c5280 00000000646c52e6 00000000646cb344
+ 00000000646ca36c:	00000000646c52f0 00000000646c530f 00000000646cb350
+ 00000000646ca378:	00000000646c5310 00000000646c53e6 00000000646cb354
+ 00000000646ca384:	00000000646c53f0 00000000646c54e8 00000000646cb364
+ 00000000646ca390:	00000000646c54f0 00000000646c551f 00000000646cb374
+ 00000000646ca39c:	00000000646c5520 00000000646c5593 00000000646cb37c
+ 00000000646ca3a8:	00000000646c55a0 00000000646c55a3 00000000646cb388
+ 00000000646ca3b4:	00000000646c55b0 00000000646c55b4 00000000646cb38c
+ 00000000646ca3c0:	00000000646c55c0 00000000646c55c4 00000000646cb390
+ 00000000646ca3cc:	00000000646c55d0 00000000646c579d 00000000646cb3a0
+ 00000000646ca3d8:	00000000646c57a0 00000000646c5a5b 00000000646cb3b0
+ 00000000646ca3e4:	00000000646c5a60 00000000646c5c00 00000000646cb3c8
+ 00000000646ca3f0:	00000000646c5c00 00000000646c5cec 00000000646cb3d0
+ 00000000646ca3fc:	00000000646c5cf0 00000000646c5ed7 00000000646cb3e0
+ 00000000646ca408:	00000000646c5ee0 00000000646c5f4a 00000000646cb3e8
+ 00000000646ca414:	00000000646c5f50 00000000646c5fcf 00000000646cb3f8
+ 00000000646ca420:	00000000646c5fd0 00000000646c6070 00000000646cb408
+ 00000000646ca42c:	00000000646c6070 00000000646c614a 00000000646cb410
+ 00000000646ca438:	00000000646c6150 00000000646c616e 00000000646cb418
+ 00000000646ca444:	00000000646c6170 00000000646c6182 00000000646cb41c
+ 00000000646ca450:	00000000646c6190 00000000646c61d4 00000000646cb420
+ 00000000646ca45c:	00000000646c61e0 00000000646c626d 00000000646cb424
+ 00000000646ca468:	00000000646c6270 00000000646c62e4 00000000646cb430
+ 00000000646ca474:	00000000646c62f0 00000000646c632e 00000000646cb438
+ 00000000646ca480:	00000000646c6330 00000000646c639f 00000000646cb440
+ 00000000646ca48c:	00000000646c63a0 00000000646c63d7 00000000646cb448
+ 00000000646ca498:	00000000646c63e0 00000000646c6471 00000000646cb450
+ 00000000646ca4a4:	00000000646c6480 00000000646c6526 00000000646cb458
+ 00000000646ca4b0:	00000000646c6530 00000000646c6533 00000000646cb460
+ 00000000646ca4bc:	00000000646c6580 00000000646c6586 00000000646cb464
+ 00000000646ca4c8:	00000000646c6590 00000000646c6596 00000000646cb468
+ 00000000646ca4d4:	00000000646c65a0 00000000646c65f4 00000000646cb46c
+ 00000000646ca4e0:	00000000646c6600 00000000646c6726 00000000646cb470
+ 00000000646ca4ec:	00000000646c6730 00000000646c6735 00000000646cb47c
+ 00000000646ca4f8:	00000000646c6740 00000000646c6817 00000000646cb480
+ 00000000646ca504:	00000000646c6820 00000000646c6914 00000000646cb484
+ 00000000646ca510:	00000000646c6950 00000000646c6b34 00000000646cb490
+ 00000000646ca51c:	00000000646c6b40 00000000646c6c60 00000000646cb49c
+ 00000000646ca528:	00000000646c6c60 00000000646c6cf6 00000000646cb4a8
+ 00000000646ca534:	00000000646c6d00 00000000646c7257 00000000646cb4b0
+ 00000000646ca540:	00000000646c7260 00000000646c74de 00000000646cb4cc
+ 00000000646ca54c:	00000000646c75b0 00000000646c766e 00000000646cb4d8
+ 00000000646ca558:	00000000646c7790 00000000646c77b5 00000000646cb4e0
+ 00000000646ca564:	00000000646c77c0 00000000646c7888 00000000646cb4e4
+ 00000000646ca570:	00000000646c7890 00000000646c78ff 00000000646cb4f4
+ 00000000646ca57c:	00000000646c7900 00000000646c791f 00000000646cb500
+ 00000000646ca588:	00000000646c79f0 00000000646c7a31 00000000646cb508
+ 00000000646ca594:	00000000646c7a40 00000000646c7a4c 00000000646cb510
+ 00000000646ca5a0:	00000000646c7a50 00000000646c7b4c 00000000646cb514
+ 00000000646ca5ac:	00000000646c7b60 00000000646c7bc9 00000000646cb394
+ 00000000646ca5b8:	00000000646c7bd0 00000000646c7bd5 00000000646cb52c
 
 Dump of .xdata
  00000000646cb000 (rva: 0000b000): 00000000646c1000 - 00000000646c100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000000646cb004 (rva: 0000b004): 00000000646c1010 - 00000000646c11ff
 	Version: 1, Flags: none
@@ -673,28 +676,28 @@
  00000000646cb21c (rva: 0000b21c): 00000000646c325d - 00000000646c34b9
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0e, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x0e: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb228 (rva: 0000b228): 00000000646c34b9 - 00000000646c38c7
+ 00000000646cb228 (rva: 0000b228): 00000000646c34b9 - 00000000646c38d0
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0c: save xmm6 at rsp + 0x30
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb238 (rva: 0000b238): 00000000646c38c7 - 00000000646c3a7b
+ 00000000646cb238 (rva: 0000b238): 00000000646c38d0 - 00000000646c3a84
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb244 (rva: 0000b244): 00000000646c3a7b - 00000000646c3bc5
+ 00000000646cb244 (rva: 0000b244): 00000000646c3a84 - 00000000646c3bce
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
  00000000646cb250 (rva: 0000b250): 00000000646c3bd0 - 00000000646c3c1a
 	Version: 1, Flags: none
@@ -789,303 +792,309 @@
 	  pc+0x01: push rbp
  00000000646cb308 (rva: 0000b308): 00000000646c4dd5 - 00000000646c4e39
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb314 (rva: 0000b314): 00000000646c4e40 - 00000000646c50b6
+ 00000000646cb314 (rva: 0000b314): 00000000646c4e39 - 00000000646c4ec4
+	Version: 1, Flags: none
+	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
+	  pc+0x08: alloc small area: rsp = rsp - 0x30
+	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
+	  pc+0x01: push rbp
+ 00000000646cb320 (rva: 0000b320): 00000000646c4ed0 - 00000000646c5146
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x11: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x09: alloc large area: rsp = rsp - 0xb8
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb324 (rva: 0000b324): 00000000646c50b6 - 00000000646c519e
+ 00000000646cb330 (rva: 0000b330): 00000000646c5146 - 00000000646c522e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb330 (rva: 0000b330): 00000000646c51b0 - 00000000646c51e5
+ 00000000646cb33c (rva: 0000b33c): 00000000646c5240 - 00000000646c5275
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb338 (rva: 0000b338): 00000000646c51f0 - 00000000646c5256
+ 00000000646cb344 (rva: 0000b344): 00000000646c5280 - 00000000646c52e6
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb344 (rva: 0000b344): 00000000646c5260 - 00000000646c527f
+ 00000000646cb350 (rva: 0000b350): 00000000646c52f0 - 00000000646c530f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb348 (rva: 0000b348): 00000000646c5280 - 00000000646c5356
+ 00000000646cb354 (rva: 0000b354): 00000000646c5310 - 00000000646c53e6
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb358 (rva: 0000b358): 00000000646c5360 - 00000000646c5458
+ 00000000646cb364 (rva: 0000b364): 00000000646c53f0 - 00000000646c54e8
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0a: alloc small area: rsp = rsp - 0x70
 	  pc+0x06: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
- 00000000646cb368 (rva: 0000b368): 00000000646c5460 - 00000000646c548f
+ 00000000646cb374 (rva: 0000b374): 00000000646c54f0 - 00000000646c551f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb370 (rva: 0000b370): 00000000646c5490 - 00000000646c5503
+ 00000000646cb37c (rva: 0000b37c): 00000000646c5520 - 00000000646c5593
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb37c (rva: 0000b37c): 00000000646c5510 - 00000000646c5513
+ 00000000646cb388 (rva: 0000b388): 00000000646c55a0 - 00000000646c55a3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb380 (rva: 0000b380): 00000000646c5520 - 00000000646c5524
+ 00000000646cb38c (rva: 0000b38c): 00000000646c55b0 - 00000000646c55b4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb384 (rva: 0000b384): 00000000646c5530 - 00000000646c5534
+ 00000000646cb390 (rva: 0000b390): 00000000646c55c0 - 00000000646c55c4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb394 (rva: 0000b394): 00000000646c5540 - 00000000646c570d
+ 00000000646cb3a0 (rva: 0000b3a0): 00000000646c55d0 - 00000000646c579d
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x50
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3a4 (rva: 0000b3a4): 00000000646c5710 - 00000000646c59cb
+ 00000000646cb3b0 (rva: 0000b3b0): 00000000646c57a0 - 00000000646c5a5b
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000000646cb3bc (rva: 0000b3bc): 00000000646c59d0 - 00000000646c5b70
+ 00000000646cb3c8 (rva: 0000b3c8): 00000000646c5a60 - 00000000646c5c00
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb3c4 (rva: 0000b3c4): 00000000646c5b70 - 00000000646c5c5c
+ 00000000646cb3d0 (rva: 0000b3d0): 00000000646c5c00 - 00000000646c5cec
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3d4 (rva: 0000b3d4): 00000000646c5c60 - 00000000646c5e47
+ 00000000646cb3e0 (rva: 0000b3e0): 00000000646c5cf0 - 00000000646c5ed7
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3dc (rva: 0000b3dc): 00000000646c5e50 - 00000000646c5eba
+ 00000000646cb3e8 (rva: 0000b3e8): 00000000646c5ee0 - 00000000646c5f4a
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3ec (rva: 0000b3ec): 00000000646c5ec0 - 00000000646c5f3f
+ 00000000646cb3f8 (rva: 0000b3f8): 00000000646c5f50 - 00000000646c5fcf
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3fc (rva: 0000b3fc): 00000000646c5f40 - 00000000646c5fe0
+ 00000000646cb408 (rva: 0000b408): 00000000646c5fd0 - 00000000646c6070
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb404 (rva: 0000b404): 00000000646c5fe0 - 00000000646c60ba
+ 00000000646cb410 (rva: 0000b410): 00000000646c6070 - 00000000646c614a
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb40c (rva: 0000b40c): 00000000646c60c0 - 00000000646c60de
+ 00000000646cb418 (rva: 0000b418): 00000000646c6150 - 00000000646c616e
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb410 (rva: 0000b410): 00000000646c60e0 - 00000000646c60f2
+ 00000000646cb41c (rva: 0000b41c): 00000000646c6170 - 00000000646c6182
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb414 (rva: 0000b414): 00000000646c6100 - 00000000646c6144
+ 00000000646cb420 (rva: 0000b420): 00000000646c6190 - 00000000646c61d4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb418 (rva: 0000b418): 00000000646c6150 - 00000000646c61dd
+ 00000000646cb424 (rva: 0000b424): 00000000646c61e0 - 00000000646c626d
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb424 (rva: 0000b424): 00000000646c61e0 - 00000000646c6254
+ 00000000646cb430 (rva: 0000b430): 00000000646c6270 - 00000000646c62e4
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb42c (rva: 0000b42c): 00000000646c6260 - 00000000646c629e
+ 00000000646cb438 (rva: 0000b438): 00000000646c62f0 - 00000000646c632e
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb434 (rva: 0000b434): 00000000646c62a0 - 00000000646c630f
+ 00000000646cb440 (rva: 0000b440): 00000000646c6330 - 00000000646c639f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb43c (rva: 0000b43c): 00000000646c6310 - 00000000646c6347
+ 00000000646cb448 (rva: 0000b448): 00000000646c63a0 - 00000000646c63d7
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb444 (rva: 0000b444): 00000000646c6350 - 00000000646c63e1
+ 00000000646cb450 (rva: 0000b450): 00000000646c63e0 - 00000000646c6471
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb44c (rva: 0000b44c): 00000000646c63f0 - 00000000646c6496
+ 00000000646cb458 (rva: 0000b458): 00000000646c6480 - 00000000646c6526
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb454 (rva: 0000b454): 00000000646c64a0 - 00000000646c64a3
+ 00000000646cb460 (rva: 0000b460): 00000000646c6530 - 00000000646c6533
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb458 (rva: 0000b458): 00000000646c64f0 - 00000000646c64f6
+ 00000000646cb464 (rva: 0000b464): 00000000646c6580 - 00000000646c6586
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb45c (rva: 0000b45c): 00000000646c6500 - 00000000646c6506
+ 00000000646cb468 (rva: 0000b468): 00000000646c6590 - 00000000646c6596
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb460 (rva: 0000b460): 00000000646c6510 - 00000000646c6564
+ 00000000646cb46c (rva: 0000b46c): 00000000646c65a0 - 00000000646c65f4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb464 (rva: 0000b464): 00000000646c6570 - 00000000646c6696
+ 00000000646cb470 (rva: 0000b470): 00000000646c6600 - 00000000646c6726
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb470 (rva: 0000b470): 00000000646c66a0 - 00000000646c66a5
+ 00000000646cb47c (rva: 0000b47c): 00000000646c6730 - 00000000646c6735
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb474 (rva: 0000b474): 00000000646c66b0 - 00000000646c6787
+ 00000000646cb480 (rva: 0000b480): 00000000646c6740 - 00000000646c6817
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb478 (rva: 0000b478): 00000000646c6790 - 00000000646c6884
+ 00000000646cb484 (rva: 0000b484): 00000000646c6820 - 00000000646c6914
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb484 (rva: 0000b484): 00000000646c68c0 - 00000000646c6aa4
+ 00000000646cb490 (rva: 0000b490): 00000000646c6950 - 00000000646c6b34
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb490 (rva: 0000b490): 00000000646c6ab0 - 00000000646c6bd0
+ 00000000646cb49c (rva: 0000b49c): 00000000646c6b40 - 00000000646c6c60
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb49c (rva: 0000b49c): 00000000646c6bd0 - 00000000646c6c66
+ 00000000646cb4a8 (rva: 0000b4a8): 00000000646c6c60 - 00000000646c6cf6
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
- 00000000646cb4a4 (rva: 0000b4a4): 00000000646c6c70 - 00000000646c71c7
+ 00000000646cb4b0 (rva: 0000b4b0): 00000000646c6d00 - 00000000646c7257
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save xmm7 at rsp + 0x80
 	  pc+0x12: save xmm6 at rsp + 0x70
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb4c0 (rva: 0000b4c0): 00000000646c71d0 - 00000000646c744e
+ 00000000646cb4cc (rva: 0000b4cc): 00000000646c7260 - 00000000646c74de
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: save xmm6 at rsp + 0x40
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb4cc (rva: 0000b4cc): 00000000646c7520 - 00000000646c75de
+ 00000000646cb4d8 (rva: 0000b4d8): 00000000646c75b0 - 00000000646c766e
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x30
 	  pc+0x01: push rbx
- 00000000646cb4d4 (rva: 0000b4d4): 00000000646c7700 - 00000000646c7725
+ 00000000646cb4e0 (rva: 0000b4e0): 00000000646c7790 - 00000000646c77b5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb4d8 (rva: 0000b4d8): 00000000646c7730 - 00000000646c77f8
+ 00000000646cb4e4 (rva: 0000b4e4): 00000000646c77c0 - 00000000646c7888
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb4e8 (rva: 0000b4e8): 00000000646c7800 - 00000000646c786f
+ 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7890 - 00000000646c78ff
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7870 - 00000000646c788f
+ 00000000646cb500 (rva: 0000b500): 00000000646c7900 - 00000000646c791f
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb4fc (rva: 0000b4fc): 00000000646c7960 - 00000000646c79a1
+ 00000000646cb508 (rva: 0000b508): 00000000646c79f0 - 00000000646c7a31
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb504 (rva: 0000b504): 00000000646c79b0 - 00000000646c79bc
+ 00000000646cb510 (rva: 0000b510): 00000000646c7a40 - 00000000646c7a4c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb508 (rva: 0000b508): 00000000646c79c0 - 00000000646c7abc
+ 00000000646cb514 (rva: 0000b514): 00000000646c7a50 - 00000000646c7b4c
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x16, Frame offset: 0x0, Frame reg: none
 	  pc+0x16: save xmm8 at rsp + 0x60
 	  pc+0x10: save xmm7 at rsp + 0x50
 	  pc+0x0b: save xmm6 at rsp + 0x40
 	  pc+0x06: alloc small area: rsp = rsp - 0x78
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb388 (rva: 0000b388): 00000000646c7ad0 - 00000000646c7b39
+ 00000000646cb394 (rva: 0000b394): 00000000646c7b60 - 00000000646c7bc9
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb520 (rva: 0000b520): 00000000646c7b40 - 00000000646c7b45
+ 00000000646cb52c (rva: 0000b52c): 00000000646c7bd0 - 00000000646c7bd5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00007000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  b58 [7b58] DIR64
+	reloc    0 offset  be8 [7be8] DIR64
 	reloc    1 offset    0 [7000] ABSOLUTE
 
 Virtual Address: 00008000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset    0 [8000] DIR64
 	reloc    1 offset   50 [8050] DIR64
 	reloc    2 offset   58 [8058] DIR64
 	reloc    3 offset   60 [8060] DIR64
@@ -1120,47 +1129,47 @@
 	reloc    0 offset   18 [f018] DIR64
 	reloc    1 offset   30 [f030] DIR64
 	reloc    2 offset   38 [f038] DIR64
 	reloc    3 offset    0 [f000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00006b78  00000000646c1000  00000000646c1000  00000600  2**4
+  0 .text         00006c08  00000000646c1000  00000000646c1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
-  1 .data         000000a0  00000000646c8000  00000000646c8000  00007200  2**4
+  1 .data         000000a0  00000000646c8000  00000000646c8000  00007400  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  2 .rdata        000008e0  00000000646c9000  00000000646c9000  00007400  2**5
+  2 .rdata        000008e0  00000000646c9000  00000000646c9000  00007600  2**5
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  3 .pdata        000005b8  00000000646ca000  00000000646ca000  00007e00  2**2
+  3 .pdata        000005c4  00000000646ca000  00000000646ca000  00008000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        00000524  00000000646cb000  00000000646cb000  00008400  2**2
+  4 .xdata        00000530  00000000646cb000  00000000646cb000  00008600  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .bss          00000b90  00000000646cc000  00000000646cc000  00000000  2**5
                   ALLOC
-  6 .edata        00000674  00000000646cd000  00000000646cd000  00008a00  2**2
+  6 .edata        0000068c  00000000646cd000  00000000646cd000  00008c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000720  00000000646ce000  00000000646ce000  00009200  2**2
+  7 .idata        00000720  00000000646ce000  00000000646ce000  00009400  2**2
                   CONTENTS, ALLOC, LOAD, DATA
-  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009a00  2**3
+  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009c00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
-  9 .tls          00000010  00000000646d0000  00000000646d0000  00009c00  2**3
+  9 .tls          00000010  00000000646d0000  00000000646d0000  00009e00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
- 10 .reloc        00000064  00000000646d1000  00000000646d1000  00009e00  2**2
+ 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
- 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a000  2**4
+ 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a200  2**4
                   CONTENTS, READONLY, DEBUGGING
- 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a200  2**0
+ 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a400  2**0
                   CONTENTS, READONLY, DEBUGGING
- 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c200  2**0
+ 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c400  2**0
                   CONTENTS, READONLY, DEBUGGING
- 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c400  2**0
+ 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c600  2**0
                   CONTENTS, READONLY, DEBUGGING
- 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000c800  2**3
+ 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000ca00  2**3
                   CONTENTS, READONLY, DEBUGGING
- 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000ca00  2**0
+ 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000cc00  2**0
                   CONTENTS, READONLY, DEBUGGING
 SYMBOL TABLE:
 [  0](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000028 crtdll.c
 File 
 [  2](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000000 pre_c_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [  4](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 atexit_table
@@ -1321,18 +1330,18 @@
 [159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 pdist_temp
 [160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 datacov
 [161](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002180 sampling_state_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002231 sampling_state_update
 [164](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000225d krige_param_setting
 [165](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000024b9 simple_kriging
-[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000028c7 find_neighbor
-[167](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002a7b krige_memory_free
+[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000028d0 find_neighbor
+[167](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002a84 krige_memory_free
 [168](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002180 .text
-AUX scnlen 0xa45 nreloc 130 nlnno 0
+AUX scnlen 0xa4e nreloc 130 nlnno 0
 [170](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [172](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x148 nreloc 0 nlnno 0
 [174](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000208 .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [176](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
@@ -1407,1233 +1416,1234 @@
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [246](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002dc .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [248](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .rdata
 AUX scnlen 0x4e nreloc 0 nlnno 0
 [250](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[252](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010e sort_tools.c
+[252](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010f sort_tools.c
 File 
 [254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003c90 swaprows
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003d0e partition2d
 [257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003dd5 quicksort2d
-[258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003c90 .text
-AUX scnlen 0x1a9 nreloc 0 nlnno 0
-[260](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[258](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003e39 quickselect2d
+[259](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003c90 .text
+AUX scnlen 0x234 nreloc 0 nlnno 0
+[261](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[262](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
+[263](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[264](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .xdata
-AUX scnlen 0x24 nreloc 0 nlnno 0
-[266](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
-AUX scnlen 0x24 nreloc 9 nlnno 0
-[268](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .rdata$zzz
+[265](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .xdata
+AUX scnlen 0x30 nreloc 0 nlnno 0
+[267](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
+AUX scnlen 0x30 nreloc 12 nlnno 0
+[269](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[270](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000128 variogram.c
+[271](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000129 variogram.c
 File 
-[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003e40 variogram
+[273](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003ed0 variogram
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040b6 variance
-[275](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003e40 .text
+[275](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004146 variance
+[276](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003ed0 .text
 AUX scnlen 0x35e nreloc 11 nlnno 0
-[277](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[278](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[279](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
+[280](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000314 .xdata
+[282](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000320 .xdata
 AUX scnlen 0x1c nreloc 0 nlnno 0
-[283](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .pdata
+[284](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000033c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[285](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000150 .rdata
+[286](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000150 .rdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[287](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008a0 .rdata$zzz
+[288](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008a0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[289](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000041a0 .text
-[290](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
-[291](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .bss
-[292](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
-[293](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
-[294](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
-[295](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
-[296](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000136 fake
+[290](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000004230 .text
+[291](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
+[292](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .bss
+[293](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
+[294](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
+[295](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
+[296](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
+[297](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000137 fake
 File 
-[298](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
-[299](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
-[300](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
+[299](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
+[300](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
+[301](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004240 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[302](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[303](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[304](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
+[305](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[306](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
+[307](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[308](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
-[309](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
-[310](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000144 fake
+[309](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
+[310](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
+[311](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000145 fake
 File 
-[312](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
+[313](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004240 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[314](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[315](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[316](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
+[317](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[318](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
+[319](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[320](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
+[321](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[322](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
+[323](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
-[324](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000158 gccmain.c
+[325](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000159 gccmain.c
 File 
-[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000041b0 __do_global_dtors
+[327](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004240 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[328](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
-[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000041f0 __do_global_ctors
-[330](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005d0 .rdata$.refptr.__CTOR_LIST__
+[329](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
+[330](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004280 __do_global_ctors
+[331](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005d0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004260 __main
-[333](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 initialized
-[334](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
+[333](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000042f0 __main
+[334](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 initialized
+[335](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004240 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
-[336](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[337](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[338](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
+[339](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[340](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .xdata
+[341](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000033c .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[342](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .pdata
+[343](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[344](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000160 natstart.c
+[345](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000161 natstart.c
 File 
-[346](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004280 .text
+[347](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004310 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[348](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
+[349](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[350](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .bss
+[351](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[352](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000178 gs_support.c
+[353](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000179 gs_support.c
 File 
-[354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004280 __security_init_cookie
+[355](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004310 __security_init_cookie
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[356](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
+[357](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[358](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
+[359](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[360](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004360 __report_gsfailure
-[361](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 GS_ContextRecord
-[362](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 GS_ExceptionRecord
-[363](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 GS_ExceptionPointers
-[364](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004280 .text
+[361](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000043f0 __report_gsfailure
+[362](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 GS_ContextRecord
+[363](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 GS_ExceptionRecord
+[364](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 GS_ExceptionPointers
+[365](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004310 .text
 AUX scnlen 0x1d8 nreloc 29 nlnno 0
-[366](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[367](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[368](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .bss
+[369](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .bss
 AUX scnlen 0x578 nreloc 0 nlnno 0
-[370](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .xdata
+[371](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[372](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000036c .pdata
+[373](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000378 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[374](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .rdata
+[375](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .rdata
 AUX scnlen 0x10 nreloc 2 nlnno 0
-[376](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019e tlssup.c
+[377](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019f tlssup.c
 File 
-[378](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004460 __dyn_tls_dtor
+[379](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000044f0 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004490 __dyn_tls_init
-[381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005c0 .rdata$.refptr._CRT_MT
+[381](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004520 __dyn_tls_init
+[382](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005c0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[383](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
-[384](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004510 __tlregdtor
-[386](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004460 .text
+[384](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
+[385](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
+[386](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000045a0 __tlregdtor
+[387](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044f0 .text
 AUX scnlen 0xb3 nreloc 5 nlnno 0
-[388](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[389](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[390](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .bss
+[391](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[392](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000368 .xdata
+[393](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000374 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[394](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000384 .pdata
+[395](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000390 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[396](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
+[397](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[398](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
+[399](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[400](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .rdata
+[401](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .rdata
 AUX scnlen 0x48 nreloc 5 nlnno 0
-[402](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .CRT$XDZ
+[403](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .CRT$XDZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[404](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000048 .CRT$XDA
+[405](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000048 .CRT$XDA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[406](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .CRT$XLZ
+[407](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .CRT$XLZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[408](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .CRT$XLA
+[409](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .CRT$XLA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[410](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
+[411](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[412](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
+[413](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[414](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ae cinitexe.c
+[415](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001af cinitexe.c
 File 
-[416](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
+[417](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[418](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[419](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[420](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
+[421](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[422](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
+[423](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[424](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .CRT$XCA
+[425](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .CRT$XCA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[426](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
+[427](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[428](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
+[429](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[430](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001bd mingw_helpers.c
+[431](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001be mingw_helpers.c
 File 
-[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004520 _decode_pointer
+[433](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000045b0 _decode_pointer
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[434](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004530 _encode_pointer
-[435](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
+[435](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000045c0 _encode_pointer
+[436](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045b0 .text
 AUX scnlen 0x14 nreloc 0 nlnno 0
-[437](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[438](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[439](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
+[440](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[441](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .xdata
+[442](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000038c .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[443](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .pdata
+[444](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003b4 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[445](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001de pseudo-reloc.c
+[446](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001df pseudo-reloc.c
 File 
-[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006ad0 __report_error
+[448](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006b60 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[449](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000004540 __write_memory.part.0
-[450](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 maxSections
-[451](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 the_secs
-[452](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004710 _pei386_runtime_relocator
-[453](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 was_init.95174
-[454](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[450](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x00000000000045d0 __write_memory.part.0
+[451](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 maxSections
+[452](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 the_secs
+[453](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000047a0 _pei386_runtime_relocator
+[454](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 was_init.95174
+[455](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[456](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[457](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[458](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$.refptr.__image_base__
+[459](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$.refptr.__image_base__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004540 .text
+[461](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045d0 .text
 AUX scnlen 0x48b nreloc 36 nlnno 0
-[462](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[463](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[464](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .bss
+[465](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e0 .rdata
+[467](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e0 .rdata
 AUX scnlen 0x102 nreloc 0 nlnno 0
-[468](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ad0 .text.unlikely
+[469](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b60 .text.unlikely
 AUX scnlen 0x69 nreloc 6 nlnno 0
-[470](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000388 .xdata.unlikely
+[471](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000394 .xdata.unlikely
 AUX scnlen 0xc nreloc 0 nlnno 0
-[472](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c0 .pdata.unlikely
+[473](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata.unlikely
 AUX scnlen 0xc nreloc 3 nlnno 0
-[474](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000394 .xdata
+[475](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .xdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[476](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata
+[477](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d8 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[478](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f3 crt_handler.c
+[479](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f4 crt_handler.c
 File 
-[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000049d0 __mingw_SEH_error_handler
+[481](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004a60 __mingw_SEH_error_handler
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[482](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004b70 __mingw_init_ehandler
-[483](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000868 was_here.95013
-[484](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000980 emu_pdata
-[485](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000880 emu_xdata
-[486](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004c60 _gnu_exception_handler
-[487](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000049d0 .text
+[483](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004c00 __mingw_init_ehandler
+[484](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000868 was_here.95013
+[485](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000980 emu_pdata
+[486](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000880 emu_xdata
+[487](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004cf0 _gnu_exception_handler
+[488](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004a60 .text
 AUX scnlen 0x477 nreloc 29 nlnno 0
-[489](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[490](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[491](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .bss
+[492](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .bss
 AUX scnlen 0x2a0 nreloc 0 nlnno 0
-[493](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003bc .xdata
+[494](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c8 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[495](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e4 .pdata
+[496](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003f0 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[497](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .rdata
+[498](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .rdata
 AUX scnlen 0x7 nreloc 0 nlnno 0
-[499](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000207 tlsthrd.c
+[500](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000208 tlsthrd.c
 File 
-[501](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004e50 __mingwthr_run_key_dtors.part.0
+[502](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004ee0 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[503](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b20 __mingwthr_cs
-[504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b00 key_dtor_list
-[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004ec0 ___w64_mingwthr_add_key_dtor
-[506](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b08 __mingwthr_cs_init
-[507](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004f40 ___w64_mingwthr_remove_key_dtor
-[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004fe0 __mingw_TLScallback
-[509](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004e50 .text
+[504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b20 __mingwthr_cs
+[505](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b00 key_dtor_list
+[506](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004f50 ___w64_mingwthr_add_key_dtor
+[507](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b08 __mingwthr_cs_init
+[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004fd0 ___w64_mingwthr_remove_key_dtor
+[509](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005070 __mingw_TLScallback
+[510](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004ee0 .text
 AUX scnlen 0x26a nreloc 39 nlnno 0
-[511](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[512](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[513](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
+[514](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[515](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003dc .xdata
+[516](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e8 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
-[517](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000408 .pdata
+[518](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000414 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
-[519](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020f tlsmcrt.c
+[520](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000210 tlsmcrt.c
 File 
-[521](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
+[522](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005150 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[523](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[524](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[525](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
+[526](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[527](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000217 pseudo-reloc-list.c
+[528](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000218 pseudo-reloc-list.c
 File 
-[529](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
+[530](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005150 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[531](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[532](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[533](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
+[534](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
-[535](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022e pesect.c
+[536](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022f pesect.c
 File 
-[537](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000050c0 _ValidateImageBase.part.0
+[538](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005150 _ValidateImageBase.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000050e0 _ValidateImageBase
-[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005100 _FindPESection
-[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005150 _FindPESectionByName
-[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051e0 __mingw_GetSectionForAddress
-[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005260 __mingw_GetSectionCount
-[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052a0 _FindPESectionExec
-[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005310 _GetPEImageBase
-[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005350 _IsNonwritableInCurrentImage
-[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053f0 __mingw_enum_import_library_names
-[548](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
+[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005170 _ValidateImageBase
+[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005190 _FindPESection
+[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051e0 _FindPESectionByName
+[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005270 __mingw_GetSectionForAddress
+[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052f0 __mingw_GetSectionCount
+[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005330 _FindPESectionExec
+[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053a0 _GetPEImageBase
+[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053e0 _IsNonwritableInCurrentImage
+[548](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005480 __mingw_enum_import_library_names
+[549](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005150 .text
 AUX scnlen 0x3d6 nreloc 9 nlnno 0
-[550](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[551](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[552](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[553](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[554](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000040c .xdata
+[555](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000418 .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[556](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000438 .pdata
+[557](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000444 .pdata
 AUX scnlen 0x78 nreloc 30 nlnno 0
-[558](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023d CRT_fp10.c
+[559](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023e CRT_fp10.c
 File 
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000054a0 _fpreset
+[561](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005530 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[562](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054a0 fpreset
-[563](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054a0 .text
+[563](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005530 fpreset
+[564](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005530 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
-[565](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[566](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[567](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[568](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[569](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000454 .xdata
+[570](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[571](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b0 .pdata
+[572](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[573](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000251 fake
+[574](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000252 fake
 File 
-[575](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
+[576](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
 AUX scnlen 0x2e nreloc 7 nlnno 0
-[577](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
+[578](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
 AUX scnlen 0x14 nreloc 0 nlnno 0
-[579](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
+[580](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
 AUX scnlen 0x7b nreloc 1 nlnno 0
-[581](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054b0 .text
+[582](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005540 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
-[583](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[584](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[585](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[586](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[587](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
+[588](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[589](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
+[590](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
 AUX scnlen 0x9b nreloc 0 nlnno 0
-[591](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
+[592](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
 AUX scnlen 0x48 nreloc 2 nlnno 0
-[593](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000261 libgcc2.c
+[594](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000262 libgcc2.c
 File 
-[595](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
+[596](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005580 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[597](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[598](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[599](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[600](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[601](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
+[602](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
 AUX scnlen 0x1eda nreloc 4 nlnno 0
-[603](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .debug_abbrev
+[604](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .debug_abbrev
 AUX scnlen 0x135 nreloc 0 nlnno 0
-[605](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
+[606](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
 AUX scnlen 0x20 nreloc 1 nlnno 0
-[607](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
+[608](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
 AUX scnlen 0x1a7 nreloc 0 nlnno 0
-[609](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000026f dllentry.c
+[610](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000270 dllentry.c
 File 
-[611](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000054f0 DllEntryPoint
+[612](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005580 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[613](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
+[614](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005580 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
-[615](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[616](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[617](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[618](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[619](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000458 .xdata
+[620](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000464 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[621](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
+[622](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[623](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027d dllmain.c
+[624](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027e dllmain.c
 File 
-[625](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005500 DllMain
+[626](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005590 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[627](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005500 .text
+[628](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005590 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
-[629](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[630](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[631](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[632](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[633](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000045c .xdata
+[634](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000468 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[635](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
+[636](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[637](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028b fpclassify.c
+[638](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028c fpclassify.c
 File 
-[639](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005510 __fpclassify
+[640](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000055a0 __fpclassify
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[641](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005510 .text
+[642](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000055a0 .text
 AUX scnlen 0x54 nreloc 0 nlnno 0
-[643](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[644](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[645](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[646](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[647](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .xdata
+[648](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000046c .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[649](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
+[650](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[651](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000029b sqrt.c
+[652](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000029c sqrt.c
 File 
-[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005570 sqrt
+[654](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005600 sqrt
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005570 .text
+[656](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005600 .text
 AUX scnlen 0x126 nreloc 10 nlnno 0
-[657](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[658](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[659](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[660](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[661](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000300 .rdata
+[662](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000300 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[663](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000464 .xdata
+[664](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000470 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[665](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
+[666](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[667](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a9 vsnprintf.c
+[668](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002aa vsnprintf.c
 File 
-[669](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000056a0 __ms_vsnprintf
+[670](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005730 __ms_vsnprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[671](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000056a0 .text
+[672](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005730 .text
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[673](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[674](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[675](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[676](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[677](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000470 .xdata
+[678](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000047c .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[679](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
+[680](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[681](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c2 ceil.S
+[682](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c3 ceil.S
 File 
-[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000056b0 ceil
+[684](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005740 ceil
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[685](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005770 .is_intnaninf
-[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005780 .ret_org
-[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005730 .signed_val
-[688](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000330 .huge
-[689](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000338 .zero
-[690](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005721 .doret
-[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x000000000000571b .l1
-[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005760 .doret2
-[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005782 .ret_naninf
-[694](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000056b0 .text
+[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005800 .is_intnaninf
+[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005810 .ret_org
+[688](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000057c0 .signed_val
+[689](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000330 .huge
+[690](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000338 .zero
+[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000057b1 .doret
+[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000057ab .l1
+[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000057f0 .doret2
+[694](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005812 .ret_naninf
+[695](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005740 .text
 AUX scnlen 0xd7 nreloc 4 nlnno 0
-[696](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[697](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[698](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[699](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[700](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000474 .xdata
+[701](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000480 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[702](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
+[703](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[704](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .rdata
+[705](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[706](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d2 cos.c
+[707](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d3 cos.c
 File 
-[708](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005790 cos
+[709](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005820 cos
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005790 .text
+[711](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005820 .text
 AUX scnlen 0xf4 nreloc 8 nlnno 0
-[712](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[713](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[714](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[715](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[716](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000340 .rdata
+[717](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000340 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[718](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000478 .xdata
+[719](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000484 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[720](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
+[721](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[722](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002dc cosl_internal.S
+[723](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002dd cosl_internal.S
 File 
-[724](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005890 __cosl_internal
+[725](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005920 __cosl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[726](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005890 .text
+[727](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005920 .text
 AUX scnlen 0x30 nreloc 0 nlnno 0
-[728](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[729](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[730](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[731](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[732](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ee exp.c
+[733](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ef exp.c
 File 
-[734](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000058c0 exp
+[735](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005950 exp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[736](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
-[737](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
-[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000058c0 .text
+[737](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
+[738](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
+[739](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005950 .text
 AUX scnlen 0x1e4 nreloc 17 nlnno 0
-[740](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[741](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[742](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[743](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[744](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000350 .rdata
+[745](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000350 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[746](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000484 .xdata
+[747](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[748](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
+[749](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[750](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002fe log.c
+[751](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ff log.c
 File 
-[752](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005ab0 log
+[753](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005b40 log
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[754](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ab0 .text
+[755](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005b40 .text
 AUX scnlen 0x120 nreloc 11 nlnno 0
-[756](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[757](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[758](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[759](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[760](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .rdata
+[761](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .rdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[762](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
+[763](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000049c .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[764](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
+[765](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000528 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[766](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000030f pow.c
+[767](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000310 pow.c
 File 
-[768](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005bd0 internal_modf
+[769](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005c60 internal_modf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[770](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005c70 pow
-[771](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005bd0 .text
+[771](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005d00 pow
+[772](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005c60 .text
 AUX scnlen 0x5f7 nreloc 31 nlnno 0
-[773](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[774](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[775](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[776](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[777](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000049c .xdata
+[778](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004a8 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
-[779](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000528 .pdata
+[780](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000534 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[781](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata
+[782](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata
 AUX scnlen 0x80 nreloc 0 nlnno 0
-[783](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000031f powi.c
+[784](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000320 powi.c
 File 
-[785](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000061d0 __powi
+[786](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006260 __powi
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000061d0 .text
+[788](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006260 .text
 AUX scnlen 0x27e nreloc 15 nlnno 0
-[789](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[790](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[791](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[792](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[793](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .rdata
+[794](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .rdata
 AUX scnlen 0x60 nreloc 0 nlnno 0
-[795](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .xdata
+[796](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004cc .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[797](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000540 .pdata
+[798](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[799](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000329 exp2l.S
+[800](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000032a exp2l.S
 File 
-[801](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006450 exp2l
+[802](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064e0 exp2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[803](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006450 .text
+[804](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064e0 .text
 AUX scnlen 0x68 nreloc 0 nlnno 0
-[805](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[806](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[807](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[808](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[809](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000335 internal_logl.S
+[810](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000336 internal_logl.S
 File 
-[811](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000064c0 one
-[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000064c8 limit
-[813](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064d0 __logl_internal
+[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006550 one
+[813](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006558 limit
+[814](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006560 __logl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064c0 .text
+[816](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006550 .text
 AUX scnlen 0x51 nreloc 0 nlnno 0
-[817](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[818](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[819](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[820](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[821](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000343 ldexp.c
+[822](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000344 ldexp.c
 File 
-[823](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006520 ldexp
+[824](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000065b0 ldexp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[825](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006520 .text
+[826](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000065b0 .text
 AUX scnlen 0xbe nreloc 1 nlnno 0
-[827](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[828](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[829](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[830](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[831](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004cc .xdata
+[832](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d8 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[833](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
+[834](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000558 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[835](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003e2 log2l.S
+[836](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003e3 log2l.S
 File 
-[837](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000065e0 one
-[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000065e8 limit
-[839](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000065f0 log2l
+[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006670 one
+[839](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006678 limit
+[840](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006680 log2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000065e0 .text
+[842](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006670 .text
 AUX scnlen 0x6c nreloc 0 nlnno 0
-[843](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[844](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[845](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[846](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006650 .text
-[848](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[849](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[850](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
-[851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
-[852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
-[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
-[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006658 .text
-[855](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[856](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[857](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
-[858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
-[859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
-[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
-[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006660 .text
-[862](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[863](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[864](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
-[865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
-[866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
-[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
-[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006668 .text
-[869](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[870](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[871](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
-[872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
-[873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
-[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
-[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006670 .text
-[876](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[877](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[878](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
-[879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
-[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
-[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
-[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006678 .text
-[883](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[884](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[885](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
-[886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
-[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
-[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
-[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006680 .text
-[890](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[891](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[892](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
-[893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
-[894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
-[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
-[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006688 .text
-[897](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[899](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
-[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
-[901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
-[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
-[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006690 .text
-[904](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[906](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
-[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
-[908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
-[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
-[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006698 .text
-[911](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[912](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[913](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
-[914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
-[915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
-[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
-[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066a0 .text
-[918](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[919](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[920](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
-[921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
-[922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
-[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
-[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066a8 .text
-[925](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[926](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[927](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
-[928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
-[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
-[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
-[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066b0 .text
-[932](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[933](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[934](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
-[935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
-[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
-[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
-[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066b8 .text
-[939](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[940](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[941](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
-[942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
-[943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
-[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
-[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066c0 .text
-[946](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[948](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
-[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
-[950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
-[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
-[952](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066c8 .text
-[953](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[954](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[955](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
-[956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
-[957](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
-[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
-[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066d0 .text
-[960](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[961](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[962](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
-[963](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
-[964](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
-[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
-[966](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066d8 .text
-[967](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[968](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[969](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
-[970](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
-[971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
-[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
-[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e0 .text
-[974](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[975](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[976](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
-[977](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
-[978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
-[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
-[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e8 .text
-[981](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[982](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[983](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
-[984](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
-[985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
-[986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
-[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066f0 .text
-[988](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[989](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[990](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
-[991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
-[992](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
-[993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
-[994](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f2 onexit_table.c
+[848](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e0 .text
+[849](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[850](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
+[852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
+[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
+[854](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
+[855](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e8 .text
+[856](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[857](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
+[859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
+[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
+[861](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
+[862](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066f0 .text
+[863](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[864](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
+[866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
+[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
+[868](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
+[869](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066f8 .text
+[870](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[871](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
+[873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
+[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
+[875](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
+[876](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006700 .text
+[877](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[878](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
+[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
+[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
+[882](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
+[883](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006708 .text
+[884](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[885](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
+[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
+[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
+[889](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
+[890](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006710 .text
+[891](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[892](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
+[894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
+[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
+[896](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
+[897](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006718 .text
+[898](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[899](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
+[901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
+[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
+[903](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
+[904](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006720 .text
+[905](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[906](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
+[908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
+[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
+[910](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
+[911](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006728 .text
+[912](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[913](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
+[915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
+[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
+[917](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
+[918](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006730 .text
+[919](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[920](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
+[922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
+[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
+[924](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
+[925](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006738 .text
+[926](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[927](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
+[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
+[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
+[931](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
+[932](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006740 .text
+[933](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[934](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
+[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
+[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
+[938](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
+[939](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006748 .text
+[940](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[941](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
+[943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
+[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
+[945](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
+[946](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006750 .text
+[947](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[948](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
+[950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
+[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
+[952](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
+[953](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006758 .text
+[954](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[955](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
+[957](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
+[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
+[959](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
+[960](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006760 .text
+[961](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[962](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[963](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
+[964](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
+[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
+[966](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
+[967](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006768 .text
+[968](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[969](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[970](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
+[971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
+[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
+[973](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
+[974](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006770 .text
+[975](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[976](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[977](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
+[978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
+[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
+[980](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
+[981](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006778 .text
+[982](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[983](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[984](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
+[985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
+[986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
+[987](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
+[988](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006780 .text
+[989](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[990](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
+[992](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
+[993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
+[994](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
+[995](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f3 onexit_table.c
 File 
-[996](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006700 _initialize_onexit_table
+[997](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006790 _initialize_onexit_table
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[998](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006730 _register_onexit_function
-[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006800 _execute_onexit_table
-[1000](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006700 .text
+[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000067c0 _register_onexit_function
+[1000](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006890 _execute_onexit_table
+[1001](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006790 .text
 AUX scnlen 0x16f nreloc 8 nlnno 0
-[1002](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[1003](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x18 nreloc 3 nlnno 0
-[1004](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[1005](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1006](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .xdata
+[1007](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[1008](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000558 .pdata
+[1009](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000564 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[1010](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000400 acrt_iob_func.c
+[1011](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000401 acrt_iob_func.c
 File 
-[1012](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006870 __acrt_iob_func
+[1013](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006900 __acrt_iob_func
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1014](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006870 .text
+[1015](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006900 .text
 AUX scnlen 0x1f nreloc 1 nlnno 0
-[1016](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
+[1017](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1018](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[1019](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1020](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f4 .xdata
+[1021](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000500 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1022](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000057c .pdata
+[1023](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000588 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1024](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000042a fake
+[1025](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000042b fake
 File 
-[1026](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
-[1027](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
-[1028](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006890 .text
+[1027](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
+[1028](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
+[1029](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006920 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1030](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1031](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1032](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[1033](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1034](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
+[1035](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[1036](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
-[1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006890 .text
-[1039](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1041](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
-[1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
-[1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
-[1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
-[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006898 .text
-[1046](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1048](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
-[1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
-[1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
-[1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
-[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a0 .text
-[1053](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1054](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1055](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
-[1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
-[1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
-[1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
-[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a8 .text
-[1060](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1061](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1062](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
-[1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
-[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
-[1066](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004cb fake
+[1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
+[1038](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
+[1039](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006920 .text
+[1040](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1041](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
+[1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
+[1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
+[1045](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
+[1046](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006928 .text
+[1047](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1048](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
+[1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
+[1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
+[1052](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
+[1053](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006930 .text
+[1054](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1055](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
+[1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
+[1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
+[1059](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
+[1060](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006938 .text
+[1061](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1062](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
+[1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
+[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
+[1066](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
+[1067](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004cc fake
 File 
-[1068](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068b0 .text
+[1069](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006940 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1070](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1071](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1072](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[1073](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
+[1075](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1076](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
+[1077](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1078](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
+[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
 AUX scnlen 0xb nreloc 0 nlnno 0
-[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b0 .text
-[1081](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1082](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1083](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
-[1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
-[1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
-[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
-[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b8 .text
-[1088](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1089](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1090](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
-[1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
-[1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
-[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
-[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c0 .text
-[1095](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1096](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1097](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
-[1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
-[1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
-[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
-[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c8 .text
-[1102](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1103](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1104](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
-[1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
-[1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
-[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
-[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d0 .text
-[1109](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1111](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
-[1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
-[1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
-[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
-[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d8 .text
-[1116](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1117](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1118](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
-[1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
-[1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
-[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
-[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e0 .text
-[1123](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1124](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1125](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
-[1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
-[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
-[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
-[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e8 .text
-[1130](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1131](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1132](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
-[1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
-[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
-[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
-[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f0 .text
-[1137](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1139](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
-[1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
-[1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
-[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
-[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f8 .text
-[1144](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1146](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
-[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
-[1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
-[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
-[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006900 .text
-[1151](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1153](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
-[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
-[1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
-[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
-[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006908 .text
-[1158](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1160](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
-[1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
-[1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
-[1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
-[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006910 .text
-[1165](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1166](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1167](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
-[1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
-[1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
-[1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
-[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006918 .text
-[1172](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1173](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1174](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
-[1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
-[1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
-[1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
-[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006920 .text
-[1179](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1180](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1181](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
-[1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
-[1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
-[1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
-[1185](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006928 .text
-[1186](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1187](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1188](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
-[1189](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
-[1190](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
-[1191](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
-[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006930 .text
-[1193](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1194](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1195](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
-[1196](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
-[1197](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
-[1198](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
-[1199](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006938 .text
-[1200](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1201](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1202](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
-[1203](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
-[1204](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
-[1205](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
-[1206](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
-[1207](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1208](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1209](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
-[1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
-[1211](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
-[1212](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
-[1213](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
-[1214](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1216](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
-[1217](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
-[1218](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
-[1219](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
-[1220](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
-[1221](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1222](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
-[1223](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
-[1224](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
-[1225](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
-[1226](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
-[1227](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004e5 merr.c
+[1081](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
+[1082](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1083](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
+[1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
+[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
+[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
+[1088](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
+[1089](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1090](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
+[1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
+[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
+[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
+[1095](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
+[1096](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1097](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
+[1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
+[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
+[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
+[1102](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006958 .text
+[1103](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1104](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
+[1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
+[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
+[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
+[1109](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006960 .text
+[1110](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1111](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
+[1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
+[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
+[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
+[1116](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006968 .text
+[1117](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1118](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
+[1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
+[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
+[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
+[1123](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006970 .text
+[1124](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1125](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
+[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
+[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
+[1129](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
+[1130](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006978 .text
+[1131](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1132](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
+[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
+[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
+[1136](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
+[1137](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006980 .text
+[1138](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1139](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
+[1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
+[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
+[1143](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
+[1144](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006988 .text
+[1145](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1146](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
+[1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
+[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
+[1150](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
+[1151](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006990 .text
+[1152](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1153](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
+[1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
+[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
+[1157](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
+[1158](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006998 .text
+[1159](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
+[1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
+[1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
+[1164](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
+[1165](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a0 .text
+[1166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1167](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
+[1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
+[1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
+[1171](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
+[1172](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a8 .text
+[1173](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1174](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
+[1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
+[1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
+[1178](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
+[1179](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b0 .text
+[1180](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1181](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
+[1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
+[1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
+[1185](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
+[1186](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b8 .text
+[1187](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1188](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1189](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
+[1190](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
+[1191](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
+[1192](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
+[1193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c0 .text
+[1194](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1195](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1196](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
+[1197](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
+[1198](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
+[1199](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
+[1200](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c8 .text
+[1201](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1202](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1203](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
+[1204](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
+[1205](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
+[1206](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
+[1207](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d0 .text
+[1208](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1209](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
+[1211](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
+[1212](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
+[1213](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
+[1214](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d8 .text
+[1215](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1216](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1217](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
+[1218](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
+[1219](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
+[1220](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
+[1221](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069e0 .text
+[1222](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1223](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
+[1224](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
+[1225](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
+[1226](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
+[1227](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
+[1228](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004e6 merr.c
 File 
-[1229](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006960 __mingw_raise_matherr
+[1230](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000069f0 __mingw_raise_matherr
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 stUserMathErr
-[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b0 __mingw_setusermatherr
-[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c0 _matherr
-[1234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006960 .text
+[1232](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 stUserMathErr
+[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a40 __mingw_setusermatherr
+[1234](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a50 _matherr
+[1235](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000069f0 .text
 AUX scnlen 0x15c nreloc 14 nlnno 0
-[1236](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1237](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1238](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
+[1239](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1240](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004fc .xdata
+[1241](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000508 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
-[1242](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000588 .pdata
+[1243](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000594 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[1244](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000480 .rdata
+[1245](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000480 .rdata
 AUX scnlen 0x140 nreloc 7 nlnno 0
-[1246](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ac0 .text
-[1247](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1248](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b80 .bss
-[1249](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
-[1250](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
-[1251](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
-[1252](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
-[1253](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004f7 cygming-crtend.c
+[1247](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b50 .text
+[1248](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1249](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b80 .bss
+[1250](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
+[1251](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
+[1252](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
+[1253](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
+[1254](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004f8 cygming-crtend.c
 File 
-[1255](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006b40 register_frame_ctor
+[1256](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006bd0 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1257](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ad0 .text
+[1258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b60 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1259](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1260](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1261](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b80 .bss
+[1262](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b80 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1263](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b40 .text.startup
+[1264](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006bd0 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[1265](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000520 .xdata.startup
+[1266](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000052c .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[1267](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005ac .pdata.startup
+[1268](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005b8 .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1269](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b58 .ctors.65535
+[1270](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006be8 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1271](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
-[1272](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST__
-[1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
-[1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
-[1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
-[1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 ___DTOR_LIST__
-[1278](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
-[1279](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006670 printf
-[1280](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
-[1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
-[1282](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068d8 SetUnhandledExceptionFilter
-[1283](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066d0 _vsnprintf
-[1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
-[1285](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a0 _lock
-[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066d8 _mkdir
-[1287](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
-[1288](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000640 .refptr.__native_startup_state
-[1289](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
-[1290](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006928 GetLastError
-[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006920 GetSystemTimeAsFileTime
-[1293](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000820 mingw_initltssuo_force
-[1294](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_start
-[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
-[1296](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a8 __iob_func
-[1298](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
-[1299](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
-[1300](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
-[1301](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
-[1302](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
-[1303](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
-[1304](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005d0 .refptr.__CTOR_LIST__
-[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068b0 VirtualQuery
-[1306](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
-[1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
-[1308](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
-[1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
-[1310](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006678 perror
-[1312](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005f0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
-[1313](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000860 __mingw_oldexcpt_handler
-[1314](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
-[1315](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006680 malloc
-[1316](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006938 GetCurrentProcessId
-[1317](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
-[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068c8 TlsGetValue
-[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068d0 TerminateProcess
-[1320](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
-[1321](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068e8 RtlLookupFunctionEntry
-[1323](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
-[1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
-[1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
-[1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
-[1327](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068b8 VirtualProtect
-[1328](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000830 mingw_app_type
-[1329](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
-[1330](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
-[1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
-[1332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066c8 abort
-[1333](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005e0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
-[1334](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
-[1335](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
-[1336](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
-[1337](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
-[1338](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006948 EnterCriticalSection
-[1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000670 .refptr.__xi_a
-[1340](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
-[1341](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005c0 .refptr._CRT_MT
-[1342](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068f0 RtlCaptureContext
-[1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
-[1344](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
-[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066c0 calloc
-[1346](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001a0 _tls_used
-[1347](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068c0 UnhandledExceptionFilter
-[1348](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
-[1349](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST__
-[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066a0 fprintf
-[1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
-[1352](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000041a0 Sleep
-[1353](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
-[1354](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
-[1355](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 __CTOR_LIST__
-[1356](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
-[1357](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b90 __bss_end__
-[1358](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006918 GetTickCount
-[1360](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
-[1361](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
-[1362](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068f8 RtlAddFunctionTable
-[1364](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000630 .refptr.__native_startup_lock
-[1365](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
-[1366](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000082c _tls_index
-[1367](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006668 signal
-[1368](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b80 __native_startup_state
-[1369](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
-[1370](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
-[1371](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006658 strncmp
-[1372](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
-[1373](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
-[1374](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 ___CTOR_LIST__
-[1375](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000600 .refptr.__dyn_tls_init_callback
-[1376](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
-[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006688 log10
-[1378](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
-[1379](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006890 realloc
-[1380](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
-[1381](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
-[1382](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
-[1383](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
-[1384](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
-[1385](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
-[1386](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
-[1387](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006910 InitializeCriticalSection
-[1388](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
-[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066a8 fopen
-[1390](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
-[1391](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066b0 fclose
-[1393](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
-[1394](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
-[1395](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
-[1396](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
-[1397](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
-[1398](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000690 .refptr.mingw_app_type
-[1399](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
-[1400](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 __DTOR_LIST__
-[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068e0 RtlVirtualUnwind
-[1402](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
-[1403](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
-[1404](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
-[1405](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006908 LeaveCriticalSection
-[1406](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
-[1407](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
-[1408](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
-[1409](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
-[1410](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1411](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066f0 _amsg_exit
-[1412](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
-[1413](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
-[1414](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006940 GetCurrentProcess
-[1415](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
-[1416](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ac0 __setusermatherr
-[1417](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
-[1418](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
-[1419](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
-[1420](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1421](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006900 QueryPerformanceCounter
-[1422](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
-[1423](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
-[1424](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000824 mingw_initltsdyn_force
-[1425](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
-[1426](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
-[1427](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000180 __dyn_tls_init_callback
-[1428](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000610 .refptr.__image_base__
-[1429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e0 _initterm
-[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006690 fwrite
-[1431](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
-[1432](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
-[1433](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
-[1434](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
-[1435](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1436](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000054b0 ___chkstk_ms
-[1437](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b88 __native_startup_lock
-[1438](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000620 .refptr.__native_dllmain_reason
-[1439](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
-[1440](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006930 GetCurrentThreadId
-[1441](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_end
-[1442](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066b8 exit
-[1443](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
-[1444](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
-[1445](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
-[1446](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e8 _errno
-[1447](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000828 mingw_initltsdrot_force
-[1448](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
-[1449](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000650 .refptr.__xc_a
-[1450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006660 strlen
-[1451](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000680 .refptr.__xi_z
-[1452](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006950 DeleteCriticalSection
-[1453](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
-[1454](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST_END__
-[1455](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
-[1456](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006898 _unlock
-[1457](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
-[1458](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000660 .refptr.__xc_z
-[1459](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1460](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006650 vfprintf
-[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006698 free
-[1462](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
+[1272](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
+[1273](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST__
+[1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
+[1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
+[1276](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
+[1277](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
+[1278](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf8 ___DTOR_LIST__
+[1279](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
+[1280](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006700 printf
+[1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
+[1282](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
+[1283](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006968 SetUnhandledExceptionFilter
+[1284](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006760 _vsnprintf
+[1285](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
+[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006930 _lock
+[1287](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006768 _mkdir
+[1288](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
+[1289](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000640 .refptr.__native_startup_state
+[1290](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
+[1291](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
+[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069b8 GetLastError
+[1293](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069b0 GetSystemTimeAsFileTime
+[1294](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000820 mingw_initltssuo_force
+[1295](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_start
+[1296](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
+[1297](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
+[1298](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006938 __iob_func
+[1299](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
+[1300](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
+[1301](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
+[1302](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
+[1303](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
+[1304](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
+[1305](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005d0 .refptr.__CTOR_LIST__
+[1306](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006940 VirtualQuery
+[1307](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
+[1308](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
+[1309](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
+[1310](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
+[1311](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
+[1312](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006708 perror
+[1313](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005f0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[1314](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000860 __mingw_oldexcpt_handler
+[1315](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
+[1316](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006710 malloc
+[1317](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069c8 GetCurrentProcessId
+[1318](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
+[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006958 TlsGetValue
+[1320](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006960 TerminateProcess
+[1321](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
+[1322](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
+[1323](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006978 RtlLookupFunctionEntry
+[1324](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
+[1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
+[1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
+[1327](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
+[1328](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006948 VirtualProtect
+[1329](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000830 mingw_app_type
+[1330](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
+[1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
+[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
+[1333](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006758 abort
+[1334](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005e0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[1335](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
+[1336](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
+[1337](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
+[1338](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
+[1339](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069d8 EnterCriticalSection
+[1340](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000670 .refptr.__xi_a
+[1341](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
+[1342](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005c0 .refptr._CRT_MT
+[1343](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006980 RtlCaptureContext
+[1344](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
+[1345](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
+[1346](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006750 calloc
+[1347](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001a0 _tls_used
+[1348](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006950 UnhandledExceptionFilter
+[1349](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
+[1350](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST__
+[1351](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006730 fprintf
+[1352](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
+[1353](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000004230 Sleep
+[1354](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
+[1355](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
+[1356](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be0 __CTOR_LIST__
+[1357](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
+[1358](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b90 __bss_end__
+[1359](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
+[1360](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069a8 GetTickCount
+[1361](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
+[1362](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
+[1363](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
+[1364](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006988 RtlAddFunctionTable
+[1365](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000630 .refptr.__native_startup_lock
+[1366](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
+[1367](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000082c _tls_index
+[1368](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066f8 signal
+[1369](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b80 __native_startup_state
+[1370](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
+[1371](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
+[1372](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e8 strncmp
+[1373](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
+[1374](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
+[1375](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be0 ___CTOR_LIST__
+[1376](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000600 .refptr.__dyn_tls_init_callback
+[1377](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
+[1378](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006718 log10
+[1379](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
+[1380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006920 realloc
+[1381](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
+[1382](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
+[1383](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
+[1384](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
+[1385](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
+[1386](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
+[1387](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
+[1388](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069a0 InitializeCriticalSection
+[1389](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
+[1390](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006738 fopen
+[1391](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
+[1392](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
+[1393](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006740 fclose
+[1394](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
+[1395](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
+[1396](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
+[1397](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
+[1398](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
+[1399](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000690 .refptr.mingw_app_type
+[1400](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
+[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf8 __DTOR_LIST__
+[1402](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006970 RtlVirtualUnwind
+[1403](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
+[1404](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
+[1405](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
+[1406](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006998 LeaveCriticalSection
+[1407](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
+[1408](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
+[1409](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
+[1410](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
+[1411](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
+[1412](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006780 _amsg_exit
+[1413](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
+[1414](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
+[1415](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069d0 GetCurrentProcess
+[1416](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
+[1417](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b50 __setusermatherr
+[1418](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
+[1419](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
+[1420](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
+[1421](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
+[1422](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006990 QueryPerformanceCounter
+[1423](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
+[1424](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
+[1425](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000824 mingw_initltsdyn_force
+[1426](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
+[1427](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
+[1428](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000180 __dyn_tls_init_callback
+[1429](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000610 .refptr.__image_base__
+[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006770 _initterm
+[1431](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006720 fwrite
+[1432](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
+[1433](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
+[1434](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
+[1435](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
+[1436](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
+[1437](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000005540 ___chkstk_ms
+[1438](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b88 __native_startup_lock
+[1439](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000620 .refptr.__native_dllmain_reason
+[1440](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
+[1441](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069c0 GetCurrentThreadId
+[1442](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_end
+[1443](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006748 exit
+[1444](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
+[1445](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
+[1446](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
+[1447](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006778 _errno
+[1448](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000828 mingw_initltsdrot_force
+[1449](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
+[1450](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000650 .refptr.__xc_a
+[1451](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066f0 strlen
+[1452](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000680 .refptr.__xi_z
+[1453](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000069e0 DeleteCriticalSection
+[1454](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
+[1455](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST_END__
+[1456](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
+[1457](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006928 _unlock
+[1458](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
+[1459](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000660 .refptr.__xc_z
+[1460](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
+[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e0 vfprintf
+[1462](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006728 free
+[1463](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
 
 
 
 Disassembly of section .text:
 
 00000000646c1000 <pre_c_init>:
     646c1000:	lea    0xaff9(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c1007:	jmp    646c7700 <_initialize_onexit_table>
+    646c1007:	jmp    646c7790 <_initialize_onexit_table>
     646c100c:	nopl   0x0(%rax)
 
 00000000646c1010 <_CRT_INIT>:
     646c1010:	push   %r13
     646c1012:	push   %r12
     646c1014:	push   %rbp
     646c1015:	push   %rdi
@@ -2663,15 +2673,15 @@
     646c1065:	mov    %rax,%rsi
     646c1068:	jne    646c1052 <_CRT_INIT+0x42>
     646c106a:	mov    0x85cf(%rip),%rdi        # 646c9640 <.refptr.__native_startup_state>
     646c1071:	mov    (%rdi),%eax
     646c1073:	cmp    $0x2,%eax
     646c1076:	je     646c1165 <_CRT_INIT+0x155>
     646c107c:	mov    $0x1f,%ecx
-    646c1081:	call   646c76f0 <_amsg_exit>
+    646c1081:	call   646c7780 <_amsg_exit>
     646c1086:	mov    $0x1,%eax
     646c108b:	add    $0x28,%rsp
     646c108f:	pop    %rbx
     646c1090:	pop    %rsi
     646c1091:	pop    %rdi
     646c1092:	pop    %rbp
     646c1093:	pop    %r12
@@ -2732,15 +2742,15 @@
     646c115d:	pop    %rsi
     646c115e:	pop    %rdi
     646c115f:	pop    %rbp
     646c1160:	pop    %r12
     646c1162:	pop    %r13
     646c1164:	ret
     646c1165:	lea    0xae94(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c116c:	call   646c7800 <_execute_onexit_table>
+    646c116c:	call   646c7890 <_execute_onexit_table>
     646c1171:	movl   $0x0,(%rdi)
     646c1177:	xchg   %rsi,(%rbx)
     646c117a:	mov    $0x1,%eax
     646c117f:	add    $0x28,%rsp
     646c1183:	pop    %rbx
     646c1184:	pop    %rsi
     646c1185:	pop    %rdi
@@ -2755,25 +2765,25 @@
     646c11a0:	xor    %eax,%eax
     646c11a2:	xchg   %rax,(%rbx)
     646c11a5:	jmp    646c111e <_CRT_INIT+0x10e>
     646c11aa:	nopw   0x0(%rax,%rax,1)
     646c11b0:	mov    0x84c9(%rip),%rdx        # 646c9680 <.refptr.__xi_z>
     646c11b7:	movl   $0x1,(%rsi)
     646c11bd:	mov    0x84ac(%rip),%rcx        # 646c9670 <.refptr.__xi_a>
-    646c11c4:	call   646c76e0 <_initterm>
+    646c11c4:	call   646c7770 <_initterm>
     646c11c9:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ce:	xchg   %ax,%ax
     646c11d0:	mov    0x8489(%rip),%rdx        # 646c9660 <.refptr.__xc_z>
     646c11d7:	mov    0x8472(%rip),%rcx        # 646c9650 <.refptr.__xc_a>
-    646c11de:	call   646c76e0 <_initterm>
+    646c11de:	call   646c7770 <_initterm>
     646c11e3:	movl   $0x2,(%rsi)
     646c11e9:	jmp    646c1116 <_CRT_INIT+0x106>
     646c11ee:	xchg   %ax,%ax
     646c11f0:	mov    $0x1f,%ecx
-    646c11f5:	call   646c76f0 <_amsg_exit>
+    646c11f5:	call   646c7780 <_amsg_exit>
     646c11fa:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ff:	nop
 
 00000000646c1200 <__DllMainCRTStartup>:
     646c1200:	push   %r12
     646c1202:	push   %rbp
     646c1203:	push   %rdi
@@ -2786,23 +2796,23 @@
     646c1216:	mov    %edx,%ebx
     646c1218:	mov    %edx,(%rsi)
     646c121a:	mov    %r8,%rbp
     646c121d:	jne    646c1273 <__DllMainCRTStartup+0x73>
     646c121f:	mov    0xadf3(%rip),%eax        # 646cc018 <__proc_attached>
     646c1225:	test   %eax,%eax
     646c1227:	je     646c125c <__DllMainCRTStartup+0x5c>
-    646c1229:	call   646c5710 <_pei386_runtime_relocator>
+    646c1229:	call   646c57a0 <_pei386_runtime_relocator>
     646c122e:	mov    %rbp,%r8
     646c1231:	xor    %edx,%edx
     646c1233:	mov    %rdi,%rcx
-    646c1236:	call   646c6500 <DllMain>
+    646c1236:	call   646c6590 <DllMain>
     646c123b:	mov    %rbp,%r8
     646c123e:	mov    %ebx,%edx
     646c1240:	mov    %rdi,%rcx
-    646c1243:	call   646c64f0 <DllEntryPoint>
+    646c1243:	call   646c6580 <DllEntryPoint>
     646c1248:	mov    %rbp,%r8
     646c124b:	mov    %ebx,%edx
     646c124d:	mov    %rdi,%rcx
     646c1250:	mov    %eax,%r12d
     646c1253:	call   646c1010 <_CRT_INIT>
     646c1258:	test   %eax,%eax
     646c125a:	jne    646c125f <__DllMainCRTStartup+0x5f>
@@ -2812,58 +2822,58 @@
     646c1268:	add    $0x20,%rsp
     646c126c:	pop    %rbx
     646c126d:	pop    %rsi
     646c126e:	pop    %rdi
     646c126f:	pop    %rbp
     646c1270:	pop    %r12
     646c1272:	ret
-    646c1273:	call   646c5710 <_pei386_runtime_relocator>
+    646c1273:	call   646c57a0 <_pei386_runtime_relocator>
     646c1278:	lea    -0x1(%rbx),%eax
     646c127b:	cmp    $0x1,%eax
     646c127e:	jbe    646c12a0 <__DllMainCRTStartup+0xa0>
     646c1280:	mov    %rbp,%r8
     646c1283:	mov    %ebx,%edx
     646c1285:	mov    %rdi,%rcx
-    646c1288:	call   646c6500 <DllMain>
+    646c1288:	call   646c6590 <DllMain>
     646c128d:	cmp    $0x3,%ebx
     646c1290:	mov    %eax,%r12d
     646c1293:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c1295:	jmp    646c123b <__DllMainCRTStartup+0x3b>
     646c1297:	nopw   0x0(%rax,%rax,1)
     646c12a0:	mov    %rbp,%r8
     646c12a3:	mov    %ebx,%edx
     646c12a5:	mov    %rdi,%rcx
     646c12a8:	call   646c1010 <_CRT_INIT>
     646c12ad:	test   %eax,%eax
     646c12af:	je     646c125c <__DllMainCRTStartup+0x5c>
     646c12b1:	mov    %rbp,%r8
     646c12b4:	mov    %ebx,%edx
     646c12b6:	mov    %rdi,%rcx
-    646c12b9:	call   646c64f0 <DllEntryPoint>
+    646c12b9:	call   646c6580 <DllEntryPoint>
     646c12be:	test   %eax,%eax
     646c12c0:	mov    %eax,%r12d
     646c12c3:	je     646c1320 <__DllMainCRTStartup+0x120>
     646c12c5:	cmp    $0x1,%ebx
     646c12c8:	jne    646c1280 <__DllMainCRTStartup+0x80>
-    646c12ca:	call   646c5260 <__main>
+    646c12ca:	call   646c52f0 <__main>
     646c12cf:	mov    %rbp,%r8
     646c12d2:	mov    $0x1,%edx
     646c12d7:	mov    %rdi,%rcx
-    646c12da:	call   646c6500 <DllMain>
+    646c12da:	call   646c6590 <DllMain>
     646c12df:	test   %eax,%eax
     646c12e1:	mov    %eax,%r12d
     646c12e4:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c12ea:	mov    %rbp,%r8
     646c12ed:	xor    %edx,%edx
     646c12ef:	mov    %rdi,%rcx
-    646c12f2:	call   646c6500 <DllMain>
+    646c12f2:	call   646c6590 <DllMain>
     646c12f7:	mov    %rbp,%r8
     646c12fa:	xor    %edx,%edx
     646c12fc:	mov    %rdi,%rcx
-    646c12ff:	call   646c64f0 <DllEntryPoint>
+    646c12ff:	call   646c6580 <DllEntryPoint>
     646c1304:	mov    %rbp,%r8
     646c1307:	xor    %edx,%edx
     646c1309:	mov    %rdi,%rcx
     646c130c:	call   646c1010 <_CRT_INIT>
     646c1311:	jmp    646c125f <__DllMainCRTStartup+0x5f>
     646c1316:	cs nopw 0x0(%rax,%rax,1)
     646c1320:	cmp    $0x1,%ebx
@@ -2879,27 +2889,27 @@
     646c1344:	je     646c1350 <DllMainCRTStartup+0x20>
     646c1346:	add    $0x48,%rsp
     646c134a:	jmp    646c1200 <__DllMainCRTStartup>
     646c134f:	nop
     646c1350:	mov    %r8,0x38(%rsp)
     646c1355:	mov    %edx,0x34(%rsp)
     646c1359:	mov    %rcx,0x28(%rsp)
-    646c135e:	call   646c5280 <__security_init_cookie>
-    646c1363:	call   646c5b70 <__mingw_init_ehandler>
+    646c135e:	call   646c5310 <__security_init_cookie>
+    646c1363:	call   646c5c00 <__mingw_init_ehandler>
     646c1368:	mov    0x38(%rsp),%r8
     646c136d:	mov    0x34(%rsp),%edx
     646c1371:	mov    0x28(%rsp),%rcx
     646c1376:	add    $0x48,%rsp
     646c137a:	jmp    646c1200 <__DllMainCRTStartup>
     646c137f:	nop
 
 00000000646c1380 <atexit>:
     646c1380:	mov    %rcx,%rdx
     646c1383:	lea    0xac76(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c138a:	jmp    646c7730 <_register_onexit_function>
+    646c138a:	jmp    646c77c0 <_register_onexit_function>
     646c138f:	nop
 
 00000000646c1390 <__gcc_register_frame>:
     646c1390:	lea    0x9(%rip),%rcx        # 646c13a0 <__gcc_deregister_frame>
     646c1397:	jmp    646c1380 <atexit>
     646c139c:	nopl   0x0(%rax)
 
@@ -3933,15 +3943,15 @@
     646c227e:	lea    0x0(,%rax,4),%rdx
     646c2286:	mov    0x10(%rbp),%rax
     646c228a:	add    %rdx,%rax
     646c228d:	mov    (%rax),%eax
     646c228f:	cvtsi2sd %eax,%xmm0
     646c2293:	subsd  0x20(%rbp),%xmm0
     646c2298:	movsd  0x6d80(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c22a0:	call   646c6c70 <pow>
+    646c22a0:	call   646c6d00 <pow>
     646c22a5:	movapd %xmm0,%xmm1
     646c22a9:	movsd  -0x8(%rbp),%xmm0
     646c22ae:	addsd  %xmm1,%xmm0
     646c22b2:	movsd  %xmm0,-0x8(%rbp)
     646c22b7:	addl   $0x1,-0xc(%rbp)
     646c22bb:	mov    -0xc(%rbp),%eax
     646c22be:	cmp    0x18(%rbp),%eax
@@ -3971,15 +3981,15 @@
     646c230c:	lea    0x0(,%rax,8),%rdx
     646c2314:	mov    0x10(%rbp),%rax
     646c2318:	add    %rdx,%rax
     646c231b:	mov    (%rax),%rax
     646c231e:	cvtsi2sd %rax,%xmm0
     646c2323:	subsd  0x20(%rbp),%xmm0
     646c2328:	movsd  0x6cf0(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2330:	call   646c6c70 <pow>
+    646c2330:	call   646c6d00 <pow>
     646c2335:	movapd %xmm0,%xmm1
     646c2339:	movsd  -0x8(%rbp),%xmm0
     646c233e:	addsd  %xmm1,%xmm0
     646c2342:	movsd  %xmm0,-0x8(%rbp)
     646c2347:	addl   $0x1,-0xc(%rbp)
     646c234b:	mov    -0xc(%rbp),%eax
     646c234e:	cmp    0x18(%rbp),%eax
@@ -4009,15 +4019,15 @@
     646c239c:	lea    0x0(,%rax,4),%rdx
     646c23a4:	mov    0x10(%rbp),%rax
     646c23a8:	add    %rdx,%rax
     646c23ab:	movss  (%rax),%xmm0
     646c23af:	cvtss2sd %xmm0,%xmm0
     646c23b3:	subsd  0x20(%rbp),%xmm0
     646c23b8:	movsd  0x6c60(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c23c0:	call   646c6c70 <pow>
+    646c23c0:	call   646c6d00 <pow>
     646c23c5:	movapd %xmm0,%xmm1
     646c23c9:	movsd  -0x8(%rbp),%xmm0
     646c23ce:	addsd  %xmm1,%xmm0
     646c23d2:	movsd  %xmm0,-0x8(%rbp)
     646c23d7:	addl   $0x1,-0xc(%rbp)
     646c23db:	mov    -0xc(%rbp),%eax
     646c23de:	cmp    0x18(%rbp),%eax
@@ -4046,15 +4056,15 @@
     646c242a:	cltq
     646c242c:	lea    0x0(,%rax,8),%rdx
     646c2434:	mov    0x10(%rbp),%rax
     646c2438:	add    %rdx,%rax
     646c243b:	movsd  (%rax),%xmm0
     646c243f:	subsd  0x20(%rbp),%xmm0
     646c2444:	movsd  0x6bd4(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c244c:	call   646c6c70 <pow>
+    646c244c:	call   646c6d00 <pow>
     646c2451:	movapd %xmm0,%xmm1
     646c2455:	movsd  -0x8(%rbp),%xmm0
     646c245a:	addsd  %xmm1,%xmm0
     646c245e:	movsd  %xmm0,-0x8(%rbp)
     646c2463:	addl   $0x1,-0xc(%rbp)
     646c2467:	mov    -0xc(%rbp),%eax
     646c246a:	cmp    0x18(%rbp),%eax
@@ -4084,27 +4094,27 @@
     646c24b8:	lea    0x0(,%rax,4),%rdx
     646c24c0:	mov    0x10(%rbp),%rax
     646c24c4:	add    %rdx,%rax
     646c24c7:	mov    (%rax),%eax
     646c24c9:	cvtsi2sd %eax,%xmm0
     646c24cd:	subsd  0x20(%rbp),%xmm0
     646c24d2:	movsd  0x6b46(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c24da:	call   646c6c70 <pow>
+    646c24da:	call   646c6d00 <pow>
     646c24df:	movapd %xmm0,%xmm1
     646c24e3:	movsd  -0x8(%rbp),%xmm0
     646c24e8:	addsd  %xmm1,%xmm0
     646c24ec:	movsd  %xmm0,-0x8(%rbp)
     646c24f1:	addl   $0x1,-0xc(%rbp)
     646c24f5:	mov    -0xc(%rbp),%eax
     646c24f8:	cmp    0x18(%rbp),%eax
     646c24fb:	jl     646c24b3 <c_array_std_int+0x26>
     646c24fd:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2502:	movsd  -0x8(%rbp),%xmm0
     646c2507:	divsd  %xmm1,%xmm0
-    646c250b:	call   646c6570 <sqrt>
+    646c250b:	call   646c6600 <sqrt>
     646c2510:	movq   %xmm0,%rax
     646c2515:	movq   %rax,%xmm0
     646c251a:	add    $0x30,%rsp
     646c251e:	pop    %rbp
     646c251f:	ret
 
 00000000646c2520 <c_array_std_long_long>:
@@ -4123,27 +4133,27 @@
     646c254b:	lea    0x0(,%rax,8),%rdx
     646c2553:	mov    0x10(%rbp),%rax
     646c2557:	add    %rdx,%rax
     646c255a:	mov    (%rax),%rax
     646c255d:	cvtsi2sd %rax,%xmm0
     646c2562:	subsd  0x20(%rbp),%xmm0
     646c2567:	movsd  0x6ab1(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c256f:	call   646c6c70 <pow>
+    646c256f:	call   646c6d00 <pow>
     646c2574:	movapd %xmm0,%xmm1
     646c2578:	movsd  -0x8(%rbp),%xmm0
     646c257d:	addsd  %xmm1,%xmm0
     646c2581:	movsd  %xmm0,-0x8(%rbp)
     646c2586:	addl   $0x1,-0xc(%rbp)
     646c258a:	mov    -0xc(%rbp),%eax
     646c258d:	cmp    0x18(%rbp),%eax
     646c2590:	jl     646c2546 <c_array_std_long_long+0x26>
     646c2592:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2597:	movsd  -0x8(%rbp),%xmm0
     646c259c:	divsd  %xmm1,%xmm0
-    646c25a0:	call   646c6570 <sqrt>
+    646c25a0:	call   646c6600 <sqrt>
     646c25a5:	movq   %xmm0,%rax
     646c25aa:	movq   %rax,%xmm0
     646c25af:	add    $0x30,%rsp
     646c25b3:	pop    %rbp
     646c25b4:	ret
 
 00000000646c25b5 <c_array_std_float>:
@@ -4162,27 +4172,27 @@
     646c25e0:	lea    0x0(,%rax,4),%rdx
     646c25e8:	mov    0x10(%rbp),%rax
     646c25ec:	add    %rdx,%rax
     646c25ef:	movss  (%rax),%xmm0
     646c25f3:	cvtss2sd %xmm0,%xmm0
     646c25f7:	subsd  0x20(%rbp),%xmm0
     646c25fc:	movsd  0x6a1c(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2604:	call   646c6c70 <pow>
+    646c2604:	call   646c6d00 <pow>
     646c2609:	movapd %xmm0,%xmm1
     646c260d:	movsd  -0x8(%rbp),%xmm0
     646c2612:	addsd  %xmm1,%xmm0
     646c2616:	movsd  %xmm0,-0x8(%rbp)
     646c261b:	addl   $0x1,-0xc(%rbp)
     646c261f:	mov    -0xc(%rbp),%eax
     646c2622:	cmp    0x18(%rbp),%eax
     646c2625:	jl     646c25db <c_array_std_float+0x26>
     646c2627:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c262c:	movsd  -0x8(%rbp),%xmm0
     646c2631:	divsd  %xmm1,%xmm0
-    646c2635:	call   646c6570 <sqrt>
+    646c2635:	call   646c6600 <sqrt>
     646c263a:	movq   %xmm0,%rax
     646c263f:	movq   %rax,%xmm0
     646c2644:	add    $0x30,%rsp
     646c2648:	pop    %rbp
     646c2649:	ret
 
 00000000646c264a <c_array_std_double>:
@@ -4200,27 +4210,27 @@
     646c2673:	cltq
     646c2675:	lea    0x0(,%rax,8),%rdx
     646c267d:	mov    0x10(%rbp),%rax
     646c2681:	add    %rdx,%rax
     646c2684:	movsd  (%rax),%xmm0
     646c2688:	subsd  0x20(%rbp),%xmm0
     646c268d:	movsd  0x698b(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2695:	call   646c6c70 <pow>
+    646c2695:	call   646c6d00 <pow>
     646c269a:	movapd %xmm0,%xmm1
     646c269e:	movsd  -0x8(%rbp),%xmm0
     646c26a3:	addsd  %xmm1,%xmm0
     646c26a7:	movsd  %xmm0,-0x8(%rbp)
     646c26ac:	addl   $0x1,-0xc(%rbp)
     646c26b0:	mov    -0xc(%rbp),%eax
     646c26b3:	cmp    0x18(%rbp),%eax
     646c26b6:	jl     646c2670 <c_array_std_double+0x26>
     646c26b8:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c26bd:	movsd  -0x8(%rbp),%xmm0
     646c26c2:	divsd  %xmm1,%xmm0
-    646c26c6:	call   646c6570 <sqrt>
+    646c26c6:	call   646c6600 <sqrt>
     646c26cb:	movq   %xmm0,%rax
     646c26d0:	movq   %rax,%xmm0
     646c26d5:	add    $0x30,%rsp
     646c26d9:	pop    %rbp
     646c26da:	ret
 
 00000000646c26db <c_array_mean_int>:
@@ -4820,24 +4830,24 @@
     646c2e45:	mov    %rax,-0x18(%rbp)
     646c2e49:	mov    0x10(%rbp),%rcx
     646c2e4d:	call   646c2d5e <mt19937_get_double>
     646c2e52:	movq   %xmm0,%rax
     646c2e57:	mov    %rax,-0x20(%rbp)
     646c2e5b:	mov    -0x18(%rbp),%rax
     646c2e5f:	movq   %rax,%xmm0
-    646c2e64:	call   646c6ab0 <log>
+    646c2e64:	call   646c6b40 <log>
     646c2e69:	movapd %xmm0,%xmm1
     646c2e6d:	movsd  0x61cb(%rip),%xmm0        # 646c9040 <.rdata+0x10>
     646c2e75:	mulsd  %xmm1,%xmm0
-    646c2e79:	call   646c6570 <sqrt>
+    646c2e79:	call   646c6600 <sqrt>
     646c2e7e:	movapd %xmm0,%xmm6
     646c2e82:	movsd  -0x20(%rbp),%xmm1
     646c2e87:	movsd  0x61b9(%rip),%xmm0        # 646c9048 <.rdata+0x18>
     646c2e8f:	mulsd  %xmm1,%xmm0
-    646c2e93:	call   646c6790 <cos>
+    646c2e93:	call   646c6820 <cos>
     646c2e98:	mulsd  %xmm6,%xmm0
     646c2e9c:	movsd  %xmm0,-0x28(%rbp)
     646c2ea1:	movsd  -0x28(%rbp),%xmm0
     646c2ea6:	movq   %xmm0,%rax
     646c2eab:	movq   %rax,%xmm0
     646c2eb0:	movaps -0x10(%rbp),%xmm6
     646c2eb4:	add    $0x50,%rsp
@@ -4915,15 +4925,15 @@
     646c2f9f:	mulsd  %xmm1,%xmm0
     646c2fa3:	mov    0x28(%rbp),%rax
     646c2fa7:	movsd  0x10(%rax),%xmm2
     646c2fac:	mov    0x28(%rbp),%rax
     646c2fb0:	movsd  0x10(%rax),%xmm1
     646c2fb5:	mulsd  %xmm2,%xmm1
     646c2fb9:	divsd  %xmm1,%xmm0
-    646c2fbd:	call   646c68c0 <exp>
+    646c2fbd:	call   646c6950 <exp>
     646c2fc2:	movapd %xmm0,%xmm1
     646c2fc6:	movsd  0x608a(%rip),%xmm0        # 646c9058 <.rdata+0x8>
     646c2fce:	subsd  %xmm1,%xmm0
     646c2fd2:	movsd  %xmm0,-0x18(%rbp)
     646c2fd7:	mov    0x28(%rbp),%rax
     646c2fdb:	movsd  0x18(%rax),%xmm0
     646c2fe0:	movsd  -0x10(%rbp),%xmm1
@@ -4994,15 +5004,15 @@
     646c30da:	mulsd  %xmm1,%xmm0
     646c30de:	mov    0x28(%rbp),%rax
     646c30e2:	movsd  0x10(%rax),%xmm2
     646c30e7:	mov    0x28(%rbp),%rax
     646c30eb:	movsd  0x10(%rax),%xmm1
     646c30f0:	mulsd  %xmm2,%xmm1
     646c30f4:	divsd  %xmm1,%xmm0
-    646c30f8:	call   646c68c0 <exp>
+    646c30f8:	call   646c6950 <exp>
     646c30fd:	movapd %xmm0,%xmm1
     646c3101:	movsd  0x5f4f(%rip),%xmm0        # 646c9058 <.rdata+0x8>
     646c3109:	subsd  %xmm1,%xmm0
     646c310d:	movsd  %xmm0,-0x20(%rbp)
     646c3112:	mov    0x28(%rbp),%rax
     646c3116:	movsd  0x18(%rax),%xmm0
     646c311b:	movsd  -0x18(%rbp),%xmm1
@@ -5058,15 +5068,15 @@
     646c31cc:	cltq
     646c31ce:	mov    0x10(%rbp),%rdx
     646c31d2:	mov    %rax,0x28(%rdx)
     646c31d6:	mov    0x18(%rbp),%eax
     646c31d9:	cltq
     646c31db:	mov    $0x8,%edx
     646c31e0:	mov    %rax,%rcx
-    646c31e3:	call   646c76c0 <calloc>
+    646c31e3:	call   646c7750 <calloc>
     646c31e8:	mov    %rax,%rdx
     646c31eb:	mov    0x10(%rbp),%rax
     646c31ef:	mov    %rdx,0x18(%rax)
     646c31f3:	mov    0x18(%rbp),%eax
     646c31f6:	cltq
     646c31f8:	mov    0x10(%rbp),%rdx
     646c31fc:	mov    %rax,0x38(%rdx)
@@ -5074,15 +5084,15 @@
     646c3203:	cltq
     646c3205:	mov    0x10(%rbp),%rdx
     646c3209:	mov    %rax,0x40(%rdx)
     646c320d:	mov    0x18(%rbp),%eax
     646c3210:	cltq
     646c3212:	mov    $0x8,%edx
     646c3217:	mov    %rax,%rcx
-    646c321a:	call   646c76c0 <calloc>
+    646c321a:	call   646c7750 <calloc>
     646c321f:	mov    %rax,%rdx
     646c3222:	mov    0x10(%rbp),%rax
     646c3226:	mov    %rdx,0x30(%rax)
     646c322a:	nop
     646c322b:	add    $0x20,%rsp
     646c322f:	pop    %rbp
     646c3230:	ret
@@ -5115,101 +5125,101 @@
     646c327d:	mov    -0x28(%rbp),%rax
     646c3281:	movsd  0x10(%rax),%xmm0
     646c3286:	movsd  %xmm0,0x8d9a(%rip)        # 646cc028 <k_range>
     646c328e:	movq   $0xa,0x8dbf(%rip)        # 646cc058 <location+0x8>
     646c3299:	movq   $0xa,0x8dbc(%rip)        # 646cc060 <location+0x10>
     646c32a4:	mov    $0x8,%edx
     646c32a9:	mov    $0xa,%ecx
-    646c32ae:	call   646c76c0 <calloc>
+    646c32ae:	call   646c7750 <calloc>
     646c32b3:	mov    %rax,0x8d96(%rip)        # 646cc050 <location>
     646c32ba:	movq   $0xa,0x8db3(%rip)        # 646cc078 <loc_cov+0x8>
     646c32c5:	movq   $0xa,0x8db0(%rip)        # 646cc080 <loc_cov+0x10>
     646c32d0:	mov    $0x8,%edx
     646c32d5:	mov    $0xa,%ecx
-    646c32da:	call   646c76c0 <calloc>
+    646c32da:	call   646c7750 <calloc>
     646c32df:	mov    %rax,0x8d8a(%rip)        # 646cc070 <loc_cov>
     646c32e6:	movq   $0xa,0x8dc7(%rip)        # 646cc0b8 <loc_cov2+0x8>
     646c32f1:	movq   $0xa,0x8dc4(%rip)        # 646cc0c0 <loc_cov2+0x10>
     646c32fc:	mov    $0x8,%edx
     646c3301:	mov    $0xa,%ecx
-    646c3306:	call   646c76c0 <calloc>
+    646c3306:	call   646c7750 <calloc>
     646c330b:	mov    %rax,0x8d9e(%rip)        # 646cc0b0 <loc_cov2>
     646c3312:	movq   $0xa,0x8ddb(%rip)        # 646cc0f8 <weights+0x8>
     646c331d:	movq   $0xa,0x8dd8(%rip)        # 646cc100 <weights+0x10>
     646c3328:	mov    $0x8,%edx
     646c332d:	mov    $0xa,%ecx
-    646c3332:	call   646c76c0 <calloc>
+    646c3332:	call   646c7750 <calloc>
     646c3337:	mov    %rax,0x8db2(%rip)        # 646cc0f0 <weights>
     646c333e:	movq   $0x64,0x8d8f(%rip)        # 646cc0d8 <flatten_temp+0x8>
     646c3349:	movq   $0x64,0x8d8c(%rip)        # 646cc0e0 <flatten_temp+0x10>
     646c3354:	mov    $0x8,%edx
     646c3359:	mov    $0x64,%ecx
-    646c335e:	call   646c76c0 <calloc>
+    646c335e:	call   646c7750 <calloc>
     646c3363:	mov    %rax,0x8d66(%rip)        # 646cc0d0 <flatten_temp>
     646c336a:	movq   $0xa,0x8d23(%rip)        # 646cc098 <data_temp+0x8>
     646c3375:	movq   $0xa,0x8d20(%rip)        # 646cc0a0 <data_temp+0x10>
     646c3380:	mov    $0x8,%edx
     646c3385:	mov    $0xa,%ecx
-    646c338a:	call   646c76c0 <calloc>
+    646c338a:	call   646c7750 <calloc>
     646c338f:	mov    %rax,0x8cfa(%rip)        # 646cc090 <data_temp>
     646c3396:	movq   $0xa,0x8d97(%rip)        # 646cc138 <pdist_temp+0x8>
     646c33a1:	movq   $0xa,0x8d94(%rip)        # 646cc140 <pdist_temp+0x10>
     646c33ac:	mov    $0x50,%ecx
-    646c33b1:	call   646c7680 <malloc>
+    646c33b1:	call   646c7710 <malloc>
     646c33b6:	mov    %rax,0x8d73(%rip)        # 646cc130 <pdist_temp>
     646c33bd:	movl   $0x0,-0x54(%rbp)
     646c33c4:	jmp    646c33eb <krige_param_setting+0x18e>
     646c33c6:	mov    0x8d63(%rip),%rdx        # 646cc130 <pdist_temp>
     646c33cd:	mov    -0x54(%rbp),%eax
     646c33d0:	cltq
     646c33d2:	shl    $0x3,%rax
     646c33d6:	lea    (%rdx,%rax,1),%rbx
     646c33da:	mov    $0x50,%ecx
-    646c33df:	call   646c7680 <malloc>
+    646c33df:	call   646c7710 <malloc>
     646c33e4:	mov    %rax,(%rbx)
     646c33e7:	addl   $0x1,-0x54(%rbp)
     646c33eb:	cmpl   $0x9,-0x54(%rbp)
     646c33ef:	jle    646c33c6 <krige_param_setting+0x169>
     646c33f1:	movq   $0xa,0x8d5c(%rip)        # 646cc158 <datacov+0x8>
     646c33fc:	movq   $0xa,0x8d59(%rip)        # 646cc160 <datacov+0x10>
     646c3407:	mov    $0x50,%ecx
-    646c340c:	call   646c7680 <malloc>
+    646c340c:	call   646c7710 <malloc>
     646c3411:	mov    %rax,0x8d38(%rip)        # 646cc150 <datacov>
     646c3418:	movl   $0x0,-0x58(%rbp)
     646c341f:	jmp    646c3446 <krige_param_setting+0x1e9>
     646c3421:	mov    0x8d28(%rip),%rdx        # 646cc150 <datacov>
     646c3428:	mov    -0x58(%rbp),%eax
     646c342b:	cltq
     646c342d:	shl    $0x3,%rax
     646c3431:	lea    (%rdx,%rax,1),%rbx
     646c3435:	mov    $0x50,%ecx
-    646c343a:	call   646c7680 <malloc>
+    646c343a:	call   646c7710 <malloc>
     646c343f:	mov    %rax,(%rbx)
     646c3442:	addl   $0x1,-0x58(%rbp)
     646c3446:	cmpl   $0x9,-0x58(%rbp)
     646c344a:	jle    646c3421 <krige_param_setting+0x1c4>
     646c344c:	mov    -0x30(%rbp),%eax
     646c344f:	cltq
     646c3451:	mov    %rax,0x8cc0(%rip)        # 646cc118 <array2d_temp+0x8>
     646c3458:	movq   $0x3,0x8cbd(%rip)        # 646cc120 <array2d_temp+0x10>
     646c3463:	mov    -0x30(%rbp),%eax
     646c3466:	cltq
     646c3468:	shl    $0x3,%rax
     646c346c:	mov    %rax,%rcx
-    646c346f:	call   646c7680 <malloc>
+    646c346f:	call   646c7710 <malloc>
     646c3474:	mov    %rax,0x8c95(%rip)        # 646cc110 <array2d_temp>
     646c347b:	movl   $0x0,-0x5c(%rbp)
     646c3482:	jmp    646c34a9 <krige_param_setting+0x24c>
     646c3484:	mov    0x8c85(%rip),%rdx        # 646cc110 <array2d_temp>
     646c348b:	mov    -0x5c(%rbp),%eax
     646c348e:	cltq
     646c3490:	shl    $0x3,%rax
     646c3494:	lea    (%rdx,%rax,1),%rbx
     646c3498:	mov    $0x18,%ecx
-    646c349d:	call   646c7680 <malloc>
+    646c349d:	call   646c7710 <malloc>
     646c34a2:	mov    %rax,(%rbx)
     646c34a5:	addl   $0x1,-0x5c(%rbp)
     646c34a9:	mov    -0x5c(%rbp),%eax
     646c34ac:	cmp    -0x30(%rbp),%eax
     646c34af:	jl     646c3484 <krige_param_setting+0x227>
     646c34b1:	nop
     646c34b2:	add    $0x38,%rsp
@@ -5226,18 +5236,18 @@
     646c34c9:	mov    %rdx,0x18(%rbp)
     646c34cd:	mov    %r8,0x20(%rbp)
     646c34d1:	mov    0x20(%rbp),%rdx
     646c34d5:	mov    0x18(%rbp),%rax
     646c34d9:	mov    %rdx,%r8
     646c34dc:	mov    %rax,%rdx
     646c34df:	mov    0x10(%rbp),%rcx
-    646c34e3:	call   646c38c7 <find_neighbor>
+    646c34e3:	call   646c38d0 <find_neighbor>
     646c34e8:	mov    %eax,-0x20(%rbp)
     646c34eb:	cmpl   $0x0,-0x20(%rbp)
-    646c34ef:	je     646c38bc <simple_kriging+0x403>
+    646c34ef:	je     646c38c5 <simple_kriging+0x40c>
     646c34f5:	movl   $0x0,-0x14(%rbp)
     646c34fc:	jmp    646c35bc <simple_kriging+0x103>
     646c3501:	mov    0x18(%rbp),%rax
     646c3505:	mov    0x18(%rax),%rdx
     646c3509:	mov    -0x14(%rbp),%eax
     646c350c:	cltq
     646c350e:	shl    $0x3,%rax
@@ -5290,392 +5300,386 @@
     646c35bc:	mov    0x18(%rbp),%rax
     646c35c0:	mov    0x4(%rax),%eax
     646c35c3:	cmp    %eax,-0x14(%rbp)
     646c35c6:	jl     646c3501 <simple_kriging+0x48>
     646c35cc:	mov    0x18(%rbp),%rax
     646c35d0:	mov    (%rax),%eax
     646c35d2:	cmp    $0x1,%eax
-    646c35d5:	jle    646c35f8 <simple_kriging+0x13f>
+    646c35d5:	jle    646c3601 <simple_kriging+0x148>
     646c35d7:	mov    0x18(%rbp),%rax
-    646c35db:	mov    0x4(%rax),%eax
-    646c35de:	lea    -0x1(%rax),%edx
-    646c35e1:	mov    0x8b28(%rip),%rax        # 646cc110 <array2d_temp>
-    646c35e8:	mov    %edx,%r8d
-    646c35eb:	mov    $0x0,%edx
-    646c35f0:	mov    %rax,%rcx
-    646c35f3:	call   646c4dd5 <quicksort2d>
-    646c35f8:	movl   $0x0,-0x18(%rbp)
-    646c35ff:	jmp    646c3668 <simple_kriging+0x1af>
-    646c3601:	mov    0x8b08(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3608:	mov    -0x18(%rbp),%eax
-    646c360b:	cltq
-    646c360d:	shl    $0x3,%rax
-    646c3611:	add    %rdx,%rax
-    646c3614:	mov    (%rax),%rdx
-    646c3617:	mov    0x8a32(%rip),%rcx        # 646cc050 <location>
-    646c361e:	mov    -0x18(%rbp),%eax
-    646c3621:	cltq
-    646c3623:	shl    $0x3,%rax
-    646c3627:	add    %rcx,%rax
-    646c362a:	movsd  (%rdx),%xmm0
-    646c362e:	movsd  %xmm0,(%rax)
-    646c3632:	mov    0x8ad7(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3639:	mov    -0x18(%rbp),%eax
-    646c363c:	cltq
-    646c363e:	shl    $0x3,%rax
-    646c3642:	add    %rdx,%rax
-    646c3645:	mov    (%rax),%rdx
-    646c3648:	mov    0x8a61(%rip),%rcx        # 646cc0b0 <loc_cov2>
-    646c364f:	mov    -0x18(%rbp),%eax
-    646c3652:	cltq
-    646c3654:	shl    $0x3,%rax
-    646c3658:	add    %rcx,%rax
-    646c365b:	movsd  0x10(%rdx),%xmm0
-    646c3660:	movsd  %xmm0,(%rax)
-    646c3664:	addl   $0x1,-0x18(%rbp)
-    646c3668:	mov    0x18(%rbp),%rax
-    646c366c:	mov    (%rax),%eax
-    646c366e:	cmp    %eax,-0x18(%rbp)
-    646c3671:	jl     646c3601 <simple_kriging+0x148>
-    646c3673:	mov    0x18(%rbp),%rax
-    646c3677:	mov    (%rax),%ecx
-    646c3679:	mov    0x8ab0(%rip),%rdx        # 646cc130 <pdist_temp>
-    646c3680:	mov    0x89c9(%rip),%rax        # 646cc050 <location>
-    646c3687:	mov    %ecx,%r8d
-    646c368a:	mov    %rax,%rcx
-    646c368d:	call   646c43dd <pdist>
-    646c3692:	mov    0x8987(%rip),%r8        # 646cc020 <model>
-    646c3699:	mov    0x18(%rbp),%rax
-    646c369d:	mov    (%rax),%ecx
-    646c369f:	mov    0x8a2a(%rip),%rdx        # 646cc0d0 <flatten_temp>
-    646c36a6:	mov    0x8a83(%rip),%rax        # 646cc130 <pdist_temp>
-    646c36ad:	mov    %r8,%r9
-    646c36b0:	mov    %ecx,%r8d
-    646c36b3:	mov    %rax,%rcx
-    646c36b6:	call   646c302e <cov_model2d>
-    646c36bb:	mov    0x18(%rbp),%rax
-    646c36bf:	mov    (%rax),%ecx
-    646c36c1:	mov    0x8a88(%rip),%rdx        # 646cc150 <datacov>
-    646c36c8:	mov    0x8a01(%rip),%rax        # 646cc0d0 <flatten_temp>
-    646c36cf:	mov    %ecx,%r8d
-    646c36d2:	mov    %rax,%rcx
-    646c36d5:	call   646c4490 <matrixform>
-    646c36da:	mov    0x893f(%rip),%r8        # 646cc020 <model>
-    646c36e1:	mov    0x18(%rbp),%rax
-    646c36e5:	mov    (%rax),%ecx
-    646c36e7:	mov    0x8982(%rip),%rdx        # 646cc070 <loc_cov>
-    646c36ee:	mov    0x89bb(%rip),%rax        # 646cc0b0 <loc_cov2>
-    646c36f5:	mov    %r8,%r9
-    646c36f8:	mov    %ecx,%r8d
-    646c36fb:	mov    %rax,%rcx
-    646c36fe:	call   646c2f24 <cov_model>
-    646c3703:	mov    0x18(%rbp),%rax
-    646c3707:	mov    (%rax),%eax
-    646c3709:	test   %eax,%eax
-    646c370b:	jle    646c3737 <simple_kriging+0x27e>
-    646c370d:	mov    0x18(%rbp),%rax
-    646c3711:	mov    (%rax),%r8d
-    646c3714:	mov    0x89d5(%rip),%rcx        # 646cc0f0 <weights>
-    646c371b:	mov    0x894e(%rip),%rdx        # 646cc070 <loc_cov>
-    646c3722:	mov    0x8a27(%rip),%rax        # 646cc150 <datacov>
-    646c3729:	mov    %r8d,%r9d
-    646c372c:	mov    %rcx,%r8
-    646c372f:	mov    %rax,%rcx
-    646c3732:	call   646c3c1a <lu_inverse_solver>
-    646c3737:	pxor   %xmm0,%xmm0
-    646c373b:	movsd  %xmm0,0x88ed(%rip)        # 646cc030 <estimation>
-    646c3743:	pxor   %xmm0,%xmm0
-    646c3747:	movsd  %xmm0,0x88e9(%rip)        # 646cc038 <krige_var>
-    646c374f:	pxor   %xmm0,%xmm0
-    646c3753:	movsd  %xmm0,0x88e5(%rip)        # 646cc040 <fix>
-    646c375b:	movl   $0x0,-0x1c(%rbp)
-    646c3762:	jmp    646c37fe <simple_kriging+0x345>
-    646c3767:	mov    0x89a2(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c376e:	mov    -0x1c(%rbp),%eax
-    646c3771:	cltq
-    646c3773:	shl    $0x3,%rax
-    646c3777:	add    %rdx,%rax
-    646c377a:	mov    (%rax),%rax
-    646c377d:	add    $0x8,%rax
-    646c3781:	movsd  (%rax),%xmm1
-    646c3785:	mov    0x8964(%rip),%rdx        # 646cc0f0 <weights>
-    646c378c:	mov    -0x1c(%rbp),%eax
-    646c378f:	cltq
-    646c3791:	shl    $0x3,%rax
-    646c3795:	add    %rdx,%rax
-    646c3798:	movsd  (%rax),%xmm0
-    646c379c:	mulsd  %xmm0,%xmm1
-    646c37a0:	movsd  0x8888(%rip),%xmm0        # 646cc030 <estimation>
-    646c37a8:	addsd  %xmm1,%xmm0
-    646c37ac:	movsd  %xmm0,0x887c(%rip)        # 646cc030 <estimation>
-    646c37b4:	mov    0x88b5(%rip),%rdx        # 646cc070 <loc_cov>
-    646c37bb:	mov    -0x1c(%rbp),%eax
-    646c37be:	cltq
-    646c37c0:	shl    $0x3,%rax
-    646c37c4:	add    %rdx,%rax
-    646c37c7:	movsd  (%rax),%xmm1
-    646c37cb:	mov    0x891e(%rip),%rdx        # 646cc0f0 <weights>
-    646c37d2:	mov    -0x1c(%rbp),%eax
-    646c37d5:	cltq
-    646c37d7:	shl    $0x3,%rax
-    646c37db:	add    %rdx,%rax
-    646c37de:	movsd  (%rax),%xmm0
-    646c37e2:	mulsd  %xmm0,%xmm1
-    646c37e6:	movsd  0x884a(%rip),%xmm0        # 646cc038 <krige_var>
-    646c37ee:	addsd  %xmm1,%xmm0
-    646c37f2:	movsd  %xmm0,0x883e(%rip)        # 646cc038 <krige_var>
-    646c37fa:	addl   $0x1,-0x1c(%rbp)
-    646c37fe:	mov    0x18(%rbp),%rax
-    646c3802:	mov    (%rax),%eax
-    646c3804:	cmp    %eax,-0x1c(%rbp)
-    646c3807:	jl     646c3767 <simple_kriging+0x2ae>
-    646c380d:	mov    0x880c(%rip),%rax        # 646cc020 <model>
-    646c3814:	movsd  0x18(%rax),%xmm0
-    646c3819:	movsd  0x8817(%rip),%xmm1        # 646cc038 <krige_var>
-    646c3821:	subsd  %xmm1,%xmm0
-    646c3825:	movsd  %xmm0,0x880b(%rip)        # 646cc038 <krige_var>
-    646c382d:	movsd  0x8803(%rip),%xmm1        # 646cc038 <krige_var>
-    646c3835:	pxor   %xmm0,%xmm0
-    646c3839:	comisd %xmm1,%xmm0
-    646c383d:	jbe    646c384b <simple_kriging+0x392>
-    646c383f:	pxor   %xmm0,%xmm0
-    646c3843:	movsd  %xmm0,0x87ed(%rip)        # 646cc038 <krige_var>
-    646c384b:	mov    0x20(%rbp),%rax
-    646c384f:	mov    %rax,%rcx
-    646c3852:	call   646c2e27 <mt19937_random_normal>
-    646c3857:	movapd %xmm0,%xmm6
-    646c385b:	mov    0x87d6(%rip),%rax        # 646cc038 <krige_var>
-    646c3862:	movsd  0x57f6(%rip),%xmm0        # 646c9060 <.rdata>
-    646c386a:	movapd %xmm0,%xmm1
-    646c386e:	movq   %rax,%xmm0
-    646c3873:	call   646c6c70 <pow>
-    646c3878:	mulsd  %xmm6,%xmm0
-    646c387c:	movsd  %xmm0,0x87bc(%rip)        # 646cc040 <fix>
-    646c3884:	movsd  0x87a4(%rip),%xmm1        # 646cc030 <estimation>
-    646c388c:	movsd  0x87ac(%rip),%xmm0        # 646cc040 <fix>
-    646c3894:	mov    0x18(%rbp),%rax
-    646c3898:	movsd  0x10(%rax),%xmm2
-    646c389d:	cvttsd2si %xmm2,%eax
-    646c38a1:	cltq
-    646c38a3:	lea    0x0(,%rax,8),%rdx
-    646c38ab:	mov    0x10(%rbp),%rax
-    646c38af:	add    %rdx,%rax
-    646c38b2:	addsd  %xmm1,%xmm0
-    646c38b6:	movsd  %xmm0,(%rax)
-    646c38ba:	jmp    646c38bd <simple_kriging+0x404>
-    646c38bc:	nop
-    646c38bd:	movaps -0x10(%rbp),%xmm6
-    646c38c1:	add    $0x40,%rsp
-    646c38c5:	pop    %rbp
-    646c38c6:	ret
-
-00000000646c38c7 <find_neighbor>:
-    646c38c7:	push   %rbp
-    646c38c8:	mov    %rsp,%rbp
-    646c38cb:	sub    $0x30,%rsp
-    646c38cf:	mov    %rcx,0x10(%rbp)
-    646c38d3:	mov    %rdx,0x18(%rbp)
-    646c38d7:	mov    %r8,0x20(%rbp)
-    646c38db:	mov    0x18(%rbp),%rax
-    646c38df:	mov    (%rax),%eax
-    646c38e1:	test   %eax,%eax
-    646c38e3:	jne    646c3956 <find_neighbor+0x8f>
-    646c38e5:	mov    0x20(%rbp),%rax
-    646c38e9:	mov    %rax,%rcx
-    646c38ec:	call   646c2e27 <mt19937_random_normal>
-    646c38f1:	movapd %xmm0,%xmm1
-    646c38f5:	mov    0x8724(%rip),%rax        # 646cc020 <model>
-    646c38fc:	movsd  0x18(%rax),%xmm0
-    646c3901:	mov    0x18(%rbp),%rax
-    646c3905:	movsd  0x10(%rax),%xmm2
-    646c390a:	cvttsd2si %xmm2,%eax
-    646c390e:	cltq
-    646c3910:	lea    0x0(,%rax,8),%rdx
-    646c3918:	mov    0x10(%rbp),%rax
-    646c391c:	add    %rdx,%rax
-    646c391f:	mulsd  %xmm1,%xmm0
-    646c3923:	movsd  %xmm0,(%rax)
-    646c3927:	mov    0x18(%rbp),%rax
-    646c392b:	mov    0x18(%rax),%rdx
-    646c392f:	mov    0x18(%rbp),%rax
-    646c3933:	mov    0x8(%rax),%eax
-    646c3936:	cltq
-    646c3938:	shl    $0x3,%rax
-    646c393c:	add    %rdx,%rax
-    646c393f:	mov    0x18(%rbp),%rdx
-    646c3943:	movsd  0x10(%rdx),%xmm0
-    646c3948:	movsd  %xmm0,(%rax)
-    646c394c:	mov    $0x0,%eax
-    646c3951:	jmp    646c3a75 <find_neighbor+0x1ae>
-    646c3956:	movl   $0x0,-0x4(%rbp)
-    646c395d:	movl   $0x0,-0x8(%rbp)
-    646c3964:	jmp    646c39ec <find_neighbor+0x125>
-    646c3969:	mov    0x18(%rbp),%rax
-    646c396d:	mov    0x18(%rax),%rdx
-    646c3971:	mov    -0x8(%rbp),%eax
-    646c3974:	cltq
-    646c3976:	shl    $0x3,%rax
-    646c397a:	add    %rdx,%rax
-    646c397d:	movsd  (%rax),%xmm0
-    646c3981:	mov    0x18(%rbp),%rax
-    646c3985:	movsd  0x10(%rax),%xmm1
-    646c398a:	subsd  %xmm1,%xmm0
-    646c398e:	mov    0x18(%rbp),%rax
-    646c3992:	mov    0x30(%rax),%rdx
-    646c3996:	mov    -0x8(%rbp),%eax
-    646c3999:	cltq
-    646c399b:	shl    $0x3,%rax
-    646c399f:	add    %rdx,%rax
-    646c39a2:	movq   0x56c6(%rip),%xmm1        # 646c9070 <.rdata+0x10>
-    646c39aa:	andpd  %xmm1,%xmm0
-    646c39ae:	movsd  %xmm0,(%rax)
-    646c39b2:	mov    0x18(%rbp),%rax
-    646c39b6:	mov    0x30(%rax),%rdx
-    646c39ba:	mov    -0x8(%rbp),%eax
-    646c39bd:	cltq
-    646c39bf:	shl    $0x3,%rax
-    646c39c3:	add    %rdx,%rax
-    646c39c6:	movsd  (%rax),%xmm1
-    646c39ca:	movsd  0x8656(%rip),%xmm2        # 646cc028 <k_range>
-    646c39d2:	movsd  0x56a6(%rip),%xmm0        # 646c9080 <.rdata+0x20>
-    646c39da:	mulsd  %xmm2,%xmm0
-    646c39de:	comisd %xmm1,%xmm0
-    646c39e2:	jbe    646c39e8 <find_neighbor+0x121>
-    646c39e4:	addl   $0x1,-0x4(%rbp)
-    646c39e8:	addl   $0x1,-0x8(%rbp)
-    646c39ec:	mov    0x18(%rbp),%rax
-    646c39f0:	mov    0x4(%rax),%eax
-    646c39f3:	cmp    %eax,-0x8(%rbp)
-    646c39f6:	jl     646c3969 <find_neighbor+0xa2>
-    646c39fc:	cmpl   $0x0,-0x4(%rbp)
-    646c3a00:	jne    646c3a70 <find_neighbor+0x1a9>
-    646c3a02:	mov    0x20(%rbp),%rax
-    646c3a06:	mov    %rax,%rcx
-    646c3a09:	call   646c2e27 <mt19937_random_normal>
-    646c3a0e:	movapd %xmm0,%xmm1
-    646c3a12:	mov    0x8607(%rip),%rax        # 646cc020 <model>
-    646c3a19:	movsd  0x18(%rax),%xmm0
-    646c3a1e:	mov    0x18(%rbp),%rax
-    646c3a22:	movsd  0x10(%rax),%xmm2
-    646c3a27:	cvttsd2si %xmm2,%eax
-    646c3a2b:	cltq
-    646c3a2d:	lea    0x0(,%rax,8),%rdx
-    646c3a35:	mov    0x10(%rbp),%rax
-    646c3a39:	add    %rdx,%rax
-    646c3a3c:	mulsd  %xmm1,%xmm0
-    646c3a40:	movsd  %xmm0,(%rax)
-    646c3a44:	mov    0x18(%rbp),%rax
-    646c3a48:	mov    0x18(%rax),%rdx
-    646c3a4c:	mov    0x18(%rbp),%rax
-    646c3a50:	mov    0x8(%rax),%eax
-    646c3a53:	cltq
-    646c3a55:	shl    $0x3,%rax
-    646c3a59:	add    %rdx,%rax
-    646c3a5c:	mov    0x18(%rbp),%rdx
-    646c3a60:	movsd  0x10(%rdx),%xmm0
-    646c3a65:	movsd  %xmm0,(%rax)
-    646c3a69:	mov    $0x0,%eax
-    646c3a6e:	jmp    646c3a75 <find_neighbor+0x1ae>
-    646c3a70:	mov    $0x1,%eax
-    646c3a75:	add    $0x30,%rsp
-    646c3a79:	pop    %rbp
-    646c3a7a:	ret
-
-00000000646c3a7b <krige_memory_free>:
-    646c3a7b:	push   %rbp
-    646c3a7c:	mov    %rsp,%rbp
-    646c3a7f:	sub    $0x30,%rsp
-    646c3a83:	mov    0x85c6(%rip),%rax        # 646cc050 <location>
-    646c3a8a:	mov    %rax,%rcx
-    646c3a8d:	call   646c7698 <free>
-    646c3a92:	mov    0x85d7(%rip),%rax        # 646cc070 <loc_cov>
-    646c3a99:	mov    %rax,%rcx
-    646c3a9c:	call   646c7698 <free>
-    646c3aa1:	mov    0x85e8(%rip),%rax        # 646cc090 <data_temp>
-    646c3aa8:	mov    %rax,%rcx
-    646c3aab:	call   646c7698 <free>
-    646c3ab0:	mov    0x85f9(%rip),%rax        # 646cc0b0 <loc_cov2>
-    646c3ab7:	mov    %rax,%rcx
-    646c3aba:	call   646c7698 <free>
-    646c3abf:	mov    0x860a(%rip),%rax        # 646cc0d0 <flatten_temp>
-    646c3ac6:	mov    %rax,%rcx
-    646c3ac9:	call   646c7698 <free>
-    646c3ace:	mov    0x861b(%rip),%rax        # 646cc0f0 <weights>
-    646c3ad5:	mov    %rax,%rcx
-    646c3ad8:	call   646c7698 <free>
-    646c3add:	movl   $0x0,-0x4(%rbp)
-    646c3ae4:	jmp    646c3b08 <krige_memory_free+0x8d>
-    646c3ae6:	mov    0x8623(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3aed:	mov    -0x4(%rbp),%eax
-    646c3af0:	cltq
-    646c3af2:	shl    $0x3,%rax
-    646c3af6:	add    %rdx,%rax
-    646c3af9:	mov    (%rax),%rax
-    646c3afc:	mov    %rax,%rcx
-    646c3aff:	call   646c7698 <free>
-    646c3b04:	addl   $0x1,-0x4(%rbp)
-    646c3b08:	mov    -0x4(%rbp),%eax
-    646c3b0b:	cltq
-    646c3b0d:	mov    0x8604(%rip),%rdx        # 646cc118 <array2d_temp+0x8>
-    646c3b14:	cmp    %rdx,%rax
-    646c3b17:	jb     646c3ae6 <krige_memory_free+0x6b>
-    646c3b19:	mov    0x85f0(%rip),%rax        # 646cc110 <array2d_temp>
-    646c3b20:	mov    %rax,%rcx
-    646c3b23:	call   646c7698 <free>
-    646c3b28:	movl   $0x0,-0x8(%rbp)
-    646c3b2f:	jmp    646c3b53 <krige_memory_free+0xd8>
-    646c3b31:	mov    0x85f8(%rip),%rdx        # 646cc130 <pdist_temp>
-    646c3b38:	mov    -0x8(%rbp),%eax
-    646c3b3b:	cltq
-    646c3b3d:	shl    $0x3,%rax
-    646c3b41:	add    %rdx,%rax
-    646c3b44:	mov    (%rax),%rax
-    646c3b47:	mov    %rax,%rcx
-    646c3b4a:	call   646c7698 <free>
-    646c3b4f:	addl   $0x1,-0x8(%rbp)
-    646c3b53:	mov    -0x8(%rbp),%eax
-    646c3b56:	cltq
-    646c3b58:	mov    0x85d9(%rip),%rdx        # 646cc138 <pdist_temp+0x8>
-    646c3b5f:	cmp    %rdx,%rax
-    646c3b62:	jb     646c3b31 <krige_memory_free+0xb6>
-    646c3b64:	mov    0x85c5(%rip),%rax        # 646cc130 <pdist_temp>
-    646c3b6b:	mov    %rax,%rcx
-    646c3b6e:	call   646c7698 <free>
-    646c3b73:	movl   $0x0,-0xc(%rbp)
-    646c3b7a:	jmp    646c3b9e <krige_memory_free+0x123>
-    646c3b7c:	mov    0x85cd(%rip),%rdx        # 646cc150 <datacov>
-    646c3b83:	mov    -0xc(%rbp),%eax
-    646c3b86:	cltq
-    646c3b88:	shl    $0x3,%rax
-    646c3b8c:	add    %rdx,%rax
-    646c3b8f:	mov    (%rax),%rax
-    646c3b92:	mov    %rax,%rcx
-    646c3b95:	call   646c7698 <free>
-    646c3b9a:	addl   $0x1,-0xc(%rbp)
-    646c3b9e:	mov    -0xc(%rbp),%eax
-    646c3ba1:	cltq
-    646c3ba3:	mov    0x85ae(%rip),%rdx        # 646cc158 <datacov+0x8>
-    646c3baa:	cmp    %rdx,%rax
-    646c3bad:	jb     646c3b7c <krige_memory_free+0x101>
-    646c3baf:	mov    0x859a(%rip),%rax        # 646cc150 <datacov>
-    646c3bb6:	mov    %rax,%rcx
-    646c3bb9:	call   646c7698 <free>
-    646c3bbe:	nop
-    646c3bbf:	add    $0x30,%rsp
-    646c3bc3:	pop    %rbp
-    646c3bc4:	ret
-    646c3bc5:	nop
-    646c3bc6:	nop
+    646c35db:	mov    (%rax),%ecx
+    646c35dd:	mov    0x18(%rbp),%rax
+    646c35e1:	mov    0x4(%rax),%eax
+    646c35e4:	lea    -0x1(%rax),%edx
+    646c35e7:	mov    0x8b22(%rip),%rax        # 646cc110 <array2d_temp>
+    646c35ee:	mov    %ecx,%r9d
+    646c35f1:	mov    %edx,%r8d
+    646c35f4:	mov    $0x0,%edx
+    646c35f9:	mov    %rax,%rcx
+    646c35fc:	call   646c4e39 <quickselect2d>
+    646c3601:	movl   $0x0,-0x18(%rbp)
+    646c3608:	jmp    646c3671 <simple_kriging+0x1b8>
+    646c360a:	mov    0x8aff(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3611:	mov    -0x18(%rbp),%eax
+    646c3614:	cltq
+    646c3616:	shl    $0x3,%rax
+    646c361a:	add    %rdx,%rax
+    646c361d:	mov    (%rax),%rdx
+    646c3620:	mov    0x8a29(%rip),%rcx        # 646cc050 <location>
+    646c3627:	mov    -0x18(%rbp),%eax
+    646c362a:	cltq
+    646c362c:	shl    $0x3,%rax
+    646c3630:	add    %rcx,%rax
+    646c3633:	movsd  (%rdx),%xmm0
+    646c3637:	movsd  %xmm0,(%rax)
+    646c363b:	mov    0x8ace(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3642:	mov    -0x18(%rbp),%eax
+    646c3645:	cltq
+    646c3647:	shl    $0x3,%rax
+    646c364b:	add    %rdx,%rax
+    646c364e:	mov    (%rax),%rdx
+    646c3651:	mov    0x8a58(%rip),%rcx        # 646cc0b0 <loc_cov2>
+    646c3658:	mov    -0x18(%rbp),%eax
+    646c365b:	cltq
+    646c365d:	shl    $0x3,%rax
+    646c3661:	add    %rcx,%rax
+    646c3664:	movsd  0x10(%rdx),%xmm0
+    646c3669:	movsd  %xmm0,(%rax)
+    646c366d:	addl   $0x1,-0x18(%rbp)
+    646c3671:	mov    0x18(%rbp),%rax
+    646c3675:	mov    (%rax),%eax
+    646c3677:	cmp    %eax,-0x18(%rbp)
+    646c367a:	jl     646c360a <simple_kriging+0x151>
+    646c367c:	mov    0x18(%rbp),%rax
+    646c3680:	mov    (%rax),%ecx
+    646c3682:	mov    0x8aa7(%rip),%rdx        # 646cc130 <pdist_temp>
+    646c3689:	mov    0x89c0(%rip),%rax        # 646cc050 <location>
+    646c3690:	mov    %ecx,%r8d
+    646c3693:	mov    %rax,%rcx
+    646c3696:	call   646c43dd <pdist>
+    646c369b:	mov    0x897e(%rip),%r8        # 646cc020 <model>
+    646c36a2:	mov    0x18(%rbp),%rax
+    646c36a6:	mov    (%rax),%ecx
+    646c36a8:	mov    0x8a21(%rip),%rdx        # 646cc0d0 <flatten_temp>
+    646c36af:	mov    0x8a7a(%rip),%rax        # 646cc130 <pdist_temp>
+    646c36b6:	mov    %r8,%r9
+    646c36b9:	mov    %ecx,%r8d
+    646c36bc:	mov    %rax,%rcx
+    646c36bf:	call   646c302e <cov_model2d>
+    646c36c4:	mov    0x18(%rbp),%rax
+    646c36c8:	mov    (%rax),%ecx
+    646c36ca:	mov    0x8a7f(%rip),%rdx        # 646cc150 <datacov>
+    646c36d1:	mov    0x89f8(%rip),%rax        # 646cc0d0 <flatten_temp>
+    646c36d8:	mov    %ecx,%r8d
+    646c36db:	mov    %rax,%rcx
+    646c36de:	call   646c4490 <matrixform>
+    646c36e3:	mov    0x8936(%rip),%r8        # 646cc020 <model>
+    646c36ea:	mov    0x18(%rbp),%rax
+    646c36ee:	mov    (%rax),%ecx
+    646c36f0:	mov    0x8979(%rip),%rdx        # 646cc070 <loc_cov>
+    646c36f7:	mov    0x89b2(%rip),%rax        # 646cc0b0 <loc_cov2>
+    646c36fe:	mov    %r8,%r9
+    646c3701:	mov    %ecx,%r8d
+    646c3704:	mov    %rax,%rcx
+    646c3707:	call   646c2f24 <cov_model>
+    646c370c:	mov    0x18(%rbp),%rax
+    646c3710:	mov    (%rax),%eax
+    646c3712:	test   %eax,%eax
+    646c3714:	jle    646c3740 <simple_kriging+0x287>
+    646c3716:	mov    0x18(%rbp),%rax
+    646c371a:	mov    (%rax),%r8d
+    646c371d:	mov    0x89cc(%rip),%rcx        # 646cc0f0 <weights>
+    646c3724:	mov    0x8945(%rip),%rdx        # 646cc070 <loc_cov>
+    646c372b:	mov    0x8a1e(%rip),%rax        # 646cc150 <datacov>
+    646c3732:	mov    %r8d,%r9d
+    646c3735:	mov    %rcx,%r8
+    646c3738:	mov    %rax,%rcx
+    646c373b:	call   646c3c1a <lu_inverse_solver>
+    646c3740:	pxor   %xmm0,%xmm0
+    646c3744:	movsd  %xmm0,0x88e4(%rip)        # 646cc030 <estimation>
+    646c374c:	pxor   %xmm0,%xmm0
+    646c3750:	movsd  %xmm0,0x88e0(%rip)        # 646cc038 <krige_var>
+    646c3758:	pxor   %xmm0,%xmm0
+    646c375c:	movsd  %xmm0,0x88dc(%rip)        # 646cc040 <fix>
+    646c3764:	movl   $0x0,-0x1c(%rbp)
+    646c376b:	jmp    646c3807 <simple_kriging+0x34e>
+    646c3770:	mov    0x8999(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3777:	mov    -0x1c(%rbp),%eax
+    646c377a:	cltq
+    646c377c:	shl    $0x3,%rax
+    646c3780:	add    %rdx,%rax
+    646c3783:	mov    (%rax),%rax
+    646c3786:	add    $0x8,%rax
+    646c378a:	movsd  (%rax),%xmm1
+    646c378e:	mov    0x895b(%rip),%rdx        # 646cc0f0 <weights>
+    646c3795:	mov    -0x1c(%rbp),%eax
+    646c3798:	cltq
+    646c379a:	shl    $0x3,%rax
+    646c379e:	add    %rdx,%rax
+    646c37a1:	movsd  (%rax),%xmm0
+    646c37a5:	mulsd  %xmm0,%xmm1
+    646c37a9:	movsd  0x887f(%rip),%xmm0        # 646cc030 <estimation>
+    646c37b1:	addsd  %xmm1,%xmm0
+    646c37b5:	movsd  %xmm0,0x8873(%rip)        # 646cc030 <estimation>
+    646c37bd:	mov    0x88ac(%rip),%rdx        # 646cc070 <loc_cov>
+    646c37c4:	mov    -0x1c(%rbp),%eax
+    646c37c7:	cltq
+    646c37c9:	shl    $0x3,%rax
+    646c37cd:	add    %rdx,%rax
+    646c37d0:	movsd  (%rax),%xmm1
+    646c37d4:	mov    0x8915(%rip),%rdx        # 646cc0f0 <weights>
+    646c37db:	mov    -0x1c(%rbp),%eax
+    646c37de:	cltq
+    646c37e0:	shl    $0x3,%rax
+    646c37e4:	add    %rdx,%rax
+    646c37e7:	movsd  (%rax),%xmm0
+    646c37eb:	mulsd  %xmm0,%xmm1
+    646c37ef:	movsd  0x8841(%rip),%xmm0        # 646cc038 <krige_var>
+    646c37f7:	addsd  %xmm1,%xmm0
+    646c37fb:	movsd  %xmm0,0x8835(%rip)        # 646cc038 <krige_var>
+    646c3803:	addl   $0x1,-0x1c(%rbp)
+    646c3807:	mov    0x18(%rbp),%rax
+    646c380b:	mov    (%rax),%eax
+    646c380d:	cmp    %eax,-0x1c(%rbp)
+    646c3810:	jl     646c3770 <simple_kriging+0x2b7>
+    646c3816:	mov    0x8803(%rip),%rax        # 646cc020 <model>
+    646c381d:	movsd  0x18(%rax),%xmm0
+    646c3822:	movsd  0x880e(%rip),%xmm1        # 646cc038 <krige_var>
+    646c382a:	subsd  %xmm1,%xmm0
+    646c382e:	movsd  %xmm0,0x8802(%rip)        # 646cc038 <krige_var>
+    646c3836:	movsd  0x87fa(%rip),%xmm1        # 646cc038 <krige_var>
+    646c383e:	pxor   %xmm0,%xmm0
+    646c3842:	comisd %xmm1,%xmm0
+    646c3846:	jbe    646c3854 <simple_kriging+0x39b>
+    646c3848:	pxor   %xmm0,%xmm0
+    646c384c:	movsd  %xmm0,0x87e4(%rip)        # 646cc038 <krige_var>
+    646c3854:	mov    0x20(%rbp),%rax
+    646c3858:	mov    %rax,%rcx
+    646c385b:	call   646c2e27 <mt19937_random_normal>
+    646c3860:	movapd %xmm0,%xmm6
+    646c3864:	mov    0x87cd(%rip),%rax        # 646cc038 <krige_var>
+    646c386b:	movsd  0x57ed(%rip),%xmm0        # 646c9060 <.rdata>
+    646c3873:	movapd %xmm0,%xmm1
+    646c3877:	movq   %rax,%xmm0
+    646c387c:	call   646c6d00 <pow>
+    646c3881:	mulsd  %xmm6,%xmm0
+    646c3885:	movsd  %xmm0,0x87b3(%rip)        # 646cc040 <fix>
+    646c388d:	movsd  0x879b(%rip),%xmm1        # 646cc030 <estimation>
+    646c3895:	movsd  0x87a3(%rip),%xmm0        # 646cc040 <fix>
+    646c389d:	mov    0x18(%rbp),%rax
+    646c38a1:	movsd  0x10(%rax),%xmm2
+    646c38a6:	cvttsd2si %xmm2,%eax
+    646c38aa:	cltq
+    646c38ac:	lea    0x0(,%rax,8),%rdx
+    646c38b4:	mov    0x10(%rbp),%rax
+    646c38b8:	add    %rdx,%rax
+    646c38bb:	addsd  %xmm1,%xmm0
+    646c38bf:	movsd  %xmm0,(%rax)
+    646c38c3:	jmp    646c38c6 <simple_kriging+0x40d>
+    646c38c5:	nop
+    646c38c6:	movaps -0x10(%rbp),%xmm6
+    646c38ca:	add    $0x40,%rsp
+    646c38ce:	pop    %rbp
+    646c38cf:	ret
+
+00000000646c38d0 <find_neighbor>:
+    646c38d0:	push   %rbp
+    646c38d1:	mov    %rsp,%rbp
+    646c38d4:	sub    $0x30,%rsp
+    646c38d8:	mov    %rcx,0x10(%rbp)
+    646c38dc:	mov    %rdx,0x18(%rbp)
+    646c38e0:	mov    %r8,0x20(%rbp)
+    646c38e4:	mov    0x18(%rbp),%rax
+    646c38e8:	mov    (%rax),%eax
+    646c38ea:	test   %eax,%eax
+    646c38ec:	jne    646c395f <find_neighbor+0x8f>
+    646c38ee:	mov    0x20(%rbp),%rax
+    646c38f2:	mov    %rax,%rcx
+    646c38f5:	call   646c2e27 <mt19937_random_normal>
+    646c38fa:	movapd %xmm0,%xmm1
+    646c38fe:	mov    0x871b(%rip),%rax        # 646cc020 <model>
+    646c3905:	movsd  0x18(%rax),%xmm0
+    646c390a:	mov    0x18(%rbp),%rax
+    646c390e:	movsd  0x10(%rax),%xmm2
+    646c3913:	cvttsd2si %xmm2,%eax
+    646c3917:	cltq
+    646c3919:	lea    0x0(,%rax,8),%rdx
+    646c3921:	mov    0x10(%rbp),%rax
+    646c3925:	add    %rdx,%rax
+    646c3928:	mulsd  %xmm1,%xmm0
+    646c392c:	movsd  %xmm0,(%rax)
+    646c3930:	mov    0x18(%rbp),%rax
+    646c3934:	mov    0x18(%rax),%rdx
+    646c3938:	mov    0x18(%rbp),%rax
+    646c393c:	mov    0x8(%rax),%eax
+    646c393f:	cltq
+    646c3941:	shl    $0x3,%rax
+    646c3945:	add    %rdx,%rax
+    646c3948:	mov    0x18(%rbp),%rdx
+    646c394c:	movsd  0x10(%rdx),%xmm0
+    646c3951:	movsd  %xmm0,(%rax)
+    646c3955:	mov    $0x0,%eax
+    646c395a:	jmp    646c3a7e <find_neighbor+0x1ae>
+    646c395f:	movl   $0x0,-0x4(%rbp)
+    646c3966:	movl   $0x0,-0x8(%rbp)
+    646c396d:	jmp    646c39f5 <find_neighbor+0x125>
+    646c3972:	mov    0x18(%rbp),%rax
+    646c3976:	mov    0x18(%rax),%rdx
+    646c397a:	mov    -0x8(%rbp),%eax
+    646c397d:	cltq
+    646c397f:	shl    $0x3,%rax
+    646c3983:	add    %rdx,%rax
+    646c3986:	movsd  (%rax),%xmm0
+    646c398a:	mov    0x18(%rbp),%rax
+    646c398e:	movsd  0x10(%rax),%xmm1
+    646c3993:	subsd  %xmm1,%xmm0
+    646c3997:	mov    0x18(%rbp),%rax
+    646c399b:	mov    0x30(%rax),%rdx
+    646c399f:	mov    -0x8(%rbp),%eax
+    646c39a2:	cltq
+    646c39a4:	shl    $0x3,%rax
+    646c39a8:	add    %rdx,%rax
+    646c39ab:	movq   0x56bd(%rip),%xmm1        # 646c9070 <.rdata+0x10>
+    646c39b3:	andpd  %xmm1,%xmm0
+    646c39b7:	movsd  %xmm0,(%rax)
+    646c39bb:	mov    0x18(%rbp),%rax
+    646c39bf:	mov    0x30(%rax),%rdx
+    646c39c3:	mov    -0x8(%rbp),%eax
+    646c39c6:	cltq
+    646c39c8:	shl    $0x3,%rax
+    646c39cc:	add    %rdx,%rax
+    646c39cf:	movsd  (%rax),%xmm1
+    646c39d3:	movsd  0x864d(%rip),%xmm2        # 646cc028 <k_range>
+    646c39db:	movsd  0x569d(%rip),%xmm0        # 646c9080 <.rdata+0x20>
+    646c39e3:	mulsd  %xmm2,%xmm0
+    646c39e7:	comisd %xmm1,%xmm0
+    646c39eb:	jbe    646c39f1 <find_neighbor+0x121>
+    646c39ed:	addl   $0x1,-0x4(%rbp)
+    646c39f1:	addl   $0x1,-0x8(%rbp)
+    646c39f5:	mov    0x18(%rbp),%rax
+    646c39f9:	mov    0x4(%rax),%eax
+    646c39fc:	cmp    %eax,-0x8(%rbp)
+    646c39ff:	jl     646c3972 <find_neighbor+0xa2>
+    646c3a05:	cmpl   $0x0,-0x4(%rbp)
+    646c3a09:	jne    646c3a79 <find_neighbor+0x1a9>
+    646c3a0b:	mov    0x20(%rbp),%rax
+    646c3a0f:	mov    %rax,%rcx
+    646c3a12:	call   646c2e27 <mt19937_random_normal>
+    646c3a17:	movapd %xmm0,%xmm1
+    646c3a1b:	mov    0x85fe(%rip),%rax        # 646cc020 <model>
+    646c3a22:	movsd  0x18(%rax),%xmm0
+    646c3a27:	mov    0x18(%rbp),%rax
+    646c3a2b:	movsd  0x10(%rax),%xmm2
+    646c3a30:	cvttsd2si %xmm2,%eax
+    646c3a34:	cltq
+    646c3a36:	lea    0x0(,%rax,8),%rdx
+    646c3a3e:	mov    0x10(%rbp),%rax
+    646c3a42:	add    %rdx,%rax
+    646c3a45:	mulsd  %xmm1,%xmm0
+    646c3a49:	movsd  %xmm0,(%rax)
+    646c3a4d:	mov    0x18(%rbp),%rax
+    646c3a51:	mov    0x18(%rax),%rdx
+    646c3a55:	mov    0x18(%rbp),%rax
+    646c3a59:	mov    0x8(%rax),%eax
+    646c3a5c:	cltq
+    646c3a5e:	shl    $0x3,%rax
+    646c3a62:	add    %rdx,%rax
+    646c3a65:	mov    0x18(%rbp),%rdx
+    646c3a69:	movsd  0x10(%rdx),%xmm0
+    646c3a6e:	movsd  %xmm0,(%rax)
+    646c3a72:	mov    $0x0,%eax
+    646c3a77:	jmp    646c3a7e <find_neighbor+0x1ae>
+    646c3a79:	mov    $0x1,%eax
+    646c3a7e:	add    $0x30,%rsp
+    646c3a82:	pop    %rbp
+    646c3a83:	ret
+
+00000000646c3a84 <krige_memory_free>:
+    646c3a84:	push   %rbp
+    646c3a85:	mov    %rsp,%rbp
+    646c3a88:	sub    $0x30,%rsp
+    646c3a8c:	mov    0x85bd(%rip),%rax        # 646cc050 <location>
+    646c3a93:	mov    %rax,%rcx
+    646c3a96:	call   646c7728 <free>
+    646c3a9b:	mov    0x85ce(%rip),%rax        # 646cc070 <loc_cov>
+    646c3aa2:	mov    %rax,%rcx
+    646c3aa5:	call   646c7728 <free>
+    646c3aaa:	mov    0x85df(%rip),%rax        # 646cc090 <data_temp>
+    646c3ab1:	mov    %rax,%rcx
+    646c3ab4:	call   646c7728 <free>
+    646c3ab9:	mov    0x85f0(%rip),%rax        # 646cc0b0 <loc_cov2>
+    646c3ac0:	mov    %rax,%rcx
+    646c3ac3:	call   646c7728 <free>
+    646c3ac8:	mov    0x8601(%rip),%rax        # 646cc0d0 <flatten_temp>
+    646c3acf:	mov    %rax,%rcx
+    646c3ad2:	call   646c7728 <free>
+    646c3ad7:	mov    0x8612(%rip),%rax        # 646cc0f0 <weights>
+    646c3ade:	mov    %rax,%rcx
+    646c3ae1:	call   646c7728 <free>
+    646c3ae6:	movl   $0x0,-0x4(%rbp)
+    646c3aed:	jmp    646c3b11 <krige_memory_free+0x8d>
+    646c3aef:	mov    0x861a(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3af6:	mov    -0x4(%rbp),%eax
+    646c3af9:	cltq
+    646c3afb:	shl    $0x3,%rax
+    646c3aff:	add    %rdx,%rax
+    646c3b02:	mov    (%rax),%rax
+    646c3b05:	mov    %rax,%rcx
+    646c3b08:	call   646c7728 <free>
+    646c3b0d:	addl   $0x1,-0x4(%rbp)
+    646c3b11:	mov    -0x4(%rbp),%eax
+    646c3b14:	cltq
+    646c3b16:	mov    0x85fb(%rip),%rdx        # 646cc118 <array2d_temp+0x8>
+    646c3b1d:	cmp    %rdx,%rax
+    646c3b20:	jb     646c3aef <krige_memory_free+0x6b>
+    646c3b22:	mov    0x85e7(%rip),%rax        # 646cc110 <array2d_temp>
+    646c3b29:	mov    %rax,%rcx
+    646c3b2c:	call   646c7728 <free>
+    646c3b31:	movl   $0x0,-0x8(%rbp)
+    646c3b38:	jmp    646c3b5c <krige_memory_free+0xd8>
+    646c3b3a:	mov    0x85ef(%rip),%rdx        # 646cc130 <pdist_temp>
+    646c3b41:	mov    -0x8(%rbp),%eax
+    646c3b44:	cltq
+    646c3b46:	shl    $0x3,%rax
+    646c3b4a:	add    %rdx,%rax
+    646c3b4d:	mov    (%rax),%rax
+    646c3b50:	mov    %rax,%rcx
+    646c3b53:	call   646c7728 <free>
+    646c3b58:	addl   $0x1,-0x8(%rbp)
+    646c3b5c:	mov    -0x8(%rbp),%eax
+    646c3b5f:	cltq
+    646c3b61:	mov    0x85d0(%rip),%rdx        # 646cc138 <pdist_temp+0x8>
+    646c3b68:	cmp    %rdx,%rax
+    646c3b6b:	jb     646c3b3a <krige_memory_free+0xb6>
+    646c3b6d:	mov    0x85bc(%rip),%rax        # 646cc130 <pdist_temp>
+    646c3b74:	mov    %rax,%rcx
+    646c3b77:	call   646c7728 <free>
+    646c3b7c:	movl   $0x0,-0xc(%rbp)
+    646c3b83:	jmp    646c3ba7 <krige_memory_free+0x123>
+    646c3b85:	mov    0x85c4(%rip),%rdx        # 646cc150 <datacov>
+    646c3b8c:	mov    -0xc(%rbp),%eax
+    646c3b8f:	cltq
+    646c3b91:	shl    $0x3,%rax
+    646c3b95:	add    %rdx,%rax
+    646c3b98:	mov    (%rax),%rax
+    646c3b9b:	mov    %rax,%rcx
+    646c3b9e:	call   646c7728 <free>
+    646c3ba3:	addl   $0x1,-0xc(%rbp)
+    646c3ba7:	mov    -0xc(%rbp),%eax
+    646c3baa:	cltq
+    646c3bac:	mov    0x85a5(%rip),%rdx        # 646cc158 <datacov+0x8>
+    646c3bb3:	cmp    %rdx,%rax
+    646c3bb6:	jb     646c3b85 <krige_memory_free+0x101>
+    646c3bb8:	mov    0x8591(%rip),%rax        # 646cc150 <datacov>
+    646c3bbf:	mov    %rax,%rcx
+    646c3bc2:	call   646c7728 <free>
     646c3bc7:	nop
-    646c3bc8:	nop
-    646c3bc9:	nop
-    646c3bca:	nop
-    646c3bcb:	nop
-    646c3bcc:	nop
-    646c3bcd:	nop
+    646c3bc8:	add    $0x30,%rsp
+    646c3bcc:	pop    %rbp
+    646c3bcd:	ret
     646c3bce:	nop
     646c3bcf:	nop
 
 00000000646c3bd0 <snprintf>:
     646c3bd0:	push   %rbp
     646c3bd1:	mov    %rsp,%rbp
     646c3bd4:	sub    $0x30,%rsp
@@ -5688,15 +5692,15 @@
     646c3bf0:	mov    -0x10(%rbp),%rcx
     646c3bf4:	mov    0x20(%rbp),%rdx
     646c3bf8:	mov    0x18(%rbp),%rax
     646c3bfc:	mov    %rcx,%r9
     646c3bff:	mov    %rdx,%r8
     646c3c02:	mov    %rax,%rdx
     646c3c05:	mov    0x10(%rbp),%rcx
-    646c3c09:	call   646c66a0 <__ms_vsnprintf>
+    646c3c09:	call   646c6730 <__ms_vsnprintf>
     646c3c0e:	mov    %eax,-0x4(%rbp)
     646c3c11:	mov    -0x4(%rbp),%eax
     646c3c14:	add    $0x30,%rsp
     646c3c18:	pop    %rbp
     646c3c19:	ret
 
 00000000646c3c1a <lu_inverse_solver>:
@@ -5707,43 +5711,43 @@
     646c3c2b:	mov    %rcx,0x70(%rbp)
     646c3c2f:	mov    %rdx,0x78(%rbp)
     646c3c33:	mov    %r8,0x80(%rbp)
     646c3c3a:	mov    %r9d,0x88(%rbp)
     646c3c41:	movq   $0xa,0x18(%rbp)
     646c3c49:	movq   $0xa,0x20(%rbp)
     646c3c51:	mov    $0x50,%ecx
-    646c3c56:	call   646c7680 <malloc>
+    646c3c56:	call   646c7710 <malloc>
     646c3c5b:	mov    %rax,0x10(%rbp)
     646c3c5f:	movl   $0x0,0x4c(%rbp)
     646c3c66:	jmp    646c3c8a <lu_inverse_solver+0x70>
     646c3c68:	mov    0x10(%rbp),%rdx
     646c3c6c:	mov    0x4c(%rbp),%eax
     646c3c6f:	cltq
     646c3c71:	shl    $0x3,%rax
     646c3c75:	lea    (%rdx,%rax,1),%rbx
     646c3c79:	mov    $0x50,%ecx
-    646c3c7e:	call   646c7680 <malloc>
+    646c3c7e:	call   646c7710 <malloc>
     646c3c83:	mov    %rax,(%rbx)
     646c3c86:	addl   $0x1,0x4c(%rbp)
     646c3c8a:	cmpl   $0x9,0x4c(%rbp)
     646c3c8e:	jle    646c3c68 <lu_inverse_solver+0x4e>
     646c3c90:	movq   $0xa,-0x8(%rbp)
     646c3c98:	movq   $0xa,0x0(%rbp)
     646c3ca0:	mov    $0x50,%ecx
-    646c3ca5:	call   646c7680 <malloc>
+    646c3ca5:	call   646c7710 <malloc>
     646c3caa:	mov    %rax,-0x10(%rbp)
     646c3cae:	movl   $0x0,0x48(%rbp)
     646c3cb5:	jmp    646c3cd9 <lu_inverse_solver+0xbf>
     646c3cb7:	mov    -0x10(%rbp),%rdx
     646c3cbb:	mov    0x48(%rbp),%eax
     646c3cbe:	cltq
     646c3cc0:	shl    $0x3,%rax
     646c3cc4:	lea    (%rdx,%rax,1),%rbx
     646c3cc8:	mov    $0x50,%ecx
-    646c3ccd:	call   646c7680 <malloc>
+    646c3ccd:	call   646c7710 <malloc>
     646c3cd2:	mov    %rax,(%rbx)
     646c3cd5:	addl   $0x1,0x48(%rbp)
     646c3cd9:	cmpl   $0x9,0x48(%rbp)
     646c3cdd:	jle    646c3cb7 <lu_inverse_solver+0x9d>
     646c3cdf:	mov    -0x10(%rbp),%rdx
     646c3ce3:	mov    0x10(%rbp),%rax
     646c3ce7:	mov    0x88(%rbp),%ecx
@@ -5889,43 +5893,43 @@
     646c3f12:	mov    0x10(%rbp),%rdx
     646c3f16:	mov    0x34(%rbp),%eax
     646c3f19:	cltq
     646c3f1b:	shl    $0x3,%rax
     646c3f1f:	add    %rdx,%rax
     646c3f22:	mov    (%rax),%rax
     646c3f25:	mov    %rax,%rcx
-    646c3f28:	call   646c7698 <free>
+    646c3f28:	call   646c7728 <free>
     646c3f2d:	addl   $0x1,0x34(%rbp)
     646c3f31:	mov    0x34(%rbp),%eax
     646c3f34:	cltq
     646c3f36:	mov    0x18(%rbp),%rdx
     646c3f3a:	cmp    %rdx,%rax
     646c3f3d:	jb     646c3f12 <lu_inverse_solver+0x2f8>
     646c3f3f:	mov    0x10(%rbp),%rax
     646c3f43:	mov    %rax,%rcx
-    646c3f46:	call   646c7698 <free>
+    646c3f46:	call   646c7728 <free>
     646c3f4b:	movl   $0x0,0x30(%rbp)
     646c3f52:	jmp    646c3f73 <lu_inverse_solver+0x359>
     646c3f54:	mov    -0x10(%rbp),%rdx
     646c3f58:	mov    0x30(%rbp),%eax
     646c3f5b:	cltq
     646c3f5d:	shl    $0x3,%rax
     646c3f61:	add    %rdx,%rax
     646c3f64:	mov    (%rax),%rax
     646c3f67:	mov    %rax,%rcx
-    646c3f6a:	call   646c7698 <free>
+    646c3f6a:	call   646c7728 <free>
     646c3f6f:	addl   $0x1,0x30(%rbp)
     646c3f73:	mov    0x30(%rbp),%eax
     646c3f76:	cltq
     646c3f78:	mov    -0x8(%rbp),%rdx
     646c3f7c:	cmp    %rdx,%rax
     646c3f7f:	jb     646c3f54 <lu_inverse_solver+0x33a>
     646c3f81:	mov    -0x10(%rbp),%rax
     646c3f85:	mov    %rax,%rcx
-    646c3f88:	call   646c7698 <free>
+    646c3f88:	call   646c7728 <free>
     646c3f8d:	nop
     646c3f8e:	add    $0xd8,%rsp
     646c3f95:	pop    %rbx
     646c3f96:	pop    %rbp
     646c3f97:	ret
 
 00000000646c3f98 <lu_decomposition>:
@@ -6184,15 +6188,15 @@
     646c432a:	mov    %rsp,%rbp
     646c432d:	sub    $0x30,%rsp
     646c4331:	mov    %ecx,0x10(%rbp)
     646c4334:	mov    0x10(%rbp),%eax
     646c4337:	cltq
     646c4339:	shl    $0x2,%rax
     646c433d:	mov    %rax,%rcx
-    646c4340:	call   646c7680 <malloc>
+    646c4340:	call   646c7710 <malloc>
     646c4345:	mov    %rax,-0x10(%rbp)
     646c4349:	movl   $0x0,-0x4(%rbp)
     646c4350:	jmp    646c436f <arange+0x46>
     646c4352:	mov    -0x4(%rbp),%eax
     646c4355:	cltq
     646c4357:	lea    0x0(,%rax,4),%rdx
     646c435f:	mov    -0x10(%rbp),%rax
@@ -6213,15 +6217,15 @@
     646c4382:	mov    %rsp,%rbp
     646c4385:	sub    $0x30,%rsp
     646c4389:	mov    %ecx,0x10(%rbp)
     646c438c:	mov    0x10(%rbp),%eax
     646c438f:	cltq
     646c4391:	shl    $0x3,%rax
     646c4395:	mov    %rax,%rcx
-    646c4398:	call   646c7680 <malloc>
+    646c4398:	call   646c7710 <malloc>
     646c439d:	mov    %rax,-0x10(%rbp)
     646c43a1:	movl   $0x0,-0x4(%rbp)
     646c43a8:	jmp    646c43cb <d_arange+0x4a>
     646c43aa:	mov    -0x4(%rbp),%eax
     646c43ad:	cltq
     646c43af:	lea    0x0(,%rax,8),%rdx
     646c43b7:	mov    -0x10(%rbp),%rax
@@ -6335,18 +6339,18 @@
     646c4520:	sub    $0x1e0,%rsp
     646c4527:	lea    0x80(%rsp),%rbp
     646c452f:	mov    %rcx,0x170(%rbp)
     646c4536:	mov    %edx,0x178(%rbp)
     646c453c:	mov    %r8,0x180(%rbp)
     646c4543:	mov    %r9,0x188(%rbp)
     646c454a:	cvtsi2sdl 0x190(%rbp),%xmm0
-    646c4552:	call   646c7688 <log10>
+    646c4552:	call   646c7718 <log10>
     646c4557:	movq   %xmm0,%rax
     646c455c:	movq   %rax,%xmm0
-    646c4561:	call   646c66b0 <ceil>
+    646c4561:	call   646c6740 <ceil>
     646c4566:	cvttsd2si %xmm0,%eax
     646c456a:	add    $0x1,%eax
     646c456d:	mov    %eax,0x158(%rbp)
     646c4573:	mov    0x188(%rbp),%rcx
     646c457a:	lea    0x80(%rbp),%rax
     646c4581:	mov    0x158(%rbp),%edx
     646c4587:	mov    %edx,0x28(%rsp)
@@ -6355,43 +6359,43 @@
     646c4597:	mov    %rcx,%r9
     646c459a:	lea    0x4aef(%rip),%r8        # 646c9090 <.rdata>
     646c45a1:	mov    $0xc8,%edx
     646c45a6:	mov    %rax,%rcx
     646c45a9:	call   646c3bd0 <snprintf>
     646c45ae:	mov    0x188(%rbp),%rax
     646c45b5:	mov    %rax,%rcx
-    646c45b8:	call   646c76d8 <_mkdir>
+    646c45b8:	call   646c7768 <_mkdir>
     646c45bd:	cmp    $0xffffffff,%eax
     646c45c0:	jne    646c45de <save_1darray+0xbf>
     646c45c2:	mov    0x9cd3(%rip),%rax        # 646ce29c <__imp__errno>
     646c45c9:	call   *%rax
     646c45cb:	mov    (%rax),%eax
     646c45cd:	cmp    $0x11,%eax
     646c45d0:	je     646c45de <save_1darray+0xbf>
     646c45d2:	lea    0x4ac6(%rip),%rcx        # 646c909f <.rdata+0xf>
-    646c45d9:	call   646c7670 <printf>
+    646c45d9:	call   646c7700 <printf>
     646c45de:	mov    0x198(%rbp),%ecx
     646c45e4:	lea    0x80(%rbp),%rdx
     646c45eb:	lea    -0x50(%rbp),%rax
     646c45ef:	mov    %ecx,%r9d
     646c45f2:	mov    %rdx,%r8
     646c45f5:	mov    $0xc8,%edx
     646c45fa:	mov    %rax,%rcx
     646c45fd:	call   646c3bd0 <snprintf>
     646c4602:	lea    -0x50(%rbp),%rax
     646c4606:	lea    0x4aa8(%rip),%rdx        # 646c90b5 <.rdata+0x25>
     646c460d:	mov    %rax,%rcx
-    646c4610:	call   646c76a8 <fopen>
+    646c4610:	call   646c7738 <fopen>
     646c4615:	mov    %rax,0x150(%rbp)
     646c461c:	cmpq   $0x0,0x150(%rbp)
     646c4624:	jne    646c463c <save_1darray+0x11d>
     646c4626:	lea    0x4a8a(%rip),%rcx        # 646c90b7 <.rdata+0x27>
-    646c462d:	call   646c7678 <perror>
+    646c462d:	call   646c7708 <perror>
     646c4632:	mov    $0x1,%ecx
-    646c4637:	call   646c76b8 <exit>
+    646c4637:	call   646c7748 <exit>
     646c463c:	movl   $0x0,0x15c(%rbp)
     646c4646:	jmp    646c46a6 <save_1darray+0x187>
     646c4648:	mov    0x15c(%rbp),%eax
     646c464e:	cltq
     646c4650:	lea    0x0(,%rax,8),%rdx
     646c4658:	mov    0x170(%rbp),%rax
     646c465f:	add    %rdx,%rax
@@ -6403,22 +6407,22 @@
     646c4676:	mov    0x15c(%rbp),%edx
     646c467c:	mov    0x150(%rbp),%rax
     646c4683:	movq   %rcx,%xmm3
     646c4688:	movq   %xmm0,%r9
     646c468d:	mov    %edx,%r8d
     646c4690:	lea    0x4a38(%rip),%rdx        # 646c90cf <.rdata+0x3f>
     646c4697:	mov    %rax,%rcx
-    646c469a:	call   646c76a0 <fprintf>
+    646c469a:	call   646c7730 <fprintf>
     646c469f:	addl   $0x1,0x15c(%rbp)
     646c46a6:	mov    0x15c(%rbp),%eax
     646c46ac:	cmp    0x178(%rbp),%eax
     646c46b2:	jl     646c4648 <save_1darray+0x129>
     646c46b4:	mov    0x150(%rbp),%rax
     646c46bb:	mov    %rax,%rcx
-    646c46be:	call   646c76b0 <fclose>
+    646c46be:	call   646c7740 <fclose>
     646c46c3:	nop
     646c46c4:	add    $0x1e0,%rsp
     646c46cb:	pop    %rbp
     646c46cc:	ret
     646c46cd:	nop
     646c46ce:	nop
     646c46cf:	nop
@@ -6498,15 +6502,15 @@
     646c47b8:	jne    646c47df <sgsim_init+0x5f>
     646c47ba:	mov    0x18(%rbp),%eax
     646c47bd:	imul   0x20(%rbp),%eax
     646c47c1:	mov    %eax,-0x4(%rbp)
     646c47c4:	mov    -0x4(%rbp),%eax
     646c47c7:	mov    $0x8,%edx
     646c47cc:	mov    %rax,%rcx
-    646c47cf:	call   646c76c0 <calloc>
+    646c47cf:	call   646c7750 <calloc>
     646c47d4:	mov    %rax,%rdx
     646c47d7:	mov    0x10(%rbp),%rax
     646c47db:	mov    %rdx,0x10(%rax)
     646c47df:	nop
     646c47e0:	add    $0x30,%rsp
     646c47e4:	pop    %rbp
     646c47e5:	ret
@@ -6538,30 +6542,30 @@
     646c4857:	cltq
     646c4859:	mov    %rax,0x7990(%rip)        # 646cc1f0 <variogram_array+0x10>
     646c4860:	mov    0x998(%rbp),%rax
     646c4867:	mov    0x8(%rax),%eax
     646c486a:	cltq
     646c486c:	mov    $0x8,%edx
     646c4871:	mov    %rax,%rcx
-    646c4874:	call   646c76c0 <calloc>
+    646c4874:	call   646c7750 <calloc>
     646c4879:	mov    %rax,0x7960(%rip)        # 646cc1e0 <variogram_array>
     646c4880:	mov    0x990(%rbp),%rax
     646c4887:	mov    (%rax),%eax
     646c4889:	cltq
     646c488b:	mov    %rax,0x7976(%rip)        # 646cc208 <sgsim_array+0x8>
     646c4892:	mov    0x990(%rbp),%rax
     646c4899:	mov    (%rax),%eax
     646c489b:	cltq
     646c489d:	mov    %rax,0x796c(%rip)        # 646cc210 <sgsim_array+0x10>
     646c48a4:	mov    0x990(%rbp),%rax
     646c48ab:	mov    (%rax),%eax
     646c48ad:	cltq
     646c48af:	mov    $0x8,%edx
     646c48b4:	mov    %rax,%rcx
-    646c48b7:	call   646c76c0 <calloc>
+    646c48b7:	call   646c7750 <calloc>
     646c48bc:	mov    %rax,0x793d(%rip)        # 646cc200 <sgsim_array>
     646c48c3:	mov    0x990(%rbp),%rax
     646c48ca:	mov    (%rax),%eax
     646c48cc:	mov    0x998(%rbp),%rdx
     646c48d3:	mov    %eax,%ecx
     646c48d5:	call   646c325d <krige_param_setting>
     646c48da:	mov    0x990(%rbp),%rax
@@ -6570,15 +6574,15 @@
     646c48e5:	call   646c4329 <arange>
     646c48ea:	mov    %rax,0x788f(%rip)        # 646cc180 <x_grid>
     646c48f1:	movl   $0x0,0x7971(%rip)        # 646cc26c <count>
     646c48fb:	jmp    646c4bde <sgsim_run+0x3f8>
     646c4900:	mov    0x7966(%rip),%eax        # 646cc26c <count>
     646c4906:	mov    %eax,%edx
     646c4908:	lea    0x47f1(%rip),%rcx        # 646c9100 <.rdata>
-    646c490f:	call   646c7670 <printf>
+    646c490f:	call   646c7700 <printf>
     646c4914:	movl   $0x0,0x7906(%rip)        # 646cc224 <_sampling+0x4>
     646c491e:	movl   $0x0,0x78f8(%rip)        # 646cc220 <_sampling>
     646c4928:	movl   $0x0,0x7936(%rip)        # 646cc268 <flag>
     646c4932:	mov    0x990(%rbp),%rax
     646c4939:	mov    (%rax),%edx
     646c493b:	mov    0x783e(%rip),%rax        # 646cc180 <x_grid>
     646c4942:	lea    -0x50(%rbp),%rcx
@@ -6664,15 +6668,15 @@
     646c4aa6:	add    %rcx,%rax
     646c4aa9:	mov    (%rax),%eax
     646c4aab:	cltq
     646c4aad:	shl    $0x3,%rax
     646c4ab1:	add    %rdx,%rax
     646c4ab4:	mov    (%rax),%rax
     646c4ab7:	movq   %rax,%xmm0
-    646c4abc:	call   646c6510 <__fpclassify>
+    646c4abc:	call   646c65a0 <__fpclassify>
     646c4ac1:	and    $0x100,%eax
     646c4ac6:	test   %eax,%eax
     646c4ac8:	je     646c4ad9 <sgsim_run+0x2f3>
     646c4aca:	mov    0x7798(%rip),%eax        # 646cc268 <flag>
     646c4ad0:	add    $0x1,%eax
     646c4ad3:	mov    %eax,0x778f(%rip)        # 646cc268 <flag>
     646c4ad9:	addl   $0x1,0x97c(%rbp)
@@ -6688,15 +6692,15 @@
     646c4b0f:	mov    0x8(%rax),%r9d
     646c4b13:	mov    0x990(%rbp),%rax
     646c4b1a:	mov    (%rax),%r8d
     646c4b1d:	mov    0x76bc(%rip),%rdx        # 646cc1e0 <variogram_array>
     646c4b24:	mov    0x76d5(%rip),%rax        # 646cc200 <sgsim_array>
     646c4b2b:	mov    %ecx,0x20(%rsp)
     646c4b2f:	mov    %rax,%rcx
-    646c4b32:	call   646c4e40 <variogram>
+    646c4b32:	call   646c4ed0 <variogram>
     646c4b37:	mov    0x772b(%rip),%eax        # 646cc268 <flag>
     646c4b3d:	test   %eax,%eax
     646c4b3f:	jne    646c4bde <sgsim_run+0x3f8>
     646c4b45:	mov    0x7720(%rip),%r8d        # 646cc26c <count>
     646c4b4c:	mov    0x990(%rbp),%rax
     646c4b53:	mov    0x4(%rax),%ecx
     646c4b56:	mov    0x990(%rbp),%rax
@@ -6726,54 +6730,54 @@
     646c4bd5:	add    $0x1,%eax
     646c4bd8:	mov    %eax,0x768e(%rip)        # 646cc26c <count>
     646c4bde:	mov    0x990(%rbp),%rax
     646c4be5:	mov    0x4(%rax),%edx
     646c4be8:	mov    0x767e(%rip),%eax        # 646cc26c <count>
     646c4bee:	cmp    %eax,%edx
     646c4bf0:	jg     646c4900 <sgsim_run+0x11a>
-    646c4bf6:	call   646c3a7b <krige_memory_free>
+    646c4bf6:	call   646c3a84 <krige_memory_free>
     646c4bfb:	call   646c4c2d <sgsim_memory_free>
     646c4c00:	nop
     646c4c01:	add    $0xa00,%rsp
     646c4c08:	pop    %rbp
     646c4c09:	ret
 
 00000000646c4c0a <sgsim_t_free>:
     646c4c0a:	push   %rbp
     646c4c0b:	mov    %rsp,%rbp
     646c4c0e:	sub    $0x20,%rsp
     646c4c12:	mov    %rcx,0x10(%rbp)
     646c4c16:	mov    0x10(%rbp),%rax
     646c4c1a:	mov    0x10(%rax),%rax
     646c4c1e:	mov    %rax,%rcx
-    646c4c21:	call   646c7698 <free>
+    646c4c21:	call   646c7728 <free>
     646c4c26:	nop
     646c4c27:	add    $0x20,%rsp
     646c4c2b:	pop    %rbp
     646c4c2c:	ret
 
 00000000646c4c2d <sgsim_memory_free>:
     646c4c2d:	push   %rbp
     646c4c2e:	mov    %rsp,%rbp
     646c4c31:	sub    $0x20,%rsp
     646c4c35:	mov    0x75fc(%rip),%rax        # 646cc238 <_sampling+0x18>
     646c4c3c:	mov    %rax,%rcx
-    646c4c3f:	call   646c7698 <free>
+    646c4c3f:	call   646c7728 <free>
     646c4c44:	mov    0x7605(%rip),%rax        # 646cc250 <_sampling+0x30>
     646c4c4b:	mov    %rax,%rcx
-    646c4c4e:	call   646c7698 <free>
+    646c4c4e:	call   646c7728 <free>
     646c4c53:	mov    0x75a6(%rip),%rax        # 646cc200 <sgsim_array>
     646c4c5a:	mov    %rax,%rcx
-    646c4c5d:	call   646c7698 <free>
+    646c4c5d:	call   646c7728 <free>
     646c4c62:	mov    0x7517(%rip),%rax        # 646cc180 <x_grid>
     646c4c69:	mov    %rax,%rcx
-    646c4c6c:	call   646c7698 <free>
+    646c4c6c:	call   646c7728 <free>
     646c4c71:	mov    0x7568(%rip),%rax        # 646cc1e0 <variogram_array>
     646c4c78:	mov    %rax,%rcx
-    646c4c7b:	call   646c7698 <free>
+    646c4c7b:	call   646c7728 <free>
     646c4c80:	nop
     646c4c81:	add    $0x20,%rsp
     646c4c85:	pop    %rbp
     646c4c86:	ret
     646c4c87:	nop
     646c4c88:	nop
     646c4c89:	nop
@@ -6912,3550 +6916,3602 @@
     646c4e27:	mov    %eax,%edx
     646c4e29:	mov    0x10(%rbp),%rcx
     646c4e2d:	call   646c4dd5 <quicksort2d>
     646c4e32:	nop
     646c4e33:	add    $0x30,%rsp
     646c4e37:	pop    %rbp
     646c4e38:	ret
-    646c4e39:	nop
-    646c4e3a:	nop
-    646c4e3b:	nop
-    646c4e3c:	nop
-    646c4e3d:	nop
-    646c4e3e:	nop
-    646c4e3f:	nop
-
-00000000646c4e40 <variogram>:
-    646c4e40:	push   %rbp
-    646c4e41:	push   %rbx
-    646c4e42:	sub    $0xb8,%rsp
-    646c4e49:	lea    0x80(%rsp),%rbp
-    646c4e51:	mov    %rcx,0x50(%rbp)
-    646c4e55:	mov    %rdx,0x58(%rbp)
-    646c4e59:	mov    %r8d,0x60(%rbp)
-    646c4e5d:	mov    %r9d,0x68(%rbp)
-    646c4e61:	mov    0x60(%rbp),%eax
-    646c4e64:	cltq
-    646c4e66:	mov    %rax,-0x58(%rbp)
-    646c4e6a:	mov    0x60(%rbp),%eax
-    646c4e6d:	cltq
-    646c4e6f:	mov    %rax,-0x50(%rbp)
-    646c4e73:	mov    0x60(%rbp),%eax
-    646c4e76:	cltq
-    646c4e78:	shl    $0x3,%rax
-    646c4e7c:	mov    %rax,%rcx
-    646c4e7f:	call   646c7680 <malloc>
-    646c4e84:	mov    %rax,-0x60(%rbp)
-    646c4e88:	movl   $0x0,0x1c(%rbp)
-    646c4e8f:	jmp    646c4ebb <variogram+0x7b>
-    646c4e91:	mov    0x60(%rbp),%eax
-    646c4e94:	cltq
-    646c4e96:	shl    $0x3,%rax
-    646c4e9a:	mov    -0x60(%rbp),%rcx
-    646c4e9e:	mov    0x1c(%rbp),%edx
-    646c4ea1:	movslq %edx,%rdx
-    646c4ea4:	shl    $0x3,%rdx
-    646c4ea8:	lea    (%rcx,%rdx,1),%rbx
-    646c4eac:	mov    %rax,%rcx
-    646c4eaf:	call   646c7680 <malloc>
-    646c4eb4:	mov    %rax,(%rbx)
-    646c4eb7:	addl   $0x1,0x1c(%rbp)
-    646c4ebb:	mov    0x1c(%rbp),%eax
-    646c4ebe:	cmp    0x60(%rbp),%eax
-    646c4ec1:	jl     646c4e91 <variogram+0x51>
-    646c4ec3:	mov    0x60(%rbp),%eax
-    646c4ec6:	mov    %eax,%ecx
-    646c4ec8:	call   646c4381 <d_arange>
-    646c4ecd:	mov    %rax,-0x40(%rbp)
-    646c4ed1:	mov    -0x60(%rbp),%rdx
-    646c4ed5:	mov    -0x40(%rbp),%rax
-    646c4ed9:	mov    0x60(%rbp),%ecx
-    646c4edc:	mov    %ecx,%r8d
-    646c4edf:	mov    %rax,%rcx
-    646c4ee2:	call   646c43dd <pdist>
-    646c4ee7:	movl   $0x0,0x18(%rbp)
-    646c4eee:	jmp    646c5051 <variogram+0x211>
-    646c4ef3:	pxor   %xmm0,%xmm0
-    646c4ef7:	movsd  %xmm0,0x28(%rbp)
-    646c4efc:	pxor   %xmm0,%xmm0
-    646c4f00:	movsd  %xmm0,0x20(%rbp)
-    646c4f05:	mov    0x18(%rbp),%eax
-    646c4f08:	sub    0x70(%rbp),%eax
-    646c4f0b:	cvtsi2sd %eax,%xmm0
-    646c4f0f:	movsd  %xmm0,0x0(%rbp)
-    646c4f14:	mov    0x18(%rbp),%edx
-    646c4f17:	mov    0x70(%rbp),%eax
-    646c4f1a:	add    %edx,%eax
-    646c4f1c:	cvtsi2sd %eax,%xmm0
-    646c4f20:	movsd  %xmm0,-0x8(%rbp)
-    646c4f25:	movl   $0x0,0x14(%rbp)
-    646c4f2c:	jmp    646c5002 <variogram+0x1c2>
-    646c4f31:	mov    0x14(%rbp),%eax
-    646c4f34:	cltq
-    646c4f36:	lea    0x0(,%rax,8),%rdx
-    646c4f3e:	mov    0x50(%rbp),%rax
-    646c4f42:	add    %rdx,%rax
-    646c4f45:	movsd  (%rax),%xmm0
-    646c4f49:	movsd  %xmm0,-0x10(%rbp)
-    646c4f4e:	movl   $0x0,0x10(%rbp)
-    646c4f55:	jmp    646c4ff2 <variogram+0x1b2>
-    646c4f5a:	mov    -0x60(%rbp),%rdx
-    646c4f5e:	mov    0x14(%rbp),%eax
-    646c4f61:	cltq
-    646c4f63:	shl    $0x3,%rax
-    646c4f67:	add    %rdx,%rax
-    646c4f6a:	mov    (%rax),%rdx
-    646c4f6d:	mov    0x10(%rbp),%eax
-    646c4f70:	cltq
-    646c4f72:	shl    $0x3,%rax
-    646c4f76:	add    %rdx,%rax
-    646c4f79:	movsd  (%rax),%xmm0
-    646c4f7d:	movsd  %xmm0,-0x18(%rbp)
-    646c4f82:	movsd  -0x18(%rbp),%xmm0
-    646c4f87:	comisd 0x0(%rbp),%xmm0
-    646c4f8c:	jb     646c4fee <variogram+0x1ae>
-    646c4f8e:	movsd  -0x8(%rbp),%xmm0
-    646c4f93:	comisd -0x18(%rbp),%xmm0
-    646c4f98:	jb     646c4fee <variogram+0x1ae>
-    646c4f9a:	mov    0x10(%rbp),%eax
-    646c4f9d:	cltq
-    646c4f9f:	lea    0x0(,%rax,8),%rdx
-    646c4fa7:	mov    0x50(%rbp),%rax
-    646c4fab:	add    %rdx,%rax
-    646c4fae:	movsd  (%rax),%xmm1
-    646c4fb2:	movsd  -0x10(%rbp),%xmm0
-    646c4fb7:	subsd  %xmm1,%xmm0
-    646c4fbb:	movsd  %xmm0,-0x20(%rbp)
-    646c4fc0:	movsd  -0x20(%rbp),%xmm0
-    646c4fc5:	mulsd  -0x20(%rbp),%xmm0
-    646c4fca:	movsd  0x28(%rbp),%xmm1
-    646c4fcf:	addsd  %xmm1,%xmm0
-    646c4fd3:	movsd  %xmm0,0x28(%rbp)
-    646c4fd8:	movsd  0x20(%rbp),%xmm1
-    646c4fdd:	movsd  0x416b(%rip),%xmm0        # 646c9150 <.rdata>
-    646c4fe5:	addsd  %xmm1,%xmm0
-    646c4fe9:	movsd  %xmm0,0x20(%rbp)
-    646c4fee:	addl   $0x1,0x10(%rbp)
-    646c4ff2:	mov    0x10(%rbp),%eax
-    646c4ff5:	cmp    0x14(%rbp),%eax
-    646c4ff8:	jl     646c4f5a <variogram+0x11a>
-    646c4ffe:	addl   $0x1,0x14(%rbp)
-    646c5002:	mov    0x14(%rbp),%eax
-    646c5005:	cmp    0x60(%rbp),%eax
-    646c5008:	jl     646c4f31 <variogram+0xf1>
-    646c500e:	movsd  0x28(%rbp),%xmm0
-    646c5013:	comisd 0x413d(%rip),%xmm0        # 646c9158 <.rdata+0x8>
-    646c501b:	jb     646c504b <variogram+0x20b>
-    646c501d:	movsd  0x20(%rbp),%xmm0
-    646c5022:	movapd %xmm0,%xmm1
-    646c5026:	addsd  %xmm0,%xmm1
-    646c502a:	mov    0x18(%rbp),%eax
+
+00000000646c4e39 <quickselect2d>:
+    646c4e39:	push   %rbp
+    646c4e3a:	mov    %rsp,%rbp
+    646c4e3d:	sub    $0x30,%rsp
+    646c4e41:	mov    %rcx,0x10(%rbp)
+    646c4e45:	mov    %edx,0x18(%rbp)
+    646c4e48:	mov    %r8d,0x20(%rbp)
+    646c4e4c:	mov    %r9d,0x28(%rbp)
+    646c4e50:	mov    0x18(%rbp),%eax
+    646c4e53:	cmp    0x20(%rbp),%eax
+    646c4e56:	jge    646c4ebe <quickselect2d+0x85>
+    646c4e58:	mov    0x20(%rbp),%edx
+    646c4e5b:	mov    0x18(%rbp),%eax
+    646c4e5e:	mov    %edx,%r8d
+    646c4e61:	mov    %eax,%edx
+    646c4e63:	mov    0x10(%rbp),%rcx
+    646c4e67:	call   646c4d0e <partition2d>
+    646c4e6c:	mov    %eax,-0x4(%rbp)
+    646c4e6f:	mov    0x28(%rbp),%eax
+    646c4e72:	sub    $0x1,%eax
+    646c4e75:	cmp    %eax,-0x4(%rbp)
+    646c4e78:	je     646c4ebd <quickselect2d+0x84>
+    646c4e7a:	mov    0x28(%rbp),%eax
+    646c4e7d:	cmp    -0x4(%rbp),%eax
+    646c4e80:	jg     646c4e9e <quickselect2d+0x65>
+    646c4e82:	mov    0x28(%rbp),%ecx
+    646c4e85:	mov    -0x4(%rbp),%edx
+    646c4e88:	mov    0x18(%rbp),%eax
+    646c4e8b:	mov    %ecx,%r9d
+    646c4e8e:	mov    %edx,%r8d
+    646c4e91:	mov    %eax,%edx
+    646c4e93:	mov    0x10(%rbp),%rcx
+    646c4e97:	call   646c4e39 <quickselect2d>
+    646c4e9c:	jmp    646c4ebe <quickselect2d+0x85>
+    646c4e9e:	mov    -0x4(%rbp),%eax
+    646c4ea1:	add    $0x1,%eax
+    646c4ea4:	mov    0x28(%rbp),%ecx
+    646c4ea7:	mov    0x20(%rbp),%edx
+    646c4eaa:	mov    %ecx,%r9d
+    646c4ead:	mov    %edx,%r8d
+    646c4eb0:	mov    %eax,%edx
+    646c4eb2:	mov    0x10(%rbp),%rcx
+    646c4eb6:	call   646c4e39 <quickselect2d>
+    646c4ebb:	jmp    646c4ebe <quickselect2d+0x85>
+    646c4ebd:	nop
+    646c4ebe:	add    $0x30,%rsp
+    646c4ec2:	pop    %rbp
+    646c4ec3:	ret
+    646c4ec4:	nop
+    646c4ec5:	nop
+    646c4ec6:	nop
+    646c4ec7:	nop
+    646c4ec8:	nop
+    646c4ec9:	nop
+    646c4eca:	nop
+    646c4ecb:	nop
+    646c4ecc:	nop
+    646c4ecd:	nop
+    646c4ece:	nop
+    646c4ecf:	nop
+
+00000000646c4ed0 <variogram>:
+    646c4ed0:	push   %rbp
+    646c4ed1:	push   %rbx
+    646c4ed2:	sub    $0xb8,%rsp
+    646c4ed9:	lea    0x80(%rsp),%rbp
+    646c4ee1:	mov    %rcx,0x50(%rbp)
+    646c4ee5:	mov    %rdx,0x58(%rbp)
+    646c4ee9:	mov    %r8d,0x60(%rbp)
+    646c4eed:	mov    %r9d,0x68(%rbp)
+    646c4ef1:	mov    0x60(%rbp),%eax
+    646c4ef4:	cltq
+    646c4ef6:	mov    %rax,-0x58(%rbp)
+    646c4efa:	mov    0x60(%rbp),%eax
+    646c4efd:	cltq
+    646c4eff:	mov    %rax,-0x50(%rbp)
+    646c4f03:	mov    0x60(%rbp),%eax
+    646c4f06:	cltq
+    646c4f08:	shl    $0x3,%rax
+    646c4f0c:	mov    %rax,%rcx
+    646c4f0f:	call   646c7710 <malloc>
+    646c4f14:	mov    %rax,-0x60(%rbp)
+    646c4f18:	movl   $0x0,0x1c(%rbp)
+    646c4f1f:	jmp    646c4f4b <variogram+0x7b>
+    646c4f21:	mov    0x60(%rbp),%eax
+    646c4f24:	cltq
+    646c4f26:	shl    $0x3,%rax
+    646c4f2a:	mov    -0x60(%rbp),%rcx
+    646c4f2e:	mov    0x1c(%rbp),%edx
+    646c4f31:	movslq %edx,%rdx
+    646c4f34:	shl    $0x3,%rdx
+    646c4f38:	lea    (%rcx,%rdx,1),%rbx
+    646c4f3c:	mov    %rax,%rcx
+    646c4f3f:	call   646c7710 <malloc>
+    646c4f44:	mov    %rax,(%rbx)
+    646c4f47:	addl   $0x1,0x1c(%rbp)
+    646c4f4b:	mov    0x1c(%rbp),%eax
+    646c4f4e:	cmp    0x60(%rbp),%eax
+    646c4f51:	jl     646c4f21 <variogram+0x51>
+    646c4f53:	mov    0x60(%rbp),%eax
+    646c4f56:	mov    %eax,%ecx
+    646c4f58:	call   646c4381 <d_arange>
+    646c4f5d:	mov    %rax,-0x40(%rbp)
+    646c4f61:	mov    -0x60(%rbp),%rdx
+    646c4f65:	mov    -0x40(%rbp),%rax
+    646c4f69:	mov    0x60(%rbp),%ecx
+    646c4f6c:	mov    %ecx,%r8d
+    646c4f6f:	mov    %rax,%rcx
+    646c4f72:	call   646c43dd <pdist>
+    646c4f77:	movl   $0x0,0x18(%rbp)
+    646c4f7e:	jmp    646c50e1 <variogram+0x211>
+    646c4f83:	pxor   %xmm0,%xmm0
+    646c4f87:	movsd  %xmm0,0x28(%rbp)
+    646c4f8c:	pxor   %xmm0,%xmm0
+    646c4f90:	movsd  %xmm0,0x20(%rbp)
+    646c4f95:	mov    0x18(%rbp),%eax
+    646c4f98:	sub    0x70(%rbp),%eax
+    646c4f9b:	cvtsi2sd %eax,%xmm0
+    646c4f9f:	movsd  %xmm0,0x0(%rbp)
+    646c4fa4:	mov    0x18(%rbp),%edx
+    646c4fa7:	mov    0x70(%rbp),%eax
+    646c4faa:	add    %edx,%eax
+    646c4fac:	cvtsi2sd %eax,%xmm0
+    646c4fb0:	movsd  %xmm0,-0x8(%rbp)
+    646c4fb5:	movl   $0x0,0x14(%rbp)
+    646c4fbc:	jmp    646c5092 <variogram+0x1c2>
+    646c4fc1:	mov    0x14(%rbp),%eax
+    646c4fc4:	cltq
+    646c4fc6:	lea    0x0(,%rax,8),%rdx
+    646c4fce:	mov    0x50(%rbp),%rax
+    646c4fd2:	add    %rdx,%rax
+    646c4fd5:	movsd  (%rax),%xmm0
+    646c4fd9:	movsd  %xmm0,-0x10(%rbp)
+    646c4fde:	movl   $0x0,0x10(%rbp)
+    646c4fe5:	jmp    646c5082 <variogram+0x1b2>
+    646c4fea:	mov    -0x60(%rbp),%rdx
+    646c4fee:	mov    0x14(%rbp),%eax
+    646c4ff1:	cltq
+    646c4ff3:	shl    $0x3,%rax
+    646c4ff7:	add    %rdx,%rax
+    646c4ffa:	mov    (%rax),%rdx
+    646c4ffd:	mov    0x10(%rbp),%eax
+    646c5000:	cltq
+    646c5002:	shl    $0x3,%rax
+    646c5006:	add    %rdx,%rax
+    646c5009:	movsd  (%rax),%xmm0
+    646c500d:	movsd  %xmm0,-0x18(%rbp)
+    646c5012:	movsd  -0x18(%rbp),%xmm0
+    646c5017:	comisd 0x0(%rbp),%xmm0
+    646c501c:	jb     646c507e <variogram+0x1ae>
+    646c501e:	movsd  -0x8(%rbp),%xmm0
+    646c5023:	comisd -0x18(%rbp),%xmm0
+    646c5028:	jb     646c507e <variogram+0x1ae>
+    646c502a:	mov    0x10(%rbp),%eax
     646c502d:	cltq
     646c502f:	lea    0x0(,%rax,8),%rdx
-    646c5037:	mov    0x58(%rbp),%rax
+    646c5037:	mov    0x50(%rbp),%rax
     646c503b:	add    %rdx,%rax
-    646c503e:	movsd  0x28(%rbp),%xmm0
-    646c5043:	divsd  %xmm1,%xmm0
-    646c5047:	movsd  %xmm0,(%rax)
-    646c504b:	mov    0x70(%rbp),%eax
-    646c504e:	add    %eax,0x18(%rbp)
-    646c5051:	mov    0x18(%rbp),%eax
-    646c5054:	cmp    0x68(%rbp),%eax
-    646c5057:	jl     646c4ef3 <variogram+0xb3>
-    646c505d:	mov    -0x40(%rbp),%rax
-    646c5061:	mov    %rax,%rcx
-    646c5064:	call   646c7698 <free>
-    646c5069:	movl   $0x0,0xc(%rbp)
-    646c5070:	jmp    646c5091 <variogram+0x251>
-    646c5072:	mov    -0x60(%rbp),%rdx
-    646c5076:	mov    0xc(%rbp),%eax
-    646c5079:	cltq
-    646c507b:	shl    $0x3,%rax
-    646c507f:	add    %rdx,%rax
-    646c5082:	mov    (%rax),%rax
-    646c5085:	mov    %rax,%rcx
-    646c5088:	call   646c7698 <free>
-    646c508d:	addl   $0x1,0xc(%rbp)
-    646c5091:	mov    0xc(%rbp),%eax
-    646c5094:	cltq
-    646c5096:	mov    -0x58(%rbp),%rdx
-    646c509a:	cmp    %rdx,%rax
-    646c509d:	jb     646c5072 <variogram+0x232>
-    646c509f:	mov    -0x60(%rbp),%rax
-    646c50a3:	mov    %rax,%rcx
-    646c50a6:	call   646c7698 <free>
-    646c50ab:	nop
-    646c50ac:	add    $0xb8,%rsp
-    646c50b3:	pop    %rbx
-    646c50b4:	pop    %rbp
-    646c50b5:	ret
-
-00000000646c50b6 <variance>:
-    646c50b6:	push   %rbp
-    646c50b7:	mov    %rsp,%rbp
-    646c50ba:	sub    $0x40,%rsp
-    646c50be:	mov    %rcx,0x10(%rbp)
-    646c50c2:	mov    %edx,0x18(%rbp)
-    646c50c5:	pxor   %xmm0,%xmm0
-    646c50c9:	movsd  %xmm0,-0x8(%rbp)
-    646c50ce:	pxor   %xmm0,%xmm0
-    646c50d2:	movsd  %xmm0,-0x10(%rbp)
-    646c50d7:	movl   $0x0,-0x14(%rbp)
-    646c50de:	jmp    646c510a <variance+0x54>
-    646c50e0:	mov    -0x14(%rbp),%eax
-    646c50e3:	cltq
-    646c50e5:	lea    0x0(,%rax,8),%rdx
-    646c50ed:	mov    0x10(%rbp),%rax
-    646c50f1:	add    %rdx,%rax
-    646c50f4:	movsd  (%rax),%xmm0
-    646c50f8:	movsd  -0x8(%rbp),%xmm1
-    646c50fd:	addsd  %xmm1,%xmm0
-    646c5101:	movsd  %xmm0,-0x8(%rbp)
-    646c5106:	addl   $0x1,-0x14(%rbp)
-    646c510a:	mov    -0x14(%rbp),%eax
-    646c510d:	cmp    0x18(%rbp),%eax
-    646c5110:	jl     646c50e0 <variance+0x2a>
-    646c5112:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c5117:	movsd  -0x8(%rbp),%xmm0
-    646c511c:	divsd  %xmm1,%xmm0
-    646c5120:	movsd  %xmm0,-0x8(%rbp)
-    646c5125:	movl   $0x0,-0x18(%rbp)
-    646c512c:	jmp    646c516e <variance+0xb8>
-    646c512e:	mov    -0x18(%rbp),%eax
-    646c5131:	cltq
-    646c5133:	lea    0x0(,%rax,8),%rdx
-    646c513b:	mov    0x10(%rbp),%rax
-    646c513f:	add    %rdx,%rax
-    646c5142:	movsd  (%rax),%xmm0
-    646c5146:	subsd  -0x8(%rbp),%xmm0
-    646c514b:	movsd  0x400d(%rip),%xmm1        # 646c9160 <.rdata+0x10>
-    646c5153:	call   646c6c70 <pow>
-    646c5158:	movapd %xmm0,%xmm1
-    646c515c:	movsd  -0x10(%rbp),%xmm0
-    646c5161:	addsd  %xmm1,%xmm0
-    646c5165:	movsd  %xmm0,-0x10(%rbp)
-    646c516a:	addl   $0x1,-0x18(%rbp)
-    646c516e:	mov    -0x18(%rbp),%eax
-    646c5171:	cmp    0x18(%rbp),%eax
-    646c5174:	jl     646c512e <variance+0x78>
-    646c5176:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c517b:	movsd  -0x10(%rbp),%xmm0
-    646c5180:	divsd  %xmm1,%xmm0
-    646c5184:	movsd  %xmm0,-0x10(%rbp)
-    646c5189:	movsd  -0x10(%rbp),%xmm0
-    646c518e:	movq   %xmm0,%rax
-    646c5193:	movq   %rax,%xmm0
-    646c5198:	add    $0x40,%rsp
-    646c519c:	pop    %rbp
-    646c519d:	ret
-    646c519e:	nop
-    646c519f:	nop
-
-00000000646c51a0 <Sleep>:
-    646c51a0:	jmp    *0x90a6(%rip)        # 646ce24c <__imp_Sleep>
-    646c51a6:	nop
-    646c51a7:	nop
-    646c51a8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c51b0 <__do_global_dtors>:
-    646c51b0:	sub    $0x28,%rsp
-    646c51b4:	mov    0x2e45(%rip),%rax        # 646c8000 <__data_start__>
-    646c51bb:	mov    (%rax),%rax
-    646c51be:	test   %rax,%rax
-    646c51c1:	je     646c51e0 <__do_global_dtors+0x30>
-    646c51c3:	call   *%rax
-    646c51c5:	mov    0x2e34(%rip),%rax        # 646c8000 <__data_start__>
-    646c51cc:	lea    0x8(%rax),%rdx
-    646c51d0:	mov    0x8(%rax),%rax
-    646c51d4:	mov    %rdx,0x2e25(%rip)        # 646c8000 <__data_start__>
-    646c51db:	test   %rax,%rax
-    646c51de:	jne    646c51c3 <__do_global_dtors+0x13>
-    646c51e0:	add    $0x28,%rsp
-    646c51e4:	ret
-    646c51e5:	nop
-    646c51e6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c51f0 <__do_global_ctors>:
-    646c51f0:	push   %rsi
-    646c51f1:	push   %rbx
-    646c51f2:	sub    $0x28,%rsp
-    646c51f6:	mov    0x43d3(%rip),%rcx        # 646c95d0 <.refptr.__CTOR_LIST__>
-    646c51fd:	mov    (%rcx),%rdx
-    646c5200:	cmp    $0xffffffff,%edx
-    646c5203:	mov    %edx,%eax
-    646c5205:	je     646c5240 <__do_global_ctors+0x50>
-    646c5207:	test   %eax,%eax
-    646c5209:	je     646c522b <__do_global_ctors+0x3b>
-    646c520b:	mov    %eax,%edx
-    646c520d:	sub    $0x1,%eax
-    646c5210:	lea    (%rcx,%rdx,8),%rbx
-    646c5214:	sub    %rax,%rdx
-    646c5217:	lea    -0x8(%rcx,%rdx,8),%rsi
-    646c521c:	nopl   0x0(%rax)
-    646c5220:	call   *(%rbx)
-    646c5222:	sub    $0x8,%rbx
-    646c5226:	cmp    %rsi,%rbx
-    646c5229:	jne    646c5220 <__do_global_ctors+0x30>
-    646c522b:	lea    -0x82(%rip),%rcx        # 646c51b0 <__do_global_dtors>
-    646c5232:	add    $0x28,%rsp
-    646c5236:	pop    %rbx
-    646c5237:	pop    %rsi
-    646c5238:	jmp    646c1380 <atexit>
-    646c523d:	nopl   (%rax)
-    646c5240:	xor    %eax,%eax
-    646c5242:	jmp    646c5246 <__do_global_ctors+0x56>
-    646c5244:	mov    %edx,%eax
-    646c5246:	lea    0x1(%rax),%r8d
-    646c524a:	cmpq   $0x0,(%rcx,%r8,8)
-    646c524f:	mov    %r8,%rdx
-    646c5252:	jne    646c5244 <__do_global_ctors+0x54>
-    646c5254:	jmp    646c5207 <__do_global_ctors+0x17>
-    646c5256:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5260 <__main>:
-    646c5260:	mov    0x701a(%rip),%eax        # 646cc280 <initialized>
-    646c5266:	test   %eax,%eax
-    646c5268:	je     646c5270 <__main+0x10>
-    646c526a:	ret
-    646c526b:	nopl   0x0(%rax,%rax,1)
-    646c5270:	movl   $0x1,0x7006(%rip)        # 646cc280 <initialized>
-    646c527a:	jmp    646c51f0 <__do_global_ctors>
-    646c527f:	nop
-
-00000000646c5280 <__security_init_cookie>:
-    646c5280:	push   %r12
-    646c5282:	push   %rbp
-    646c5283:	push   %rdi
-    646c5284:	push   %rsi
-    646c5285:	push   %rbx
-    646c5286:	sub    $0x30,%rsp
-    646c528a:	mov    0x2def(%rip),%rbx        # 646c8080 <__security_cookie>
-    646c5291:	movabs $0x2b992ddfa232,%rax
-    646c529b:	cmp    %rax,%rbx
-    646c529e:	movq   $0x0,0x20(%rsp)
-    646c52a7:	je     646c52c0 <__security_init_cookie+0x40>
-    646c52a9:	not    %rbx
-    646c52ac:	mov    %rbx,0x2ddd(%rip)        # 646c8090 <__security_cookie_complement>
-    646c52b3:	add    $0x30,%rsp
-    646c52b7:	pop    %rbx
-    646c52b8:	pop    %rsi
-    646c52b9:	pop    %rdi
-    646c52ba:	pop    %rbp
-    646c52bb:	pop    %r12
-    646c52bd:	ret
-    646c52be:	xchg   %ax,%ax
-    646c52c0:	lea    0x20(%rsp),%rcx
-    646c52c5:	call   *0x8f31(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c52cb:	mov    0x20(%rsp),%rsi
-    646c52d0:	call   *0x8f0e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c52d6:	mov    %eax,%r12d
-    646c52d9:	call   *0x8f0d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c52df:	mov    %eax,%ebp
-    646c52e1:	call   *0x8f1d(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c52e7:	lea    0x28(%rsp),%rcx
-    646c52ec:	mov    %eax,%edi
-    646c52ee:	call   *0x8f28(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c52f4:	xor    0x28(%rsp),%rsi
-    646c52f9:	mov    %r12d,%eax
-    646c52fc:	movabs $0xffffffffffff,%rdx
-    646c5306:	xor    %rsi,%rax
-    646c5309:	mov    %ebp,%esi
-    646c530b:	xor    %rax,%rsi
-    646c530e:	mov    %edi,%eax
-    646c5310:	xor    %rsi,%rax
-    646c5313:	and    %rdx,%rax
-    646c5316:	cmp    %rbx,%rax
-    646c5319:	je     646c5340 <__security_init_cookie+0xc0>
-    646c531b:	mov    %rax,%rdx
-    646c531e:	not    %rdx
-    646c5321:	mov    %rax,0x2d58(%rip)        # 646c8080 <__security_cookie>
-    646c5328:	mov    %rdx,0x2d61(%rip)        # 646c8090 <__security_cookie_complement>
-    646c532f:	add    $0x30,%rsp
-    646c5333:	pop    %rbx
-    646c5334:	pop    %rsi
-    646c5335:	pop    %rdi
-    646c5336:	pop    %rbp
-    646c5337:	pop    %r12
-    646c5339:	ret
-    646c533a:	nopw   0x0(%rax,%rax,1)
-    646c5340:	movabs $0xffffd466d2205dcc,%rdx
-    646c534a:	movabs $0x2b992ddfa233,%rax
-    646c5354:	jmp    646c5321 <__security_init_cookie+0xa1>
-    646c5356:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5360 <__report_gsfailure>:
-    646c5360:	push   %rbp
-    646c5361:	push   %rsi
-    646c5362:	push   %rbx
-    646c5363:	mov    %rsp,%rbp
-    646c5366:	sub    $0x70,%rsp
-    646c536a:	mov    %rcx,%rsi
-    646c536d:	lea    0x6f2c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c5374:	call   *0x8eb2(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c537a:	mov    0x7017(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
-    646c5381:	lea    -0x28(%rbp),%rdx
-    646c5385:	xor    %r8d,%r8d
-    646c5388:	mov    %rbx,%rcx
-    646c538b:	call   *0x8ea3(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c5391:	test   %rax,%rax
-    646c5394:	je     646c543d <__report_gsfailure+0xdd>
-    646c539a:	lea    -0x20(%rbp),%rdx
-    646c539e:	mov    %rax,%r9
-    646c53a1:	mov    %rbx,%r8
-    646c53a4:	movq   $0x0,0x38(%rsp)
-    646c53ad:	lea    0x6eec(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c53b4:	mov    %rdx,0x30(%rsp)
-    646c53b9:	lea    -0x18(%rbp),%rdx
-    646c53bd:	mov    %rcx,0x20(%rsp)
-    646c53c2:	xor    %ecx,%ecx
-    646c53c4:	mov    %rdx,0x28(%rsp)
-    646c53c9:	mov    -0x28(%rbp),%rdx
-    646c53cd:	call   *0x8e69(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c53d3:	mov    0x6fbe(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
-    646c53da:	xor    %ecx,%ecx
-    646c53dc:	mov    %rsi,0x6f3d(%rip)        # 646cc320 <GS_ContextRecord+0x80>
-    646c53e3:	mov    %rax,0x73a6(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
-    646c53ea:	movabs $0x1c0000409,%rax
-    646c53f4:	mov    %rax,0x7385(%rip)        # 646cc780 <GS_ExceptionRecord>
-    646c53fb:	mov    0x2c7e(%rip),%rax        # 646c8080 <__security_cookie>
-    646c5402:	mov    %rax,-0x10(%rbp)
-    646c5406:	mov    0x2c83(%rip),%rax        # 646c8090 <__security_cookie_complement>
-    646c540d:	mov    %rax,-0x8(%rbp)
-    646c5411:	call   *0x8e2d(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c5417:	lea    0x3d52(%rip),%rcx        # 646c9170 <GS_ExceptionPointers>
-    646c541e:	call   *0x8e40(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c5424:	call   *0x8db2(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c542a:	mov    $0xc0000409,%edx
-    646c542f:	mov    %rax,%rcx
-    646c5432:	call   *0x8e1c(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c5438:	call   646c76c8 <abort>
-    646c543d:	mov    0x18(%rbp),%rax
-    646c5441:	mov    %rax,0x6f50(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
-    646c5448:	lea    0x8(%rbp),%rax
-    646c544c:	mov    %rax,0x6ee5(%rip)        # 646cc338 <GS_ContextRecord+0x98>
-    646c5453:	jmp    646c53d3 <__report_gsfailure+0x73>
-    646c5458:	nop
-    646c5459:	nop
-    646c545a:	nop
-    646c545b:	nop
-    646c545c:	nop
-    646c545d:	nop
-    646c545e:	nop
-    646c545f:	nop
-
-00000000646c5460 <__dyn_tls_dtor>:
-    646c5460:	sub    $0x28,%rsp
-    646c5464:	cmp    $0x3,%edx
-    646c5467:	je     646c5480 <__dyn_tls_dtor+0x20>
-    646c5469:	test   %edx,%edx
-    646c546b:	je     646c5480 <__dyn_tls_dtor+0x20>
-    646c546d:	mov    $0x1,%eax
-    646c5472:	add    $0x28,%rsp
-    646c5476:	ret
-    646c5477:	nopw   0x0(%rax,%rax,1)
-    646c5480:	call   646c5fe0 <__mingw_TLScallback>
-    646c5485:	mov    $0x1,%eax
-    646c548a:	add    $0x28,%rsp
-    646c548e:	ret
-    646c548f:	nop
-
-00000000646c5490 <__dyn_tls_init>:
-    646c5490:	push   %rsi
-    646c5491:	push   %rbx
-    646c5492:	sub    $0x28,%rsp
-    646c5496:	mov    0x4123(%rip),%rax        # 646c95c0 <.refptr._CRT_MT>
-    646c549d:	cmpl   $0x2,(%rax)
-    646c54a0:	je     646c54a8 <__dyn_tls_init+0x18>
-    646c54a2:	movl   $0x2,(%rax)
-    646c54a8:	cmp    $0x2,%edx
-    646c54ab:	je     646c54c0 <__dyn_tls_init+0x30>
-    646c54ad:	cmp    $0x1,%edx
-    646c54b0:	je     646c54f2 <__dyn_tls_init+0x62>
-    646c54b2:	mov    $0x1,%eax
-    646c54b7:	add    $0x28,%rsp
-    646c54bb:	pop    %rbx
-    646c54bc:	pop    %rsi
-    646c54bd:	ret
-    646c54be:	xchg   %ax,%ax
-    646c54c0:	lea    0x9b89(%rip),%rbx        # 646cf050 <__xd_z>
-    646c54c7:	lea    0x9b82(%rip),%rsi        # 646cf050 <__xd_z>
-    646c54ce:	cmp    %rbx,%rsi
-    646c54d1:	je     646c54b2 <__dyn_tls_init+0x22>
-    646c54d3:	mov    (%rbx),%rax
-    646c54d6:	test   %rax,%rax
-    646c54d9:	je     646c54dd <__dyn_tls_init+0x4d>
-    646c54db:	call   *%rax
-    646c54dd:	add    $0x8,%rbx
-    646c54e1:	cmp    %rbx,%rsi
-    646c54e4:	jne    646c54d3 <__dyn_tls_init+0x43>
-    646c54e6:	mov    $0x1,%eax
-    646c54eb:	add    $0x28,%rsp
-    646c54ef:	pop    %rbx
-    646c54f0:	pop    %rsi
-    646c54f1:	ret
-    646c54f2:	call   646c5fe0 <__mingw_TLScallback>
-    646c54f7:	mov    $0x1,%eax
-    646c54fc:	add    $0x28,%rsp
-    646c5500:	pop    %rbx
-    646c5501:	pop    %rsi
-    646c5502:	ret
-    646c5503:	nopl   (%rax)
-    646c5506:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5510 <__tlregdtor>:
-    646c5510:	xor    %eax,%eax
-    646c5512:	ret
-    646c5513:	nop
-    646c5514:	nop
-    646c5515:	nop
-    646c5516:	nop
-    646c5517:	nop
-    646c5518:	nop
-    646c5519:	nop
-    646c551a:	nop
-    646c551b:	nop
-    646c551c:	nop
-    646c551d:	nop
-    646c551e:	nop
+    646c503e:	movsd  (%rax),%xmm1
+    646c5042:	movsd  -0x10(%rbp),%xmm0
+    646c5047:	subsd  %xmm1,%xmm0
+    646c504b:	movsd  %xmm0,-0x20(%rbp)
+    646c5050:	movsd  -0x20(%rbp),%xmm0
+    646c5055:	mulsd  -0x20(%rbp),%xmm0
+    646c505a:	movsd  0x28(%rbp),%xmm1
+    646c505f:	addsd  %xmm1,%xmm0
+    646c5063:	movsd  %xmm0,0x28(%rbp)
+    646c5068:	movsd  0x20(%rbp),%xmm1
+    646c506d:	movsd  0x40db(%rip),%xmm0        # 646c9150 <.rdata>
+    646c5075:	addsd  %xmm1,%xmm0
+    646c5079:	movsd  %xmm0,0x20(%rbp)
+    646c507e:	addl   $0x1,0x10(%rbp)
+    646c5082:	mov    0x10(%rbp),%eax
+    646c5085:	cmp    0x14(%rbp),%eax
+    646c5088:	jl     646c4fea <variogram+0x11a>
+    646c508e:	addl   $0x1,0x14(%rbp)
+    646c5092:	mov    0x14(%rbp),%eax
+    646c5095:	cmp    0x60(%rbp),%eax
+    646c5098:	jl     646c4fc1 <variogram+0xf1>
+    646c509e:	movsd  0x28(%rbp),%xmm0
+    646c50a3:	comisd 0x40ad(%rip),%xmm0        # 646c9158 <.rdata+0x8>
+    646c50ab:	jb     646c50db <variogram+0x20b>
+    646c50ad:	movsd  0x20(%rbp),%xmm0
+    646c50b2:	movapd %xmm0,%xmm1
+    646c50b6:	addsd  %xmm0,%xmm1
+    646c50ba:	mov    0x18(%rbp),%eax
+    646c50bd:	cltq
+    646c50bf:	lea    0x0(,%rax,8),%rdx
+    646c50c7:	mov    0x58(%rbp),%rax
+    646c50cb:	add    %rdx,%rax
+    646c50ce:	movsd  0x28(%rbp),%xmm0
+    646c50d3:	divsd  %xmm1,%xmm0
+    646c50d7:	movsd  %xmm0,(%rax)
+    646c50db:	mov    0x70(%rbp),%eax
+    646c50de:	add    %eax,0x18(%rbp)
+    646c50e1:	mov    0x18(%rbp),%eax
+    646c50e4:	cmp    0x68(%rbp),%eax
+    646c50e7:	jl     646c4f83 <variogram+0xb3>
+    646c50ed:	mov    -0x40(%rbp),%rax
+    646c50f1:	mov    %rax,%rcx
+    646c50f4:	call   646c7728 <free>
+    646c50f9:	movl   $0x0,0xc(%rbp)
+    646c5100:	jmp    646c5121 <variogram+0x251>
+    646c5102:	mov    -0x60(%rbp),%rdx
+    646c5106:	mov    0xc(%rbp),%eax
+    646c5109:	cltq
+    646c510b:	shl    $0x3,%rax
+    646c510f:	add    %rdx,%rax
+    646c5112:	mov    (%rax),%rax
+    646c5115:	mov    %rax,%rcx
+    646c5118:	call   646c7728 <free>
+    646c511d:	addl   $0x1,0xc(%rbp)
+    646c5121:	mov    0xc(%rbp),%eax
+    646c5124:	cltq
+    646c5126:	mov    -0x58(%rbp),%rdx
+    646c512a:	cmp    %rdx,%rax
+    646c512d:	jb     646c5102 <variogram+0x232>
+    646c512f:	mov    -0x60(%rbp),%rax
+    646c5133:	mov    %rax,%rcx
+    646c5136:	call   646c7728 <free>
+    646c513b:	nop
+    646c513c:	add    $0xb8,%rsp
+    646c5143:	pop    %rbx
+    646c5144:	pop    %rbp
+    646c5145:	ret
+
+00000000646c5146 <variance>:
+    646c5146:	push   %rbp
+    646c5147:	mov    %rsp,%rbp
+    646c514a:	sub    $0x40,%rsp
+    646c514e:	mov    %rcx,0x10(%rbp)
+    646c5152:	mov    %edx,0x18(%rbp)
+    646c5155:	pxor   %xmm0,%xmm0
+    646c5159:	movsd  %xmm0,-0x8(%rbp)
+    646c515e:	pxor   %xmm0,%xmm0
+    646c5162:	movsd  %xmm0,-0x10(%rbp)
+    646c5167:	movl   $0x0,-0x14(%rbp)
+    646c516e:	jmp    646c519a <variance+0x54>
+    646c5170:	mov    -0x14(%rbp),%eax
+    646c5173:	cltq
+    646c5175:	lea    0x0(,%rax,8),%rdx
+    646c517d:	mov    0x10(%rbp),%rax
+    646c5181:	add    %rdx,%rax
+    646c5184:	movsd  (%rax),%xmm0
+    646c5188:	movsd  -0x8(%rbp),%xmm1
+    646c518d:	addsd  %xmm1,%xmm0
+    646c5191:	movsd  %xmm0,-0x8(%rbp)
+    646c5196:	addl   $0x1,-0x14(%rbp)
+    646c519a:	mov    -0x14(%rbp),%eax
+    646c519d:	cmp    0x18(%rbp),%eax
+    646c51a0:	jl     646c5170 <variance+0x2a>
+    646c51a2:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c51a7:	movsd  -0x8(%rbp),%xmm0
+    646c51ac:	divsd  %xmm1,%xmm0
+    646c51b0:	movsd  %xmm0,-0x8(%rbp)
+    646c51b5:	movl   $0x0,-0x18(%rbp)
+    646c51bc:	jmp    646c51fe <variance+0xb8>
+    646c51be:	mov    -0x18(%rbp),%eax
+    646c51c1:	cltq
+    646c51c3:	lea    0x0(,%rax,8),%rdx
+    646c51cb:	mov    0x10(%rbp),%rax
+    646c51cf:	add    %rdx,%rax
+    646c51d2:	movsd  (%rax),%xmm0
+    646c51d6:	subsd  -0x8(%rbp),%xmm0
+    646c51db:	movsd  0x3f7d(%rip),%xmm1        # 646c9160 <.rdata+0x10>
+    646c51e3:	call   646c6d00 <pow>
+    646c51e8:	movapd %xmm0,%xmm1
+    646c51ec:	movsd  -0x10(%rbp),%xmm0
+    646c51f1:	addsd  %xmm1,%xmm0
+    646c51f5:	movsd  %xmm0,-0x10(%rbp)
+    646c51fa:	addl   $0x1,-0x18(%rbp)
+    646c51fe:	mov    -0x18(%rbp),%eax
+    646c5201:	cmp    0x18(%rbp),%eax
+    646c5204:	jl     646c51be <variance+0x78>
+    646c5206:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c520b:	movsd  -0x10(%rbp),%xmm0
+    646c5210:	divsd  %xmm1,%xmm0
+    646c5214:	movsd  %xmm0,-0x10(%rbp)
+    646c5219:	movsd  -0x10(%rbp),%xmm0
+    646c521e:	movq   %xmm0,%rax
+    646c5223:	movq   %rax,%xmm0
+    646c5228:	add    $0x40,%rsp
+    646c522c:	pop    %rbp
+    646c522d:	ret
+    646c522e:	nop
+    646c522f:	nop
+
+00000000646c5230 <Sleep>:
+    646c5230:	jmp    *0x9016(%rip)        # 646ce24c <__imp_Sleep>
+    646c5236:	nop
+    646c5237:	nop
+    646c5238:	nopl   0x0(%rax,%rax,1)
+
+00000000646c5240 <__do_global_dtors>:
+    646c5240:	sub    $0x28,%rsp
+    646c5244:	mov    0x2db5(%rip),%rax        # 646c8000 <__data_start__>
+    646c524b:	mov    (%rax),%rax
+    646c524e:	test   %rax,%rax
+    646c5251:	je     646c5270 <__do_global_dtors+0x30>
+    646c5253:	call   *%rax
+    646c5255:	mov    0x2da4(%rip),%rax        # 646c8000 <__data_start__>
+    646c525c:	lea    0x8(%rax),%rdx
+    646c5260:	mov    0x8(%rax),%rax
+    646c5264:	mov    %rdx,0x2d95(%rip)        # 646c8000 <__data_start__>
+    646c526b:	test   %rax,%rax
+    646c526e:	jne    646c5253 <__do_global_dtors+0x13>
+    646c5270:	add    $0x28,%rsp
+    646c5274:	ret
+    646c5275:	nop
+    646c5276:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5280 <__do_global_ctors>:
+    646c5280:	push   %rsi
+    646c5281:	push   %rbx
+    646c5282:	sub    $0x28,%rsp
+    646c5286:	mov    0x4343(%rip),%rcx        # 646c95d0 <.refptr.__CTOR_LIST__>
+    646c528d:	mov    (%rcx),%rdx
+    646c5290:	cmp    $0xffffffff,%edx
+    646c5293:	mov    %edx,%eax
+    646c5295:	je     646c52d0 <__do_global_ctors+0x50>
+    646c5297:	test   %eax,%eax
+    646c5299:	je     646c52bb <__do_global_ctors+0x3b>
+    646c529b:	mov    %eax,%edx
+    646c529d:	sub    $0x1,%eax
+    646c52a0:	lea    (%rcx,%rdx,8),%rbx
+    646c52a4:	sub    %rax,%rdx
+    646c52a7:	lea    -0x8(%rcx,%rdx,8),%rsi
+    646c52ac:	nopl   0x0(%rax)
+    646c52b0:	call   *(%rbx)
+    646c52b2:	sub    $0x8,%rbx
+    646c52b6:	cmp    %rsi,%rbx
+    646c52b9:	jne    646c52b0 <__do_global_ctors+0x30>
+    646c52bb:	lea    -0x82(%rip),%rcx        # 646c5240 <__do_global_dtors>
+    646c52c2:	add    $0x28,%rsp
+    646c52c6:	pop    %rbx
+    646c52c7:	pop    %rsi
+    646c52c8:	jmp    646c1380 <atexit>
+    646c52cd:	nopl   (%rax)
+    646c52d0:	xor    %eax,%eax
+    646c52d2:	jmp    646c52d6 <__do_global_ctors+0x56>
+    646c52d4:	mov    %edx,%eax
+    646c52d6:	lea    0x1(%rax),%r8d
+    646c52da:	cmpq   $0x0,(%rcx,%r8,8)
+    646c52df:	mov    %r8,%rdx
+    646c52e2:	jne    646c52d4 <__do_global_ctors+0x54>
+    646c52e4:	jmp    646c5297 <__do_global_ctors+0x17>
+    646c52e6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c52f0 <__main>:
+    646c52f0:	mov    0x6f8a(%rip),%eax        # 646cc280 <initialized>
+    646c52f6:	test   %eax,%eax
+    646c52f8:	je     646c5300 <__main+0x10>
+    646c52fa:	ret
+    646c52fb:	nopl   0x0(%rax,%rax,1)
+    646c5300:	movl   $0x1,0x6f76(%rip)        # 646cc280 <initialized>
+    646c530a:	jmp    646c5280 <__do_global_ctors>
+    646c530f:	nop
+
+00000000646c5310 <__security_init_cookie>:
+    646c5310:	push   %r12
+    646c5312:	push   %rbp
+    646c5313:	push   %rdi
+    646c5314:	push   %rsi
+    646c5315:	push   %rbx
+    646c5316:	sub    $0x30,%rsp
+    646c531a:	mov    0x2d5f(%rip),%rbx        # 646c8080 <__security_cookie>
+    646c5321:	movabs $0x2b992ddfa232,%rax
+    646c532b:	cmp    %rax,%rbx
+    646c532e:	movq   $0x0,0x20(%rsp)
+    646c5337:	je     646c5350 <__security_init_cookie+0x40>
+    646c5339:	not    %rbx
+    646c533c:	mov    %rbx,0x2d4d(%rip)        # 646c8090 <__security_cookie_complement>
+    646c5343:	add    $0x30,%rsp
+    646c5347:	pop    %rbx
+    646c5348:	pop    %rsi
+    646c5349:	pop    %rdi
+    646c534a:	pop    %rbp
+    646c534b:	pop    %r12
+    646c534d:	ret
+    646c534e:	xchg   %ax,%ax
+    646c5350:	lea    0x20(%rsp),%rcx
+    646c5355:	call   *0x8ea1(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c535b:	mov    0x20(%rsp),%rsi
+    646c5360:	call   *0x8e7e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c5366:	mov    %eax,%r12d
+    646c5369:	call   *0x8e7d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c536f:	mov    %eax,%ebp
+    646c5371:	call   *0x8e8d(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c5377:	lea    0x28(%rsp),%rcx
+    646c537c:	mov    %eax,%edi
+    646c537e:	call   *0x8e98(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c5384:	xor    0x28(%rsp),%rsi
+    646c5389:	mov    %r12d,%eax
+    646c538c:	movabs $0xffffffffffff,%rdx
+    646c5396:	xor    %rsi,%rax
+    646c5399:	mov    %ebp,%esi
+    646c539b:	xor    %rax,%rsi
+    646c539e:	mov    %edi,%eax
+    646c53a0:	xor    %rsi,%rax
+    646c53a3:	and    %rdx,%rax
+    646c53a6:	cmp    %rbx,%rax
+    646c53a9:	je     646c53d0 <__security_init_cookie+0xc0>
+    646c53ab:	mov    %rax,%rdx
+    646c53ae:	not    %rdx
+    646c53b1:	mov    %rax,0x2cc8(%rip)        # 646c8080 <__security_cookie>
+    646c53b8:	mov    %rdx,0x2cd1(%rip)        # 646c8090 <__security_cookie_complement>
+    646c53bf:	add    $0x30,%rsp
+    646c53c3:	pop    %rbx
+    646c53c4:	pop    %rsi
+    646c53c5:	pop    %rdi
+    646c53c6:	pop    %rbp
+    646c53c7:	pop    %r12
+    646c53c9:	ret
+    646c53ca:	nopw   0x0(%rax,%rax,1)
+    646c53d0:	movabs $0xffffd466d2205dcc,%rdx
+    646c53da:	movabs $0x2b992ddfa233,%rax
+    646c53e4:	jmp    646c53b1 <__security_init_cookie+0xa1>
+    646c53e6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c53f0 <__report_gsfailure>:
+    646c53f0:	push   %rbp
+    646c53f1:	push   %rsi
+    646c53f2:	push   %rbx
+    646c53f3:	mov    %rsp,%rbp
+    646c53f6:	sub    $0x70,%rsp
+    646c53fa:	mov    %rcx,%rsi
+    646c53fd:	lea    0x6e9c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c5404:	call   *0x8e22(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c540a:	mov    0x6f87(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
+    646c5411:	lea    -0x28(%rbp),%rdx
+    646c5415:	xor    %r8d,%r8d
+    646c5418:	mov    %rbx,%rcx
+    646c541b:	call   *0x8e13(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c5421:	test   %rax,%rax
+    646c5424:	je     646c54cd <__report_gsfailure+0xdd>
+    646c542a:	lea    -0x20(%rbp),%rdx
+    646c542e:	mov    %rax,%r9
+    646c5431:	mov    %rbx,%r8
+    646c5434:	movq   $0x0,0x38(%rsp)
+    646c543d:	lea    0x6e5c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c5444:	mov    %rdx,0x30(%rsp)
+    646c5449:	lea    -0x18(%rbp),%rdx
+    646c544d:	mov    %rcx,0x20(%rsp)
+    646c5452:	xor    %ecx,%ecx
+    646c5454:	mov    %rdx,0x28(%rsp)
+    646c5459:	mov    -0x28(%rbp),%rdx
+    646c545d:	call   *0x8dd9(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c5463:	mov    0x6f2e(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
+    646c546a:	xor    %ecx,%ecx
+    646c546c:	mov    %rsi,0x6ead(%rip)        # 646cc320 <GS_ContextRecord+0x80>
+    646c5473:	mov    %rax,0x7316(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
+    646c547a:	movabs $0x1c0000409,%rax
+    646c5484:	mov    %rax,0x72f5(%rip)        # 646cc780 <GS_ExceptionRecord>
+    646c548b:	mov    0x2bee(%rip),%rax        # 646c8080 <__security_cookie>
+    646c5492:	mov    %rax,-0x10(%rbp)
+    646c5496:	mov    0x2bf3(%rip),%rax        # 646c8090 <__security_cookie_complement>
+    646c549d:	mov    %rax,-0x8(%rbp)
+    646c54a1:	call   *0x8d9d(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c54a7:	lea    0x3cc2(%rip),%rcx        # 646c9170 <GS_ExceptionPointers>
+    646c54ae:	call   *0x8db0(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c54b4:	call   *0x8d22(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c54ba:	mov    $0xc0000409,%edx
+    646c54bf:	mov    %rax,%rcx
+    646c54c2:	call   *0x8d8c(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c54c8:	call   646c7758 <abort>
+    646c54cd:	mov    0x18(%rbp),%rax
+    646c54d1:	mov    %rax,0x6ec0(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
+    646c54d8:	lea    0x8(%rbp),%rax
+    646c54dc:	mov    %rax,0x6e55(%rip)        # 646cc338 <GS_ContextRecord+0x98>
+    646c54e3:	jmp    646c5463 <__report_gsfailure+0x73>
+    646c54e8:	nop
+    646c54e9:	nop
+    646c54ea:	nop
+    646c54eb:	nop
+    646c54ec:	nop
+    646c54ed:	nop
+    646c54ee:	nop
+    646c54ef:	nop
+
+00000000646c54f0 <__dyn_tls_dtor>:
+    646c54f0:	sub    $0x28,%rsp
+    646c54f4:	cmp    $0x3,%edx
+    646c54f7:	je     646c5510 <__dyn_tls_dtor+0x20>
+    646c54f9:	test   %edx,%edx
+    646c54fb:	je     646c5510 <__dyn_tls_dtor+0x20>
+    646c54fd:	mov    $0x1,%eax
+    646c5502:	add    $0x28,%rsp
+    646c5506:	ret
+    646c5507:	nopw   0x0(%rax,%rax,1)
+    646c5510:	call   646c6070 <__mingw_TLScallback>
+    646c5515:	mov    $0x1,%eax
+    646c551a:	add    $0x28,%rsp
+    646c551e:	ret
     646c551f:	nop
 
-00000000646c5520 <_decode_pointer>:
-    646c5520:	mov    %rcx,%rax
-    646c5523:	ret
-    646c5524:	xchg   %ax,%ax
-    646c5526:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5530 <_encode_pointer>:
-    646c5530:	mov    %rcx,%rax
-    646c5533:	ret
-    646c5534:	nop
-    646c5535:	nop
-    646c5536:	nop
-    646c5537:	nop
-    646c5538:	nop
-    646c5539:	nop
-    646c553a:	nop
-    646c553b:	nop
-    646c553c:	nop
-    646c553d:	nop
-    646c553e:	nop
-    646c553f:	nop
-
-00000000646c5540 <__write_memory.part.0>:
-    646c5540:	push   %r12
-    646c5542:	push   %rbp
-    646c5543:	push   %rdi
-    646c5544:	push   %rsi
-    646c5545:	push   %rbx
-    646c5546:	sub    $0x50,%rsp
-    646c554a:	movslq 0x72f3(%rip),%rsi        # 646cc844 <maxSections>
-    646c5551:	test   %esi,%esi
-    646c5553:	mov    %rcx,%rbx
-    646c5556:	mov    %rdx,%rbp
-    646c5559:	mov    %r8,%rdi
-    646c555c:	jle    646c56c8 <__write_memory.part.0+0x188>
-    646c5562:	mov    0x72df(%rip),%rax        # 646cc848 <the_secs>
-    646c5569:	xor    %ecx,%ecx
-    646c556b:	add    $0x18,%rax
-    646c556f:	nop
-    646c5570:	mov    (%rax),%rdx
-    646c5573:	cmp    %rdx,%rbx
-    646c5576:	jb     646c558c <__write_memory.part.0+0x4c>
-    646c5578:	mov    0x8(%rax),%r8
-    646c557c:	mov    0x8(%r8),%r8d
-    646c5580:	add    %r8,%rdx
-    646c5583:	cmp    %rdx,%rbx
-    646c5586:	jb     646c5615 <__write_memory.part.0+0xd5>
-    646c558c:	add    $0x1,%ecx
-    646c558f:	add    $0x28,%rax
-    646c5593:	cmp    %esi,%ecx
-    646c5595:	jne    646c5570 <__write_memory.part.0+0x30>
-    646c5597:	mov    %rbx,%rcx
-    646c559a:	call   646c61e0 <__mingw_GetSectionForAddress>
-    646c559f:	test   %rax,%rax
-    646c55a2:	mov    %rax,%r12
-    646c55a5:	je     646c56fd <__write_memory.part.0+0x1bd>
-    646c55ab:	mov    0x7296(%rip),%rax        # 646cc848 <the_secs>
-    646c55b2:	lea    (%rsi,%rsi,4),%rsi
-    646c55b6:	shl    $0x3,%rsi
-    646c55ba:	add    %rsi,%rax
-    646c55bd:	mov    %r12,0x20(%rax)
-    646c55c1:	movl   $0x0,(%rax)
-    646c55c7:	call   646c6310 <_GetPEImageBase>
-    646c55cc:	mov    0xc(%r12),%ecx
-    646c55d1:	lea    0x20(%rsp),%rdx
-    646c55d6:	mov    $0x30,%r8d
-    646c55dc:	add    %rax,%rcx
-    646c55df:	mov    0x7262(%rip),%rax        # 646cc848 <the_secs>
-    646c55e6:	mov    %rcx,0x18(%rax,%rsi,1)
-    646c55eb:	call   *0x8c83(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c55f1:	test   %rax,%rax
-    646c55f4:	je     646c56e0 <__write_memory.part.0+0x1a0>
-    646c55fa:	mov    0x44(%rsp),%eax
-    646c55fe:	lea    -0x4(%rax),%edx
-    646c5601:	and    $0xfffffffb,%edx
-    646c5604:	je     646c560e <__write_memory.part.0+0xce>
-    646c5606:	sub    $0x40,%eax
-    646c5609:	and    $0xffffffbf,%eax
-    646c560c:	jne    646c5670 <__write_memory.part.0+0x130>
-    646c560e:	addl   $0x1,0x722f(%rip)        # 646cc844 <maxSections>
-    646c5615:	cmp    $0x8,%edi
-    646c5618:	jae    646c5643 <__write_memory.part.0+0x103>
-    646c561a:	test   $0x4,%dil
-    646c561e:	jne    646c56b4 <__write_memory.part.0+0x174>
-    646c5624:	test   %edi,%edi
-    646c5626:	je     646c5638 <__write_memory.part.0+0xf8>
-    646c5628:	movzbl 0x0(%rbp),%eax
-    646c562c:	test   $0x2,%dil
-    646c5630:	mov    %al,(%rbx)
-    646c5632:	jne    646c56cf <__write_memory.part.0+0x18f>
-    646c5638:	add    $0x50,%rsp
-    646c563c:	pop    %rbx
-    646c563d:	pop    %rsi
-    646c563e:	pop    %rdi
-    646c563f:	pop    %rbp
-    646c5640:	pop    %r12
-    646c5642:	ret
-    646c5643:	mov    %edi,%eax
-    646c5645:	sub    $0x1,%edi
-    646c5648:	mov    -0x8(%rbp,%rax,1),%rdx
-    646c564d:	cmp    $0x8,%edi
-    646c5650:	mov    %rdx,-0x8(%rbx,%rax,1)
-    646c5655:	jb     646c5638 <__write_memory.part.0+0xf8>
-    646c5657:	and    $0xfffffff8,%edi
-    646c565a:	xor    %eax,%eax
-    646c565c:	mov    %eax,%edx
-    646c565e:	add    $0x8,%eax
-    646c5661:	mov    0x0(%rbp,%rdx,1),%rcx
-    646c5666:	cmp    %edi,%eax
-    646c5668:	mov    %rcx,(%rbx,%rdx,1)
-    646c566c:	jb     646c565c <__write_memory.part.0+0x11c>
-    646c566e:	jmp    646c5638 <__write_memory.part.0+0xf8>
-    646c5670:	add    0x71d1(%rip),%rsi        # 646cc848 <the_secs>
-    646c5677:	mov    $0x40,%r8d
-    646c567d:	mov    0x20(%rsp),%rcx
-    646c5682:	mov    0x38(%rsp),%rdx
-    646c5687:	mov    %rsi,%r9
-    646c568a:	mov    %rcx,0x8(%rsi)
-    646c568e:	mov    %rdx,0x10(%rsi)
-    646c5692:	call   *0x8bd4(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c5698:	test   %eax,%eax
-    646c569a:	jne    646c560e <__write_memory.part.0+0xce>
-    646c56a0:	call   *0x8b4e(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c56a6:	lea    0x3bab(%rip),%rcx        # 646c9258 <.rdata+0x78>
-    646c56ad:	mov    %eax,%edx
-    646c56af:	call   646c7ad0 <__report_error>
-    646c56b4:	mov    0x0(%rbp),%eax
-    646c56b7:	mov    %edi,%edi
-    646c56b9:	mov    %eax,(%rbx)
-    646c56bb:	mov    -0x4(%rbp,%rdi,1),%eax
-    646c56bf:	mov    %eax,-0x4(%rbx,%rdi,1)
-    646c56c3:	jmp    646c5638 <__write_memory.part.0+0xf8>
-    646c56c8:	xor    %esi,%esi
-    646c56ca:	jmp    646c5597 <__write_memory.part.0+0x57>
-    646c56cf:	mov    %edi,%edi
-    646c56d1:	movzwl -0x2(%rbp,%rdi,1),%eax
-    646c56d6:	mov    %ax,-0x2(%rbx,%rdi,1)
-    646c56db:	jmp    646c5638 <__write_memory.part.0+0xf8>
-    646c56e0:	mov    0x7161(%rip),%rax        # 646cc848 <the_secs>
-    646c56e7:	lea    0x3b32(%rip),%rcx        # 646c9220 <.rdata+0x40>
-    646c56ee:	mov    0x8(%r12),%edx
-    646c56f3:	mov    0x18(%rax,%rsi,1),%r8
-    646c56f8:	call   646c7ad0 <__report_error>
-    646c56fd:	lea    0x3afc(%rip),%rcx        # 646c9200 <.rdata+0x20>
-    646c5704:	mov    %rbx,%rdx
-    646c5707:	call   646c7ad0 <__report_error>
-    646c570c:	nop
-    646c570d:	nopl   (%rax)
-
-00000000646c5710 <_pei386_runtime_relocator>:
-    646c5710:	push   %rbp
-    646c5711:	push   %r15
-    646c5713:	push   %r14
-    646c5715:	push   %r13
-    646c5717:	push   %r12
-    646c5719:	push   %rdi
-    646c571a:	push   %rsi
-    646c571b:	push   %rbx
-    646c571c:	sub    $0x38,%rsp
-    646c5720:	lea    0x80(%rsp),%rbp
-    646c5728:	mov    0x7112(%rip),%ebx        # 646cc840 <was_init.95174>
-    646c572e:	test   %ebx,%ebx
-    646c5730:	je     646c5743 <_pei386_runtime_relocator+0x33>
-    646c5732:	lea    -0x48(%rbp),%rsp
-    646c5736:	pop    %rbx
-    646c5737:	pop    %rsi
-    646c5738:	pop    %rdi
-    646c5739:	pop    %r12
-    646c573b:	pop    %r13
-    646c573d:	pop    %r14
-    646c573f:	pop    %r15
-    646c5741:	pop    %rbp
-    646c5742:	ret
-    646c5743:	movl   $0x1,0x70f3(%rip)        # 646cc840 <was_init.95174>
-    646c574d:	call   646c6260 <__mingw_GetSectionCount>
-    646c5752:	cltq
-    646c5754:	lea    (%rax,%rax,4),%rax
-    646c5758:	lea    0x1e(,%rax,8),%rax
-    646c5760:	and    $0xfffffffffffffff0,%rax
-    646c5764:	call   646c64b0 <___chkstk_ms>
-    646c5769:	mov    0x3e70(%rip),%r12        # 646c95e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-    646c5770:	movl   $0x0,0x70ca(%rip)        # 646cc844 <maxSections>
-    646c577a:	mov    0x3e6f(%rip),%rsi        # 646c95f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
-    646c5781:	sub    %rax,%rsp
-    646c5784:	lea    0x20(%rsp),%rax
-    646c5789:	mov    %rax,0x70b8(%rip)        # 646cc848 <the_secs>
-    646c5790:	mov    %r12,%rax
-    646c5793:	sub    %rsi,%rax
-    646c5796:	cmp    $0x7,%rax
-    646c579a:	jle    646c5732 <_pei386_runtime_relocator+0x22>
-    646c579c:	cmp    $0xb,%rax
-    646c57a0:	mov    (%rsi),%edx
-    646c57a2:	jle    646c5870 <_pei386_runtime_relocator+0x160>
-    646c57a8:	test   %edx,%edx
-    646c57aa:	je     646c5854 <_pei386_runtime_relocator+0x144>
-    646c57b0:	cmp    %r12,%rsi
-    646c57b3:	jae    646c5732 <_pei386_runtime_relocator+0x22>
-    646c57b9:	lea    0x8(%rsi),%r14
-    646c57bd:	add    $0x7,%r12
-    646c57c1:	mov    0x3e48(%rip),%r13        # 646c9610 <.refptr.__image_base__>
-    646c57c8:	lea    -0x58(%rbp),%rdi
-    646c57cc:	sub    %r14,%r12
-    646c57cf:	shr    $0x3,%r12
-    646c57d3:	lea    0x8(%rsi,%r12,8),%r12
-    646c57d8:	jmp    646c57e4 <_pei386_runtime_relocator+0xd4>
-    646c57da:	nopw   0x0(%rax,%rax,1)
-    646c57e0:	add    $0x8,%r14
-    646c57e4:	mov    0x4(%rsi),%ecx
-    646c57e7:	mov    $0x4,%r8d
-    646c57ed:	mov    %rdi,%rdx
-    646c57f0:	mov    (%rsi),%eax
-    646c57f2:	mov    %r14,%rsi
-    646c57f5:	add    %r13,%rcx
-    646c57f8:	add    (%rcx),%eax
-    646c57fa:	mov    %eax,-0x58(%rbp)
-    646c57fd:	call   646c5540 <__write_memory.part.0>
-    646c5802:	cmp    %r12,%r14
-    646c5805:	jne    646c57e0 <_pei386_runtime_relocator+0xd0>
-    646c5807:	mov    0x7037(%rip),%eax        # 646cc844 <maxSections>
-    646c580d:	xor    %esi,%esi
-    646c580f:	mov    0x8a56(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
-    646c5816:	test   %eax,%eax
-    646c5818:	jle    646c5732 <_pei386_runtime_relocator+0x22>
-    646c581e:	xchg   %ax,%ax
-    646c5820:	mov    0x7021(%rip),%rax        # 646cc848 <the_secs>
-    646c5827:	add    %rsi,%rax
-    646c582a:	mov    (%rax),%r8d
-    646c582d:	test   %r8d,%r8d
-    646c5830:	je     646c5840 <_pei386_runtime_relocator+0x130>
-    646c5832:	mov    0x10(%rax),%rdx
-    646c5836:	mov    %rdi,%r9
-    646c5839:	mov    0x8(%rax),%rcx
-    646c583d:	call   *%r12
-    646c5840:	add    $0x1,%ebx
-    646c5843:	add    $0x28,%rsi
-    646c5847:	cmp    0x6ff7(%rip),%ebx        # 646cc844 <maxSections>
-    646c584d:	jl     646c5820 <_pei386_runtime_relocator+0x110>
-    646c584f:	jmp    646c5732 <_pei386_runtime_relocator+0x22>
-    646c5854:	mov    0x4(%rsi),%ecx
-    646c5857:	test   %ecx,%ecx
-    646c5859:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
-    646c585f:	mov    0x8(%rsi),%edx
-    646c5862:	test   %edx,%edx
-    646c5864:	jne    646c5883 <_pei386_runtime_relocator+0x173>
-    646c5866:	mov    0xc(%rsi),%edx
-    646c5869:	add    $0xc,%rsi
-    646c586d:	nopl   (%rax)
-    646c5870:	test   %edx,%edx
-    646c5872:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
-    646c5878:	mov    0x4(%rsi),%eax
-    646c587b:	test   %eax,%eax
-    646c587d:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
-    646c5883:	mov    0x8(%rsi),%edx
-    646c5886:	cmp    $0x1,%edx
-    646c5889:	jne    646c59be <_pei386_runtime_relocator+0x2ae>
-    646c588f:	mov    0x3d7a(%rip),%r13        # 646c9610 <.refptr.__image_base__>
-    646c5896:	add    $0xc,%rsi
-    646c589a:	movabs $0xffffffff00000000,%r15
-    646c58a4:	lea    -0x58(%rbp),%r14
-    646c58a8:	cmp    %r12,%rsi
-    646c58ab:	jb     646c58f5 <_pei386_runtime_relocator+0x1e5>
-    646c58ad:	jmp    646c5732 <_pei386_runtime_relocator+0x22>
-    646c58b2:	jbe    646c5970 <_pei386_runtime_relocator+0x260>
-    646c58b8:	cmp    $0x20,%edx
-    646c58bb:	je     646c5940 <_pei386_runtime_relocator+0x230>
-    646c58c1:	cmp    $0x40,%edx
-    646c58c4:	jne    646c59aa <_pei386_runtime_relocator+0x29a>
-    646c58ca:	mov    (%rcx),%rdx
-    646c58cd:	mov    $0x8,%r8d
-    646c58d3:	mov    %r14,%rdi
-    646c58d6:	sub    %rax,%rdx
-    646c58d9:	add    %r9,%rdx
-    646c58dc:	mov    %rdx,-0x58(%rbp)
-    646c58e0:	mov    %r14,%rdx
-    646c58e3:	call   646c5540 <__write_memory.part.0>
-    646c58e8:	add    $0xc,%rsi
-    646c58ec:	cmp    %r12,%rsi
-    646c58ef:	jae    646c5807 <_pei386_runtime_relocator+0xf7>
-    646c58f5:	mov    0x4(%rsi),%ecx
-    646c58f8:	mov    (%rsi),%eax
-    646c58fa:	movzbl 0x8(%rsi),%edx
-    646c58fe:	add    %r13,%rcx
-    646c5901:	add    %r13,%rax
-    646c5904:	cmp    $0x10,%edx
-    646c5907:	mov    (%rax),%r9
-    646c590a:	jne    646c58b2 <_pei386_runtime_relocator+0x1a2>
-    646c590c:	movzwl (%rcx),%r8d
-    646c5910:	mov    %r14,%rdx
-    646c5913:	mov    %r14,%rdi
-    646c5916:	mov    %r8,%r10
-    646c5919:	or     $0xffffffffffff0000,%r10
-    646c5920:	test   %r8w,%r8w
-    646c5924:	cmovs  %r10,%r8
-    646c5928:	sub    %rax,%r8
-    646c592b:	add    %r9,%r8
-    646c592e:	mov    %r8,-0x58(%rbp)
-    646c5932:	mov    $0x2,%r8d
-    646c5938:	call   646c5540 <__write_memory.part.0>
-    646c593d:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
-    646c593f:	nop
-    646c5940:	mov    (%rcx),%edx
-    646c5942:	mov    %r14,%rdi
-    646c5945:	mov    %rdx,%r8
-    646c5948:	or     %r15,%rdx
-    646c594b:	test   %r8d,%r8d
-    646c594e:	cmovns %r8,%rdx
-    646c5952:	mov    $0x4,%r8d
-    646c5958:	sub    %rax,%rdx
-    646c595b:	add    %r9,%rdx
-    646c595e:	mov    %rdx,-0x58(%rbp)
-    646c5962:	mov    %r14,%rdx
-    646c5965:	call   646c5540 <__write_memory.part.0>
-    646c596a:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
-    646c596f:	nop
-    646c5970:	cmp    $0x8,%edx
-    646c5973:	jne    646c59aa <_pei386_runtime_relocator+0x29a>
-    646c5975:	movzbl (%rcx),%r8d
-    646c5979:	mov    %r14,%rdx
-    646c597c:	mov    %r14,%rdi
-    646c597f:	mov    %r8,%r10
-    646c5982:	or     $0xffffffffffffff00,%r10
-    646c5989:	test   %r8b,%r8b
-    646c598c:	cmovs  %r10,%r8
-    646c5990:	sub    %rax,%r8
-    646c5993:	add    %r9,%r8
-    646c5996:	mov    %r8,-0x58(%rbp)
-    646c599a:	mov    $0x1,%r8d
-    646c59a0:	call   646c5540 <__write_memory.part.0>
-    646c59a5:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
-    646c59aa:	lea    0x3907(%rip),%rcx        # 646c92b8 <.rdata+0xd8>
-    646c59b1:	movq   $0x0,-0x58(%rbp)
-    646c59b9:	call   646c7ad0 <__report_error>
-    646c59be:	lea    0x38bb(%rip),%rcx        # 646c9280 <.rdata+0xa0>
-    646c59c5:	call   646c7ad0 <__report_error>
-    646c59ca:	nop
-    646c59cb:	nop
-    646c59cc:	nop
-    646c59cd:	nop
-    646c59ce:	nop
+00000000646c5520 <__dyn_tls_init>:
+    646c5520:	push   %rsi
+    646c5521:	push   %rbx
+    646c5522:	sub    $0x28,%rsp
+    646c5526:	mov    0x4093(%rip),%rax        # 646c95c0 <.refptr._CRT_MT>
+    646c552d:	cmpl   $0x2,(%rax)
+    646c5530:	je     646c5538 <__dyn_tls_init+0x18>
+    646c5532:	movl   $0x2,(%rax)
+    646c5538:	cmp    $0x2,%edx
+    646c553b:	je     646c5550 <__dyn_tls_init+0x30>
+    646c553d:	cmp    $0x1,%edx
+    646c5540:	je     646c5582 <__dyn_tls_init+0x62>
+    646c5542:	mov    $0x1,%eax
+    646c5547:	add    $0x28,%rsp
+    646c554b:	pop    %rbx
+    646c554c:	pop    %rsi
+    646c554d:	ret
+    646c554e:	xchg   %ax,%ax
+    646c5550:	lea    0x9af9(%rip),%rbx        # 646cf050 <__xd_z>
+    646c5557:	lea    0x9af2(%rip),%rsi        # 646cf050 <__xd_z>
+    646c555e:	cmp    %rbx,%rsi
+    646c5561:	je     646c5542 <__dyn_tls_init+0x22>
+    646c5563:	mov    (%rbx),%rax
+    646c5566:	test   %rax,%rax
+    646c5569:	je     646c556d <__dyn_tls_init+0x4d>
+    646c556b:	call   *%rax
+    646c556d:	add    $0x8,%rbx
+    646c5571:	cmp    %rbx,%rsi
+    646c5574:	jne    646c5563 <__dyn_tls_init+0x43>
+    646c5576:	mov    $0x1,%eax
+    646c557b:	add    $0x28,%rsp
+    646c557f:	pop    %rbx
+    646c5580:	pop    %rsi
+    646c5581:	ret
+    646c5582:	call   646c6070 <__mingw_TLScallback>
+    646c5587:	mov    $0x1,%eax
+    646c558c:	add    $0x28,%rsp
+    646c5590:	pop    %rbx
+    646c5591:	pop    %rsi
+    646c5592:	ret
+    646c5593:	nopl   (%rax)
+    646c5596:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c55a0 <__tlregdtor>:
+    646c55a0:	xor    %eax,%eax
+    646c55a2:	ret
+    646c55a3:	nop
+    646c55a4:	nop
+    646c55a5:	nop
+    646c55a6:	nop
+    646c55a7:	nop
+    646c55a8:	nop
+    646c55a9:	nop
+    646c55aa:	nop
+    646c55ab:	nop
+    646c55ac:	nop
+    646c55ad:	nop
+    646c55ae:	nop
+    646c55af:	nop
+
+00000000646c55b0 <_decode_pointer>:
+    646c55b0:	mov    %rcx,%rax
+    646c55b3:	ret
+    646c55b4:	xchg   %ax,%ax
+    646c55b6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c55c0 <_encode_pointer>:
+    646c55c0:	mov    %rcx,%rax
+    646c55c3:	ret
+    646c55c4:	nop
+    646c55c5:	nop
+    646c55c6:	nop
+    646c55c7:	nop
+    646c55c8:	nop
+    646c55c9:	nop
+    646c55ca:	nop
+    646c55cb:	nop
+    646c55cc:	nop
+    646c55cd:	nop
+    646c55ce:	nop
+    646c55cf:	nop
+
+00000000646c55d0 <__write_memory.part.0>:
+    646c55d0:	push   %r12
+    646c55d2:	push   %rbp
+    646c55d3:	push   %rdi
+    646c55d4:	push   %rsi
+    646c55d5:	push   %rbx
+    646c55d6:	sub    $0x50,%rsp
+    646c55da:	movslq 0x7263(%rip),%rsi        # 646cc844 <maxSections>
+    646c55e1:	test   %esi,%esi
+    646c55e3:	mov    %rcx,%rbx
+    646c55e6:	mov    %rdx,%rbp
+    646c55e9:	mov    %r8,%rdi
+    646c55ec:	jle    646c5758 <__write_memory.part.0+0x188>
+    646c55f2:	mov    0x724f(%rip),%rax        # 646cc848 <the_secs>
+    646c55f9:	xor    %ecx,%ecx
+    646c55fb:	add    $0x18,%rax
+    646c55ff:	nop
+    646c5600:	mov    (%rax),%rdx
+    646c5603:	cmp    %rdx,%rbx
+    646c5606:	jb     646c561c <__write_memory.part.0+0x4c>
+    646c5608:	mov    0x8(%rax),%r8
+    646c560c:	mov    0x8(%r8),%r8d
+    646c5610:	add    %r8,%rdx
+    646c5613:	cmp    %rdx,%rbx
+    646c5616:	jb     646c56a5 <__write_memory.part.0+0xd5>
+    646c561c:	add    $0x1,%ecx
+    646c561f:	add    $0x28,%rax
+    646c5623:	cmp    %esi,%ecx
+    646c5625:	jne    646c5600 <__write_memory.part.0+0x30>
+    646c5627:	mov    %rbx,%rcx
+    646c562a:	call   646c6270 <__mingw_GetSectionForAddress>
+    646c562f:	test   %rax,%rax
+    646c5632:	mov    %rax,%r12
+    646c5635:	je     646c578d <__write_memory.part.0+0x1bd>
+    646c563b:	mov    0x7206(%rip),%rax        # 646cc848 <the_secs>
+    646c5642:	lea    (%rsi,%rsi,4),%rsi
+    646c5646:	shl    $0x3,%rsi
+    646c564a:	add    %rsi,%rax
+    646c564d:	mov    %r12,0x20(%rax)
+    646c5651:	movl   $0x0,(%rax)
+    646c5657:	call   646c63a0 <_GetPEImageBase>
+    646c565c:	mov    0xc(%r12),%ecx
+    646c5661:	lea    0x20(%rsp),%rdx
+    646c5666:	mov    $0x30,%r8d
+    646c566c:	add    %rax,%rcx
+    646c566f:	mov    0x71d2(%rip),%rax        # 646cc848 <the_secs>
+    646c5676:	mov    %rcx,0x18(%rax,%rsi,1)
+    646c567b:	call   *0x8bf3(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c5681:	test   %rax,%rax
+    646c5684:	je     646c5770 <__write_memory.part.0+0x1a0>
+    646c568a:	mov    0x44(%rsp),%eax
+    646c568e:	lea    -0x4(%rax),%edx
+    646c5691:	and    $0xfffffffb,%edx
+    646c5694:	je     646c569e <__write_memory.part.0+0xce>
+    646c5696:	sub    $0x40,%eax
+    646c5699:	and    $0xffffffbf,%eax
+    646c569c:	jne    646c5700 <__write_memory.part.0+0x130>
+    646c569e:	addl   $0x1,0x719f(%rip)        # 646cc844 <maxSections>
+    646c56a5:	cmp    $0x8,%edi
+    646c56a8:	jae    646c56d3 <__write_memory.part.0+0x103>
+    646c56aa:	test   $0x4,%dil
+    646c56ae:	jne    646c5744 <__write_memory.part.0+0x174>
+    646c56b4:	test   %edi,%edi
+    646c56b6:	je     646c56c8 <__write_memory.part.0+0xf8>
+    646c56b8:	movzbl 0x0(%rbp),%eax
+    646c56bc:	test   $0x2,%dil
+    646c56c0:	mov    %al,(%rbx)
+    646c56c2:	jne    646c575f <__write_memory.part.0+0x18f>
+    646c56c8:	add    $0x50,%rsp
+    646c56cc:	pop    %rbx
+    646c56cd:	pop    %rsi
+    646c56ce:	pop    %rdi
+    646c56cf:	pop    %rbp
+    646c56d0:	pop    %r12
+    646c56d2:	ret
+    646c56d3:	mov    %edi,%eax
+    646c56d5:	sub    $0x1,%edi
+    646c56d8:	mov    -0x8(%rbp,%rax,1),%rdx
+    646c56dd:	cmp    $0x8,%edi
+    646c56e0:	mov    %rdx,-0x8(%rbx,%rax,1)
+    646c56e5:	jb     646c56c8 <__write_memory.part.0+0xf8>
+    646c56e7:	and    $0xfffffff8,%edi
+    646c56ea:	xor    %eax,%eax
+    646c56ec:	mov    %eax,%edx
+    646c56ee:	add    $0x8,%eax
+    646c56f1:	mov    0x0(%rbp,%rdx,1),%rcx
+    646c56f6:	cmp    %edi,%eax
+    646c56f8:	mov    %rcx,(%rbx,%rdx,1)
+    646c56fc:	jb     646c56ec <__write_memory.part.0+0x11c>
+    646c56fe:	jmp    646c56c8 <__write_memory.part.0+0xf8>
+    646c5700:	add    0x7141(%rip),%rsi        # 646cc848 <the_secs>
+    646c5707:	mov    $0x40,%r8d
+    646c570d:	mov    0x20(%rsp),%rcx
+    646c5712:	mov    0x38(%rsp),%rdx
+    646c5717:	mov    %rsi,%r9
+    646c571a:	mov    %rcx,0x8(%rsi)
+    646c571e:	mov    %rdx,0x10(%rsi)
+    646c5722:	call   *0x8b44(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c5728:	test   %eax,%eax
+    646c572a:	jne    646c569e <__write_memory.part.0+0xce>
+    646c5730:	call   *0x8abe(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c5736:	lea    0x3b1b(%rip),%rcx        # 646c9258 <.rdata+0x78>
+    646c573d:	mov    %eax,%edx
+    646c573f:	call   646c7b60 <__report_error>
+    646c5744:	mov    0x0(%rbp),%eax
+    646c5747:	mov    %edi,%edi
+    646c5749:	mov    %eax,(%rbx)
+    646c574b:	mov    -0x4(%rbp,%rdi,1),%eax
+    646c574f:	mov    %eax,-0x4(%rbx,%rdi,1)
+    646c5753:	jmp    646c56c8 <__write_memory.part.0+0xf8>
+    646c5758:	xor    %esi,%esi
+    646c575a:	jmp    646c5627 <__write_memory.part.0+0x57>
+    646c575f:	mov    %edi,%edi
+    646c5761:	movzwl -0x2(%rbp,%rdi,1),%eax
+    646c5766:	mov    %ax,-0x2(%rbx,%rdi,1)
+    646c576b:	jmp    646c56c8 <__write_memory.part.0+0xf8>
+    646c5770:	mov    0x70d1(%rip),%rax        # 646cc848 <the_secs>
+    646c5777:	lea    0x3aa2(%rip),%rcx        # 646c9220 <.rdata+0x40>
+    646c577e:	mov    0x8(%r12),%edx
+    646c5783:	mov    0x18(%rax,%rsi,1),%r8
+    646c5788:	call   646c7b60 <__report_error>
+    646c578d:	lea    0x3a6c(%rip),%rcx        # 646c9200 <.rdata+0x20>
+    646c5794:	mov    %rbx,%rdx
+    646c5797:	call   646c7b60 <__report_error>
+    646c579c:	nop
+    646c579d:	nopl   (%rax)
+
+00000000646c57a0 <_pei386_runtime_relocator>:
+    646c57a0:	push   %rbp
+    646c57a1:	push   %r15
+    646c57a3:	push   %r14
+    646c57a5:	push   %r13
+    646c57a7:	push   %r12
+    646c57a9:	push   %rdi
+    646c57aa:	push   %rsi
+    646c57ab:	push   %rbx
+    646c57ac:	sub    $0x38,%rsp
+    646c57b0:	lea    0x80(%rsp),%rbp
+    646c57b8:	mov    0x7082(%rip),%ebx        # 646cc840 <was_init.95174>
+    646c57be:	test   %ebx,%ebx
+    646c57c0:	je     646c57d3 <_pei386_runtime_relocator+0x33>
+    646c57c2:	lea    -0x48(%rbp),%rsp
+    646c57c6:	pop    %rbx
+    646c57c7:	pop    %rsi
+    646c57c8:	pop    %rdi
+    646c57c9:	pop    %r12
+    646c57cb:	pop    %r13
+    646c57cd:	pop    %r14
+    646c57cf:	pop    %r15
+    646c57d1:	pop    %rbp
+    646c57d2:	ret
+    646c57d3:	movl   $0x1,0x7063(%rip)        # 646cc840 <was_init.95174>
+    646c57dd:	call   646c62f0 <__mingw_GetSectionCount>
+    646c57e2:	cltq
+    646c57e4:	lea    (%rax,%rax,4),%rax
+    646c57e8:	lea    0x1e(,%rax,8),%rax
+    646c57f0:	and    $0xfffffffffffffff0,%rax
+    646c57f4:	call   646c6540 <___chkstk_ms>
+    646c57f9:	mov    0x3de0(%rip),%r12        # 646c95e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+    646c5800:	movl   $0x0,0x703a(%rip)        # 646cc844 <maxSections>
+    646c580a:	mov    0x3ddf(%rip),%rsi        # 646c95f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+    646c5811:	sub    %rax,%rsp
+    646c5814:	lea    0x20(%rsp),%rax
+    646c5819:	mov    %rax,0x7028(%rip)        # 646cc848 <the_secs>
+    646c5820:	mov    %r12,%rax
+    646c5823:	sub    %rsi,%rax
+    646c5826:	cmp    $0x7,%rax
+    646c582a:	jle    646c57c2 <_pei386_runtime_relocator+0x22>
+    646c582c:	cmp    $0xb,%rax
+    646c5830:	mov    (%rsi),%edx
+    646c5832:	jle    646c5900 <_pei386_runtime_relocator+0x160>
+    646c5838:	test   %edx,%edx
+    646c583a:	je     646c58e4 <_pei386_runtime_relocator+0x144>
+    646c5840:	cmp    %r12,%rsi
+    646c5843:	jae    646c57c2 <_pei386_runtime_relocator+0x22>
+    646c5849:	lea    0x8(%rsi),%r14
+    646c584d:	add    $0x7,%r12
+    646c5851:	mov    0x3db8(%rip),%r13        # 646c9610 <.refptr.__image_base__>
+    646c5858:	lea    -0x58(%rbp),%rdi
+    646c585c:	sub    %r14,%r12
+    646c585f:	shr    $0x3,%r12
+    646c5863:	lea    0x8(%rsi,%r12,8),%r12
+    646c5868:	jmp    646c5874 <_pei386_runtime_relocator+0xd4>
+    646c586a:	nopw   0x0(%rax,%rax,1)
+    646c5870:	add    $0x8,%r14
+    646c5874:	mov    0x4(%rsi),%ecx
+    646c5877:	mov    $0x4,%r8d
+    646c587d:	mov    %rdi,%rdx
+    646c5880:	mov    (%rsi),%eax
+    646c5882:	mov    %r14,%rsi
+    646c5885:	add    %r13,%rcx
+    646c5888:	add    (%rcx),%eax
+    646c588a:	mov    %eax,-0x58(%rbp)
+    646c588d:	call   646c55d0 <__write_memory.part.0>
+    646c5892:	cmp    %r12,%r14
+    646c5895:	jne    646c5870 <_pei386_runtime_relocator+0xd0>
+    646c5897:	mov    0x6fa7(%rip),%eax        # 646cc844 <maxSections>
+    646c589d:	xor    %esi,%esi
+    646c589f:	mov    0x89c6(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
+    646c58a6:	test   %eax,%eax
+    646c58a8:	jle    646c57c2 <_pei386_runtime_relocator+0x22>
+    646c58ae:	xchg   %ax,%ax
+    646c58b0:	mov    0x6f91(%rip),%rax        # 646cc848 <the_secs>
+    646c58b7:	add    %rsi,%rax
+    646c58ba:	mov    (%rax),%r8d
+    646c58bd:	test   %r8d,%r8d
+    646c58c0:	je     646c58d0 <_pei386_runtime_relocator+0x130>
+    646c58c2:	mov    0x10(%rax),%rdx
+    646c58c6:	mov    %rdi,%r9
+    646c58c9:	mov    0x8(%rax),%rcx
+    646c58cd:	call   *%r12
+    646c58d0:	add    $0x1,%ebx
+    646c58d3:	add    $0x28,%rsi
+    646c58d7:	cmp    0x6f67(%rip),%ebx        # 646cc844 <maxSections>
+    646c58dd:	jl     646c58b0 <_pei386_runtime_relocator+0x110>
+    646c58df:	jmp    646c57c2 <_pei386_runtime_relocator+0x22>
+    646c58e4:	mov    0x4(%rsi),%ecx
+    646c58e7:	test   %ecx,%ecx
+    646c58e9:	jne    646c5840 <_pei386_runtime_relocator+0xa0>
+    646c58ef:	mov    0x8(%rsi),%edx
+    646c58f2:	test   %edx,%edx
+    646c58f4:	jne    646c5913 <_pei386_runtime_relocator+0x173>
+    646c58f6:	mov    0xc(%rsi),%edx
+    646c58f9:	add    $0xc,%rsi
+    646c58fd:	nopl   (%rax)
+    646c5900:	test   %edx,%edx
+    646c5902:	jne    646c5840 <_pei386_runtime_relocator+0xa0>
+    646c5908:	mov    0x4(%rsi),%eax
+    646c590b:	test   %eax,%eax
+    646c590d:	jne    646c5840 <_pei386_runtime_relocator+0xa0>
+    646c5913:	mov    0x8(%rsi),%edx
+    646c5916:	cmp    $0x1,%edx
+    646c5919:	jne    646c5a4e <_pei386_runtime_relocator+0x2ae>
+    646c591f:	mov    0x3cea(%rip),%r13        # 646c9610 <.refptr.__image_base__>
+    646c5926:	add    $0xc,%rsi
+    646c592a:	movabs $0xffffffff00000000,%r15
+    646c5934:	lea    -0x58(%rbp),%r14
+    646c5938:	cmp    %r12,%rsi
+    646c593b:	jb     646c5985 <_pei386_runtime_relocator+0x1e5>
+    646c593d:	jmp    646c57c2 <_pei386_runtime_relocator+0x22>
+    646c5942:	jbe    646c5a00 <_pei386_runtime_relocator+0x260>
+    646c5948:	cmp    $0x20,%edx
+    646c594b:	je     646c59d0 <_pei386_runtime_relocator+0x230>
+    646c5951:	cmp    $0x40,%edx
+    646c5954:	jne    646c5a3a <_pei386_runtime_relocator+0x29a>
+    646c595a:	mov    (%rcx),%rdx
+    646c595d:	mov    $0x8,%r8d
+    646c5963:	mov    %r14,%rdi
+    646c5966:	sub    %rax,%rdx
+    646c5969:	add    %r9,%rdx
+    646c596c:	mov    %rdx,-0x58(%rbp)
+    646c5970:	mov    %r14,%rdx
+    646c5973:	call   646c55d0 <__write_memory.part.0>
+    646c5978:	add    $0xc,%rsi
+    646c597c:	cmp    %r12,%rsi
+    646c597f:	jae    646c5897 <_pei386_runtime_relocator+0xf7>
+    646c5985:	mov    0x4(%rsi),%ecx
+    646c5988:	mov    (%rsi),%eax
+    646c598a:	movzbl 0x8(%rsi),%edx
+    646c598e:	add    %r13,%rcx
+    646c5991:	add    %r13,%rax
+    646c5994:	cmp    $0x10,%edx
+    646c5997:	mov    (%rax),%r9
+    646c599a:	jne    646c5942 <_pei386_runtime_relocator+0x1a2>
+    646c599c:	movzwl (%rcx),%r8d
+    646c59a0:	mov    %r14,%rdx
+    646c59a3:	mov    %r14,%rdi
+    646c59a6:	mov    %r8,%r10
+    646c59a9:	or     $0xffffffffffff0000,%r10
+    646c59b0:	test   %r8w,%r8w
+    646c59b4:	cmovs  %r10,%r8
+    646c59b8:	sub    %rax,%r8
+    646c59bb:	add    %r9,%r8
+    646c59be:	mov    %r8,-0x58(%rbp)
+    646c59c2:	mov    $0x2,%r8d
+    646c59c8:	call   646c55d0 <__write_memory.part.0>
+    646c59cd:	jmp    646c5978 <_pei386_runtime_relocator+0x1d8>
     646c59cf:	nop
-
-00000000646c59d0 <__mingw_SEH_error_handler>:
-    646c59d0:	sub    $0x28,%rsp
-    646c59d4:	mov    (%rcx),%eax
-    646c59d6:	cmp    $0xc0000091,%eax
-    646c59db:	ja     646c5a40 <__mingw_SEH_error_handler+0x70>
-    646c59dd:	cmp    $0xc000008d,%eax
-    646c59e2:	jae    646c5a5f <__mingw_SEH_error_handler+0x8f>
-    646c59e4:	cmp    $0xc0000008,%eax
-    646c59e9:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
-    646c59ef:	ja     646c5ac0 <__mingw_SEH_error_handler+0xf0>
-    646c59f5:	cmp    $0x80000002,%eax
-    646c59fa:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
-    646c5a00:	cmp    $0xc0000005,%eax
-    646c5a05:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
-    646c5a0b:	xor    %edx,%edx
-    646c5a0d:	mov    $0xb,%ecx
-    646c5a12:	call   646c7668 <signal>
-    646c5a17:	cmp    $0x1,%rax
-    646c5a1b:	je     646c5b50 <__mingw_SEH_error_handler+0x180>
-    646c5a21:	test   %rax,%rax
-    646c5a24:	je     646c5b66 <__mingw_SEH_error_handler+0x196>
-    646c5a2a:	mov    $0xb,%ecx
-    646c5a2f:	call   *%rax
-    646c5a31:	xor    %eax,%eax
-    646c5a33:	add    $0x28,%rsp
-    646c5a37:	ret
-    646c5a38:	nopl   0x0(%rax,%rax,1)
-    646c5a40:	cmp    $0xc0000094,%eax
-    646c5a45:	je     646c5b00 <__mingw_SEH_error_handler+0x130>
-    646c5a4b:	ja     646c5a84 <__mingw_SEH_error_handler+0xb4>
-    646c5a4d:	cmp    $0xc0000092,%eax
-    646c5a52:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
-    646c5a58:	cmp    $0xc0000093,%eax
-    646c5a5d:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
-    646c5a5f:	xor    %edx,%edx
-    646c5a61:	mov    $0x8,%ecx
-    646c5a66:	call   646c7668 <signal>
-    646c5a6b:	cmp    $0x1,%rax
-    646c5a6f:	je     646c5ae0 <__mingw_SEH_error_handler+0x110>
-    646c5a71:	test   %rax,%rax
-    646c5a74:	je     646c5ace <__mingw_SEH_error_handler+0xfe>
-    646c5a76:	mov    $0x8,%ecx
-    646c5a7b:	call   *%rax
-    646c5a7d:	xor    %eax,%eax
-    646c5a7f:	add    $0x28,%rsp
-    646c5a83:	ret
-    646c5a84:	cmp    $0xc0000095,%eax
-    646c5a89:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
-    646c5a8b:	cmp    $0xc0000096,%eax
-    646c5a90:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
-    646c5a92:	xor    %edx,%edx
-    646c5a94:	mov    $0x4,%ecx
-    646c5a99:	call   646c7668 <signal>
-    646c5a9e:	cmp    $0x1,%rax
-    646c5aa2:	je     646c5b30 <__mingw_SEH_error_handler+0x160>
-    646c5aa8:	test   %rax,%rax
-    646c5aab:	je     646c5b66 <__mingw_SEH_error_handler+0x196>
-    646c5ab1:	mov    $0x4,%ecx
-    646c5ab6:	call   *%rax
-    646c5ab8:	xor    %eax,%eax
-    646c5aba:	add    $0x28,%rsp
-    646c5abe:	ret
-    646c5abf:	nop
-    646c5ac0:	cmp    $0xc000001d,%eax
-    646c5ac5:	je     646c5a92 <__mingw_SEH_error_handler+0xc2>
-    646c5ac7:	cmp    $0xc000008c,%eax
-    646c5acc:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
-    646c5ace:	mov    $0x1,%eax
-    646c5ad3:	add    $0x28,%rsp
-    646c5ad7:	ret
-    646c5ad8:	nopl   0x0(%rax,%rax,1)
-    646c5ae0:	mov    $0x1,%edx
-    646c5ae5:	mov    $0x8,%ecx
-    646c5aea:	call   646c7668 <signal>
-    646c5aef:	call   646c64a0 <_fpreset>
-    646c5af4:	xor    %eax,%eax
-    646c5af6:	add    $0x28,%rsp
-    646c5afa:	ret
-    646c5afb:	nopl   0x0(%rax,%rax,1)
-    646c5b00:	xor    %edx,%edx
-    646c5b02:	mov    $0x8,%ecx
-    646c5b07:	call   646c7668 <signal>
-    646c5b0c:	cmp    $0x1,%rax
-    646c5b10:	jne    646c5a71 <__mingw_SEH_error_handler+0xa1>
-    646c5b16:	mov    $0x1,%edx
-    646c5b1b:	mov    $0x8,%ecx
-    646c5b20:	call   646c7668 <signal>
-    646c5b25:	xor    %eax,%eax
-    646c5b27:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
-    646c5b2c:	nopl   0x0(%rax)
-    646c5b30:	mov    $0x1,%edx
-    646c5b35:	mov    $0x4,%ecx
-    646c5b3a:	call   646c7668 <signal>
-    646c5b3f:	xor    %eax,%eax
-    646c5b41:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
-    646c5b46:	cs nopw 0x0(%rax,%rax,1)
-    646c5b50:	mov    $0x1,%edx
-    646c5b55:	mov    $0xb,%ecx
-    646c5b5a:	call   646c7668 <signal>
-    646c5b5f:	xor    %eax,%eax
-    646c5b61:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
-    646c5b66:	mov    $0x4,%eax
-    646c5b6b:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
-
-00000000646c5b70 <__mingw_init_ehandler>:
-    646c5b70:	push   %r12
-    646c5b72:	push   %rbp
-    646c5b73:	push   %rdi
-    646c5b74:	push   %rsi
-    646c5b75:	push   %rbx
-    646c5b76:	sub    $0x20,%rsp
-    646c5b7a:	call   646c6310 <_GetPEImageBase>
-    646c5b7f:	mov    %rax,%rbp
-    646c5b82:	mov    0x6ce0(%rip),%eax        # 646cc868 <was_here.95013>
-    646c5b88:	test   %eax,%eax
-    646c5b8a:	jne    646c5bb1 <__mingw_init_ehandler+0x41>
-    646c5b8c:	test   %rbp,%rbp
-    646c5b8f:	je     646c5bb1 <__mingw_init_ehandler+0x41>
-    646c5b91:	lea    0x3758(%rip),%rcx        # 646c92f0 <.rdata>
-    646c5b98:	movl   $0x1,0x6cc6(%rip)        # 646cc868 <was_here.95013>
-    646c5ba2:	call   646c6150 <_FindPESectionByName>
-    646c5ba7:	test   %rax,%rax
-    646c5baa:	je     646c5bc0 <__mingw_init_ehandler+0x50>
-    646c5bac:	mov    $0x1,%eax
-    646c5bb1:	add    $0x20,%rsp
-    646c5bb5:	pop    %rbx
-    646c5bb6:	pop    %rsi
-    646c5bb7:	pop    %rdi
-    646c5bb8:	pop    %rbp
-    646c5bb9:	pop    %r12
-    646c5bbb:	ret
+    646c59d0:	mov    (%rcx),%edx
+    646c59d2:	mov    %r14,%rdi
+    646c59d5:	mov    %rdx,%r8
+    646c59d8:	or     %r15,%rdx
+    646c59db:	test   %r8d,%r8d
+    646c59de:	cmovns %r8,%rdx
+    646c59e2:	mov    $0x4,%r8d
+    646c59e8:	sub    %rax,%rdx
+    646c59eb:	add    %r9,%rdx
+    646c59ee:	mov    %rdx,-0x58(%rbp)
+    646c59f2:	mov    %r14,%rdx
+    646c59f5:	call   646c55d0 <__write_memory.part.0>
+    646c59fa:	jmp    646c5978 <_pei386_runtime_relocator+0x1d8>
+    646c59ff:	nop
+    646c5a00:	cmp    $0x8,%edx
+    646c5a03:	jne    646c5a3a <_pei386_runtime_relocator+0x29a>
+    646c5a05:	movzbl (%rcx),%r8d
+    646c5a09:	mov    %r14,%rdx
+    646c5a0c:	mov    %r14,%rdi
+    646c5a0f:	mov    %r8,%r10
+    646c5a12:	or     $0xffffffffffffff00,%r10
+    646c5a19:	test   %r8b,%r8b
+    646c5a1c:	cmovs  %r10,%r8
+    646c5a20:	sub    %rax,%r8
+    646c5a23:	add    %r9,%r8
+    646c5a26:	mov    %r8,-0x58(%rbp)
+    646c5a2a:	mov    $0x1,%r8d
+    646c5a30:	call   646c55d0 <__write_memory.part.0>
+    646c5a35:	jmp    646c5978 <_pei386_runtime_relocator+0x1d8>
+    646c5a3a:	lea    0x3877(%rip),%rcx        # 646c92b8 <.rdata+0xd8>
+    646c5a41:	movq   $0x0,-0x58(%rbp)
+    646c5a49:	call   646c7b60 <__report_error>
+    646c5a4e:	lea    0x382b(%rip),%rcx        # 646c9280 <.rdata+0xa0>
+    646c5a55:	call   646c7b60 <__report_error>
+    646c5a5a:	nop
+    646c5a5b:	nop
+    646c5a5c:	nop
+    646c5a5d:	nop
+    646c5a5e:	nop
+    646c5a5f:	nop
+
+00000000646c5a60 <__mingw_SEH_error_handler>:
+    646c5a60:	sub    $0x28,%rsp
+    646c5a64:	mov    (%rcx),%eax
+    646c5a66:	cmp    $0xc0000091,%eax
+    646c5a6b:	ja     646c5ad0 <__mingw_SEH_error_handler+0x70>
+    646c5a6d:	cmp    $0xc000008d,%eax
+    646c5a72:	jae    646c5aef <__mingw_SEH_error_handler+0x8f>
+    646c5a74:	cmp    $0xc0000008,%eax
+    646c5a79:	je     646c5b84 <__mingw_SEH_error_handler+0x124>
+    646c5a7f:	ja     646c5b50 <__mingw_SEH_error_handler+0xf0>
+    646c5a85:	cmp    $0x80000002,%eax
+    646c5a8a:	je     646c5b84 <__mingw_SEH_error_handler+0x124>
+    646c5a90:	cmp    $0xc0000005,%eax
+    646c5a95:	jne    646c5b5e <__mingw_SEH_error_handler+0xfe>
+    646c5a9b:	xor    %edx,%edx
+    646c5a9d:	mov    $0xb,%ecx
+    646c5aa2:	call   646c76f8 <signal>
+    646c5aa7:	cmp    $0x1,%rax
+    646c5aab:	je     646c5be0 <__mingw_SEH_error_handler+0x180>
+    646c5ab1:	test   %rax,%rax
+    646c5ab4:	je     646c5bf6 <__mingw_SEH_error_handler+0x196>
+    646c5aba:	mov    $0xb,%ecx
+    646c5abf:	call   *%rax
+    646c5ac1:	xor    %eax,%eax
+    646c5ac3:	add    $0x28,%rsp
+    646c5ac7:	ret
+    646c5ac8:	nopl   0x0(%rax,%rax,1)
+    646c5ad0:	cmp    $0xc0000094,%eax
+    646c5ad5:	je     646c5b90 <__mingw_SEH_error_handler+0x130>
+    646c5adb:	ja     646c5b14 <__mingw_SEH_error_handler+0xb4>
+    646c5add:	cmp    $0xc0000092,%eax
+    646c5ae2:	je     646c5b84 <__mingw_SEH_error_handler+0x124>
+    646c5ae8:	cmp    $0xc0000093,%eax
+    646c5aed:	jne    646c5b5e <__mingw_SEH_error_handler+0xfe>
+    646c5aef:	xor    %edx,%edx
+    646c5af1:	mov    $0x8,%ecx
+    646c5af6:	call   646c76f8 <signal>
+    646c5afb:	cmp    $0x1,%rax
+    646c5aff:	je     646c5b70 <__mingw_SEH_error_handler+0x110>
+    646c5b01:	test   %rax,%rax
+    646c5b04:	je     646c5b5e <__mingw_SEH_error_handler+0xfe>
+    646c5b06:	mov    $0x8,%ecx
+    646c5b0b:	call   *%rax
+    646c5b0d:	xor    %eax,%eax
+    646c5b0f:	add    $0x28,%rsp
+    646c5b13:	ret
+    646c5b14:	cmp    $0xc0000095,%eax
+    646c5b19:	je     646c5b84 <__mingw_SEH_error_handler+0x124>
+    646c5b1b:	cmp    $0xc0000096,%eax
+    646c5b20:	jne    646c5b5e <__mingw_SEH_error_handler+0xfe>
+    646c5b22:	xor    %edx,%edx
+    646c5b24:	mov    $0x4,%ecx
+    646c5b29:	call   646c76f8 <signal>
+    646c5b2e:	cmp    $0x1,%rax
+    646c5b32:	je     646c5bc0 <__mingw_SEH_error_handler+0x160>
+    646c5b38:	test   %rax,%rax
+    646c5b3b:	je     646c5bf6 <__mingw_SEH_error_handler+0x196>
+    646c5b41:	mov    $0x4,%ecx
+    646c5b46:	call   *%rax
+    646c5b48:	xor    %eax,%eax
+    646c5b4a:	add    $0x28,%rsp
+    646c5b4e:	ret
+    646c5b4f:	nop
+    646c5b50:	cmp    $0xc000001d,%eax
+    646c5b55:	je     646c5b22 <__mingw_SEH_error_handler+0xc2>
+    646c5b57:	cmp    $0xc000008c,%eax
+    646c5b5c:	je     646c5b84 <__mingw_SEH_error_handler+0x124>
+    646c5b5e:	mov    $0x1,%eax
+    646c5b63:	add    $0x28,%rsp
+    646c5b67:	ret
+    646c5b68:	nopl   0x0(%rax,%rax,1)
+    646c5b70:	mov    $0x1,%edx
+    646c5b75:	mov    $0x8,%ecx
+    646c5b7a:	call   646c76f8 <signal>
+    646c5b7f:	call   646c6530 <_fpreset>
+    646c5b84:	xor    %eax,%eax
+    646c5b86:	add    $0x28,%rsp
+    646c5b8a:	ret
+    646c5b8b:	nopl   0x0(%rax,%rax,1)
+    646c5b90:	xor    %edx,%edx
+    646c5b92:	mov    $0x8,%ecx
+    646c5b97:	call   646c76f8 <signal>
+    646c5b9c:	cmp    $0x1,%rax
+    646c5ba0:	jne    646c5b01 <__mingw_SEH_error_handler+0xa1>
+    646c5ba6:	mov    $0x1,%edx
+    646c5bab:	mov    $0x8,%ecx
+    646c5bb0:	call   646c76f8 <signal>
+    646c5bb5:	xor    %eax,%eax
+    646c5bb7:	jmp    646c5ac3 <__mingw_SEH_error_handler+0x63>
     646c5bbc:	nopl   0x0(%rax)
-    646c5bc0:	lea    0x6db9(%rip),%rbx        # 646cc980 <emu_pdata>
-    646c5bc7:	mov    $0x30,%ecx
-    646c5bcc:	xor    %esi,%esi
-    646c5bce:	lea    0x6cab(%rip),%rdx        # 646cc880 <emu_xdata>
-    646c5bd5:	mov    %rbx,%rdi
-    646c5bd8:	rep stos %rax,%es:(%rdi)
-    646c5bdb:	lea    -0x212(%rip),%r12        # 646c59d0 <__mingw_SEH_error_handler>
-    646c5be2:	mov    $0x20,%ecx
-    646c5be7:	mov    %rdx,%rdi
-    646c5bea:	rep stos %rax,%es:(%rdi)
-    646c5bed:	sub    %rbp,%r12
-    646c5bf0:	mov    %rdx,%rdi
-    646c5bf3:	jmp    646c5c23 <__mingw_init_ehandler+0xb3>
-    646c5bf5:	movb   $0x9,(%rdi)
-    646c5bf8:	add    $0x1,%rsi
-    646c5bfc:	add    $0xc,%rbx
-    646c5c00:	mov    %r12d,0x4(%rdi)
-    646c5c04:	mov    0xc(%rax),%ecx
-    646c5c07:	mov    %ecx,-0xc(%rbx)
-    646c5c0a:	add    0x8(%rax),%ecx
-    646c5c0d:	mov    %rdi,%rax
-    646c5c10:	add    $0x8,%rdi
-    646c5c14:	sub    %rbp,%rax
-    646c5c17:	mov    %eax,-0x4(%rbx)
-    646c5c1a:	mov    %ecx,-0x8(%rbx)
-    646c5c1d:	cmp    $0x20,%rsi
-    646c5c21:	je     646c5c55 <__mingw_init_ehandler+0xe5>
-    646c5c23:	mov    %rsi,%rcx
-    646c5c26:	call   646c62a0 <_FindPESectionExec>
-    646c5c2b:	test   %rax,%rax
-    646c5c2e:	jne    646c5bf5 <__mingw_init_ehandler+0x85>
-    646c5c30:	test   %rsi,%rsi
-    646c5c33:	mov    %esi,%edx
-    646c5c35:	je     646c5bac <__mingw_init_ehandler+0x3c>
-    646c5c3b:	nopl   0x0(%rax,%rax,1)
-    646c5c40:	lea    0x6d39(%rip),%rcx        # 646cc980 <emu_pdata>
-    646c5c47:	mov    %rbp,%r8
-    646c5c4a:	call   *0x85d4(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c5c50:	jmp    646c5bac <__mingw_init_ehandler+0x3c>
-    646c5c55:	mov    $0x20,%edx
-    646c5c5a:	jmp    646c5c40 <__mingw_init_ehandler+0xd0>
-    646c5c5c:	nopl   0x0(%rax)
-
-00000000646c5c60 <_gnu_exception_handler>:
-    646c5c60:	push   %rbx
-    646c5c61:	sub    $0x20,%rsp
-    646c5c65:	mov    (%rcx),%rdx
-    646c5c68:	mov    (%rdx),%eax
-    646c5c6a:	mov    %rcx,%rbx
-    646c5c6d:	mov    %eax,%ecx
-    646c5c6f:	and    $0x20ffffff,%ecx
-    646c5c75:	cmp    $0x20474343,%ecx
-    646c5c7b:	je     646c5d40 <_gnu_exception_handler+0xe0>
-    646c5c81:	cmp    $0xc0000091,%eax
-    646c5c86:	ja     646c5cf0 <_gnu_exception_handler+0x90>
-    646c5c88:	cmp    $0xc000008d,%eax
-    646c5c8d:	jae    646c5d0b <_gnu_exception_handler+0xab>
-    646c5c8f:	cmp    $0xc0000008,%eax
-    646c5c94:	je     646c5d4a <_gnu_exception_handler+0xea>
-    646c5c9a:	ja     646c5d94 <_gnu_exception_handler+0x134>
-    646c5ca0:	cmp    $0x80000002,%eax
-    646c5ca5:	je     646c5d4a <_gnu_exception_handler+0xea>
-    646c5cab:	cmp    $0xc0000005,%eax
-    646c5cb0:	jne    646c5cd1 <_gnu_exception_handler+0x71>
-    646c5cb2:	xor    %edx,%edx
-    646c5cb4:	mov    $0xb,%ecx
-    646c5cb9:	call   646c7668 <signal>
-    646c5cbe:	cmp    $0x1,%rax
-    646c5cc2:	je     646c5e19 <_gnu_exception_handler+0x1b9>
-    646c5cc8:	test   %rax,%rax
-    646c5ccb:	jne    646c5de0 <_gnu_exception_handler+0x180>
-    646c5cd1:	mov    0x6b88(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
-    646c5cd8:	test   %rax,%rax
-    646c5cdb:	je     646c5df1 <_gnu_exception_handler+0x191>
-    646c5ce1:	mov    %rbx,%rcx
-    646c5ce4:	add    $0x20,%rsp
-    646c5ce8:	pop    %rbx
-    646c5ce9:	rex.W jmp *%rax
+    646c5bc0:	mov    $0x1,%edx
+    646c5bc5:	mov    $0x4,%ecx
+    646c5bca:	call   646c76f8 <signal>
+    646c5bcf:	xor    %eax,%eax
+    646c5bd1:	jmp    646c5ac3 <__mingw_SEH_error_handler+0x63>
+    646c5bd6:	cs nopw 0x0(%rax,%rax,1)
+    646c5be0:	mov    $0x1,%edx
+    646c5be5:	mov    $0xb,%ecx
+    646c5bea:	call   646c76f8 <signal>
+    646c5bef:	xor    %eax,%eax
+    646c5bf1:	jmp    646c5ac3 <__mingw_SEH_error_handler+0x63>
+    646c5bf6:	mov    $0x4,%eax
+    646c5bfb:	jmp    646c5ac3 <__mingw_SEH_error_handler+0x63>
+
+00000000646c5c00 <__mingw_init_ehandler>:
+    646c5c00:	push   %r12
+    646c5c02:	push   %rbp
+    646c5c03:	push   %rdi
+    646c5c04:	push   %rsi
+    646c5c05:	push   %rbx
+    646c5c06:	sub    $0x20,%rsp
+    646c5c0a:	call   646c63a0 <_GetPEImageBase>
+    646c5c0f:	mov    %rax,%rbp
+    646c5c12:	mov    0x6c50(%rip),%eax        # 646cc868 <was_here.95013>
+    646c5c18:	test   %eax,%eax
+    646c5c1a:	jne    646c5c41 <__mingw_init_ehandler+0x41>
+    646c5c1c:	test   %rbp,%rbp
+    646c5c1f:	je     646c5c41 <__mingw_init_ehandler+0x41>
+    646c5c21:	lea    0x36c8(%rip),%rcx        # 646c92f0 <.rdata>
+    646c5c28:	movl   $0x1,0x6c36(%rip)        # 646cc868 <was_here.95013>
+    646c5c32:	call   646c61e0 <_FindPESectionByName>
+    646c5c37:	test   %rax,%rax
+    646c5c3a:	je     646c5c50 <__mingw_init_ehandler+0x50>
+    646c5c3c:	mov    $0x1,%eax
+    646c5c41:	add    $0x20,%rsp
+    646c5c45:	pop    %rbx
+    646c5c46:	pop    %rsi
+    646c5c47:	pop    %rdi
+    646c5c48:	pop    %rbp
+    646c5c49:	pop    %r12
+    646c5c4b:	ret
+    646c5c4c:	nopl   0x0(%rax)
+    646c5c50:	lea    0x6d29(%rip),%rbx        # 646cc980 <emu_pdata>
+    646c5c57:	mov    $0x30,%ecx
+    646c5c5c:	xor    %esi,%esi
+    646c5c5e:	lea    0x6c1b(%rip),%rdx        # 646cc880 <emu_xdata>
+    646c5c65:	mov    %rbx,%rdi
+    646c5c68:	rep stos %rax,%es:(%rdi)
+    646c5c6b:	lea    -0x212(%rip),%r12        # 646c5a60 <__mingw_SEH_error_handler>
+    646c5c72:	mov    $0x20,%ecx
+    646c5c77:	mov    %rdx,%rdi
+    646c5c7a:	rep stos %rax,%es:(%rdi)
+    646c5c7d:	sub    %rbp,%r12
+    646c5c80:	mov    %rdx,%rdi
+    646c5c83:	jmp    646c5cb3 <__mingw_init_ehandler+0xb3>
+    646c5c85:	movb   $0x9,(%rdi)
+    646c5c88:	add    $0x1,%rsi
+    646c5c8c:	add    $0xc,%rbx
+    646c5c90:	mov    %r12d,0x4(%rdi)
+    646c5c94:	mov    0xc(%rax),%ecx
+    646c5c97:	mov    %ecx,-0xc(%rbx)
+    646c5c9a:	add    0x8(%rax),%ecx
+    646c5c9d:	mov    %rdi,%rax
+    646c5ca0:	add    $0x8,%rdi
+    646c5ca4:	sub    %rbp,%rax
+    646c5ca7:	mov    %eax,-0x4(%rbx)
+    646c5caa:	mov    %ecx,-0x8(%rbx)
+    646c5cad:	cmp    $0x20,%rsi
+    646c5cb1:	je     646c5ce5 <__mingw_init_ehandler+0xe5>
+    646c5cb3:	mov    %rsi,%rcx
+    646c5cb6:	call   646c6330 <_FindPESectionExec>
+    646c5cbb:	test   %rax,%rax
+    646c5cbe:	jne    646c5c85 <__mingw_init_ehandler+0x85>
+    646c5cc0:	test   %rsi,%rsi
+    646c5cc3:	mov    %esi,%edx
+    646c5cc5:	je     646c5c3c <__mingw_init_ehandler+0x3c>
+    646c5ccb:	nopl   0x0(%rax,%rax,1)
+    646c5cd0:	lea    0x6ca9(%rip),%rcx        # 646cc980 <emu_pdata>
+    646c5cd7:	mov    %rbp,%r8
+    646c5cda:	call   *0x8544(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c5ce0:	jmp    646c5c3c <__mingw_init_ehandler+0x3c>
+    646c5ce5:	mov    $0x20,%edx
+    646c5cea:	jmp    646c5cd0 <__mingw_init_ehandler+0xd0>
     646c5cec:	nopl   0x0(%rax)
-    646c5cf0:	cmp    $0xc0000094,%eax
-    646c5cf5:	je     646c5db0 <_gnu_exception_handler+0x150>
-    646c5cfb:	ja     646c5d55 <_gnu_exception_handler+0xf5>
-    646c5cfd:	cmp    $0xc0000092,%eax
-    646c5d02:	je     646c5d4a <_gnu_exception_handler+0xea>
-    646c5d04:	cmp    $0xc0000093,%eax
-    646c5d09:	jne    646c5cd1 <_gnu_exception_handler+0x71>
-    646c5d0b:	xor    %edx,%edx
-    646c5d0d:	mov    $0x8,%ecx
-    646c5d12:	call   646c7668 <signal>
-    646c5d17:	cmp    $0x1,%rax
-    646c5d1b:	je     646c5e00 <_gnu_exception_handler+0x1a0>
-    646c5d21:	test   %rax,%rax
-    646c5d24:	je     646c5cd1 <_gnu_exception_handler+0x71>
-    646c5d26:	mov    $0x8,%ecx
-    646c5d2b:	call   *%rax
-    646c5d2d:	mov    $0xffffffff,%eax
-    646c5d32:	add    $0x20,%rsp
-    646c5d36:	pop    %rbx
-    646c5d37:	ret
-    646c5d38:	nopl   0x0(%rax,%rax,1)
-    646c5d40:	testb  $0x1,0x4(%rdx)
-    646c5d44:	jne    646c5c81 <_gnu_exception_handler+0x21>
-    646c5d4a:	mov    $0xffffffff,%eax
-    646c5d4f:	add    $0x20,%rsp
-    646c5d53:	pop    %rbx
-    646c5d54:	ret
-    646c5d55:	cmp    $0xc0000095,%eax
-    646c5d5a:	je     646c5d4a <_gnu_exception_handler+0xea>
-    646c5d5c:	cmp    $0xc0000096,%eax
-    646c5d61:	jne    646c5cd1 <_gnu_exception_handler+0x71>
-    646c5d67:	xor    %edx,%edx
-    646c5d69:	mov    $0x4,%ecx
-    646c5d6e:	call   646c7668 <signal>
-    646c5d73:	cmp    $0x1,%rax
-    646c5d77:	je     646c5e30 <_gnu_exception_handler+0x1d0>
-    646c5d7d:	test   %rax,%rax
-    646c5d80:	je     646c5cd1 <_gnu_exception_handler+0x71>
-    646c5d86:	mov    $0x4,%ecx
-    646c5d8b:	call   *%rax
-    646c5d8d:	mov    $0xffffffff,%eax
-    646c5d92:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5d94:	cmp    $0xc000001d,%eax
-    646c5d99:	je     646c5d67 <_gnu_exception_handler+0x107>
-    646c5d9b:	cmp    $0xc000008c,%eax
-    646c5da0:	jne    646c5cd1 <_gnu_exception_handler+0x71>
-    646c5da6:	jmp    646c5d4a <_gnu_exception_handler+0xea>
-    646c5da8:	nopl   0x0(%rax,%rax,1)
-    646c5db0:	xor    %edx,%edx
-    646c5db2:	mov    $0x8,%ecx
-    646c5db7:	call   646c7668 <signal>
-    646c5dbc:	cmp    $0x1,%rax
-    646c5dc0:	jne    646c5d21 <_gnu_exception_handler+0xc1>
-    646c5dc6:	mov    $0x1,%edx
-    646c5dcb:	mov    $0x8,%ecx
-    646c5dd0:	call   646c7668 <signal>
-    646c5dd5:	mov    $0xffffffff,%eax
-    646c5dda:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5ddf:	nop
-    646c5de0:	mov    $0xb,%ecx
-    646c5de5:	call   *%rax
-    646c5de7:	mov    $0xffffffff,%eax
-    646c5dec:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5df1:	xor    %eax,%eax
-    646c5df3:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5df8:	nopl   0x0(%rax,%rax,1)
-    646c5e00:	mov    $0x1,%edx
-    646c5e05:	mov    $0x8,%ecx
-    646c5e0a:	call   646c7668 <signal>
-    646c5e0f:	call   646c64a0 <_fpreset>
-    646c5e14:	jmp    646c5d4a <_gnu_exception_handler+0xea>
-    646c5e19:	mov    $0x1,%edx
-    646c5e1e:	mov    $0xb,%ecx
-    646c5e23:	call   646c7668 <signal>
-    646c5e28:	or     $0xffffffff,%eax
-    646c5e2b:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5e30:	mov    $0x1,%edx
-    646c5e35:	mov    $0x4,%ecx
-    646c5e3a:	call   646c7668 <signal>
-    646c5e3f:	or     $0xffffffff,%eax
-    646c5e42:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
-    646c5e47:	nop
-    646c5e48:	nop
-    646c5e49:	nop
-    646c5e4a:	nop
-    646c5e4b:	nop
-    646c5e4c:	nop
-    646c5e4d:	nop
-    646c5e4e:	nop
-    646c5e4f:	nop
-
-00000000646c5e50 <__mingwthr_run_key_dtors.part.0>:
-    646c5e50:	push   %rbp
-    646c5e51:	push   %rdi
-    646c5e52:	push   %rsi
-    646c5e53:	push   %rbx
-    646c5e54:	sub    $0x28,%rsp
-    646c5e58:	lea    0x6cc1(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5e5f:	call   *0x836f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c5e65:	mov    0x6c94(%rip),%rbx        # 646ccb00 <key_dtor_list>
-    646c5e6c:	test   %rbx,%rbx
-    646c5e6f:	je     646c5ea4 <__mingwthr_run_key_dtors.part.0+0x54>
-    646c5e71:	mov    0x83e4(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
-    646c5e78:	mov    0x8375(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
-    646c5e7f:	nop
-    646c5e80:	mov    (%rbx),%ecx
-    646c5e82:	call   *%rbp
-    646c5e84:	mov    %rax,%rsi
-    646c5e87:	call   *%rdi
-    646c5e89:	test   %eax,%eax
-    646c5e8b:	jne    646c5e9b <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c5e8d:	test   %rsi,%rsi
-    646c5e90:	je     646c5e9b <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c5e92:	mov    0x8(%rbx),%rax
-    646c5e96:	mov    %rsi,%rcx
-    646c5e99:	call   *%rax
-    646c5e9b:	mov    0x10(%rbx),%rbx
-    646c5e9f:	test   %rbx,%rbx
-    646c5ea2:	jne    646c5e80 <__mingwthr_run_key_dtors.part.0+0x30>
-    646c5ea4:	lea    0x6c75(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5eab:	add    $0x28,%rsp
-    646c5eaf:	pop    %rbx
-    646c5eb0:	pop    %rsi
-    646c5eb1:	pop    %rdi
-    646c5eb2:	pop    %rbp
-    646c5eb3:	rex.W jmp *0x835a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c5eba:	nopw   0x0(%rax,%rax,1)
-
-00000000646c5ec0 <___w64_mingwthr_add_key_dtor>:
-    646c5ec0:	push   %rbp
-    646c5ec1:	push   %rdi
-    646c5ec2:	push   %rsi
-    646c5ec3:	push   %rbx
-    646c5ec4:	sub    $0x28,%rsp
-    646c5ec8:	mov    0x6c3a(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c5ece:	xor    %esi,%esi
-    646c5ed0:	test   %eax,%eax
-    646c5ed2:	mov    %ecx,%ebp
-    646c5ed4:	mov    %rdx,%rdi
-    646c5ed7:	jne    646c5ee4 <___w64_mingwthr_add_key_dtor+0x24>
-    646c5ed9:	mov    %esi,%eax
-    646c5edb:	add    $0x28,%rsp
-    646c5edf:	pop    %rbx
-    646c5ee0:	pop    %rsi
-    646c5ee1:	pop    %rdi
-    646c5ee2:	pop    %rbp
-    646c5ee3:	ret
-    646c5ee4:	mov    $0x18,%edx
-    646c5ee9:	mov    $0x1,%ecx
-    646c5eee:	call   646c76c0 <calloc>
-    646c5ef3:	test   %rax,%rax
-    646c5ef6:	mov    %rax,%rbx
-    646c5ef9:	je     646c5f38 <___w64_mingwthr_add_key_dtor+0x78>
-    646c5efb:	mov    %ebp,(%rax)
-    646c5efd:	lea    0x6c1c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5f04:	mov    %rdi,0x8(%rax)
-    646c5f08:	call   *0x82c6(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c5f0e:	mov    0x6beb(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c5f15:	lea    0x6c04(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5f1c:	mov    %rbx,0x6bdd(%rip)        # 646ccb00 <key_dtor_list>
-    646c5f23:	mov    %rax,0x10(%rbx)
-    646c5f27:	call   *0x82e7(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c5f2d:	mov    %esi,%eax
-    646c5f2f:	add    $0x28,%rsp
-    646c5f33:	pop    %rbx
-    646c5f34:	pop    %rsi
-    646c5f35:	pop    %rdi
-    646c5f36:	pop    %rbp
-    646c5f37:	ret
-    646c5f38:	mov    $0xffffffff,%esi
-    646c5f3d:	jmp    646c5ed9 <___w64_mingwthr_add_key_dtor+0x19>
-    646c5f3f:	nop
-
-00000000646c5f40 <___w64_mingwthr_remove_key_dtor>:
-    646c5f40:	push   %rbx
-    646c5f41:	sub    $0x20,%rsp
-    646c5f45:	mov    0x6bbd(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c5f4b:	test   %eax,%eax
-    646c5f4d:	mov    %ecx,%ebx
-    646c5f4f:	jne    646c5f60 <___w64_mingwthr_remove_key_dtor+0x20>
-    646c5f51:	xor    %eax,%eax
-    646c5f53:	add    $0x20,%rsp
-    646c5f57:	pop    %rbx
-    646c5f58:	ret
-    646c5f59:	nopl   0x0(%rax)
-    646c5f60:	lea    0x6bb9(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5f67:	call   *0x8267(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c5f6d:	mov    0x6b8c(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c5f74:	test   %rax,%rax
-    646c5f77:	je     646c5f93 <___w64_mingwthr_remove_key_dtor+0x53>
-    646c5f79:	mov    (%rax),%edx
-    646c5f7b:	cmp    %edx,%ebx
-    646c5f7d:	jne    646c5f8a <___w64_mingwthr_remove_key_dtor+0x4a>
-    646c5f7f:	jmp    646c5fd0 <___w64_mingwthr_remove_key_dtor+0x90>
-    646c5f81:	mov    (%rcx),%edx
-    646c5f83:	cmp    %ebx,%edx
-    646c5f85:	je     646c5fb0 <___w64_mingwthr_remove_key_dtor+0x70>
-    646c5f87:	mov    %rcx,%rax
-    646c5f8a:	mov    0x10(%rax),%rcx
-    646c5f8e:	test   %rcx,%rcx
-    646c5f91:	jne    646c5f81 <___w64_mingwthr_remove_key_dtor+0x41>
-    646c5f93:	lea    0x6b86(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5f9a:	call   *0x8274(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c5fa0:	xor    %eax,%eax
-    646c5fa2:	add    $0x20,%rsp
-    646c5fa6:	pop    %rbx
-    646c5fa7:	ret
-    646c5fa8:	nopl   0x0(%rax,%rax,1)
-    646c5fb0:	mov    0x10(%rcx),%rdx
-    646c5fb4:	mov    %rdx,0x10(%rax)
-    646c5fb8:	call   646c7698 <free>
-    646c5fbd:	lea    0x6b5c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c5fc4:	call   *0x824a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c5fca:	jmp    646c5fa0 <___w64_mingwthr_remove_key_dtor+0x60>
-    646c5fcc:	nopl   0x0(%rax)
-    646c5fd0:	mov    0x10(%rax),%rdx
-    646c5fd4:	mov    %rax,%rcx
-    646c5fd7:	mov    %rdx,0x6b22(%rip)        # 646ccb00 <key_dtor_list>
-    646c5fde:	jmp    646c5fb8 <___w64_mingwthr_remove_key_dtor+0x78>
-
-00000000646c5fe0 <__mingw_TLScallback>:
-    646c5fe0:	push   %rbx
-    646c5fe1:	sub    $0x20,%rsp
-    646c5fe5:	cmp    $0x1,%edx
-    646c5fe8:	je     646c6080 <__mingw_TLScallback+0xa0>
-    646c5fee:	jb     646c6020 <__mingw_TLScallback+0x40>
-    646c5ff0:	cmp    $0x2,%edx
-    646c5ff3:	je     646c6010 <__mingw_TLScallback+0x30>
-    646c5ff5:	cmp    $0x3,%edx
-    646c5ff8:	jne    646c6015 <__mingw_TLScallback+0x35>
-    646c5ffa:	mov    0x6b08(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6000:	test   %eax,%eax
-    646c6002:	je     646c6015 <__mingw_TLScallback+0x35>
-    646c6004:	call   646c5e50 <__mingwthr_run_key_dtors.part.0>
-    646c6009:	jmp    646c6015 <__mingw_TLScallback+0x35>
-    646c600b:	nopl   0x0(%rax,%rax,1)
-    646c6010:	call   646c64a0 <_fpreset>
-    646c6015:	mov    $0x1,%eax
-    646c601a:	add    $0x20,%rsp
-    646c601e:	pop    %rbx
-    646c601f:	ret
-    646c6020:	mov    0x6ae2(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6026:	test   %eax,%eax
-    646c6028:	jne    646c60b0 <__mingw_TLScallback+0xd0>
-    646c602e:	mov    0x6ad4(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6034:	cmp    $0x1,%eax
-    646c6037:	jne    646c6015 <__mingw_TLScallback+0x35>
-    646c6039:	mov    0x6ac0(%rip),%rcx        # 646ccb00 <key_dtor_list>
-    646c6040:	test   %rcx,%rcx
-    646c6043:	je     646c6056 <__mingw_TLScallback+0x76>
-    646c6045:	mov    0x10(%rcx),%rbx
-    646c6049:	call   646c7698 <free>
-    646c604e:	test   %rbx,%rbx
-    646c6051:	mov    %rbx,%rcx
-    646c6054:	jne    646c6045 <__mingw_TLScallback+0x65>
-    646c6056:	lea    0x6ac3(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c605d:	movq   $0x0,0x6a98(%rip)        # 646ccb00 <key_dtor_list>
-    646c6068:	movl   $0x0,0x6a96(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c6072:	call   *0x8154(%rip)        # 646ce1cc <__IAT_start__>
-    646c6078:	jmp    646c6015 <__mingw_TLScallback+0x35>
-    646c607a:	nopw   0x0(%rax,%rax,1)
-    646c6080:	mov    0x6a82(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6086:	test   %eax,%eax
-    646c6088:	je     646c60a0 <__mingw_TLScallback+0xc0>
-    646c608a:	movl   $0x1,0x6a74(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c6094:	mov    $0x1,%eax
-    646c6099:	add    $0x20,%rsp
-    646c609d:	pop    %rbx
-    646c609e:	ret
-    646c609f:	nop
-    646c60a0:	lea    0x6a79(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c60a7:	call   *0x815f(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c60ad:	jmp    646c608a <__mingw_TLScallback+0xaa>
-    646c60af:	nop
-    646c60b0:	call   646c5e50 <__mingwthr_run_key_dtors.part.0>
-    646c60b5:	jmp    646c602e <__mingw_TLScallback+0x4e>
-    646c60ba:	nop
-    646c60bb:	nop
-    646c60bc:	nop
-    646c60bd:	nop
-    646c60be:	nop
-    646c60bf:	nop
-
-00000000646c60c0 <_ValidateImageBase.part.0>:
-    646c60c0:	movslq 0x3c(%rcx),%rax
-    646c60c4:	add    %rax,%rcx
-    646c60c7:	xor    %eax,%eax
-    646c60c9:	cmpl   $0x4550,(%rcx)
-    646c60cf:	je     646c60d2 <_ValidateImageBase.part.0+0x12>
-    646c60d1:	ret
-    646c60d2:	xor    %eax,%eax
-    646c60d4:	cmpw   $0x20b,0x18(%rcx)
-    646c60da:	sete   %al
-    646c60dd:	ret
-    646c60de:	xchg   %ax,%ax
-
-00000000646c60e0 <_ValidateImageBase>:
-    646c60e0:	cmpw   $0x5a4d,(%rcx)
-    646c60e5:	je     646c60f0 <_ValidateImageBase+0x10>
-    646c60e7:	xor    %eax,%eax
-    646c60e9:	ret
-    646c60ea:	nopw   0x0(%rax,%rax,1)
-    646c60f0:	jmp    646c60c0 <_ValidateImageBase.part.0>
-    646c60f2:	nopl   0x0(%rax)
-    646c60f6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6100 <_FindPESection>:
-    646c6100:	movslq 0x3c(%rcx),%rax
-    646c6104:	add    %rax,%rcx
-    646c6107:	movzwl 0x14(%rcx),%eax
-    646c610b:	lea    0x18(%rcx,%rax,1),%rax
-    646c6110:	movzwl 0x6(%rcx),%ecx
-    646c6114:	test   %ecx,%ecx
-    646c6116:	je     646c6141 <_FindPESection+0x41>
-    646c6118:	sub    $0x1,%ecx
-    646c611b:	lea    (%rcx,%rcx,4),%rcx
-    646c611f:	lea    0x28(%rax,%rcx,8),%r9
-    646c6124:	mov    0xc(%rax),%r8d
-    646c6128:	cmp    %rdx,%r8
-    646c612b:	mov    %r8,%rcx
-    646c612e:	ja     646c6138 <_FindPESection+0x38>
-    646c6130:	add    0x8(%rax),%ecx
-    646c6133:	cmp    %rdx,%rcx
-    646c6136:	ja     646c6143 <_FindPESection+0x43>
-    646c6138:	add    $0x28,%rax
-    646c613c:	cmp    %r9,%rax
-    646c613f:	jne    646c6124 <_FindPESection+0x24>
-    646c6141:	xor    %eax,%eax
-    646c6143:	ret
-    646c6144:	xchg   %ax,%ax
-    646c6146:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6150 <_FindPESectionByName>:
-    646c6150:	push   %rdi
-    646c6151:	push   %rsi
-    646c6152:	push   %rbx
-    646c6153:	sub    $0x20,%rsp
-    646c6157:	mov    %rcx,%rsi
-    646c615a:	call   646c7660 <strlen>
-    646c615f:	cmp    $0x8,%rax
-    646c6163:	ja     646c61d0 <_FindPESectionByName+0x80>
-    646c6165:	mov    0x34a4(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
-    646c616c:	cmpw   $0x5a4d,(%rdx)
-    646c6171:	jne    646c61d0 <_FindPESectionByName+0x80>
-    646c6173:	mov    %rdx,%rcx
-    646c6176:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c617b:	test   %eax,%eax
-    646c617d:	je     646c61d0 <_FindPESectionByName+0x80>
-    646c617f:	movslq 0x3c(%rdx),%rcx
-    646c6183:	add    %rdx,%rcx
-    646c6186:	movzwl 0x14(%rcx),%eax
-    646c618a:	lea    0x18(%rcx,%rax,1),%rbx
-    646c618f:	movzwl 0x6(%rcx),%eax
-    646c6193:	test   %eax,%eax
-    646c6195:	je     646c61d0 <_FindPESectionByName+0x80>
-    646c6197:	sub    $0x1,%eax
-    646c619a:	lea    (%rax,%rax,4),%rax
-    646c619e:	lea    0x28(%rbx,%rax,8),%rdi
-    646c61a3:	jmp    646c61ae <_FindPESectionByName+0x5e>
-    646c61a5:	add    $0x28,%rbx
-    646c61a9:	cmp    %rdi,%rbx
-    646c61ac:	je     646c61d0 <_FindPESectionByName+0x80>
-    646c61ae:	mov    $0x8,%r8d
-    646c61b4:	mov    %rsi,%rdx
-    646c61b7:	mov    %rbx,%rcx
-    646c61ba:	call   646c7658 <strncmp>
-    646c61bf:	test   %eax,%eax
-    646c61c1:	jne    646c61a5 <_FindPESectionByName+0x55>
-    646c61c3:	mov    %rbx,%rax
-    646c61c6:	add    $0x20,%rsp
-    646c61ca:	pop    %rbx
-    646c61cb:	pop    %rsi
-    646c61cc:	pop    %rdi
-    646c61cd:	ret
-    646c61ce:	xchg   %ax,%ax
-    646c61d0:	xor    %ebx,%ebx
-    646c61d2:	mov    %rbx,%rax
-    646c61d5:	add    $0x20,%rsp
-    646c61d9:	pop    %rbx
-    646c61da:	pop    %rsi
-    646c61db:	pop    %rdi
-    646c61dc:	ret
-    646c61dd:	nopl   (%rax)
-
-00000000646c61e0 <__mingw_GetSectionForAddress>:
-    646c61e0:	sub    $0x28,%rsp
-    646c61e4:	mov    0x3425(%rip),%r8        # 646c9610 <.refptr.__image_base__>
-    646c61eb:	cmpw   $0x5a4d,(%r8)
-    646c61f1:	mov    %rcx,%rdx
-    646c61f4:	jne    646c624d <__mingw_GetSectionForAddress+0x6d>
-    646c61f6:	mov    %r8,%rcx
-    646c61f9:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c61fe:	test   %eax,%eax
-    646c6200:	je     646c624d <__mingw_GetSectionForAddress+0x6d>
-    646c6202:	movslq 0x3c(%r8),%rax
-    646c6206:	mov    %rdx,%rcx
-    646c6209:	sub    %r8,%rcx
-    646c620c:	add    %rax,%r8
-    646c620f:	movzwl 0x6(%r8),%edx
-    646c6214:	movzwl 0x14(%r8),%eax
-    646c6219:	test   %edx,%edx
-    646c621b:	lea    0x18(%r8,%rax,1),%rax
-    646c6220:	je     646c624d <__mingw_GetSectionForAddress+0x6d>
-    646c6222:	sub    $0x1,%edx
-    646c6225:	lea    (%rdx,%rdx,4),%rdx
-    646c6229:	lea    0x28(%rax,%rdx,8),%r9
-    646c622e:	xchg   %ax,%ax
-    646c6230:	mov    0xc(%rax),%r8d
-    646c6234:	cmp    %r8,%rcx
-    646c6237:	mov    %r8,%rdx
-    646c623a:	jb     646c6244 <__mingw_GetSectionForAddress+0x64>
-    646c623c:	add    0x8(%rax),%edx
-    646c623f:	cmp    %rdx,%rcx
-    646c6242:	jb     646c624f <__mingw_GetSectionForAddress+0x6f>
-    646c6244:	add    $0x28,%rax
-    646c6248:	cmp    %r9,%rax
-    646c624b:	jne    646c6230 <__mingw_GetSectionForAddress+0x50>
-    646c624d:	xor    %eax,%eax
-    646c624f:	add    $0x28,%rsp
-    646c6253:	ret
-    646c6254:	xchg   %ax,%ax
-    646c6256:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6260 <__mingw_GetSectionCount>:
-    646c6260:	sub    $0x28,%rsp
-    646c6264:	mov    0x33a5(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
-    646c626b:	xor    %r8d,%r8d
-    646c626e:	cmpw   $0x5a4d,(%rdx)
-    646c6273:	je     646c6280 <__mingw_GetSectionCount+0x20>
-    646c6275:	mov    %r8d,%eax
-    646c6278:	add    $0x28,%rsp
-    646c627c:	ret
-    646c627d:	nopl   (%rax)
-    646c6280:	mov    %rdx,%rcx
-    646c6283:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c6288:	test   %eax,%eax
-    646c628a:	je     646c6275 <__mingw_GetSectionCount+0x15>
-    646c628c:	movslq 0x3c(%rdx),%rax
-    646c6290:	movzwl 0x6(%rax,%rdx,1),%r8d
-    646c6296:	mov    %r8d,%eax
-    646c6299:	add    $0x28,%rsp
-    646c629d:	ret
-    646c629e:	xchg   %ax,%ax
-
-00000000646c62a0 <_FindPESectionExec>:
-    646c62a0:	sub    $0x28,%rsp
-    646c62a4:	mov    0x3365(%rip),%r8        # 646c9610 <.refptr.__image_base__>
-    646c62ab:	cmpw   $0x5a4d,(%r8)
-    646c62b1:	mov    %rcx,%rdx
-    646c62b4:	jne    646c6308 <_FindPESectionExec+0x68>
-    646c62b6:	mov    %r8,%rcx
-    646c62b9:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c62be:	test   %eax,%eax
-    646c62c0:	je     646c6308 <_FindPESectionExec+0x68>
-    646c62c2:	movslq 0x3c(%r8),%rcx
-    646c62c6:	add    %r8,%rcx
-    646c62c9:	movzwl 0x14(%rcx),%eax
-    646c62cd:	lea    0x18(%rcx,%rax,1),%rax
-    646c62d2:	movzwl 0x6(%rcx),%ecx
-    646c62d6:	test   %ecx,%ecx
-    646c62d8:	je     646c6308 <_FindPESectionExec+0x68>
-    646c62da:	sub    $0x1,%ecx
-    646c62dd:	lea    (%rcx,%rcx,4),%rcx
-    646c62e1:	lea    0x28(%rax,%rcx,8),%rcx
+
+00000000646c5cf0 <_gnu_exception_handler>:
+    646c5cf0:	push   %rbx
+    646c5cf1:	sub    $0x20,%rsp
+    646c5cf5:	mov    (%rcx),%rdx
+    646c5cf8:	mov    (%rdx),%eax
+    646c5cfa:	mov    %rcx,%rbx
+    646c5cfd:	mov    %eax,%ecx
+    646c5cff:	and    $0x20ffffff,%ecx
+    646c5d05:	cmp    $0x20474343,%ecx
+    646c5d0b:	je     646c5dd0 <_gnu_exception_handler+0xe0>
+    646c5d11:	cmp    $0xc0000091,%eax
+    646c5d16:	ja     646c5d80 <_gnu_exception_handler+0x90>
+    646c5d18:	cmp    $0xc000008d,%eax
+    646c5d1d:	jae    646c5d9b <_gnu_exception_handler+0xab>
+    646c5d1f:	cmp    $0xc0000008,%eax
+    646c5d24:	je     646c5dda <_gnu_exception_handler+0xea>
+    646c5d2a:	ja     646c5e24 <_gnu_exception_handler+0x134>
+    646c5d30:	cmp    $0x80000002,%eax
+    646c5d35:	je     646c5dda <_gnu_exception_handler+0xea>
+    646c5d3b:	cmp    $0xc0000005,%eax
+    646c5d40:	jne    646c5d61 <_gnu_exception_handler+0x71>
+    646c5d42:	xor    %edx,%edx
+    646c5d44:	mov    $0xb,%ecx
+    646c5d49:	call   646c76f8 <signal>
+    646c5d4e:	cmp    $0x1,%rax
+    646c5d52:	je     646c5ea9 <_gnu_exception_handler+0x1b9>
+    646c5d58:	test   %rax,%rax
+    646c5d5b:	jne    646c5e70 <_gnu_exception_handler+0x180>
+    646c5d61:	mov    0x6af8(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
+    646c5d68:	test   %rax,%rax
+    646c5d6b:	je     646c5e81 <_gnu_exception_handler+0x191>
+    646c5d71:	mov    %rbx,%rcx
+    646c5d74:	add    $0x20,%rsp
+    646c5d78:	pop    %rbx
+    646c5d79:	rex.W jmp *%rax
+    646c5d7c:	nopl   0x0(%rax)
+    646c5d80:	cmp    $0xc0000094,%eax
+    646c5d85:	je     646c5e40 <_gnu_exception_handler+0x150>
+    646c5d8b:	ja     646c5de5 <_gnu_exception_handler+0xf5>
+    646c5d8d:	cmp    $0xc0000092,%eax
+    646c5d92:	je     646c5dda <_gnu_exception_handler+0xea>
+    646c5d94:	cmp    $0xc0000093,%eax
+    646c5d99:	jne    646c5d61 <_gnu_exception_handler+0x71>
+    646c5d9b:	xor    %edx,%edx
+    646c5d9d:	mov    $0x8,%ecx
+    646c5da2:	call   646c76f8 <signal>
+    646c5da7:	cmp    $0x1,%rax
+    646c5dab:	je     646c5e90 <_gnu_exception_handler+0x1a0>
+    646c5db1:	test   %rax,%rax
+    646c5db4:	je     646c5d61 <_gnu_exception_handler+0x71>
+    646c5db6:	mov    $0x8,%ecx
+    646c5dbb:	call   *%rax
+    646c5dbd:	mov    $0xffffffff,%eax
+    646c5dc2:	add    $0x20,%rsp
+    646c5dc6:	pop    %rbx
+    646c5dc7:	ret
+    646c5dc8:	nopl   0x0(%rax,%rax,1)
+    646c5dd0:	testb  $0x1,0x4(%rdx)
+    646c5dd4:	jne    646c5d11 <_gnu_exception_handler+0x21>
+    646c5dda:	mov    $0xffffffff,%eax
+    646c5ddf:	add    $0x20,%rsp
+    646c5de3:	pop    %rbx
+    646c5de4:	ret
+    646c5de5:	cmp    $0xc0000095,%eax
+    646c5dea:	je     646c5dda <_gnu_exception_handler+0xea>
+    646c5dec:	cmp    $0xc0000096,%eax
+    646c5df1:	jne    646c5d61 <_gnu_exception_handler+0x71>
+    646c5df7:	xor    %edx,%edx
+    646c5df9:	mov    $0x4,%ecx
+    646c5dfe:	call   646c76f8 <signal>
+    646c5e03:	cmp    $0x1,%rax
+    646c5e07:	je     646c5ec0 <_gnu_exception_handler+0x1d0>
+    646c5e0d:	test   %rax,%rax
+    646c5e10:	je     646c5d61 <_gnu_exception_handler+0x71>
+    646c5e16:	mov    $0x4,%ecx
+    646c5e1b:	call   *%rax
+    646c5e1d:	mov    $0xffffffff,%eax
+    646c5e22:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5e24:	cmp    $0xc000001d,%eax
+    646c5e29:	je     646c5df7 <_gnu_exception_handler+0x107>
+    646c5e2b:	cmp    $0xc000008c,%eax
+    646c5e30:	jne    646c5d61 <_gnu_exception_handler+0x71>
+    646c5e36:	jmp    646c5dda <_gnu_exception_handler+0xea>
+    646c5e38:	nopl   0x0(%rax,%rax,1)
+    646c5e40:	xor    %edx,%edx
+    646c5e42:	mov    $0x8,%ecx
+    646c5e47:	call   646c76f8 <signal>
+    646c5e4c:	cmp    $0x1,%rax
+    646c5e50:	jne    646c5db1 <_gnu_exception_handler+0xc1>
+    646c5e56:	mov    $0x1,%edx
+    646c5e5b:	mov    $0x8,%ecx
+    646c5e60:	call   646c76f8 <signal>
+    646c5e65:	mov    $0xffffffff,%eax
+    646c5e6a:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5e6f:	nop
+    646c5e70:	mov    $0xb,%ecx
+    646c5e75:	call   *%rax
+    646c5e77:	mov    $0xffffffff,%eax
+    646c5e7c:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5e81:	xor    %eax,%eax
+    646c5e83:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5e88:	nopl   0x0(%rax,%rax,1)
+    646c5e90:	mov    $0x1,%edx
+    646c5e95:	mov    $0x8,%ecx
+    646c5e9a:	call   646c76f8 <signal>
+    646c5e9f:	call   646c6530 <_fpreset>
+    646c5ea4:	jmp    646c5dda <_gnu_exception_handler+0xea>
+    646c5ea9:	mov    $0x1,%edx
+    646c5eae:	mov    $0xb,%ecx
+    646c5eb3:	call   646c76f8 <signal>
+    646c5eb8:	or     $0xffffffff,%eax
+    646c5ebb:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5ec0:	mov    $0x1,%edx
+    646c5ec5:	mov    $0x4,%ecx
+    646c5eca:	call   646c76f8 <signal>
+    646c5ecf:	or     $0xffffffff,%eax
+    646c5ed2:	jmp    646c5dc2 <_gnu_exception_handler+0xd2>
+    646c5ed7:	nop
+    646c5ed8:	nop
+    646c5ed9:	nop
+    646c5eda:	nop
+    646c5edb:	nop
+    646c5edc:	nop
+    646c5edd:	nop
+    646c5ede:	nop
+    646c5edf:	nop
+
+00000000646c5ee0 <__mingwthr_run_key_dtors.part.0>:
+    646c5ee0:	push   %rbp
+    646c5ee1:	push   %rdi
+    646c5ee2:	push   %rsi
+    646c5ee3:	push   %rbx
+    646c5ee4:	sub    $0x28,%rsp
+    646c5ee8:	lea    0x6c31(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5eef:	call   *0x82df(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5ef5:	mov    0x6c04(%rip),%rbx        # 646ccb00 <key_dtor_list>
+    646c5efc:	test   %rbx,%rbx
+    646c5eff:	je     646c5f34 <__mingwthr_run_key_dtors.part.0+0x54>
+    646c5f01:	mov    0x8354(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
+    646c5f08:	mov    0x82e5(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
+    646c5f0f:	nop
+    646c5f10:	mov    (%rbx),%ecx
+    646c5f12:	call   *%rbp
+    646c5f14:	mov    %rax,%rsi
+    646c5f17:	call   *%rdi
+    646c5f19:	test   %eax,%eax
+    646c5f1b:	jne    646c5f2b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c5f1d:	test   %rsi,%rsi
+    646c5f20:	je     646c5f2b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c5f22:	mov    0x8(%rbx),%rax
+    646c5f26:	mov    %rsi,%rcx
+    646c5f29:	call   *%rax
+    646c5f2b:	mov    0x10(%rbx),%rbx
+    646c5f2f:	test   %rbx,%rbx
+    646c5f32:	jne    646c5f10 <__mingwthr_run_key_dtors.part.0+0x30>
+    646c5f34:	lea    0x6be5(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f3b:	add    $0x28,%rsp
+    646c5f3f:	pop    %rbx
+    646c5f40:	pop    %rsi
+    646c5f41:	pop    %rdi
+    646c5f42:	pop    %rbp
+    646c5f43:	rex.W jmp *0x82ca(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5f4a:	nopw   0x0(%rax,%rax,1)
+
+00000000646c5f50 <___w64_mingwthr_add_key_dtor>:
+    646c5f50:	push   %rbp
+    646c5f51:	push   %rdi
+    646c5f52:	push   %rsi
+    646c5f53:	push   %rbx
+    646c5f54:	sub    $0x28,%rsp
+    646c5f58:	mov    0x6baa(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c5f5e:	xor    %esi,%esi
+    646c5f60:	test   %eax,%eax
+    646c5f62:	mov    %ecx,%ebp
+    646c5f64:	mov    %rdx,%rdi
+    646c5f67:	jne    646c5f74 <___w64_mingwthr_add_key_dtor+0x24>
+    646c5f69:	mov    %esi,%eax
+    646c5f6b:	add    $0x28,%rsp
+    646c5f6f:	pop    %rbx
+    646c5f70:	pop    %rsi
+    646c5f71:	pop    %rdi
+    646c5f72:	pop    %rbp
+    646c5f73:	ret
+    646c5f74:	mov    $0x18,%edx
+    646c5f79:	mov    $0x1,%ecx
+    646c5f7e:	call   646c7750 <calloc>
+    646c5f83:	test   %rax,%rax
+    646c5f86:	mov    %rax,%rbx
+    646c5f89:	je     646c5fc8 <___w64_mingwthr_add_key_dtor+0x78>
+    646c5f8b:	mov    %ebp,(%rax)
+    646c5f8d:	lea    0x6b8c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f94:	mov    %rdi,0x8(%rax)
+    646c5f98:	call   *0x8236(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5f9e:	mov    0x6b5b(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c5fa5:	lea    0x6b74(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5fac:	mov    %rbx,0x6b4d(%rip)        # 646ccb00 <key_dtor_list>
+    646c5fb3:	mov    %rax,0x10(%rbx)
+    646c5fb7:	call   *0x8257(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5fbd:	mov    %esi,%eax
+    646c5fbf:	add    $0x28,%rsp
+    646c5fc3:	pop    %rbx
+    646c5fc4:	pop    %rsi
+    646c5fc5:	pop    %rdi
+    646c5fc6:	pop    %rbp
+    646c5fc7:	ret
+    646c5fc8:	mov    $0xffffffff,%esi
+    646c5fcd:	jmp    646c5f69 <___w64_mingwthr_add_key_dtor+0x19>
+    646c5fcf:	nop
+
+00000000646c5fd0 <___w64_mingwthr_remove_key_dtor>:
+    646c5fd0:	push   %rbx
+    646c5fd1:	sub    $0x20,%rsp
+    646c5fd5:	mov    0x6b2d(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c5fdb:	test   %eax,%eax
+    646c5fdd:	mov    %ecx,%ebx
+    646c5fdf:	jne    646c5ff0 <___w64_mingwthr_remove_key_dtor+0x20>
+    646c5fe1:	xor    %eax,%eax
+    646c5fe3:	add    $0x20,%rsp
+    646c5fe7:	pop    %rbx
+    646c5fe8:	ret
+    646c5fe9:	nopl   0x0(%rax)
+    646c5ff0:	lea    0x6b29(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5ff7:	call   *0x81d7(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5ffd:	mov    0x6afc(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c6004:	test   %rax,%rax
+    646c6007:	je     646c6023 <___w64_mingwthr_remove_key_dtor+0x53>
+    646c6009:	mov    (%rax),%edx
+    646c600b:	cmp    %edx,%ebx
+    646c600d:	jne    646c601a <___w64_mingwthr_remove_key_dtor+0x4a>
+    646c600f:	jmp    646c6060 <___w64_mingwthr_remove_key_dtor+0x90>
+    646c6011:	mov    (%rcx),%edx
+    646c6013:	cmp    %ebx,%edx
+    646c6015:	je     646c6040 <___w64_mingwthr_remove_key_dtor+0x70>
+    646c6017:	mov    %rcx,%rax
+    646c601a:	mov    0x10(%rax),%rcx
+    646c601e:	test   %rcx,%rcx
+    646c6021:	jne    646c6011 <___w64_mingwthr_remove_key_dtor+0x41>
+    646c6023:	lea    0x6af6(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c602a:	call   *0x81e4(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c6030:	xor    %eax,%eax
+    646c6032:	add    $0x20,%rsp
+    646c6036:	pop    %rbx
+    646c6037:	ret
+    646c6038:	nopl   0x0(%rax,%rax,1)
+    646c6040:	mov    0x10(%rcx),%rdx
+    646c6044:	mov    %rdx,0x10(%rax)
+    646c6048:	call   646c7728 <free>
+    646c604d:	lea    0x6acc(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c6054:	call   *0x81ba(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c605a:	jmp    646c6030 <___w64_mingwthr_remove_key_dtor+0x60>
+    646c605c:	nopl   0x0(%rax)
+    646c6060:	mov    0x10(%rax),%rdx
+    646c6064:	mov    %rax,%rcx
+    646c6067:	mov    %rdx,0x6a92(%rip)        # 646ccb00 <key_dtor_list>
+    646c606e:	jmp    646c6048 <___w64_mingwthr_remove_key_dtor+0x78>
+
+00000000646c6070 <__mingw_TLScallback>:
+    646c6070:	push   %rbx
+    646c6071:	sub    $0x20,%rsp
+    646c6075:	cmp    $0x1,%edx
+    646c6078:	je     646c6110 <__mingw_TLScallback+0xa0>
+    646c607e:	jb     646c60b0 <__mingw_TLScallback+0x40>
+    646c6080:	cmp    $0x2,%edx
+    646c6083:	je     646c60a0 <__mingw_TLScallback+0x30>
+    646c6085:	cmp    $0x3,%edx
+    646c6088:	jne    646c60a5 <__mingw_TLScallback+0x35>
+    646c608a:	mov    0x6a78(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6090:	test   %eax,%eax
+    646c6092:	je     646c60a5 <__mingw_TLScallback+0x35>
+    646c6094:	call   646c5ee0 <__mingwthr_run_key_dtors.part.0>
+    646c6099:	jmp    646c60a5 <__mingw_TLScallback+0x35>
+    646c609b:	nopl   0x0(%rax,%rax,1)
+    646c60a0:	call   646c6530 <_fpreset>
+    646c60a5:	mov    $0x1,%eax
+    646c60aa:	add    $0x20,%rsp
+    646c60ae:	pop    %rbx
+    646c60af:	ret
+    646c60b0:	mov    0x6a52(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c60b6:	test   %eax,%eax
+    646c60b8:	jne    646c6140 <__mingw_TLScallback+0xd0>
+    646c60be:	mov    0x6a44(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c60c4:	cmp    $0x1,%eax
+    646c60c7:	jne    646c60a5 <__mingw_TLScallback+0x35>
+    646c60c9:	mov    0x6a30(%rip),%rcx        # 646ccb00 <key_dtor_list>
+    646c60d0:	test   %rcx,%rcx
+    646c60d3:	je     646c60e6 <__mingw_TLScallback+0x76>
+    646c60d5:	mov    0x10(%rcx),%rbx
+    646c60d9:	call   646c7728 <free>
+    646c60de:	test   %rbx,%rbx
+    646c60e1:	mov    %rbx,%rcx
+    646c60e4:	jne    646c60d5 <__mingw_TLScallback+0x65>
+    646c60e6:	lea    0x6a33(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c60ed:	movq   $0x0,0x6a08(%rip)        # 646ccb00 <key_dtor_list>
+    646c60f8:	movl   $0x0,0x6a06(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6102:	call   *0x80c4(%rip)        # 646ce1cc <__IAT_start__>
+    646c6108:	jmp    646c60a5 <__mingw_TLScallback+0x35>
+    646c610a:	nopw   0x0(%rax,%rax,1)
+    646c6110:	mov    0x69f2(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6116:	test   %eax,%eax
+    646c6118:	je     646c6130 <__mingw_TLScallback+0xc0>
+    646c611a:	movl   $0x1,0x69e4(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6124:	mov    $0x1,%eax
+    646c6129:	add    $0x20,%rsp
+    646c612d:	pop    %rbx
+    646c612e:	ret
+    646c612f:	nop
+    646c6130:	lea    0x69e9(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c6137:	call   *0x80cf(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c613d:	jmp    646c611a <__mingw_TLScallback+0xaa>
+    646c613f:	nop
+    646c6140:	call   646c5ee0 <__mingwthr_run_key_dtors.part.0>
+    646c6145:	jmp    646c60be <__mingw_TLScallback+0x4e>
+    646c614a:	nop
+    646c614b:	nop
+    646c614c:	nop
+    646c614d:	nop
+    646c614e:	nop
+    646c614f:	nop
+
+00000000646c6150 <_ValidateImageBase.part.0>:
+    646c6150:	movslq 0x3c(%rcx),%rax
+    646c6154:	add    %rax,%rcx
+    646c6157:	xor    %eax,%eax
+    646c6159:	cmpl   $0x4550,(%rcx)
+    646c615f:	je     646c6162 <_ValidateImageBase.part.0+0x12>
+    646c6161:	ret
+    646c6162:	xor    %eax,%eax
+    646c6164:	cmpw   $0x20b,0x18(%rcx)
+    646c616a:	sete   %al
+    646c616d:	ret
+    646c616e:	xchg   %ax,%ax
+
+00000000646c6170 <_ValidateImageBase>:
+    646c6170:	cmpw   $0x5a4d,(%rcx)
+    646c6175:	je     646c6180 <_ValidateImageBase+0x10>
+    646c6177:	xor    %eax,%eax
+    646c6179:	ret
+    646c617a:	nopw   0x0(%rax,%rax,1)
+    646c6180:	jmp    646c6150 <_ValidateImageBase.part.0>
+    646c6182:	nopl   0x0(%rax)
+    646c6186:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6190 <_FindPESection>:
+    646c6190:	movslq 0x3c(%rcx),%rax
+    646c6194:	add    %rax,%rcx
+    646c6197:	movzwl 0x14(%rcx),%eax
+    646c619b:	lea    0x18(%rcx,%rax,1),%rax
+    646c61a0:	movzwl 0x6(%rcx),%ecx
+    646c61a4:	test   %ecx,%ecx
+    646c61a6:	je     646c61d1 <_FindPESection+0x41>
+    646c61a8:	sub    $0x1,%ecx
+    646c61ab:	lea    (%rcx,%rcx,4),%rcx
+    646c61af:	lea    0x28(%rax,%rcx,8),%r9
+    646c61b4:	mov    0xc(%rax),%r8d
+    646c61b8:	cmp    %rdx,%r8
+    646c61bb:	mov    %r8,%rcx
+    646c61be:	ja     646c61c8 <_FindPESection+0x38>
+    646c61c0:	add    0x8(%rax),%ecx
+    646c61c3:	cmp    %rdx,%rcx
+    646c61c6:	ja     646c61d3 <_FindPESection+0x43>
+    646c61c8:	add    $0x28,%rax
+    646c61cc:	cmp    %r9,%rax
+    646c61cf:	jne    646c61b4 <_FindPESection+0x24>
+    646c61d1:	xor    %eax,%eax
+    646c61d3:	ret
+    646c61d4:	xchg   %ax,%ax
+    646c61d6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c61e0 <_FindPESectionByName>:
+    646c61e0:	push   %rdi
+    646c61e1:	push   %rsi
+    646c61e2:	push   %rbx
+    646c61e3:	sub    $0x20,%rsp
+    646c61e7:	mov    %rcx,%rsi
+    646c61ea:	call   646c76f0 <strlen>
+    646c61ef:	cmp    $0x8,%rax
+    646c61f3:	ja     646c6260 <_FindPESectionByName+0x80>
+    646c61f5:	mov    0x3414(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c61fc:	cmpw   $0x5a4d,(%rdx)
+    646c6201:	jne    646c6260 <_FindPESectionByName+0x80>
+    646c6203:	mov    %rdx,%rcx
+    646c6206:	call   646c6150 <_ValidateImageBase.part.0>
+    646c620b:	test   %eax,%eax
+    646c620d:	je     646c6260 <_FindPESectionByName+0x80>
+    646c620f:	movslq 0x3c(%rdx),%rcx
+    646c6213:	add    %rdx,%rcx
+    646c6216:	movzwl 0x14(%rcx),%eax
+    646c621a:	lea    0x18(%rcx,%rax,1),%rbx
+    646c621f:	movzwl 0x6(%rcx),%eax
+    646c6223:	test   %eax,%eax
+    646c6225:	je     646c6260 <_FindPESectionByName+0x80>
+    646c6227:	sub    $0x1,%eax
+    646c622a:	lea    (%rax,%rax,4),%rax
+    646c622e:	lea    0x28(%rbx,%rax,8),%rdi
+    646c6233:	jmp    646c623e <_FindPESectionByName+0x5e>
+    646c6235:	add    $0x28,%rbx
+    646c6239:	cmp    %rdi,%rbx
+    646c623c:	je     646c6260 <_FindPESectionByName+0x80>
+    646c623e:	mov    $0x8,%r8d
+    646c6244:	mov    %rsi,%rdx
+    646c6247:	mov    %rbx,%rcx
+    646c624a:	call   646c76e8 <strncmp>
+    646c624f:	test   %eax,%eax
+    646c6251:	jne    646c6235 <_FindPESectionByName+0x55>
+    646c6253:	mov    %rbx,%rax
+    646c6256:	add    $0x20,%rsp
+    646c625a:	pop    %rbx
+    646c625b:	pop    %rsi
+    646c625c:	pop    %rdi
+    646c625d:	ret
+    646c625e:	xchg   %ax,%ax
+    646c6260:	xor    %ebx,%ebx
+    646c6262:	mov    %rbx,%rax
+    646c6265:	add    $0x20,%rsp
+    646c6269:	pop    %rbx
+    646c626a:	pop    %rsi
+    646c626b:	pop    %rdi
+    646c626c:	ret
+    646c626d:	nopl   (%rax)
+
+00000000646c6270 <__mingw_GetSectionForAddress>:
+    646c6270:	sub    $0x28,%rsp
+    646c6274:	mov    0x3395(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c627b:	cmpw   $0x5a4d,(%r8)
+    646c6281:	mov    %rcx,%rdx
+    646c6284:	jne    646c62dd <__mingw_GetSectionForAddress+0x6d>
+    646c6286:	mov    %r8,%rcx
+    646c6289:	call   646c6150 <_ValidateImageBase.part.0>
+    646c628e:	test   %eax,%eax
+    646c6290:	je     646c62dd <__mingw_GetSectionForAddress+0x6d>
+    646c6292:	movslq 0x3c(%r8),%rax
+    646c6296:	mov    %rdx,%rcx
+    646c6299:	sub    %r8,%rcx
+    646c629c:	add    %rax,%r8
+    646c629f:	movzwl 0x6(%r8),%edx
+    646c62a4:	movzwl 0x14(%r8),%eax
+    646c62a9:	test   %edx,%edx
+    646c62ab:	lea    0x18(%r8,%rax,1),%rax
+    646c62b0:	je     646c62dd <__mingw_GetSectionForAddress+0x6d>
+    646c62b2:	sub    $0x1,%edx
+    646c62b5:	lea    (%rdx,%rdx,4),%rdx
+    646c62b9:	lea    0x28(%rax,%rdx,8),%r9
+    646c62be:	xchg   %ax,%ax
+    646c62c0:	mov    0xc(%rax),%r8d
+    646c62c4:	cmp    %r8,%rcx
+    646c62c7:	mov    %r8,%rdx
+    646c62ca:	jb     646c62d4 <__mingw_GetSectionForAddress+0x64>
+    646c62cc:	add    0x8(%rax),%edx
+    646c62cf:	cmp    %rdx,%rcx
+    646c62d2:	jb     646c62df <__mingw_GetSectionForAddress+0x6f>
+    646c62d4:	add    $0x28,%rax
+    646c62d8:	cmp    %r9,%rax
+    646c62db:	jne    646c62c0 <__mingw_GetSectionForAddress+0x50>
+    646c62dd:	xor    %eax,%eax
+    646c62df:	add    $0x28,%rsp
+    646c62e3:	ret
+    646c62e4:	xchg   %ax,%ax
     646c62e6:	cs nopw 0x0(%rax,%rax,1)
-    646c62f0:	testb  $0x20,0x27(%rax)
-    646c62f4:	je     646c62ff <_FindPESectionExec+0x5f>
-    646c62f6:	test   %rdx,%rdx
-    646c62f9:	je     646c630a <_FindPESectionExec+0x6a>
-    646c62fb:	sub    $0x1,%rdx
-    646c62ff:	add    $0x28,%rax
-    646c6303:	cmp    %rcx,%rax
-    646c6306:	jne    646c62f0 <_FindPESectionExec+0x50>
-    646c6308:	xor    %eax,%eax
-    646c630a:	add    $0x28,%rsp
-    646c630e:	ret
-    646c630f:	nop
-
-00000000646c6310 <_GetPEImageBase>:
-    646c6310:	sub    $0x28,%rsp
-    646c6314:	mov    0x32f5(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
-    646c631b:	cmpw   $0x5a4d,(%rdx)
-    646c6320:	jne    646c6340 <_GetPEImageBase+0x30>
-    646c6322:	mov    %rdx,%rcx
-    646c6325:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c632a:	test   %eax,%eax
-    646c632c:	mov    $0x0,%eax
-    646c6331:	cmovne %rdx,%rax
-    646c6335:	add    $0x28,%rsp
-    646c6339:	ret
-    646c633a:	nopw   0x0(%rax,%rax,1)
-    646c6340:	xor    %eax,%eax
-    646c6342:	add    $0x28,%rsp
-    646c6346:	ret
-    646c6347:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6350 <_IsNonwritableInCurrentImage>:
-    646c6350:	sub    $0x28,%rsp
-    646c6354:	mov    0x32b5(%rip),%r8        # 646c9610 <.refptr.__image_base__>
-    646c635b:	xor    %eax,%eax
-    646c635d:	cmpw   $0x5a4d,(%r8)
-    646c6363:	mov    %rcx,%rdx
-    646c6366:	je     646c6370 <_IsNonwritableInCurrentImage+0x20>
-    646c6368:	add    $0x28,%rsp
-    646c636c:	ret
-    646c636d:	nopl   (%rax)
-    646c6370:	mov    %r8,%rcx
-    646c6373:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c6378:	test   %eax,%eax
-    646c637a:	je     646c6368 <_IsNonwritableInCurrentImage+0x18>
-    646c637c:	movslq 0x3c(%r8),%rax
-    646c6380:	mov    %rdx,%rcx
-    646c6383:	sub    %r8,%rcx
-    646c6386:	add    %rax,%r8
-    646c6389:	movzwl 0x6(%r8),%edx
-    646c638e:	movzwl 0x14(%r8),%eax
-    646c6393:	test   %edx,%edx
-    646c6395:	lea    0x18(%r8,%rax,1),%rax
-    646c639a:	je     646c63cd <_IsNonwritableInCurrentImage+0x7d>
-    646c639c:	sub    $0x1,%edx
-    646c639f:	lea    (%rdx,%rdx,4),%rdx
-    646c63a3:	lea    0x28(%rax,%rdx,8),%r9
-    646c63a8:	nopl   0x0(%rax,%rax,1)
-    646c63b0:	mov    0xc(%rax),%r8d
-    646c63b4:	cmp    %r8,%rcx
-    646c63b7:	mov    %r8,%rdx
-    646c63ba:	jb     646c63c4 <_IsNonwritableInCurrentImage+0x74>
-    646c63bc:	add    0x8(%rax),%edx
-    646c63bf:	cmp    %rdx,%rcx
-    646c63c2:	jb     646c63d4 <_IsNonwritableInCurrentImage+0x84>
-    646c63c4:	add    $0x28,%rax
-    646c63c8:	cmp    %r9,%rax
-    646c63cb:	jne    646c63b0 <_IsNonwritableInCurrentImage+0x60>
-    646c63cd:	xor    %eax,%eax
-    646c63cf:	add    $0x28,%rsp
-    646c63d3:	ret
-    646c63d4:	mov    0x24(%rax),%eax
-    646c63d7:	not    %eax
-    646c63d9:	shr    $0x1f,%eax
-    646c63dc:	add    $0x28,%rsp
-    646c63e0:	ret
-    646c63e1:	nopl   0x0(%rax,%rax,1)
-    646c63e6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c63f0 <__mingw_enum_import_library_names>:
-    646c63f0:	sub    $0x28,%rsp
-    646c63f4:	mov    0x3215(%rip),%r11        # 646c9610 <.refptr.__image_base__>
-    646c63fb:	cmpw   $0x5a4d,(%r11)
-    646c6401:	mov    %ecx,%r9d
-    646c6404:	jne    646c645e <__mingw_enum_import_library_names+0x6e>
-    646c6406:	mov    %r11,%rcx
-    646c6409:	call   646c60c0 <_ValidateImageBase.part.0>
-    646c640e:	test   %eax,%eax
-    646c6410:	je     646c645e <__mingw_enum_import_library_names+0x6e>
-    646c6412:	movslq 0x3c(%r11),%rax
-    646c6416:	add    %r11,%rax
-    646c6419:	mov    0x90(%rax),%edx
-    646c641f:	test   %edx,%edx
-    646c6421:	je     646c645e <__mingw_enum_import_library_names+0x6e>
-    646c6423:	movzwl 0x14(%rax),%ecx
-    646c6427:	lea    0x18(%rax,%rcx,1),%rcx
-    646c642c:	movzwl 0x6(%rax),%eax
-    646c6430:	test   %eax,%eax
-    646c6432:	je     646c645e <__mingw_enum_import_library_names+0x6e>
-    646c6434:	sub    $0x1,%eax
-    646c6437:	lea    (%rax,%rax,4),%rax
-    646c643b:	lea    0x28(%rcx,%rax,8),%rax
-    646c6440:	mov    0xc(%rcx),%r10d
-    646c6444:	cmp    %r10,%rdx
-    646c6447:	mov    %r10,%r8
-    646c644a:	jb     646c6455 <__mingw_enum_import_library_names+0x65>
-    646c644c:	add    0x8(%rcx),%r8d
-    646c6450:	cmp    %r8,%rdx
-    646c6453:	jb     646c6465 <__mingw_enum_import_library_names+0x75>
-    646c6455:	add    $0x28,%rcx
-    646c6459:	cmp    %rax,%rcx
-    646c645c:	jne    646c6440 <__mingw_enum_import_library_names+0x50>
-    646c645e:	xor    %eax,%eax
-    646c6460:	add    $0x28,%rsp
-    646c6464:	ret
-    646c6465:	add    %r11,%rdx
-    646c6468:	jne    646c6478 <__mingw_enum_import_library_names+0x88>
-    646c646a:	jmp    646c645e <__mingw_enum_import_library_names+0x6e>
-    646c646c:	nopl   0x0(%rax)
-    646c6470:	sub    $0x1,%r9d
-    646c6474:	add    $0x14,%rdx
-    646c6478:	mov    0x4(%rdx),%ecx
-    646c647b:	test   %ecx,%ecx
-    646c647d:	jne    646c6486 <__mingw_enum_import_library_names+0x96>
-    646c647f:	mov    0xc(%rdx),%eax
-    646c6482:	test   %eax,%eax
-    646c6484:	je     646c645e <__mingw_enum_import_library_names+0x6e>
-    646c6486:	test   %r9d,%r9d
-    646c6489:	jg     646c6470 <__mingw_enum_import_library_names+0x80>
-    646c648b:	mov    0xc(%rdx),%eax
-    646c648e:	add    %r11,%rax
-    646c6491:	add    $0x28,%rsp
-    646c6495:	ret
-    646c6496:	nop
-    646c6497:	nop
-    646c6498:	nop
-    646c6499:	nop
-    646c649a:	nop
-    646c649b:	nop
-    646c649c:	nop
-    646c649d:	nop
-    646c649e:	nop
-    646c649f:	nop
-
-00000000646c64a0 <_fpreset>:
-    646c64a0:	fninit
-    646c64a2:	ret
-    646c64a3:	nop
-    646c64a4:	nop
-    646c64a5:	nop
-    646c64a6:	nop
-    646c64a7:	nop
-    646c64a8:	nop
-    646c64a9:	nop
-    646c64aa:	nop
-    646c64ab:	nop
-    646c64ac:	nop
-    646c64ad:	nop
-    646c64ae:	nop
-    646c64af:	nop
 
-00000000646c64b0 <___chkstk_ms>:
+00000000646c62f0 <__mingw_GetSectionCount>:
+    646c62f0:	sub    $0x28,%rsp
+    646c62f4:	mov    0x3315(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c62fb:	xor    %r8d,%r8d
+    646c62fe:	cmpw   $0x5a4d,(%rdx)
+    646c6303:	je     646c6310 <__mingw_GetSectionCount+0x20>
+    646c6305:	mov    %r8d,%eax
+    646c6308:	add    $0x28,%rsp
+    646c630c:	ret
+    646c630d:	nopl   (%rax)
+    646c6310:	mov    %rdx,%rcx
+    646c6313:	call   646c6150 <_ValidateImageBase.part.0>
+    646c6318:	test   %eax,%eax
+    646c631a:	je     646c6305 <__mingw_GetSectionCount+0x15>
+    646c631c:	movslq 0x3c(%rdx),%rax
+    646c6320:	movzwl 0x6(%rax,%rdx,1),%r8d
+    646c6326:	mov    %r8d,%eax
+    646c6329:	add    $0x28,%rsp
+    646c632d:	ret
+    646c632e:	xchg   %ax,%ax
+
+00000000646c6330 <_FindPESectionExec>:
+    646c6330:	sub    $0x28,%rsp
+    646c6334:	mov    0x32d5(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c633b:	cmpw   $0x5a4d,(%r8)
+    646c6341:	mov    %rcx,%rdx
+    646c6344:	jne    646c6398 <_FindPESectionExec+0x68>
+    646c6346:	mov    %r8,%rcx
+    646c6349:	call   646c6150 <_ValidateImageBase.part.0>
+    646c634e:	test   %eax,%eax
+    646c6350:	je     646c6398 <_FindPESectionExec+0x68>
+    646c6352:	movslq 0x3c(%r8),%rcx
+    646c6356:	add    %r8,%rcx
+    646c6359:	movzwl 0x14(%rcx),%eax
+    646c635d:	lea    0x18(%rcx,%rax,1),%rax
+    646c6362:	movzwl 0x6(%rcx),%ecx
+    646c6366:	test   %ecx,%ecx
+    646c6368:	je     646c6398 <_FindPESectionExec+0x68>
+    646c636a:	sub    $0x1,%ecx
+    646c636d:	lea    (%rcx,%rcx,4),%rcx
+    646c6371:	lea    0x28(%rax,%rcx,8),%rcx
+    646c6376:	cs nopw 0x0(%rax,%rax,1)
+    646c6380:	testb  $0x20,0x27(%rax)
+    646c6384:	je     646c638f <_FindPESectionExec+0x5f>
+    646c6386:	test   %rdx,%rdx
+    646c6389:	je     646c639a <_FindPESectionExec+0x6a>
+    646c638b:	sub    $0x1,%rdx
+    646c638f:	add    $0x28,%rax
+    646c6393:	cmp    %rcx,%rax
+    646c6396:	jne    646c6380 <_FindPESectionExec+0x50>
+    646c6398:	xor    %eax,%eax
+    646c639a:	add    $0x28,%rsp
+    646c639e:	ret
+    646c639f:	nop
+
+00000000646c63a0 <_GetPEImageBase>:
+    646c63a0:	sub    $0x28,%rsp
+    646c63a4:	mov    0x3265(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c63ab:	cmpw   $0x5a4d,(%rdx)
+    646c63b0:	jne    646c63d0 <_GetPEImageBase+0x30>
+    646c63b2:	mov    %rdx,%rcx
+    646c63b5:	call   646c6150 <_ValidateImageBase.part.0>
+    646c63ba:	test   %eax,%eax
+    646c63bc:	mov    $0x0,%eax
+    646c63c1:	cmovne %rdx,%rax
+    646c63c5:	add    $0x28,%rsp
+    646c63c9:	ret
+    646c63ca:	nopw   0x0(%rax,%rax,1)
+    646c63d0:	xor    %eax,%eax
+    646c63d2:	add    $0x28,%rsp
+    646c63d6:	ret
+    646c63d7:	nopw   0x0(%rax,%rax,1)
+
+00000000646c63e0 <_IsNonwritableInCurrentImage>:
+    646c63e0:	sub    $0x28,%rsp
+    646c63e4:	mov    0x3225(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c63eb:	xor    %eax,%eax
+    646c63ed:	cmpw   $0x5a4d,(%r8)
+    646c63f3:	mov    %rcx,%rdx
+    646c63f6:	je     646c6400 <_IsNonwritableInCurrentImage+0x20>
+    646c63f8:	add    $0x28,%rsp
+    646c63fc:	ret
+    646c63fd:	nopl   (%rax)
+    646c6400:	mov    %r8,%rcx
+    646c6403:	call   646c6150 <_ValidateImageBase.part.0>
+    646c6408:	test   %eax,%eax
+    646c640a:	je     646c63f8 <_IsNonwritableInCurrentImage+0x18>
+    646c640c:	movslq 0x3c(%r8),%rax
+    646c6410:	mov    %rdx,%rcx
+    646c6413:	sub    %r8,%rcx
+    646c6416:	add    %rax,%r8
+    646c6419:	movzwl 0x6(%r8),%edx
+    646c641e:	movzwl 0x14(%r8),%eax
+    646c6423:	test   %edx,%edx
+    646c6425:	lea    0x18(%r8,%rax,1),%rax
+    646c642a:	je     646c645d <_IsNonwritableInCurrentImage+0x7d>
+    646c642c:	sub    $0x1,%edx
+    646c642f:	lea    (%rdx,%rdx,4),%rdx
+    646c6433:	lea    0x28(%rax,%rdx,8),%r9
+    646c6438:	nopl   0x0(%rax,%rax,1)
+    646c6440:	mov    0xc(%rax),%r8d
+    646c6444:	cmp    %r8,%rcx
+    646c6447:	mov    %r8,%rdx
+    646c644a:	jb     646c6454 <_IsNonwritableInCurrentImage+0x74>
+    646c644c:	add    0x8(%rax),%edx
+    646c644f:	cmp    %rdx,%rcx
+    646c6452:	jb     646c6464 <_IsNonwritableInCurrentImage+0x84>
+    646c6454:	add    $0x28,%rax
+    646c6458:	cmp    %r9,%rax
+    646c645b:	jne    646c6440 <_IsNonwritableInCurrentImage+0x60>
+    646c645d:	xor    %eax,%eax
+    646c645f:	add    $0x28,%rsp
+    646c6463:	ret
+    646c6464:	mov    0x24(%rax),%eax
+    646c6467:	not    %eax
+    646c6469:	shr    $0x1f,%eax
+    646c646c:	add    $0x28,%rsp
+    646c6470:	ret
+    646c6471:	nopl   0x0(%rax,%rax,1)
+    646c6476:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6480 <__mingw_enum_import_library_names>:
+    646c6480:	sub    $0x28,%rsp
+    646c6484:	mov    0x3185(%rip),%r11        # 646c9610 <.refptr.__image_base__>
+    646c648b:	cmpw   $0x5a4d,(%r11)
+    646c6491:	mov    %ecx,%r9d
+    646c6494:	jne    646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c6496:	mov    %r11,%rcx
+    646c6499:	call   646c6150 <_ValidateImageBase.part.0>
+    646c649e:	test   %eax,%eax
+    646c64a0:	je     646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c64a2:	movslq 0x3c(%r11),%rax
+    646c64a6:	add    %r11,%rax
+    646c64a9:	mov    0x90(%rax),%edx
+    646c64af:	test   %edx,%edx
+    646c64b1:	je     646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c64b3:	movzwl 0x14(%rax),%ecx
+    646c64b7:	lea    0x18(%rax,%rcx,1),%rcx
+    646c64bc:	movzwl 0x6(%rax),%eax
+    646c64c0:	test   %eax,%eax
+    646c64c2:	je     646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c64c4:	sub    $0x1,%eax
+    646c64c7:	lea    (%rax,%rax,4),%rax
+    646c64cb:	lea    0x28(%rcx,%rax,8),%rax
+    646c64d0:	mov    0xc(%rcx),%r10d
+    646c64d4:	cmp    %r10,%rdx
+    646c64d7:	mov    %r10,%r8
+    646c64da:	jb     646c64e5 <__mingw_enum_import_library_names+0x65>
+    646c64dc:	add    0x8(%rcx),%r8d
+    646c64e0:	cmp    %r8,%rdx
+    646c64e3:	jb     646c64f5 <__mingw_enum_import_library_names+0x75>
+    646c64e5:	add    $0x28,%rcx
+    646c64e9:	cmp    %rax,%rcx
+    646c64ec:	jne    646c64d0 <__mingw_enum_import_library_names+0x50>
+    646c64ee:	xor    %eax,%eax
+    646c64f0:	add    $0x28,%rsp
+    646c64f4:	ret
+    646c64f5:	add    %r11,%rdx
+    646c64f8:	jne    646c6508 <__mingw_enum_import_library_names+0x88>
+    646c64fa:	jmp    646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c64fc:	nopl   0x0(%rax)
+    646c6500:	sub    $0x1,%r9d
+    646c6504:	add    $0x14,%rdx
+    646c6508:	mov    0x4(%rdx),%ecx
+    646c650b:	test   %ecx,%ecx
+    646c650d:	jne    646c6516 <__mingw_enum_import_library_names+0x96>
+    646c650f:	mov    0xc(%rdx),%eax
+    646c6512:	test   %eax,%eax
+    646c6514:	je     646c64ee <__mingw_enum_import_library_names+0x6e>
+    646c6516:	test   %r9d,%r9d
+    646c6519:	jg     646c6500 <__mingw_enum_import_library_names+0x80>
+    646c651b:	mov    0xc(%rdx),%eax
+    646c651e:	add    %r11,%rax
+    646c6521:	add    $0x28,%rsp
+    646c6525:	ret
+    646c6526:	nop
+    646c6527:	nop
+    646c6528:	nop
+    646c6529:	nop
+    646c652a:	nop
+    646c652b:	nop
+    646c652c:	nop
+    646c652d:	nop
+    646c652e:	nop
+    646c652f:	nop
+
+00000000646c6530 <_fpreset>:
+    646c6530:	fninit
+    646c6532:	ret
+    646c6533:	nop
+    646c6534:	nop
+    646c6535:	nop
+    646c6536:	nop
+    646c6537:	nop
+    646c6538:	nop
+    646c6539:	nop
+    646c653a:	nop
+    646c653b:	nop
+    646c653c:	nop
+    646c653d:	nop
+    646c653e:	nop
+    646c653f:	nop
+
+00000000646c6540 <___chkstk_ms>:
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:117
-    646c64b0:	push   %rcx
+    646c6540:	push   %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:119
-    646c64b1:	push   %rax
+    646c6541:	push   %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:121
-    646c64b2:	cmp    $0x1000,%rax
+    646c6542:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:122
-    646c64b8:	lea    0x18(%rsp),%rcx
+    646c6548:	lea    0x18(%rsp),%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:123
-    646c64bd:	jb     646c64d8 <___chkstk_ms+0x28>
+    646c654d:	jb     646c6568 <___chkstk_ms+0x28>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:125
-    646c64bf:	sub    $0x1000,%rcx
+    646c654f:	sub    $0x1000,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:126
-    646c64c6:	orq    $0x0,(%rcx)
+    646c6556:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:127
-    646c64ca:	sub    $0x1000,%rax
+    646c655a:	sub    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:128
-    646c64d0:	cmp    $0x1000,%rax
+    646c6560:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:129
-    646c64d6:	ja     646c64bf <___chkstk_ms+0xf>
+    646c6566:	ja     646c654f <___chkstk_ms+0xf>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:131
-    646c64d8:	sub    %rax,%rcx
+    646c6568:	sub    %rax,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:132
-    646c64db:	orq    $0x0,(%rcx)
+    646c656b:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:134
-    646c64df:	pop    %rax
+    646c656f:	pop    %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:136
-    646c64e0:	pop    %rcx
+    646c6570:	pop    %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:138
-    646c64e1:	ret
-    646c64e2:	nop
-    646c64e3:	nop
-    646c64e4:	nop
-    646c64e5:	nop
-    646c64e6:	nop
-    646c64e7:	nop
-    646c64e8:	nop
-    646c64e9:	nop
-    646c64ea:	nop
-    646c64eb:	nop
-    646c64ec:	nop
-    646c64ed:	nop
-    646c64ee:	nop
-    646c64ef:	nop
-
-00000000646c64f0 <DllEntryPoint>:
-    646c64f0:	mov    $0x1,%eax
-    646c64f5:	ret
-    646c64f6:	nop
-    646c64f7:	nop
-    646c64f8:	nop
-    646c64f9:	nop
-    646c64fa:	nop
-    646c64fb:	nop
-    646c64fc:	nop
-    646c64fd:	nop
-    646c64fe:	nop
-    646c64ff:	nop
-
-00000000646c6500 <DllMain>:
-    646c6500:	mov    $0x1,%eax
-    646c6505:	ret
-    646c6506:	nop
-    646c6507:	nop
-    646c6508:	nop
-    646c6509:	nop
-    646c650a:	nop
-    646c650b:	nop
-    646c650c:	nop
-    646c650d:	nop
-    646c650e:	nop
-    646c650f:	nop
-
-00000000646c6510 <__fpclassify>:
-    646c6510:	movq   %xmm0,%rax
-    646c6515:	movq   %xmm0,%rdx
-    646c651a:	shr    $0x20,%rax
-    646c651e:	mov    %eax,%ecx
-    646c6520:	and    $0xfffff,%ecx
-    646c6526:	or     %edx,%ecx
-    646c6528:	mov    %eax,%edx
-    646c652a:	mov    $0x4000,%eax
-    646c652f:	and    $0x7ff00000,%edx
-    646c6535:	mov    %ecx,%r8d
-    646c6538:	or     %edx,%r8d
-    646c653b:	je     646c6553 <__fpclassify+0x43>
-    646c653d:	test   %edx,%edx
-    646c653f:	mov    $0x4400,%eax
-    646c6544:	je     646c6553 <__fpclassify+0x43>
-    646c6546:	cmp    $0x7ff00000,%edx
-    646c654c:	mov    $0x400,%eax
-    646c6551:	je     646c6554 <__fpclassify+0x44>
-    646c6553:	ret
-    646c6554:	cmp    $0x1,%ecx
-    646c6557:	sbb    %eax,%eax
-    646c6559:	and    $0x400,%eax
-    646c655e:	add    $0x100,%eax
-    646c6563:	ret
-    646c6564:	nop
-    646c6565:	nop
-    646c6566:	nop
-    646c6567:	nop
-    646c6568:	nop
-    646c6569:	nop
-    646c656a:	nop
-    646c656b:	nop
-    646c656c:	nop
-    646c656d:	nop
-    646c656e:	nop
-    646c656f:	nop
-
-00000000646c6570 <sqrt>:
-    646c6570:	push   %rbx
-    646c6571:	sub    $0x50,%rsp
-    646c6575:	movaps %xmm6,0x40(%rsp)
-    646c657a:	movq   %xmm0,%rdx
-    646c657f:	movq   %xmm0,%rbx
-    646c6584:	shr    $0x20,%rdx
-    646c6588:	mov    %edx,%eax
-    646c658a:	mov    %edx,%ecx
-    646c658c:	and    $0xfffff,%eax
-    646c6591:	and    $0x7ff00000,%ecx
-    646c6597:	or     %ebx,%eax
-    646c6599:	mov    %eax,%r8d
-    646c659c:	or     %ecx,%r8d
-    646c659f:	je     646c65e0 <sqrt+0x70>
-    646c65a1:	test   %ecx,%ecx
-    646c65a3:	jne    646c6600 <sqrt+0x90>
-    646c65a5:	test   %edx,%edx
-    646c65a7:	js     646c6620 <sqrt+0xb0>
-    646c65a9:	movsd  0x2d6f(%rip),%xmm0        # 646c9320 <.rdata+0x20>
-    646c65b1:	movq   %rbx,%xmm1
-    646c65b6:	ucomisd %xmm0,%xmm1
-    646c65ba:	jp     646c65be <sqrt+0x4e>
-    646c65bc:	je     646c65d3 <sqrt+0x63>
-    646c65be:	mov    %rbx,0x38(%rsp)
-    646c65c3:	fldl   0x38(%rsp)
-    646c65c7:	fsqrt
-    646c65c9:	fstpl  0x38(%rsp)
-    646c65cd:	movsd  0x38(%rsp),%xmm0
-    646c65d3:	movaps 0x40(%rsp),%xmm6
-    646c65d8:	add    $0x50,%rsp
-    646c65dc:	pop    %rbx
-    646c65dd:	ret
-    646c65de:	xchg   %ax,%ax
-    646c65e0:	test   %edx,%edx
-    646c65e2:	pxor   %xmm0,%xmm0
-    646c65e6:	jns    646c65d3 <sqrt+0x63>
-    646c65e8:	movsd  0x2d18(%rip),%xmm0        # 646c9308 <.rdata+0x8>
-    646c65f0:	movaps 0x40(%rsp),%xmm6
-    646c65f5:	add    $0x50,%rsp
-    646c65f9:	pop    %rbx
-    646c65fa:	ret
-    646c65fb:	nopl   0x0(%rax,%rax,1)
-    646c6600:	cmp    $0x7ff00000,%ecx
-    646c6606:	jne    646c65a5 <sqrt+0x35>
-    646c6608:	test   %eax,%eax
-    646c660a:	jne    646c6662 <sqrt+0xf2>
-    646c660c:	test   %edx,%edx
-    646c660e:	js     646c6620 <sqrt+0xb0>
-    646c6610:	movsd  0x2d00(%rip),%xmm0        # 646c9318 <.rdata+0x18>
-    646c6618:	jmp    646c65d3 <sqrt+0x63>
-    646c661a:	nopw   0x0(%rax,%rax,1)
-    646c6620:	call   646c76e8 <_errno>
-    646c6625:	movq   %rbx,%xmm2
-    646c662a:	mov    $0x1,%ecx
-    646c662f:	movsd  0x2cd9(%rip),%xmm6        # 646c9310 <.rdata+0x10>
-    646c6637:	movl   $0x21,(%rax)
-    646c663d:	lea    0x2cbc(%rip),%rdx        # 646c9300 <.rdata>
-    646c6644:	pxor   %xmm3,%xmm3
-    646c6648:	movsd  %xmm6,0x20(%rsp)
-    646c664e:	call   646c7960 <__mingw_raise_matherr>
-    646c6653:	movapd %xmm6,%xmm0
-    646c6657:	movaps 0x40(%rsp),%xmm6
-    646c665c:	add    $0x50,%rsp
-    646c6660:	pop    %rbx
-    646c6661:	ret
-    646c6662:	call   646c76e8 <_errno>
-    646c6667:	movq   %rbx,%xmm2
-    646c666c:	mov    $0x1,%ecx
-    646c6671:	pxor   %xmm3,%xmm3
-    646c6675:	movl   $0x21,(%rax)
-    646c667b:	lea    0x2c7e(%rip),%rdx        # 646c9300 <.rdata>
-    646c6682:	mov    %rbx,0x20(%rsp)
-    646c6687:	call   646c7960 <__mingw_raise_matherr>
-    646c668c:	movq   %rbx,%xmm0
-    646c6691:	jmp    646c65d3 <sqrt+0x63>
-    646c6696:	nop
-    646c6697:	nop
-    646c6698:	nop
-    646c6699:	nop
-    646c669a:	nop
-    646c669b:	nop
-    646c669c:	nop
-    646c669d:	nop
-    646c669e:	nop
-    646c669f:	nop
-
-00000000646c66a0 <__ms_vsnprintf>:
-    646c66a0:	jmp    646c76d0 <_vsnprintf>
-    646c66a5:	nop
-    646c66a6:	nop
-    646c66a7:	nop
-    646c66a8:	nop
-    646c66a9:	nop
-    646c66aa:	nop
-    646c66ab:	nop
-    646c66ac:	nop
-    646c66ad:	nop
-    646c66ae:	nop
-    646c66af:	nop
-
-00000000646c66b0 <ceil>:
-    646c66b0:	movq   %xmm0,%rax
-    646c66b5:	mov    %rax,%rcx
-    646c66b8:	sar    $0x34,%rcx
-    646c66bc:	and    $0x7ff,%ecx
-    646c66c2:	sub    $0x3ff,%ecx
-    646c66c8:	cmp    $0x33,%ecx
-    646c66cb:	jg     646c6770 <.is_intnaninf>
-    646c66d1:	test   %rax,%rax
-    646c66d4:	je     646c6780 <.ret_org>
-    646c66da:	test   %ecx,%ecx
-    646c66dc:	js     646c6730 <.signed_val>
-    646c66de:	movabs $0xfffffffffffff,%rdx
-    646c66e8:	sar    %cl,%rdx
-    646c66eb:	test   %rax,%rdx
-    646c66ee:	je     646c6780 <.ret_org>
-    646c66f4:	addsd  0x2c34(%rip),%xmm0        # 646c9330 <.huge>
-    646c66fc:	ucomisd 0x2c34(%rip),%xmm0        # 646c9338 <.zero>
-    646c6704:	jbe    646c6721 <.doret>
-    646c6706:	test   %rax,%rax
-    646c6709:	jle    646c671b <.l1>
-    646c670b:	movabs $0x10000000000000,%r8
-    646c6715:	shr    %cl,%r8
-    646c6718:	add    %r8,%rax
-
-00000000646c671b <.l1>:
-    646c671b:	not    %rdx
-    646c671e:	and    %rdx,%rax
-
-00000000646c6721 <.doret>:
-    646c6721:	movq   %rax,%xmm0
-    646c6726:	ret
-    646c6727:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6730 <.signed_val>:
-    646c6730:	addsd  0x2bf8(%rip),%xmm0        # 646c9330 <.huge>
-    646c6738:	ucomisd 0x2bf8(%rip),%xmm0        # 646c9338 <.zero>
-    646c6740:	jbe    646c6760 <.doret2>
-    646c6742:	test   %rax,%rax
-    646c6745:	movabs $0x3ff0000000000000,%rdx
-    646c674f:	movabs $0x8000000000000000,%rax
-    646c6759:	cmovns %rdx,%rax
-    646c675d:	nopl   (%rax)
-
-00000000646c6760 <.doret2>:
-    646c6760:	movq   %rax,%xmm0
-    646c6765:	ret
-    646c6766:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6770 <.is_intnaninf>:
-    646c6770:	cmp    $0x400,%ecx
-    646c6776:	je     646c6782 <.ret_naninf>
-    646c6778:	nopl   0x0(%rax,%rax,1)
-
-00000000646c6780 <.ret_org>:
-    646c6780:	repz ret
-
-00000000646c6782 <.ret_naninf>:
-    646c6782:	addsd  %xmm0,%xmm0
-    646c6786:	ret
-    646c6787:	nop
-    646c6788:	nop
-    646c6789:	nop
-    646c678a:	nop
-    646c678b:	nop
-    646c678c:	nop
-    646c678d:	nop
-    646c678e:	nop
-    646c678f:	nop
-
-00000000646c6790 <cos>:
-    646c6790:	push   %rbx
-    646c6791:	sub    $0x70,%rsp
-    646c6795:	movaps %xmm6,0x60(%rsp)
-    646c679a:	movq   %xmm0,%rax
-    646c679f:	movq   %xmm0,%rbx
-    646c67a4:	shr    $0x20,%rax
-    646c67a8:	mov    %eax,%edx
-    646c67aa:	and    $0x7ff00000,%eax
-    646c67af:	and    $0xfffff,%edx
-    646c67b5:	or     %ebx,%edx
-    646c67b7:	mov    %edx,%ecx
-    646c67b9:	or     %eax,%ecx
-    646c67bb:	sete   %r8b
-    646c67bf:	test   %eax,%eax
-    646c67c1:	sete   %cl
-    646c67c4:	or     %cl,%r8b
-    646c67c7:	jne    646c67d0 <cos+0x40>
-    646c67c9:	cmp    $0x7ff00000,%eax
-    646c67ce:	je     646c6805 <cos+0x75>
-    646c67d0:	mov    %rbx,0x30(%rsp)
-    646c67d5:	lea    0x50(%rsp),%rcx
-    646c67da:	fldl   0x30(%rsp)
-    646c67de:	fstpt  0x40(%rsp)
-    646c67e2:	lea    0x40(%rsp),%rdx
-    646c67e7:	call   646c6890 <__cosl_internal>
-    646c67ec:	fldt   0x50(%rsp)
-    646c67f0:	fstpl  0x38(%rsp)
-    646c67f4:	movsd  0x38(%rsp),%xmm0
-    646c67fa:	movaps 0x60(%rsp),%xmm6
-    646c67ff:	add    $0x70,%rsp
-    646c6803:	pop    %rbx
-    646c6804:	ret
-    646c6805:	test   %edx,%edx
-    646c6807:	jne    646c6850 <cos+0xc0>
-    646c6809:	call   646c76e8 <_errno>
-    646c680e:	movq   %rbx,%xmm2
-    646c6813:	mov    $0x1,%ecx
-    646c6818:	movsd  0x2b28(%rip),%xmm6        # 646c9348 <.rdata+0x8>
-    646c6820:	movl   $0x21,(%rax)
-    646c6826:	lea    0x2b13(%rip),%rdx        # 646c9340 <.rdata>
-    646c682d:	pxor   %xmm3,%xmm3
-    646c6831:	movsd  %xmm6,0x20(%rsp)
-    646c6837:	call   646c7960 <__mingw_raise_matherr>
-    646c683c:	movapd %xmm6,%xmm0
-    646c6840:	movaps 0x60(%rsp),%xmm6
-    646c6845:	add    $0x70,%rsp
-    646c6849:	pop    %rbx
-    646c684a:	ret
-    646c684b:	nopl   0x0(%rax,%rax,1)
-    646c6850:	call   646c76e8 <_errno>
-    646c6855:	movq   %rbx,%xmm2
-    646c685a:	mov    $0x1,%ecx
-    646c685f:	pxor   %xmm3,%xmm3
-    646c6863:	movl   $0x21,(%rax)
-    646c6869:	lea    0x2ad0(%rip),%rdx        # 646c9340 <.rdata>
-    646c6870:	mov    %rbx,0x20(%rsp)
-    646c6875:	call   646c7960 <__mingw_raise_matherr>
-    646c687a:	movq   %rbx,%xmm0
-    646c687f:	jmp    646c67fa <cos+0x6a>
-    646c6884:	nop
-    646c6885:	nop
-    646c6886:	nop
-    646c6887:	nop
-    646c6888:	nop
-    646c6889:	nop
-    646c688a:	nop
-    646c688b:	nop
-    646c688c:	nop
-    646c688d:	nop
-    646c688e:	nop
-    646c688f:	nop
-
-00000000646c6890 <__cosl_internal>:
-    646c6890:	fldt   (%rdx)
-    646c6892:	fcos
-    646c6894:	fnstsw %ax
-    646c6896:	test   $0x400,%eax
-    646c689b:	je     646c68b2 <__cosl_internal+0x22>
-    646c689d:	fldpi
-    646c689f:	fadd   %st(0),%st
-    646c68a1:	fxch   %st(1)
-    646c68a3:	fprem1
-    646c68a5:	fnstsw %ax
-    646c68a7:	test   $0x400,%eax
-    646c68ac:	jne    646c68a3 <__cosl_internal+0x13>
-    646c68ae:	fstp   %st(1)
-    646c68b0:	fcos
-    646c68b2:	mov    %rcx,%rax
-    646c68b5:	movq   $0x0,0x8(%rcx)
-    646c68bd:	fstpt  (%rcx)
-    646c68bf:	ret
-
-00000000646c68c0 <exp>:
-    646c68c0:	push   %rbx
-    646c68c1:	sub    $0x50,%rsp
-    646c68c5:	movaps %xmm6,0x40(%rsp)
-    646c68ca:	movsd  0x2a8e(%rip),%xmm6        # 646c9360 <.rdata+0x10>
-    646c68d2:	movq   %xmm0,%rdx
-    646c68d7:	movq   %xmm0,%rbx
-    646c68dc:	shr    $0x20,%rdx
-    646c68e0:	mov    %edx,%eax
-    646c68e2:	mov    %edx,%ecx
-    646c68e4:	and    $0xfffff,%eax
-    646c68e9:	and    $0x7ff00000,%ecx
-    646c68ef:	or     %ebx,%eax
-    646c68f1:	mov    %eax,%r8d
-    646c68f4:	or     %ecx,%r8d
-    646c68f7:	je     646c6929 <exp+0x69>
-    646c68f9:	cmp    $0x7ff00000,%ecx
-    646c68ff:	je     646c69c0 <exp+0x100>
-    646c6905:	ucomisd 0x2a5b(%rip),%xmm0        # 646c9368 <.rdata+0x18>
-    646c690d:	movapd %xmm0,%xmm1
-    646c6911:	ja     646c6a12 <exp+0x152>
-    646c6917:	movsd  0x2a51(%rip),%xmm0        # 646c9370 <.rdata+0x20>
-    646c691f:	pxor   %xmm6,%xmm6
-    646c6923:	ucomisd %xmm1,%xmm0
-    646c6927:	jbe    646c6940 <exp+0x80>
-    646c6929:	movapd %xmm6,%xmm0
-    646c692d:	movaps 0x40(%rsp),%xmm6
-    646c6932:	add    $0x50,%rsp
-    646c6936:	pop    %rbx
-    646c6937:	ret
-    646c6938:	nopl   0x0(%rax,%rax,1)
-    646c6940:	mov    %rbx,0x30(%rsp)
-    646c6945:	fldl   0x30(%rsp)
-    646c6949:	fldl2e
-    646c694b:	fmul   %st(1),%st
-    646c694d:	sub    $0x8,%rsp
-    646c6951:	fnstcw 0x4(%rsp)
-    646c6955:	movzwl 0x4(%rsp),%eax
-    646c695a:	or     $0xc,%ah
-    646c695d:	mov    %ax,(%rsp)
-    646c6961:	fldcw  (%rsp)
-    646c6964:	frndint
-    646c6966:	fld    %st(1)
-    646c6968:	frndint
-    646c696a:	fldcw  0x4(%rsp)
-    646c696e:	add    $0x8,%rsp
-    646c6972:	fld    %st(1)
-    646c6974:	fldt   0x16c6(%rip)        # 646c8040 <c0>
-    646c697a:	fld    %st(2)
-    646c697c:	fmul   %st(1),%st
-    646c697e:	fsubp  %st,%st(2)
-    646c6980:	fld    %st(4)
-    646c6982:	fsub   %st(3),%st
-    646c6984:	fmulp  %st,%st(1)
-    646c6986:	faddp  %st,%st(1)
-    646c6988:	fldt   0x16a2(%rip)        # 646c8030 <c1>
-    646c698e:	fmul   %st(4),%st
-    646c6990:	faddp  %st,%st(1)
-    646c6992:	f2xm1
-    646c6994:	fld1
-    646c6996:	faddp  %st,%st(1)
-    646c6998:	fstp   %st(1)
-    646c699a:	fscale
-    646c699c:	fstp   %st(1)
-    646c699e:	fstp   %st(1)
-    646c69a0:	fstpl  0x38(%rsp)
-    646c69a4:	movsd  0x38(%rsp),%xmm6
-    646c69aa:	movapd %xmm6,%xmm0
-    646c69ae:	movaps 0x40(%rsp),%xmm6
-    646c69b3:	add    $0x50,%rsp
-    646c69b7:	pop    %rbx
-    646c69b8:	ret
-    646c69b9:	nopl   0x0(%rax)
-    646c69c0:	test   %eax,%eax
-    646c69c2:	jne    646c6a70 <exp+0x1b0>
-    646c69c8:	test   %edx,%edx
-    646c69ca:	js     646c6a54 <exp+0x194>
-    646c69d0:	call   646c76e8 <_errno>
-    646c69d5:	movsd  0x297b(%rip),%xmm6        # 646c9358 <.rdata+0x8>
-    646c69dd:	mov    $0x4,%ecx
-    646c69e2:	movl   $0x22,(%rax)
-    646c69e8:	movsd  %xmm6,0x20(%rsp)
-    646c69ee:	movq   %rbx,%xmm2
-    646c69f3:	pxor   %xmm3,%xmm3
-    646c69f7:	lea    0x2952(%rip),%rdx        # 646c9350 <.rdata>
-    646c69fe:	call   646c7960 <__mingw_raise_matherr>
-    646c6a03:	movapd %xmm6,%xmm0
-    646c6a07:	movaps 0x40(%rsp),%xmm6
-    646c6a0c:	add    $0x50,%rsp
-    646c6a10:	pop    %rbx
-    646c6a11:	ret
-    646c6a12:	call   646c76e8 <_errno>
-    646c6a17:	movq   %rbx,%xmm2
-    646c6a1c:	mov    $0x3,%ecx
-    646c6a21:	movsd  0x292f(%rip),%xmm6        # 646c9358 <.rdata+0x8>
-    646c6a29:	movl   $0x22,(%rax)
-    646c6a2f:	lea    0x291a(%rip),%rdx        # 646c9350 <.rdata>
-    646c6a36:	pxor   %xmm3,%xmm3
-    646c6a3a:	movsd  %xmm6,0x20(%rsp)
-    646c6a40:	call   646c7960 <__mingw_raise_matherr>
-    646c6a45:	movapd %xmm6,%xmm0
-    646c6a49:	movaps 0x40(%rsp),%xmm6
-    646c6a4e:	add    $0x50,%rsp
-    646c6a52:	pop    %rbx
-    646c6a53:	ret
-    646c6a54:	call   646c76e8 <_errno>
-    646c6a59:	pxor   %xmm6,%xmm6
-    646c6a5d:	mov    $0x3,%ecx
-    646c6a62:	movl   $0x22,(%rax)
-    646c6a68:	jmp    646c69e8 <exp+0x128>
-    646c6a6d:	nopl   (%rax)
-    646c6a70:	call   646c76e8 <_errno>
-    646c6a75:	movq   %rbx,%xmm2
-    646c6a7a:	mov    $0x1,%ecx
-    646c6a7f:	pxor   %xmm3,%xmm3
-    646c6a83:	movl   $0x21,(%rax)
-    646c6a89:	lea    0x28c0(%rip),%rdx        # 646c9350 <.rdata>
-    646c6a90:	movq   %rbx,%xmm6
-    646c6a95:	mov    %rbx,0x20(%rsp)
-    646c6a9a:	call   646c7960 <__mingw_raise_matherr>
-    646c6a9f:	jmp    646c6929 <exp+0x69>
-    646c6aa4:	nop
-    646c6aa5:	nop
-    646c6aa6:	nop
-    646c6aa7:	nop
-    646c6aa8:	nop
-    646c6aa9:	nop
-    646c6aaa:	nop
-    646c6aab:	nop
-    646c6aac:	nop
-    646c6aad:	nop
-    646c6aae:	nop
-    646c6aaf:	nop
-
-00000000646c6ab0 <log>:
-    646c6ab0:	push   %rbx
-    646c6ab1:	sub    $0x70,%rsp
-    646c6ab5:	movaps %xmm6,0x60(%rsp)
-    646c6aba:	movq   %xmm0,%rdx
-    646c6abf:	movq   %xmm0,%rbx
-    646c6ac4:	shr    $0x20,%rdx
-    646c6ac8:	mov    %edx,%eax
-    646c6aca:	mov    %edx,%ecx
-    646c6acc:	and    $0xfffff,%eax
-    646c6ad1:	and    $0x7ff00000,%ecx
-    646c6ad7:	or     %ebx,%eax
-    646c6ad9:	mov    %eax,%r8d
-    646c6adc:	or     %ecx,%r8d
-    646c6adf:	je     646c6b40 <log+0x90>
-    646c6ae1:	test   %ecx,%ecx
-    646c6ae3:	jne    646c6b22 <log+0x72>
-    646c6ae5:	test   %edx,%edx
-    646c6ae7:	js     646c6b8e <log+0xde>
-    646c6aed:	mov    %rbx,0x30(%rsp)
-    646c6af2:	lea    0x50(%rsp),%rcx
-    646c6af7:	fldl   0x30(%rsp)
-    646c6afb:	fstpt  0x40(%rsp)
-    646c6aff:	lea    0x40(%rsp),%rdx
-    646c6b04:	call   646c74d0 <__logl_internal>
-    646c6b09:	fldt   0x50(%rsp)
-    646c6b0d:	fstpl  0x38(%rsp)
-    646c6b11:	movsd  0x38(%rsp),%xmm0
-    646c6b17:	movaps 0x60(%rsp),%xmm6
-    646c6b1c:	add    $0x70,%rsp
-    646c6b20:	pop    %rbx
-    646c6b21:	ret
-    646c6b22:	cmp    $0x7ff00000,%ecx
-    646c6b28:	jne    646c6ae5 <log+0x35>
-    646c6b2a:	test   %eax,%eax
-    646c6b2c:	je     646c6b82 <log+0xd2>
-    646c6b2e:	test   %edx,%edx
-    646c6b30:	js     646c6b8e <log+0xde>
-    646c6b32:	movsd  0x2856(%rip),%xmm0        # 646c9390 <.rdata+0x10>
-    646c6b3a:	jmp    646c6b17 <log+0x67>
-    646c6b3c:	nopl   0x0(%rax)
-    646c6b40:	call   646c76e8 <_errno>
-    646c6b45:	movq   %rbx,%xmm2
-    646c6b4a:	mov    $0x3,%ecx
-    646c6b4f:	movsd  0x2831(%rip),%xmm6        # 646c9388 <.rdata+0x8>
-    646c6b57:	movl   $0x22,(%rax)
-    646c6b5d:	lea    0x281c(%rip),%rdx        # 646c9380 <.rdata>
-    646c6b64:	pxor   %xmm3,%xmm3
-    646c6b68:	movsd  %xmm6,0x20(%rsp)
-    646c6b6e:	call   646c7960 <__mingw_raise_matherr>
-    646c6b73:	movapd %xmm6,%xmm0
-    646c6b77:	movaps 0x60(%rsp),%xmm6
-    646c6b7c:	add    $0x70,%rsp
-    646c6b80:	pop    %rbx
-    646c6b81:	ret
-    646c6b82:	test   %edx,%edx
-    646c6b84:	movsd  0x280c(%rip),%xmm0        # 646c9398 <.rdata+0x18>
-    646c6b8c:	jns    646c6b17 <log+0x67>
-    646c6b8e:	call   646c76e8 <_errno>
-    646c6b93:	movq   %rbx,%xmm2
-    646c6b98:	mov    $0x1,%ecx
-    646c6b9d:	movsd  0x27eb(%rip),%xmm6        # 646c9390 <.rdata+0x10>
-    646c6ba5:	movl   $0x21,(%rax)
-    646c6bab:	lea    0x27ce(%rip),%rdx        # 646c9380 <.rdata>
-    646c6bb2:	pxor   %xmm3,%xmm3
-    646c6bb6:	movsd  %xmm6,0x20(%rsp)
-    646c6bbc:	call   646c7960 <__mingw_raise_matherr>
-    646c6bc1:	movapd %xmm6,%xmm0
-    646c6bc5:	movaps 0x60(%rsp),%xmm6
-    646c6bca:	add    $0x70,%rsp
-    646c6bce:	pop    %rbx
-    646c6bcf:	ret
-
-00000000646c6bd0 <internal_modf>:
-    646c6bd0:	sub    $0x18,%rsp
-    646c6bd4:	movsd  %xmm0,0x8(%rsp)
-    646c6bda:	fldl   0x8(%rsp)
-    646c6bde:	push   %rax
-    646c6bdf:	sub    $0x8,%rsp
-    646c6be3:	fnstcw 0x4(%rsp)
-    646c6be7:	movzwl 0x4(%rsp),%eax
-    646c6bec:	or     $0xc,%ah
-    646c6bef:	mov    %ax,(%rsp)
-    646c6bf3:	fldcw  (%rsp)
-    646c6bf6:	frndint
-    646c6bf8:	fldcw  0x4(%rsp)
-    646c6bfc:	add    $0x8,%rsp
-    646c6c00:	pop    %rax
-    646c6c01:	movq   %xmm0,%rax
-    646c6c06:	fstpl  0x8(%rsp)
-    646c6c0a:	movsd  0x8(%rsp),%xmm1
-    646c6c10:	shr    $0x20,%rax
-    646c6c14:	mov    %eax,%ecx
-    646c6c16:	movsd  %xmm1,(%rdx)
-    646c6c1a:	movq   %xmm0,%rdx
-    646c6c1f:	and    $0x7ff00000,%eax
-    646c6c24:	and    $0xfffff,%ecx
-    646c6c2a:	or     %edx,%ecx
-    646c6c2c:	mov    %ecx,%edx
-    646c6c2e:	or     %eax,%edx
-    646c6c30:	sete   %dl
-    646c6c33:	test   %eax,%eax
-    646c6c35:	sete   %r8b
-    646c6c39:	or     %r8d,%edx
-    646c6c3c:	xor    $0x1,%edx
-    646c6c3f:	cmp    $0x7ff00000,%eax
-    646c6c44:	sete   %al
-    646c6c47:	test   %al,%dl
-    646c6c49:	je     646c6c4f <internal_modf+0x7f>
-    646c6c4b:	test   %ecx,%ecx
-    646c6c4d:	je     646c6c60 <internal_modf+0x90>
-    646c6c4f:	subsd  0x8(%rsp),%xmm0
-    646c6c55:	add    $0x18,%rsp
-    646c6c59:	ret
-    646c6c5a:	nopw   0x0(%rax,%rax,1)
-    646c6c60:	pxor   %xmm0,%xmm0
-    646c6c64:	jmp    646c6c55 <internal_modf+0x85>
-    646c6c66:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6c70 <pow>:
-    646c6c70:	push   %r12
-    646c6c72:	push   %rbp
-    646c6c73:	push   %rdi
-    646c6c74:	push   %rsi
-    646c6c75:	push   %rbx
-    646c6c76:	sub    $0x90,%rsp
-    646c6c7d:	movaps %xmm6,0x70(%rsp)
-    646c6c82:	movaps %xmm7,0x80(%rsp)
-    646c6c8a:	mov    $0x4000,%edx
-    646c6c8f:	movq   %xmm0,%rbx
-    646c6c94:	movq   %xmm0,%rdi
-    646c6c99:	movq   %xmm1,%rbp
-    646c6c9e:	shr    $0x20,%rbx
-    646c6ca2:	mov    %ebx,%eax
-    646c6ca4:	mov    %ebx,%ecx
-    646c6ca6:	and    $0xfffff,%eax
-    646c6cab:	and    $0x7ff00000,%ecx
-    646c6cb1:	or     %edi,%eax
-    646c6cb3:	mov    %ecx,%esi
-    646c6cb5:	or     %eax,%esi
-    646c6cb7:	je     646c6cc6 <pow+0x56>
-    646c6cb9:	test   %ecx,%ecx
-    646c6cbb:	mov    $0x4400,%edx
-    646c6cc0:	jne    646c6e11 <pow+0x1a1>
-    646c6cc6:	mov    %rbp,%rsi
-    646c6cc9:	movsd  0x26ff(%rip),%xmm6        # 646c93d0 <.rdata+0x30>
-    646c6cd1:	shr    $0x20,%rsi
-    646c6cd5:	mov    %esi,%eax
-    646c6cd7:	mov    %esi,%ecx
-    646c6cd9:	and    $0xfffff,%eax
-    646c6cde:	and    $0x7ff00000,%ecx
-    646c6ce4:	or     %ebp,%eax
-    646c6ce6:	mov    %ecx,%r9d
-    646c6ce9:	or     %eax,%r9d
-    646c6cec:	je     646c6d7b <pow+0x10b>
-    646c6cf2:	test   %ecx,%ecx
-    646c6cf4:	jne    646c6da0 <pow+0x130>
-    646c6cfa:	mov    $0x4400,%r8d
-    646c6d00:	movsd  0x26c8(%rip),%xmm2        # 646c93d0 <.rdata+0x30>
-    646c6d08:	movq   %rdi,%xmm4
-    646c6d0d:	ucomisd %xmm2,%xmm4
-    646c6d11:	jp     646c6d19 <pow+0xa9>
-    646c6d13:	je     646c7168 <pow+0x4f8>
-    646c6d19:	cmp    $0x100,%edx
-    646c6d1f:	je     646c6dd0 <pow+0x160>
-    646c6d25:	cmp    $0x4000,%edx
-    646c6d2b:	je     646c6e40 <pow+0x1d0>
-    646c6d31:	cmp    $0x500,%r8d
-    646c6d38:	je     646c6e90 <pow+0x220>
-    646c6d3e:	cmp    $0x500,%edx
-    646c6d44:	jne    646c6eb5 <pow+0x245>
-    646c6d4a:	test   %ebx,%ebx
-    646c6d4c:	js     646c7051 <pow+0x3e1>
-    646c6d52:	mov    $0xffffffff,%edx
-    646c6d57:	movq   %rbp,%xmm0
-    646c6d5c:	call   646c7520 <ldexp>
-    646c6d61:	lea    0x68(%rsp),%rdx
-    646c6d66:	call   646c6bd0 <internal_modf>
-    646c6d6b:	test   %esi,%esi
-    646c6d6d:	js     646c6e72 <pow+0x202>
-    646c6d73:	movsd  0x264d(%rip),%xmm6        # 646c93c8 <.rdata+0x28>
-    646c6d7b:	movapd %xmm6,%xmm0
-    646c6d7f:	movaps 0x80(%rsp),%xmm7
-    646c6d87:	movaps 0x70(%rsp),%xmm6
-    646c6d8c:	add    $0x90,%rsp
-    646c6d93:	pop    %rbx
-    646c6d94:	pop    %rsi
-    646c6d95:	pop    %rdi
-    646c6d96:	pop    %rbp
-    646c6d97:	pop    %r12
-    646c6d99:	ret
-    646c6d9a:	nopw   0x0(%rax,%rax,1)
-    646c6da0:	cmp    $0x7ff00000,%ecx
-    646c6da6:	mov    $0x400,%r8d
-    646c6dac:	jne    646c6d00 <pow+0x90>
-    646c6db2:	test   %eax,%eax
-    646c6db4:	mov    $0x500,%r8d
-    646c6dba:	je     646c6d00 <pow+0x90>
-    646c6dc0:	movq   %rdi,%xmm5
-    646c6dc5:	ucomisd %xmm6,%xmm5
-    646c6dc9:	jp     646c6dd0 <pow+0x160>
-    646c6dcb:	je     646c6d7b <pow+0x10b>
-    646c6dcd:	nopl   (%rax)
-    646c6dd0:	test   %ebx,%ebx
-    646c6dd2:	movsd  0x25d6(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
-    646c6dda:	js     646c6e80 <pow+0x210>
-    646c6de0:	call   646c76e8 <_errno>
-    646c6de5:	movl   $0x21,(%rax)
-    646c6deb:	movsd  %xmm6,0x20(%rsp)
-    646c6df1:	movq   %rbp,%xmm3
-    646c6df6:	movq   %rdi,%xmm2
-    646c6dfb:	mov    $0x1,%ecx
-    646c6e00:	lea    0x2599(%rip),%rdx        # 646c93a0 <.rdata>
-    646c6e07:	call   646c7960 <__mingw_raise_matherr>
-    646c6e0c:	jmp    646c6d7b <pow+0x10b>
-    646c6e11:	cmp    $0x7ff00000,%ecx
-    646c6e17:	mov    $0x400,%edx
-    646c6e1c:	jne    646c6cc6 <pow+0x56>
-    646c6e22:	cmp    $0x1,%eax
-    646c6e25:	sbb    %edx,%edx
-    646c6e27:	and    $0x400,%edx
-    646c6e2d:	add    $0x100,%edx
-    646c6e33:	jmp    646c6cc6 <pow+0x56>
-    646c6e38:	nopl   0x0(%rax,%rax,1)
-    646c6e40:	cmp    $0x500,%r8d
-    646c6e47:	je     646c6e6a <pow+0x1fa>
-    646c6e49:	test   %ebx,%ebx
-    646c6e4b:	js     646c7010 <pow+0x3a0>
-    646c6e51:	mov    $0xffffffff,%edx
-    646c6e56:	movq   %rbp,%xmm0
-    646c6e5b:	call   646c7520 <ldexp>
-    646c6e60:	lea    0x68(%rsp),%rdx
-    646c6e65:	call   646c6bd0 <internal_modf>
-    646c6e6a:	test   %esi,%esi
-    646c6e6c:	js     646c6d73 <pow+0x103>
-    646c6e72:	pxor   %xmm6,%xmm6
-    646c6e76:	jmp    646c6d7b <pow+0x10b>
-    646c6e7b:	nopl   0x0(%rax,%rax,1)
-    646c6e80:	movsd  0x2520(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
-    646c6e88:	jmp    646c6de0 <pow+0x170>
-    646c6e8d:	nopl   (%rax)
-    646c6e90:	cmp    $0x500,%edx
-    646c6e96:	je     646c6d6b <pow+0xfb>
-    646c6e9c:	test   %ebx,%ebx
-    646c6e9e:	js     646c7145 <pow+0x4d5>
-    646c6ea4:	movq   %rdi,%xmm5
-    646c6ea9:	ucomisd %xmm2,%xmm5
-    646c6ead:	ja     646c6d6b <pow+0xfb>
-    646c6eb3:	jmp    646c6e6a <pow+0x1fa>
-    646c6eb5:	lea    0x68(%rsp),%rsi
-    646c6eba:	movq   %rbp,%xmm0
-    646c6ebf:	pxor   %xmm7,%xmm7
-    646c6ec3:	mov    %rsi,%rdx
-    646c6ec6:	call   646c6bd0 <internal_modf>
-    646c6ecb:	ucomisd %xmm7,%xmm0
-    646c6ecf:	jp     646c6f91 <pow+0x321>
-    646c6ed5:	jne    646c6f91 <pow+0x321>
-    646c6edb:	movsd  0x68(%rsp),%xmm0
-    646c6ee1:	movsd  0x2517(%rip),%xmm1        # 646c9400 <.rdata+0x60>
-    646c6ee9:	ucomisd %xmm0,%xmm1
-    646c6eed:	jb     646c6efd <pow+0x28d>
-    646c6eef:	ucomisd 0x2511(%rip),%xmm0        # 646c9408 <.rdata+0x68>
-    646c6ef7:	jae    646c71a3 <pow+0x533>
-    646c6efd:	lea    0x50(%rsp),%r12
-    646c6f02:	movq   %rdi,%xmm5
-    646c6f07:	andpd  0x2501(%rip),%xmm5        # 646c9410 <.rdata+0x70>
-    646c6f0f:	movsd  %xmm5,0x30(%rsp)
-    646c6f15:	lea    0x40(%rsp),%rdi
-    646c6f1a:	fldl   0x30(%rsp)
-    646c6f1e:	mov    %r12,%rcx
-    646c6f21:	fstpt  0x40(%rsp)
-    646c6f25:	mov    %rdi,%rdx
-    646c6f28:	call   646c75f0 <log2l>
-    646c6f2d:	mov    %rdi,%rdx
-    646c6f30:	mov    %r12,%rcx
-    646c6f33:	fldt   0x50(%rsp)
-    646c6f37:	mov    %rbp,0x30(%rsp)
-    646c6f3c:	fldl   0x30(%rsp)
-    646c6f40:	fmulp  %st,%st(1)
-    646c6f42:	fstpt  0x40(%rsp)
-    646c6f46:	call   646c7450 <exp2l>
-    646c6f4b:	test   %ebx,%ebx
-    646c6f4d:	fldt   0x50(%rsp)
-    646c6f51:	fstpl  0x38(%rsp)
-    646c6f55:	movsd  0x38(%rsp),%xmm6
-    646c6f5b:	jns    646c6d7b <pow+0x10b>
-    646c6f61:	mov    $0xffffffff,%edx
-    646c6f66:	movq   %rbp,%xmm0
-    646c6f6b:	call   646c7520 <ldexp>
-    646c6f70:	mov    %rsi,%rdx
-    646c6f73:	call   646c6bd0 <internal_modf>
-    646c6f78:	ucomisd %xmm7,%xmm0
-    646c6f7c:	jp     646c6f84 <pow+0x314>
-    646c6f7e:	je     646c6d7b <pow+0x10b>
-    646c6f84:	xorpd  0x2454(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
-    646c6f8c:	jmp    646c6d7b <pow+0x10b>
-    646c6f91:	test   %ebx,%ebx
-    646c6f93:	js     646c718b <pow+0x51b>
-    646c6f99:	movq   %rbp,%xmm5
-    646c6f9e:	ucomisd 0x2452(%rip),%xmm5        # 646c93f8 <.rdata+0x58>
-    646c6fa6:	jp     646c6fae <pow+0x33e>
-    646c6fa8:	je     646c7171 <pow+0x501>
-    646c6fae:	lea    0x50(%rsp),%rbx
-    646c6fb3:	movq   %rdi,%xmm3
-    646c6fb8:	andpd  0x2450(%rip),%xmm3        # 646c9410 <.rdata+0x70>
-    646c6fc0:	movsd  %xmm3,0x30(%rsp)
-    646c6fc6:	lea    0x40(%rsp),%rsi
-    646c6fcb:	fldl   0x30(%rsp)
-    646c6fcf:	mov    %rbx,%rcx
+    646c6571:	ret
+    646c6572:	nop
+    646c6573:	nop
+    646c6574:	nop
+    646c6575:	nop
+    646c6576:	nop
+    646c6577:	nop
+    646c6578:	nop
+    646c6579:	nop
+    646c657a:	nop
+    646c657b:	nop
+    646c657c:	nop
+    646c657d:	nop
+    646c657e:	nop
+    646c657f:	nop
+
+00000000646c6580 <DllEntryPoint>:
+    646c6580:	mov    $0x1,%eax
+    646c6585:	ret
+    646c6586:	nop
+    646c6587:	nop
+    646c6588:	nop
+    646c6589:	nop
+    646c658a:	nop
+    646c658b:	nop
+    646c658c:	nop
+    646c658d:	nop
+    646c658e:	nop
+    646c658f:	nop
+
+00000000646c6590 <DllMain>:
+    646c6590:	mov    $0x1,%eax
+    646c6595:	ret
+    646c6596:	nop
+    646c6597:	nop
+    646c6598:	nop
+    646c6599:	nop
+    646c659a:	nop
+    646c659b:	nop
+    646c659c:	nop
+    646c659d:	nop
+    646c659e:	nop
+    646c659f:	nop
+
+00000000646c65a0 <__fpclassify>:
+    646c65a0:	movq   %xmm0,%rax
+    646c65a5:	movq   %xmm0,%rdx
+    646c65aa:	shr    $0x20,%rax
+    646c65ae:	mov    %eax,%ecx
+    646c65b0:	and    $0xfffff,%ecx
+    646c65b6:	or     %edx,%ecx
+    646c65b8:	mov    %eax,%edx
+    646c65ba:	mov    $0x4000,%eax
+    646c65bf:	and    $0x7ff00000,%edx
+    646c65c5:	mov    %ecx,%r8d
+    646c65c8:	or     %edx,%r8d
+    646c65cb:	je     646c65e3 <__fpclassify+0x43>
+    646c65cd:	test   %edx,%edx
+    646c65cf:	mov    $0x4400,%eax
+    646c65d4:	je     646c65e3 <__fpclassify+0x43>
+    646c65d6:	cmp    $0x7ff00000,%edx
+    646c65dc:	mov    $0x400,%eax
+    646c65e1:	je     646c65e4 <__fpclassify+0x44>
+    646c65e3:	ret
+    646c65e4:	cmp    $0x1,%ecx
+    646c65e7:	sbb    %eax,%eax
+    646c65e9:	and    $0x400,%eax
+    646c65ee:	add    $0x100,%eax
+    646c65f3:	ret
+    646c65f4:	nop
+    646c65f5:	nop
+    646c65f6:	nop
+    646c65f7:	nop
+    646c65f8:	nop
+    646c65f9:	nop
+    646c65fa:	nop
+    646c65fb:	nop
+    646c65fc:	nop
+    646c65fd:	nop
+    646c65fe:	nop
+    646c65ff:	nop
+
+00000000646c6600 <sqrt>:
+    646c6600:	push   %rbx
+    646c6601:	sub    $0x50,%rsp
+    646c6605:	movaps %xmm6,0x40(%rsp)
+    646c660a:	movq   %xmm0,%rdx
+    646c660f:	movq   %xmm0,%rbx
+    646c6614:	shr    $0x20,%rdx
+    646c6618:	mov    %edx,%eax
+    646c661a:	mov    %edx,%ecx
+    646c661c:	and    $0xfffff,%eax
+    646c6621:	and    $0x7ff00000,%ecx
+    646c6627:	or     %ebx,%eax
+    646c6629:	mov    %eax,%r8d
+    646c662c:	or     %ecx,%r8d
+    646c662f:	je     646c6670 <sqrt+0x70>
+    646c6631:	test   %ecx,%ecx
+    646c6633:	jne    646c6690 <sqrt+0x90>
+    646c6635:	test   %edx,%edx
+    646c6637:	js     646c66b0 <sqrt+0xb0>
+    646c6639:	movsd  0x2cdf(%rip),%xmm0        # 646c9320 <.rdata+0x20>
+    646c6641:	movq   %rbx,%xmm1
+    646c6646:	ucomisd %xmm0,%xmm1
+    646c664a:	jp     646c664e <sqrt+0x4e>
+    646c664c:	je     646c6663 <sqrt+0x63>
+    646c664e:	mov    %rbx,0x38(%rsp)
+    646c6653:	fldl   0x38(%rsp)
+    646c6657:	fsqrt
+    646c6659:	fstpl  0x38(%rsp)
+    646c665d:	movsd  0x38(%rsp),%xmm0
+    646c6663:	movaps 0x40(%rsp),%xmm6
+    646c6668:	add    $0x50,%rsp
+    646c666c:	pop    %rbx
+    646c666d:	ret
+    646c666e:	xchg   %ax,%ax
+    646c6670:	test   %edx,%edx
+    646c6672:	pxor   %xmm0,%xmm0
+    646c6676:	jns    646c6663 <sqrt+0x63>
+    646c6678:	movsd  0x2c88(%rip),%xmm0        # 646c9308 <.rdata+0x8>
+    646c6680:	movaps 0x40(%rsp),%xmm6
+    646c6685:	add    $0x50,%rsp
+    646c6689:	pop    %rbx
+    646c668a:	ret
+    646c668b:	nopl   0x0(%rax,%rax,1)
+    646c6690:	cmp    $0x7ff00000,%ecx
+    646c6696:	jne    646c6635 <sqrt+0x35>
+    646c6698:	test   %eax,%eax
+    646c669a:	jne    646c66f2 <sqrt+0xf2>
+    646c669c:	test   %edx,%edx
+    646c669e:	js     646c66b0 <sqrt+0xb0>
+    646c66a0:	movsd  0x2c70(%rip),%xmm0        # 646c9318 <.rdata+0x18>
+    646c66a8:	jmp    646c6663 <sqrt+0x63>
+    646c66aa:	nopw   0x0(%rax,%rax,1)
+    646c66b0:	call   646c7778 <_errno>
+    646c66b5:	movq   %rbx,%xmm2
+    646c66ba:	mov    $0x1,%ecx
+    646c66bf:	movsd  0x2c49(%rip),%xmm6        # 646c9310 <.rdata+0x10>
+    646c66c7:	movl   $0x21,(%rax)
+    646c66cd:	lea    0x2c2c(%rip),%rdx        # 646c9300 <.rdata>
+    646c66d4:	pxor   %xmm3,%xmm3
+    646c66d8:	movsd  %xmm6,0x20(%rsp)
+    646c66de:	call   646c79f0 <__mingw_raise_matherr>
+    646c66e3:	movapd %xmm6,%xmm0
+    646c66e7:	movaps 0x40(%rsp),%xmm6
+    646c66ec:	add    $0x50,%rsp
+    646c66f0:	pop    %rbx
+    646c66f1:	ret
+    646c66f2:	call   646c7778 <_errno>
+    646c66f7:	movq   %rbx,%xmm2
+    646c66fc:	mov    $0x1,%ecx
+    646c6701:	pxor   %xmm3,%xmm3
+    646c6705:	movl   $0x21,(%rax)
+    646c670b:	lea    0x2bee(%rip),%rdx        # 646c9300 <.rdata>
+    646c6712:	mov    %rbx,0x20(%rsp)
+    646c6717:	call   646c79f0 <__mingw_raise_matherr>
+    646c671c:	movq   %rbx,%xmm0
+    646c6721:	jmp    646c6663 <sqrt+0x63>
+    646c6726:	nop
+    646c6727:	nop
+    646c6728:	nop
+    646c6729:	nop
+    646c672a:	nop
+    646c672b:	nop
+    646c672c:	nop
+    646c672d:	nop
+    646c672e:	nop
+    646c672f:	nop
+
+00000000646c6730 <__ms_vsnprintf>:
+    646c6730:	jmp    646c7760 <_vsnprintf>
+    646c6735:	nop
+    646c6736:	nop
+    646c6737:	nop
+    646c6738:	nop
+    646c6739:	nop
+    646c673a:	nop
+    646c673b:	nop
+    646c673c:	nop
+    646c673d:	nop
+    646c673e:	nop
+    646c673f:	nop
+
+00000000646c6740 <ceil>:
+    646c6740:	movq   %xmm0,%rax
+    646c6745:	mov    %rax,%rcx
+    646c6748:	sar    $0x34,%rcx
+    646c674c:	and    $0x7ff,%ecx
+    646c6752:	sub    $0x3ff,%ecx
+    646c6758:	cmp    $0x33,%ecx
+    646c675b:	jg     646c6800 <.is_intnaninf>
+    646c6761:	test   %rax,%rax
+    646c6764:	je     646c6810 <.ret_org>
+    646c676a:	test   %ecx,%ecx
+    646c676c:	js     646c67c0 <.signed_val>
+    646c676e:	movabs $0xfffffffffffff,%rdx
+    646c6778:	sar    %cl,%rdx
+    646c677b:	test   %rax,%rdx
+    646c677e:	je     646c6810 <.ret_org>
+    646c6784:	addsd  0x2ba4(%rip),%xmm0        # 646c9330 <.huge>
+    646c678c:	ucomisd 0x2ba4(%rip),%xmm0        # 646c9338 <.zero>
+    646c6794:	jbe    646c67b1 <.doret>
+    646c6796:	test   %rax,%rax
+    646c6799:	jle    646c67ab <.l1>
+    646c679b:	movabs $0x10000000000000,%r8
+    646c67a5:	shr    %cl,%r8
+    646c67a8:	add    %r8,%rax
+
+00000000646c67ab <.l1>:
+    646c67ab:	not    %rdx
+    646c67ae:	and    %rdx,%rax
+
+00000000646c67b1 <.doret>:
+    646c67b1:	movq   %rax,%xmm0
+    646c67b6:	ret
+    646c67b7:	nopw   0x0(%rax,%rax,1)
+
+00000000646c67c0 <.signed_val>:
+    646c67c0:	addsd  0x2b68(%rip),%xmm0        # 646c9330 <.huge>
+    646c67c8:	ucomisd 0x2b68(%rip),%xmm0        # 646c9338 <.zero>
+    646c67d0:	jbe    646c67f0 <.doret2>
+    646c67d2:	test   %rax,%rax
+    646c67d5:	movabs $0x3ff0000000000000,%rdx
+    646c67df:	movabs $0x8000000000000000,%rax
+    646c67e9:	cmovns %rdx,%rax
+    646c67ed:	nopl   (%rax)
+
+00000000646c67f0 <.doret2>:
+    646c67f0:	movq   %rax,%xmm0
+    646c67f5:	ret
+    646c67f6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6800 <.is_intnaninf>:
+    646c6800:	cmp    $0x400,%ecx
+    646c6806:	je     646c6812 <.ret_naninf>
+    646c6808:	nopl   0x0(%rax,%rax,1)
+
+00000000646c6810 <.ret_org>:
+    646c6810:	repz ret
+
+00000000646c6812 <.ret_naninf>:
+    646c6812:	addsd  %xmm0,%xmm0
+    646c6816:	ret
+    646c6817:	nop
+    646c6818:	nop
+    646c6819:	nop
+    646c681a:	nop
+    646c681b:	nop
+    646c681c:	nop
+    646c681d:	nop
+    646c681e:	nop
+    646c681f:	nop
+
+00000000646c6820 <cos>:
+    646c6820:	push   %rbx
+    646c6821:	sub    $0x70,%rsp
+    646c6825:	movaps %xmm6,0x60(%rsp)
+    646c682a:	movq   %xmm0,%rax
+    646c682f:	movq   %xmm0,%rbx
+    646c6834:	shr    $0x20,%rax
+    646c6838:	mov    %eax,%edx
+    646c683a:	and    $0x7ff00000,%eax
+    646c683f:	and    $0xfffff,%edx
+    646c6845:	or     %ebx,%edx
+    646c6847:	mov    %edx,%ecx
+    646c6849:	or     %eax,%ecx
+    646c684b:	sete   %r8b
+    646c684f:	test   %eax,%eax
+    646c6851:	sete   %cl
+    646c6854:	or     %cl,%r8b
+    646c6857:	jne    646c6860 <cos+0x40>
+    646c6859:	cmp    $0x7ff00000,%eax
+    646c685e:	je     646c6895 <cos+0x75>
+    646c6860:	mov    %rbx,0x30(%rsp)
+    646c6865:	lea    0x50(%rsp),%rcx
+    646c686a:	fldl   0x30(%rsp)
+    646c686e:	fstpt  0x40(%rsp)
+    646c6872:	lea    0x40(%rsp),%rdx
+    646c6877:	call   646c6920 <__cosl_internal>
+    646c687c:	fldt   0x50(%rsp)
+    646c6880:	fstpl  0x38(%rsp)
+    646c6884:	movsd  0x38(%rsp),%xmm0
+    646c688a:	movaps 0x60(%rsp),%xmm6
+    646c688f:	add    $0x70,%rsp
+    646c6893:	pop    %rbx
+    646c6894:	ret
+    646c6895:	test   %edx,%edx
+    646c6897:	jne    646c68e0 <cos+0xc0>
+    646c6899:	call   646c7778 <_errno>
+    646c689e:	movq   %rbx,%xmm2
+    646c68a3:	mov    $0x1,%ecx
+    646c68a8:	movsd  0x2a98(%rip),%xmm6        # 646c9348 <.rdata+0x8>
+    646c68b0:	movl   $0x21,(%rax)
+    646c68b6:	lea    0x2a83(%rip),%rdx        # 646c9340 <.rdata>
+    646c68bd:	pxor   %xmm3,%xmm3
+    646c68c1:	movsd  %xmm6,0x20(%rsp)
+    646c68c7:	call   646c79f0 <__mingw_raise_matherr>
+    646c68cc:	movapd %xmm6,%xmm0
+    646c68d0:	movaps 0x60(%rsp),%xmm6
+    646c68d5:	add    $0x70,%rsp
+    646c68d9:	pop    %rbx
+    646c68da:	ret
+    646c68db:	nopl   0x0(%rax,%rax,1)
+    646c68e0:	call   646c7778 <_errno>
+    646c68e5:	movq   %rbx,%xmm2
+    646c68ea:	mov    $0x1,%ecx
+    646c68ef:	pxor   %xmm3,%xmm3
+    646c68f3:	movl   $0x21,(%rax)
+    646c68f9:	lea    0x2a40(%rip),%rdx        # 646c9340 <.rdata>
+    646c6900:	mov    %rbx,0x20(%rsp)
+    646c6905:	call   646c79f0 <__mingw_raise_matherr>
+    646c690a:	movq   %rbx,%xmm0
+    646c690f:	jmp    646c688a <cos+0x6a>
+    646c6914:	nop
+    646c6915:	nop
+    646c6916:	nop
+    646c6917:	nop
+    646c6918:	nop
+    646c6919:	nop
+    646c691a:	nop
+    646c691b:	nop
+    646c691c:	nop
+    646c691d:	nop
+    646c691e:	nop
+    646c691f:	nop
+
+00000000646c6920 <__cosl_internal>:
+    646c6920:	fldt   (%rdx)
+    646c6922:	fcos
+    646c6924:	fnstsw %ax
+    646c6926:	test   $0x400,%eax
+    646c692b:	je     646c6942 <__cosl_internal+0x22>
+    646c692d:	fldpi
+    646c692f:	fadd   %st(0),%st
+    646c6931:	fxch   %st(1)
+    646c6933:	fprem1
+    646c6935:	fnstsw %ax
+    646c6937:	test   $0x400,%eax
+    646c693c:	jne    646c6933 <__cosl_internal+0x13>
+    646c693e:	fstp   %st(1)
+    646c6940:	fcos
+    646c6942:	mov    %rcx,%rax
+    646c6945:	movq   $0x0,0x8(%rcx)
+    646c694d:	fstpt  (%rcx)
+    646c694f:	ret
+
+00000000646c6950 <exp>:
+    646c6950:	push   %rbx
+    646c6951:	sub    $0x50,%rsp
+    646c6955:	movaps %xmm6,0x40(%rsp)
+    646c695a:	movsd  0x29fe(%rip),%xmm6        # 646c9360 <.rdata+0x10>
+    646c6962:	movq   %xmm0,%rdx
+    646c6967:	movq   %xmm0,%rbx
+    646c696c:	shr    $0x20,%rdx
+    646c6970:	mov    %edx,%eax
+    646c6972:	mov    %edx,%ecx
+    646c6974:	and    $0xfffff,%eax
+    646c6979:	and    $0x7ff00000,%ecx
+    646c697f:	or     %ebx,%eax
+    646c6981:	mov    %eax,%r8d
+    646c6984:	or     %ecx,%r8d
+    646c6987:	je     646c69b9 <exp+0x69>
+    646c6989:	cmp    $0x7ff00000,%ecx
+    646c698f:	je     646c6a50 <exp+0x100>
+    646c6995:	ucomisd 0x29cb(%rip),%xmm0        # 646c9368 <.rdata+0x18>
+    646c699d:	movapd %xmm0,%xmm1
+    646c69a1:	ja     646c6aa2 <exp+0x152>
+    646c69a7:	movsd  0x29c1(%rip),%xmm0        # 646c9370 <.rdata+0x20>
+    646c69af:	pxor   %xmm6,%xmm6
+    646c69b3:	ucomisd %xmm1,%xmm0
+    646c69b7:	jbe    646c69d0 <exp+0x80>
+    646c69b9:	movapd %xmm6,%xmm0
+    646c69bd:	movaps 0x40(%rsp),%xmm6
+    646c69c2:	add    $0x50,%rsp
+    646c69c6:	pop    %rbx
+    646c69c7:	ret
+    646c69c8:	nopl   0x0(%rax,%rax,1)
+    646c69d0:	mov    %rbx,0x30(%rsp)
+    646c69d5:	fldl   0x30(%rsp)
+    646c69d9:	fldl2e
+    646c69db:	fmul   %st(1),%st
+    646c69dd:	sub    $0x8,%rsp
+    646c69e1:	fnstcw 0x4(%rsp)
+    646c69e5:	movzwl 0x4(%rsp),%eax
+    646c69ea:	or     $0xc,%ah
+    646c69ed:	mov    %ax,(%rsp)
+    646c69f1:	fldcw  (%rsp)
+    646c69f4:	frndint
+    646c69f6:	fld    %st(1)
+    646c69f8:	frndint
+    646c69fa:	fldcw  0x4(%rsp)
+    646c69fe:	add    $0x8,%rsp
+    646c6a02:	fld    %st(1)
+    646c6a04:	fldt   0x1636(%rip)        # 646c8040 <c0>
+    646c6a0a:	fld    %st(2)
+    646c6a0c:	fmul   %st(1),%st
+    646c6a0e:	fsubp  %st,%st(2)
+    646c6a10:	fld    %st(4)
+    646c6a12:	fsub   %st(3),%st
+    646c6a14:	fmulp  %st,%st(1)
+    646c6a16:	faddp  %st,%st(1)
+    646c6a18:	fldt   0x1612(%rip)        # 646c8030 <c1>
+    646c6a1e:	fmul   %st(4),%st
+    646c6a20:	faddp  %st,%st(1)
+    646c6a22:	f2xm1
+    646c6a24:	fld1
+    646c6a26:	faddp  %st,%st(1)
+    646c6a28:	fstp   %st(1)
+    646c6a2a:	fscale
+    646c6a2c:	fstp   %st(1)
+    646c6a2e:	fstp   %st(1)
+    646c6a30:	fstpl  0x38(%rsp)
+    646c6a34:	movsd  0x38(%rsp),%xmm6
+    646c6a3a:	movapd %xmm6,%xmm0
+    646c6a3e:	movaps 0x40(%rsp),%xmm6
+    646c6a43:	add    $0x50,%rsp
+    646c6a47:	pop    %rbx
+    646c6a48:	ret
+    646c6a49:	nopl   0x0(%rax)
+    646c6a50:	test   %eax,%eax
+    646c6a52:	jne    646c6b00 <exp+0x1b0>
+    646c6a58:	test   %edx,%edx
+    646c6a5a:	js     646c6ae4 <exp+0x194>
+    646c6a60:	call   646c7778 <_errno>
+    646c6a65:	movsd  0x28eb(%rip),%xmm6        # 646c9358 <.rdata+0x8>
+    646c6a6d:	mov    $0x4,%ecx
+    646c6a72:	movl   $0x22,(%rax)
+    646c6a78:	movsd  %xmm6,0x20(%rsp)
+    646c6a7e:	movq   %rbx,%xmm2
+    646c6a83:	pxor   %xmm3,%xmm3
+    646c6a87:	lea    0x28c2(%rip),%rdx        # 646c9350 <.rdata>
+    646c6a8e:	call   646c79f0 <__mingw_raise_matherr>
+    646c6a93:	movapd %xmm6,%xmm0
+    646c6a97:	movaps 0x40(%rsp),%xmm6
+    646c6a9c:	add    $0x50,%rsp
+    646c6aa0:	pop    %rbx
+    646c6aa1:	ret
+    646c6aa2:	call   646c7778 <_errno>
+    646c6aa7:	movq   %rbx,%xmm2
+    646c6aac:	mov    $0x3,%ecx
+    646c6ab1:	movsd  0x289f(%rip),%xmm6        # 646c9358 <.rdata+0x8>
+    646c6ab9:	movl   $0x22,(%rax)
+    646c6abf:	lea    0x288a(%rip),%rdx        # 646c9350 <.rdata>
+    646c6ac6:	pxor   %xmm3,%xmm3
+    646c6aca:	movsd  %xmm6,0x20(%rsp)
+    646c6ad0:	call   646c79f0 <__mingw_raise_matherr>
+    646c6ad5:	movapd %xmm6,%xmm0
+    646c6ad9:	movaps 0x40(%rsp),%xmm6
+    646c6ade:	add    $0x50,%rsp
+    646c6ae2:	pop    %rbx
+    646c6ae3:	ret
+    646c6ae4:	call   646c7778 <_errno>
+    646c6ae9:	pxor   %xmm6,%xmm6
+    646c6aed:	mov    $0x3,%ecx
+    646c6af2:	movl   $0x22,(%rax)
+    646c6af8:	jmp    646c6a78 <exp+0x128>
+    646c6afd:	nopl   (%rax)
+    646c6b00:	call   646c7778 <_errno>
+    646c6b05:	movq   %rbx,%xmm2
+    646c6b0a:	mov    $0x1,%ecx
+    646c6b0f:	pxor   %xmm3,%xmm3
+    646c6b13:	movl   $0x21,(%rax)
+    646c6b19:	lea    0x2830(%rip),%rdx        # 646c9350 <.rdata>
+    646c6b20:	movq   %rbx,%xmm6
+    646c6b25:	mov    %rbx,0x20(%rsp)
+    646c6b2a:	call   646c79f0 <__mingw_raise_matherr>
+    646c6b2f:	jmp    646c69b9 <exp+0x69>
+    646c6b34:	nop
+    646c6b35:	nop
+    646c6b36:	nop
+    646c6b37:	nop
+    646c6b38:	nop
+    646c6b39:	nop
+    646c6b3a:	nop
+    646c6b3b:	nop
+    646c6b3c:	nop
+    646c6b3d:	nop
+    646c6b3e:	nop
+    646c6b3f:	nop
+
+00000000646c6b40 <log>:
+    646c6b40:	push   %rbx
+    646c6b41:	sub    $0x70,%rsp
+    646c6b45:	movaps %xmm6,0x60(%rsp)
+    646c6b4a:	movq   %xmm0,%rdx
+    646c6b4f:	movq   %xmm0,%rbx
+    646c6b54:	shr    $0x20,%rdx
+    646c6b58:	mov    %edx,%eax
+    646c6b5a:	mov    %edx,%ecx
+    646c6b5c:	and    $0xfffff,%eax
+    646c6b61:	and    $0x7ff00000,%ecx
+    646c6b67:	or     %ebx,%eax
+    646c6b69:	mov    %eax,%r8d
+    646c6b6c:	or     %ecx,%r8d
+    646c6b6f:	je     646c6bd0 <log+0x90>
+    646c6b71:	test   %ecx,%ecx
+    646c6b73:	jne    646c6bb2 <log+0x72>
+    646c6b75:	test   %edx,%edx
+    646c6b77:	js     646c6c1e <log+0xde>
+    646c6b7d:	mov    %rbx,0x30(%rsp)
+    646c6b82:	lea    0x50(%rsp),%rcx
+    646c6b87:	fldl   0x30(%rsp)
+    646c6b8b:	fstpt  0x40(%rsp)
+    646c6b8f:	lea    0x40(%rsp),%rdx
+    646c6b94:	call   646c7560 <__logl_internal>
+    646c6b99:	fldt   0x50(%rsp)
+    646c6b9d:	fstpl  0x38(%rsp)
+    646c6ba1:	movsd  0x38(%rsp),%xmm0
+    646c6ba7:	movaps 0x60(%rsp),%xmm6
+    646c6bac:	add    $0x70,%rsp
+    646c6bb0:	pop    %rbx
+    646c6bb1:	ret
+    646c6bb2:	cmp    $0x7ff00000,%ecx
+    646c6bb8:	jne    646c6b75 <log+0x35>
+    646c6bba:	test   %eax,%eax
+    646c6bbc:	je     646c6c12 <log+0xd2>
+    646c6bbe:	test   %edx,%edx
+    646c6bc0:	js     646c6c1e <log+0xde>
+    646c6bc2:	movsd  0x27c6(%rip),%xmm0        # 646c9390 <.rdata+0x10>
+    646c6bca:	jmp    646c6ba7 <log+0x67>
+    646c6bcc:	nopl   0x0(%rax)
+    646c6bd0:	call   646c7778 <_errno>
+    646c6bd5:	movq   %rbx,%xmm2
+    646c6bda:	mov    $0x3,%ecx
+    646c6bdf:	movsd  0x27a1(%rip),%xmm6        # 646c9388 <.rdata+0x8>
+    646c6be7:	movl   $0x22,(%rax)
+    646c6bed:	lea    0x278c(%rip),%rdx        # 646c9380 <.rdata>
+    646c6bf4:	pxor   %xmm3,%xmm3
+    646c6bf8:	movsd  %xmm6,0x20(%rsp)
+    646c6bfe:	call   646c79f0 <__mingw_raise_matherr>
+    646c6c03:	movapd %xmm6,%xmm0
+    646c6c07:	movaps 0x60(%rsp),%xmm6
+    646c6c0c:	add    $0x70,%rsp
+    646c6c10:	pop    %rbx
+    646c6c11:	ret
+    646c6c12:	test   %edx,%edx
+    646c6c14:	movsd  0x277c(%rip),%xmm0        # 646c9398 <.rdata+0x18>
+    646c6c1c:	jns    646c6ba7 <log+0x67>
+    646c6c1e:	call   646c7778 <_errno>
+    646c6c23:	movq   %rbx,%xmm2
+    646c6c28:	mov    $0x1,%ecx
+    646c6c2d:	movsd  0x275b(%rip),%xmm6        # 646c9390 <.rdata+0x10>
+    646c6c35:	movl   $0x21,(%rax)
+    646c6c3b:	lea    0x273e(%rip),%rdx        # 646c9380 <.rdata>
+    646c6c42:	pxor   %xmm3,%xmm3
+    646c6c46:	movsd  %xmm6,0x20(%rsp)
+    646c6c4c:	call   646c79f0 <__mingw_raise_matherr>
+    646c6c51:	movapd %xmm6,%xmm0
+    646c6c55:	movaps 0x60(%rsp),%xmm6
+    646c6c5a:	add    $0x70,%rsp
+    646c6c5e:	pop    %rbx
+    646c6c5f:	ret
+
+00000000646c6c60 <internal_modf>:
+    646c6c60:	sub    $0x18,%rsp
+    646c6c64:	movsd  %xmm0,0x8(%rsp)
+    646c6c6a:	fldl   0x8(%rsp)
+    646c6c6e:	push   %rax
+    646c6c6f:	sub    $0x8,%rsp
+    646c6c73:	fnstcw 0x4(%rsp)
+    646c6c77:	movzwl 0x4(%rsp),%eax
+    646c6c7c:	or     $0xc,%ah
+    646c6c7f:	mov    %ax,(%rsp)
+    646c6c83:	fldcw  (%rsp)
+    646c6c86:	frndint
+    646c6c88:	fldcw  0x4(%rsp)
+    646c6c8c:	add    $0x8,%rsp
+    646c6c90:	pop    %rax
+    646c6c91:	movq   %xmm0,%rax
+    646c6c96:	fstpl  0x8(%rsp)
+    646c6c9a:	movsd  0x8(%rsp),%xmm1
+    646c6ca0:	shr    $0x20,%rax
+    646c6ca4:	mov    %eax,%ecx
+    646c6ca6:	movsd  %xmm1,(%rdx)
+    646c6caa:	movq   %xmm0,%rdx
+    646c6caf:	and    $0x7ff00000,%eax
+    646c6cb4:	and    $0xfffff,%ecx
+    646c6cba:	or     %edx,%ecx
+    646c6cbc:	mov    %ecx,%edx
+    646c6cbe:	or     %eax,%edx
+    646c6cc0:	sete   %dl
+    646c6cc3:	test   %eax,%eax
+    646c6cc5:	sete   %r8b
+    646c6cc9:	or     %r8d,%edx
+    646c6ccc:	xor    $0x1,%edx
+    646c6ccf:	cmp    $0x7ff00000,%eax
+    646c6cd4:	sete   %al
+    646c6cd7:	test   %al,%dl
+    646c6cd9:	je     646c6cdf <internal_modf+0x7f>
+    646c6cdb:	test   %ecx,%ecx
+    646c6cdd:	je     646c6cf0 <internal_modf+0x90>
+    646c6cdf:	subsd  0x8(%rsp),%xmm0
+    646c6ce5:	add    $0x18,%rsp
+    646c6ce9:	ret
+    646c6cea:	nopw   0x0(%rax,%rax,1)
+    646c6cf0:	pxor   %xmm0,%xmm0
+    646c6cf4:	jmp    646c6ce5 <internal_modf+0x85>
+    646c6cf6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6d00 <pow>:
+    646c6d00:	push   %r12
+    646c6d02:	push   %rbp
+    646c6d03:	push   %rdi
+    646c6d04:	push   %rsi
+    646c6d05:	push   %rbx
+    646c6d06:	sub    $0x90,%rsp
+    646c6d0d:	movaps %xmm6,0x70(%rsp)
+    646c6d12:	movaps %xmm7,0x80(%rsp)
+    646c6d1a:	mov    $0x4000,%edx
+    646c6d1f:	movq   %xmm0,%rbx
+    646c6d24:	movq   %xmm0,%rdi
+    646c6d29:	movq   %xmm1,%rbp
+    646c6d2e:	shr    $0x20,%rbx
+    646c6d32:	mov    %ebx,%eax
+    646c6d34:	mov    %ebx,%ecx
+    646c6d36:	and    $0xfffff,%eax
+    646c6d3b:	and    $0x7ff00000,%ecx
+    646c6d41:	or     %edi,%eax
+    646c6d43:	mov    %ecx,%esi
+    646c6d45:	or     %eax,%esi
+    646c6d47:	je     646c6d56 <pow+0x56>
+    646c6d49:	test   %ecx,%ecx
+    646c6d4b:	mov    $0x4400,%edx
+    646c6d50:	jne    646c6ea1 <pow+0x1a1>
+    646c6d56:	mov    %rbp,%rsi
+    646c6d59:	movsd  0x266f(%rip),%xmm6        # 646c93d0 <.rdata+0x30>
+    646c6d61:	shr    $0x20,%rsi
+    646c6d65:	mov    %esi,%eax
+    646c6d67:	mov    %esi,%ecx
+    646c6d69:	and    $0xfffff,%eax
+    646c6d6e:	and    $0x7ff00000,%ecx
+    646c6d74:	or     %ebp,%eax
+    646c6d76:	mov    %ecx,%r9d
+    646c6d79:	or     %eax,%r9d
+    646c6d7c:	je     646c6e0b <pow+0x10b>
+    646c6d82:	test   %ecx,%ecx
+    646c6d84:	jne    646c6e30 <pow+0x130>
+    646c6d8a:	mov    $0x4400,%r8d
+    646c6d90:	movsd  0x2638(%rip),%xmm2        # 646c93d0 <.rdata+0x30>
+    646c6d98:	movq   %rdi,%xmm4
+    646c6d9d:	ucomisd %xmm2,%xmm4
+    646c6da1:	jp     646c6da9 <pow+0xa9>
+    646c6da3:	je     646c71f8 <pow+0x4f8>
+    646c6da9:	cmp    $0x100,%edx
+    646c6daf:	je     646c6e60 <pow+0x160>
+    646c6db5:	cmp    $0x4000,%edx
+    646c6dbb:	je     646c6ed0 <pow+0x1d0>
+    646c6dc1:	cmp    $0x500,%r8d
+    646c6dc8:	je     646c6f20 <pow+0x220>
+    646c6dce:	cmp    $0x500,%edx
+    646c6dd4:	jne    646c6f45 <pow+0x245>
+    646c6dda:	test   %ebx,%ebx
+    646c6ddc:	js     646c70e1 <pow+0x3e1>
+    646c6de2:	mov    $0xffffffff,%edx
+    646c6de7:	movq   %rbp,%xmm0
+    646c6dec:	call   646c75b0 <ldexp>
+    646c6df1:	lea    0x68(%rsp),%rdx
+    646c6df6:	call   646c6c60 <internal_modf>
+    646c6dfb:	test   %esi,%esi
+    646c6dfd:	js     646c6f02 <pow+0x202>
+    646c6e03:	movsd  0x25bd(%rip),%xmm6        # 646c93c8 <.rdata+0x28>
+    646c6e0b:	movapd %xmm6,%xmm0
+    646c6e0f:	movaps 0x80(%rsp),%xmm7
+    646c6e17:	movaps 0x70(%rsp),%xmm6
+    646c6e1c:	add    $0x90,%rsp
+    646c6e23:	pop    %rbx
+    646c6e24:	pop    %rsi
+    646c6e25:	pop    %rdi
+    646c6e26:	pop    %rbp
+    646c6e27:	pop    %r12
+    646c6e29:	ret
+    646c6e2a:	nopw   0x0(%rax,%rax,1)
+    646c6e30:	cmp    $0x7ff00000,%ecx
+    646c6e36:	mov    $0x400,%r8d
+    646c6e3c:	jne    646c6d90 <pow+0x90>
+    646c6e42:	test   %eax,%eax
+    646c6e44:	mov    $0x500,%r8d
+    646c6e4a:	je     646c6d90 <pow+0x90>
+    646c6e50:	movq   %rdi,%xmm5
+    646c6e55:	ucomisd %xmm6,%xmm5
+    646c6e59:	jp     646c6e60 <pow+0x160>
+    646c6e5b:	je     646c6e0b <pow+0x10b>
+    646c6e5d:	nopl   (%rax)
+    646c6e60:	test   %ebx,%ebx
+    646c6e62:	movsd  0x2546(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
+    646c6e6a:	js     646c6f10 <pow+0x210>
+    646c6e70:	call   646c7778 <_errno>
+    646c6e75:	movl   $0x21,(%rax)
+    646c6e7b:	movsd  %xmm6,0x20(%rsp)
+    646c6e81:	movq   %rbp,%xmm3
+    646c6e86:	movq   %rdi,%xmm2
+    646c6e8b:	mov    $0x1,%ecx
+    646c6e90:	lea    0x2509(%rip),%rdx        # 646c93a0 <.rdata>
+    646c6e97:	call   646c79f0 <__mingw_raise_matherr>
+    646c6e9c:	jmp    646c6e0b <pow+0x10b>
+    646c6ea1:	cmp    $0x7ff00000,%ecx
+    646c6ea7:	mov    $0x400,%edx
+    646c6eac:	jne    646c6d56 <pow+0x56>
+    646c6eb2:	cmp    $0x1,%eax
+    646c6eb5:	sbb    %edx,%edx
+    646c6eb7:	and    $0x400,%edx
+    646c6ebd:	add    $0x100,%edx
+    646c6ec3:	jmp    646c6d56 <pow+0x56>
+    646c6ec8:	nopl   0x0(%rax,%rax,1)
+    646c6ed0:	cmp    $0x500,%r8d
+    646c6ed7:	je     646c6efa <pow+0x1fa>
+    646c6ed9:	test   %ebx,%ebx
+    646c6edb:	js     646c70a0 <pow+0x3a0>
+    646c6ee1:	mov    $0xffffffff,%edx
+    646c6ee6:	movq   %rbp,%xmm0
+    646c6eeb:	call   646c75b0 <ldexp>
+    646c6ef0:	lea    0x68(%rsp),%rdx
+    646c6ef5:	call   646c6c60 <internal_modf>
+    646c6efa:	test   %esi,%esi
+    646c6efc:	js     646c6e03 <pow+0x103>
+    646c6f02:	pxor   %xmm6,%xmm6
+    646c6f06:	jmp    646c6e0b <pow+0x10b>
+    646c6f0b:	nopl   0x0(%rax,%rax,1)
+    646c6f10:	movsd  0x2490(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
+    646c6f18:	jmp    646c6e70 <pow+0x170>
+    646c6f1d:	nopl   (%rax)
+    646c6f20:	cmp    $0x500,%edx
+    646c6f26:	je     646c6dfb <pow+0xfb>
+    646c6f2c:	test   %ebx,%ebx
+    646c6f2e:	js     646c71d5 <pow+0x4d5>
+    646c6f34:	movq   %rdi,%xmm5
+    646c6f39:	ucomisd %xmm2,%xmm5
+    646c6f3d:	ja     646c6dfb <pow+0xfb>
+    646c6f43:	jmp    646c6efa <pow+0x1fa>
+    646c6f45:	lea    0x68(%rsp),%rsi
+    646c6f4a:	movq   %rbp,%xmm0
+    646c6f4f:	pxor   %xmm7,%xmm7
+    646c6f53:	mov    %rsi,%rdx
+    646c6f56:	call   646c6c60 <internal_modf>
+    646c6f5b:	ucomisd %xmm7,%xmm0
+    646c6f5f:	jp     646c7021 <pow+0x321>
+    646c6f65:	jne    646c7021 <pow+0x321>
+    646c6f6b:	movsd  0x68(%rsp),%xmm0
+    646c6f71:	movsd  0x2487(%rip),%xmm1        # 646c9400 <.rdata+0x60>
+    646c6f79:	ucomisd %xmm0,%xmm1
+    646c6f7d:	jb     646c6f8d <pow+0x28d>
+    646c6f7f:	ucomisd 0x2481(%rip),%xmm0        # 646c9408 <.rdata+0x68>
+    646c6f87:	jae    646c7233 <pow+0x533>
+    646c6f8d:	lea    0x50(%rsp),%r12
+    646c6f92:	movq   %rdi,%xmm5
+    646c6f97:	andpd  0x2471(%rip),%xmm5        # 646c9410 <.rdata+0x70>
+    646c6f9f:	movsd  %xmm5,0x30(%rsp)
+    646c6fa5:	lea    0x40(%rsp),%rdi
+    646c6faa:	fldl   0x30(%rsp)
+    646c6fae:	mov    %r12,%rcx
+    646c6fb1:	fstpt  0x40(%rsp)
+    646c6fb5:	mov    %rdi,%rdx
+    646c6fb8:	call   646c7680 <log2l>
+    646c6fbd:	mov    %rdi,%rdx
+    646c6fc0:	mov    %r12,%rcx
+    646c6fc3:	fldt   0x50(%rsp)
+    646c6fc7:	mov    %rbp,0x30(%rsp)
+    646c6fcc:	fldl   0x30(%rsp)
+    646c6fd0:	fmulp  %st,%st(1)
     646c6fd2:	fstpt  0x40(%rsp)
-    646c6fd6:	mov    %rsi,%rdx
-    646c6fd9:	call   646c75f0 <log2l>
-    646c6fde:	mov    %rsi,%rdx
-    646c6fe1:	mov    %rbx,%rcx
-    646c6fe4:	fldt   0x50(%rsp)
-    646c6fe8:	mov    %rbp,0x30(%rsp)
-    646c6fed:	fldl   0x30(%rsp)
-    646c6ff1:	fmulp  %st,%st(1)
-    646c6ff3:	fstpt  0x40(%rsp)
-    646c6ff7:	call   646c7450 <exp2l>
-    646c6ffc:	fldt   0x50(%rsp)
-    646c7000:	fstpl  0x38(%rsp)
-    646c7004:	movsd  0x38(%rsp),%xmm6
-    646c700a:	jmp    646c6d7b <pow+0x10b>
-    646c700f:	nop
-    646c7010:	lea    0x68(%rsp),%rbx
-    646c7015:	movq   %rbp,%xmm0
-    646c701a:	pxor   %xmm7,%xmm7
-    646c701e:	mov    %rbx,%rdx
-    646c7021:	call   646c6bd0 <internal_modf>
-    646c7026:	ucomisd %xmm7,%xmm0
-    646c702a:	jp     646c7032 <pow+0x3c2>
-    646c702c:	je     646c7111 <pow+0x4a1>
-    646c7032:	test   %esi,%esi
-    646c7034:	jns    646c6e72 <pow+0x202>
-    646c703a:	btc    $0x3f,%rdi
-    646c703f:	movq   %rdi,%xmm5
-    646c7044:	divsd  %xmm5,%xmm2
-    646c7048:	movapd %xmm2,%xmm6
-    646c704c:	jmp    646c6d7b <pow+0x10b>
-    646c7051:	lea    0x68(%rsp),%rbx
-    646c7056:	movq   %rbp,%xmm0
-    646c705b:	pxor   %xmm7,%xmm7
-    646c705f:	mov    %rbx,%rdx
-    646c7062:	call   646c6bd0 <internal_modf>
-    646c7067:	ucomisd %xmm7,%xmm0
-    646c706b:	jp     646c706f <pow+0x3ff>
-    646c706d:	je     646c7091 <pow+0x421>
-    646c706f:	test   %esi,%esi
-    646c7071:	movq   %rdi,%xmm6
-    646c7076:	xorpd  0x2362(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
-    646c707e:	jns    646c6d7b <pow+0x10b>
-    646c7084:	divsd  %xmm6,%xmm2
-    646c7088:	movapd %xmm2,%xmm6
-    646c708c:	jmp    646c6d7b <pow+0x10b>
-    646c7091:	mov    $0xffffffff,%edx
-    646c7096:	movq   %rbp,%xmm0
-    646c709b:	call   646c7520 <ldexp>
-    646c70a0:	mov    %rbx,%rdx
-    646c70a3:	call   646c6bd0 <internal_modf>
-    646c70a8:	mov    $0x0,%edx
-    646c70ad:	ucomisd %xmm7,%xmm0
-    646c70b1:	setnp  %al
-    646c70b4:	cmovne %edx,%eax
-    646c70b7:	mov    %esi,%edx
-    646c70b9:	shr    $0x1f,%edx
-    646c70bc:	test   %dl,%dl
-    646c70be:	je     646c70c8 <pow+0x458>
-    646c70c0:	test   %al,%al
-    646c70c2:	jne    646c6e72 <pow+0x202>
-    646c70c8:	mov    %esi,%edx
-    646c70ca:	mov    $0x1,%r8d
-    646c70d0:	not    %edx
-    646c70d2:	shr    $0x1f,%edx
-    646c70d5:	ucomisd %xmm7,%xmm0
-    646c70d9:	setp   %cl
-    646c70dc:	cmovne %r8d,%ecx
-    646c70e0:	test   %cl,%cl
-    646c70e2:	je     646c70e8 <pow+0x478>
-    646c70e4:	test   %dl,%dl
-    646c70e6:	jne    646c7104 <pow+0x494>
-    646c70e8:	test   %al,%al
-    646c70ea:	je     646c70f4 <pow+0x484>
-    646c70ec:	test   %dl,%dl
-    646c70ee:	jne    646c6d73 <pow+0x103>
-    646c70f4:	test   %esi,%esi
-    646c70f6:	js     646c712c <pow+0x4bc>
-    646c70f8:	ucomisd %xmm7,%xmm0
-    646c70fc:	jp     646c7104 <pow+0x494>
-    646c70fe:	je     646c6d73 <pow+0x103>
-    646c7104:	movsd  0x22b4(%rip),%xmm6        # 646c93c0 <.rdata+0x20>
-    646c710c:	jmp    646c6d7b <pow+0x10b>
-    646c7111:	mov    $0xffffffff,%edx
-    646c7116:	movq   %rbp,%xmm0
-    646c711b:	call   646c7520 <ldexp>
-    646c7120:	mov    %rbx,%rdx
-    646c7123:	call   646c6bd0 <internal_modf>
-    646c7128:	test   %esi,%esi
-    646c712a:	js     646c70f8 <pow+0x488>
-    646c712c:	ucomisd %xmm7,%xmm0
-    646c7130:	jp     646c7138 <pow+0x4c8>
-    646c7132:	je     646c6e72 <pow+0x202>
-    646c7138:	movsd  0x2278(%rip),%xmm6        # 646c93b8 <.rdata+0x18>
-    646c7140:	jmp    646c6d7b <pow+0x10b>
-    646c7145:	movq   %rdi,%xmm5
-    646c714a:	xorpd  0x228e(%rip),%xmm5        # 646c93e0 <.rdata+0x40>
-    646c7152:	movq   %xmm5,%rax
-    646c7157:	movq   %rdi,%xmm5
-    646c715c:	ucomisd 0x228c(%rip),%xmm5        # 646c93f0 <.rdata+0x50>
-    646c7164:	jp     646c71bf <pow+0x54f>
-    646c7166:	jne    646c71bf <pow+0x54f>
-    646c7168:	movapd %xmm2,%xmm6
-    646c716c:	jmp    646c6d7b <pow+0x10b>
-    646c7171:	mov    %rdi,0x30(%rsp)
-    646c7176:	fldl   0x30(%rsp)
-    646c717a:	fsqrt
-    646c717c:	fstpl  0x30(%rsp)
-    646c7180:	movsd  0x30(%rsp),%xmm6
-    646c7186:	jmp    646c6d7b <pow+0x10b>
-    646c718b:	call   646c76e8 <_errno>
-    646c7190:	movsd  0x2210(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
-    646c7198:	movl   $0x21,(%rax)
-    646c719e:	jmp    646c6deb <pow+0x17b>
-    646c71a3:	movq   %rbp,%xmm3
-    646c71a8:	movq   %rdi,%xmm0
-    646c71ad:	cvttsd2si %xmm3,%edx
-    646c71b1:	call   646c71d0 <__powi>
-    646c71b6:	movapd %xmm0,%xmm6
-    646c71ba:	jmp    646c6d7b <pow+0x10b>
-    646c71bf:	mov    %rax,%rdi
-    646c71c2:	jmp    646c6ea4 <pow+0x234>
-    646c71c7:	nop
-    646c71c8:	nop
-    646c71c9:	nop
-    646c71ca:	nop
-    646c71cb:	nop
-    646c71cc:	nop
-    646c71cd:	nop
-    646c71ce:	nop
-    646c71cf:	nop
-
-00000000646c71d0 <__powi>:
-    646c71d0:	sub    $0x58,%rsp
-    646c71d4:	movaps %xmm6,0x40(%rsp)
-    646c71d9:	movsd  0x2257(%rip),%xmm1        # 646c9438 <.rdata+0x18>
-    646c71e1:	mov    $0x0,%r10d
-    646c71e7:	movq   %xmm0,%r8
-    646c71ec:	movq   %xmm0,%rax
-    646c71f1:	shr    $0x20,%r8
-    646c71f5:	mov    %r8d,%ecx
-    646c71f8:	mov    %r8d,%r9d
-    646c71fb:	and    $0xfffff,%ecx
-    646c7201:	and    $0x7ff00000,%r9d
-    646c7208:	or     %eax,%ecx
-    646c720a:	ucomisd %xmm1,%xmm0
-    646c720e:	mov    %r9d,%r11d
-    646c7211:	setnp  %al
-    646c7214:	cmovne %r10d,%eax
-    646c7218:	test   %edx,%edx
-    646c721a:	sete   %r10b
-    646c721e:	or     %r10d,%eax
-    646c7221:	or     %ecx,%r11d
-    646c7224:	jne    646c7260 <__powi+0x90>
-    646c7226:	test   %al,%al
-    646c7228:	movapd %xmm1,%xmm6
-    646c722c:	jne    646c7250 <__powi+0x80>
-    646c722e:	mov    %edx,%eax
-    646c7230:	and    $0x1,%eax
-    646c7233:	test   %edx,%edx
-    646c7235:	js     646c7325 <__powi+0x155>
-    646c723b:	test   %eax,%eax
-    646c723d:	pxor   %xmm6,%xmm6
-    646c7241:	je     646c7250 <__powi+0x80>
-    646c7243:	test   %r8d,%r8d
-    646c7246:	jns    646c7250 <__powi+0x80>
-    646c7248:	movsd  0x21f0(%rip),%xmm6        # 646c9440 <.rdata+0x20>
-    646c7250:	movapd %xmm6,%xmm0
-    646c7254:	movaps 0x40(%rsp),%xmm6
-    646c7259:	add    $0x58,%rsp
-    646c725d:	ret
-    646c725e:	xchg   %ax,%ax
-    646c7260:	test   %r9d,%r9d
-    646c7263:	jne    646c72d0 <__powi+0x100>
-    646c7265:	test   %al,%al
-    646c7267:	movapd %xmm1,%xmm6
-    646c726b:	jne    646c7250 <__powi+0x80>
-    646c726d:	mov    %edx,%eax
-    646c726f:	movapd %xmm0,%xmm6
-    646c7273:	andpd  0x21e5(%rip),%xmm6        # 646c9460 <.rdata+0x40>
-    646c727b:	and    $0x1,%eax
-    646c727e:	test   %edx,%edx
-    646c7280:	js     646c7312 <__powi+0x142>
-    646c7286:	cmp    $0x1,%edx
-    646c7289:	je     646c72b1 <__powi+0xe1>
-    646c728b:	test   $0x1,%dl
-    646c728e:	jne    646c73c0 <__powi+0x1f0>
-    646c7294:	movapd %xmm6,%xmm0
-    646c7298:	shr    %edx
-    646c729a:	movapd %xmm1,%xmm6
-    646c729e:	xchg   %ax,%ax
-    646c72a0:	mulsd  %xmm0,%xmm0
-    646c72a4:	test   $0x1,%dl
-    646c72a7:	je     646c72ad <__powi+0xdd>
-    646c72a9:	mulsd  %xmm0,%xmm6
-    646c72ad:	shr    %edx
-    646c72af:	jne    646c72a0 <__powi+0xd0>
-    646c72b1:	shr    $0x1f,%r8d
-    646c72b5:	test   %r8b,%r8b
-    646c72b8:	je     646c7250 <__powi+0x80>
-    646c72ba:	test   %eax,%eax
-    646c72bc:	je     646c7250 <__powi+0x80>
-    646c72be:	xorpd  0x21aa(%rip),%xmm6        # 646c9470 <.rdata+0x50>
-    646c72c6:	jmp    646c7250 <__powi+0x80>
-    646c72c8:	nopl   0x0(%rax,%rax,1)
-    646c72d0:	cmp    $0x7ff00000,%r9d
-    646c72d7:	jne    646c7265 <__powi+0x95>
-    646c72d9:	test   %ecx,%ecx
-    646c72db:	jne    646c7350 <__powi+0x180>
-    646c72dd:	mov    %edx,%r9d
-    646c72e0:	movapd %xmm1,%xmm6
-    646c72e4:	and    $0x1,%r9d
-    646c72e8:	test   %al,%al
-    646c72ea:	jne    646c7250 <__powi+0x80>
-    646c72f0:	test   %r8d,%r8d
-    646c72f3:	js     646c73e0 <__powi+0x210>
-    646c72f9:	test   %edx,%edx
-    646c72fb:	movsd  0x2145(%rip),%xmm6        # 646c9448 <.rdata+0x28>
-    646c7303:	jns    646c7250 <__powi+0x80>
-    646c7309:	pxor   %xmm6,%xmm6
-    646c730d:	jmp    646c7250 <__powi+0x80>
-    646c7312:	movapd %xmm1,%xmm4
-    646c7316:	neg    %edx
-    646c7318:	divsd  %xmm6,%xmm4
-    646c731c:	movapd %xmm4,%xmm6
-    646c7320:	jmp    646c7286 <__powi+0xb6>
-    646c7325:	test   %eax,%eax
-    646c7327:	movsd  0x2119(%rip),%xmm6        # 646c9448 <.rdata+0x28>
-    646c732f:	je     646c7250 <__powi+0x80>
-    646c7335:	test   %r8d,%r8d
-    646c7338:	jns    646c7250 <__powi+0x80>
-    646c733e:	movsd  0x210a(%rip),%xmm6        # 646c9450 <.rdata+0x30>
-    646c7346:	jmp    646c7250 <__powi+0x80>
-    646c734b:	nopl   0x0(%rax,%rax,1)
-    646c7350:	test   %al,%al
-    646c7352:	movapd %xmm1,%xmm6
-    646c7356:	jne    646c7250 <__powi+0x80>
-    646c735c:	test   %r8d,%r8d
-    646c735f:	movsd  0x20c9(%rip),%xmm6        # 646c9430 <.rdata+0x10>
-    646c7367:	js     646c73d0 <__powi+0x200>
-    646c7369:	mov    %edx,0x3c(%rsp)
-    646c736d:	movsd  %xmm0,0x30(%rsp)
-    646c7373:	call   646c76e8 <_errno>
-    646c7378:	mov    0x3c(%rsp),%edx
-    646c737c:	pxor   %xmm3,%xmm3
-    646c7380:	mov    $0x1,%ecx
-    646c7385:	movsd  0x30(%rsp),%xmm0
-    646c738b:	movl   $0x21,(%rax)
-    646c7391:	movsd  %xmm6,0x20(%rsp)
-    646c7397:	movapd %xmm0,%xmm2
-    646c739b:	cvtsi2sd %edx,%xmm3
-    646c739f:	lea    0x207a(%rip),%rdx        # 646c9420 <.rdata>
-    646c73a6:	call   646c7960 <__mingw_raise_matherr>
-    646c73ab:	movapd %xmm6,%xmm0
-    646c73af:	movaps 0x40(%rsp),%xmm6
-    646c73b4:	add    $0x58,%rsp
-    646c73b8:	ret
-    646c73b9:	nopl   0x0(%rax)
-    646c73c0:	movapd %xmm6,%xmm1
-    646c73c4:	jmp    646c7294 <__powi+0xc4>
-    646c73c9:	nopl   0x0(%rax)
-    646c73d0:	movsd  0x2050(%rip),%xmm6        # 646c9428 <.rdata+0x8>
-    646c73d8:	jmp    646c7369 <__powi+0x199>
-    646c73da:	nopw   0x0(%rax,%rax,1)
-    646c73e0:	mov    %edx,%eax
-    646c73e2:	not    %eax
-    646c73e4:	mov    %eax,%ecx
-    646c73e6:	and    $0x1,%ecx
-    646c73e9:	test   %edx,%edx
-    646c73eb:	jns    646c73f9 <__powi+0x229>
-    646c73ed:	test   %cl,%cl
-    646c73ef:	pxor   %xmm6,%xmm6
-    646c73f3:	jne    646c7250 <__powi+0x80>
-    646c73f9:	shr    $0x1f,%eax
-    646c73fc:	test   $0x1,%dl
-    646c73ff:	je     646c7411 <__powi+0x241>
-    646c7401:	test   %al,%al
-    646c7403:	movsd  0x2045(%rip),%xmm6        # 646c9450 <.rdata+0x30>
-    646c740b:	jne    646c7250 <__powi+0x80>
-    646c7411:	test   %cl,%cl
-    646c7413:	je     646c7425 <__powi+0x255>
-    646c7415:	test   %al,%al
-    646c7417:	movsd  0x2029(%rip),%xmm6        # 646c9448 <.rdata+0x28>
-    646c741f:	jne    646c7250 <__powi+0x80>
-    646c7425:	test   %edx,%edx
-    646c7427:	js     646c7440 <__powi+0x270>
-    646c7429:	and    $0x1,%dl
-    646c742c:	jne    646c733e <__powi+0x16e>
-    646c7432:	movsd  0x200e(%rip),%xmm6        # 646c9448 <.rdata+0x28>
-    646c743a:	jmp    646c7250 <__powi+0x80>
-    646c743f:	nop
-    646c7440:	test   %r9d,%r9d
-    646c7443:	jne    646c7248 <__powi+0x78>
-    646c7449:	jmp    646c7309 <__powi+0x139>
-    646c744e:	nop
-    646c744f:	nop
-
-00000000646c7450 <exp2l>:
-    646c7450:	fldt   (%rdx)
-    646c7452:	fxam
-    646c7454:	fstsw  %ax
-    646c7457:	mov    $0x45,%dh
-    646c7459:	and    %ah,%dh
-    646c745b:	cmp    $0x5,%dh
-    646c745e:	je     646c749f <exp2l+0x4f>
-    646c7460:	fld    %st(0)
-    646c7462:	sub    $0x8,%rsp
-    646c7466:	fnstcw 0x4(%rsp)
-    646c746a:	movzwl 0x4(%rsp),%eax
-    646c746f:	or     $0xc,%ah
-    646c7472:	mov    %ax,(%rsp)
-    646c7476:	fldcw  (%rsp)
-    646c7479:	frndint
-    646c747b:	fldcw  0x4(%rsp)
-    646c747f:	add    $0x8,%rsp
-    646c7483:	fsubr  %st,%st(1)
-    646c7485:	fxch   %st(1)
-    646c7487:	f2xm1
-    646c7489:	fld1
-    646c748b:	faddp  %st,%st(1)
-    646c748d:	fscale
-    646c748f:	fstp   %st(1)
-    646c7491:	mov    %rcx,%rax
-    646c7494:	movq   $0x0,0x8(%rcx)
-    646c749c:	fstpt  (%rcx)
-    646c749e:	ret
-    646c749f:	test   $0x200,%eax
-    646c74a4:	je     646c74aa <exp2l+0x5a>
-    646c74a6:	fstp   %st(0)
-    646c74a8:	fldz
-    646c74aa:	mov    %rcx,%rax
-    646c74ad:	movq   $0x0,0x8(%rcx)
-    646c74b5:	fstpt  (%rcx)
-    646c74b7:	ret
-    646c74b8:	nop
-    646c74b9:	nop
-    646c74ba:	nop
-    646c74bb:	nop
-    646c74bc:	nop
-    646c74bd:	nop
-    646c74be:	nop
-    646c74bf:	nop
-
-00000000646c74c0 <one>:
-    646c74c0:	add    %al,(%rax)
-    646c74c2:	add    %al,(%rax)
-    646c74c4:	add    %al,(%rax)
-    646c74c6:	lock (bad)
-
-00000000646c74c8 <limit>:
-    646c74c8:	pop    %rdx
-    646c74ca:	cmc
-    646c74cb:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c74cf:	(bad)
-
-00000000646c74d0 <__logl_internal>:
-    646c74d0:	fldln2
-    646c74d2:	fldt   (%rdx)
-    646c74d4:	fld    %st(0)
-    646c74d6:	fsubl  -0x1c(%rip)        # 646c74c0 <one>
-    646c74dc:	fld    %st(0)
-    646c74de:	fabs
-    646c74e0:	fcompl -0x1e(%rip)        # 646c74c8 <limit>
-    646c74e6:	fnstsw %ax
-    646c74e8:	and    $0x45,%ah
-    646c74eb:	je     646c74ff <__logl_internal+0x2f>
-    646c74ed:	fstp   %st(1)
-    646c74ef:	fyl2xp1
-    646c74f1:	mov    %rcx,%rax
-    646c74f4:	movq   $0x0,0x8(%rcx)
-    646c74fc:	fstpt  (%rcx)
-    646c74fe:	ret
-    646c74ff:	fstp   %st(0)
-    646c7501:	fyl2x
-    646c7503:	mov    %rcx,%rax
-    646c7506:	movq   $0x0,0x8(%rcx)
-    646c750e:	fstpt  (%rcx)
-    646c7510:	ret
-    646c7511:	nop
-    646c7512:	nop
-    646c7513:	nop
-    646c7514:	nop
-    646c7515:	nop
-    646c7516:	nop
-    646c7517:	nop
-    646c7518:	nop
-    646c7519:	nop
-    646c751a:	nop
-    646c751b:	nop
-    646c751c:	nop
-    646c751d:	nop
-    646c751e:	nop
-    646c751f:	nop
-
-00000000646c7520 <ldexp>:
-    646c7520:	push   %rbx
-    646c7521:	sub    $0x30,%rsp
-    646c7525:	movq   %xmm0,%rax
-    646c752a:	movq   %xmm0,%rbx
-    646c752f:	shr    $0x20,%rax
-    646c7533:	mov    %eax,%r8d
-    646c7536:	and    $0x7fffffff,%r8d
-    646c753d:	or     %ebx,%r8d
-    646c7540:	sete   %r8b
-    646c7544:	and    $0x7ff00000,%eax
-    646c7549:	sete   %cl
-    646c754c:	or     %cl,%r8b
-    646c754f:	jne    646c7558 <ldexp+0x38>
-    646c7551:	cmp    $0x7ff00000,%eax
-    646c7556:	je     646c75d3 <ldexp+0xb3>
-    646c7558:	movq   %rbx,%xmm1
-    646c755d:	pxor   %xmm0,%xmm0
-    646c7561:	ucomisd %xmm0,%xmm1
-    646c7565:	jp     646c7569 <ldexp+0x49>
-    646c7567:	je     646c75d3 <ldexp+0xb3>
-    646c7569:	pxor   %xmm2,%xmm2
-    646c756d:	cvtsi2sd %edx,%xmm2
-    646c7571:	mov    %rbx,0x20(%rsp)
-    646c7576:	fldl   0x20(%rsp)
-    646c757a:	movsd  %xmm2,0x28(%rsp)
-    646c7580:	fldl   0x28(%rsp)
-    646c7584:	fxch   %st(1)
-    646c7586:	fscale
-    646c7588:	fstp   %st(1)
-    646c758a:	fstpl  0x20(%rsp)
-    646c758e:	mov    0x20(%rsp),%rbx
-    646c7593:	mov    %rbx,%rax
-    646c7596:	shr    $0x20,%rax
-    646c759a:	mov    %eax,%ecx
-    646c759c:	and    $0x7fffffff,%ecx
-    646c75a2:	or     %ebx,%ecx
-    646c75a4:	sete   %cl
-    646c75a7:	and    $0x7ff00000,%eax
-    646c75ac:	sete   %dl
-    646c75af:	or     %dl,%cl
-    646c75b1:	jne    646c75ba <ldexp+0x9a>
-    646c75b3:	cmp    $0x7ff00000,%eax
-    646c75b8:	je     646c75c8 <ldexp+0xa8>
-    646c75ba:	movsd  0x20(%rsp),%xmm3
-    646c75c0:	ucomisd %xmm0,%xmm3
-    646c75c4:	jp     646c75d3 <ldexp+0xb3>
-    646c75c6:	jne    646c75d3 <ldexp+0xb3>
-    646c75c8:	call   646c76e8 <_errno>
-    646c75cd:	movl   $0x22,(%rax)
-    646c75d3:	movq   %rbx,%xmm0
-    646c75d8:	add    $0x30,%rsp
-    646c75dc:	pop    %rbx
-    646c75dd:	ret
-    646c75de:	nop
-    646c75df:	nop
-
-00000000646c75e0 <one>:
-    646c75e0:	add    %al,(%rax)
-    646c75e2:	add    %al,(%rax)
-    646c75e4:	add    %al,(%rax)
-    646c75e6:	lock (bad)
-
-00000000646c75e8 <limit>:
-    646c75e8:	pop    %rdx
-    646c75ea:	cmc
-    646c75eb:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c75ef:	(bad)
-
-00000000646c75f0 <log2l>:
-    646c75f0:	fldl   -0x16(%rip)        # 646c75e0 <one>
-    646c75f6:	fldt   (%rdx)
-    646c75f8:	fxam
-    646c75fa:	fnstsw %ax
-    646c75fc:	fld    %st(0)
-    646c75fe:	sahf
-    646c75ff:	jb     646c7638 <log2l+0x48>
-    646c7601:	fsub   %st(2),%st
-    646c7603:	fld    %st(0)
-    646c7605:	fabs
-    646c7607:	fcompl -0x25(%rip)        # 646c75e8 <limit>
-    646c760d:	fnstsw %ax
-    646c760f:	and    $0x45,%ah
-    646c7612:	je     646c7626 <log2l+0x36>
-    646c7614:	fstp   %st(1)
-    646c7616:	fyl2xp1
-    646c7618:	mov    %rcx,%rax
-    646c761b:	movq   $0x0,0x8(%rcx)
-    646c7623:	fstpt  (%rcx)
-    646c7625:	ret
-    646c7626:	fstp   %st(0)
-    646c7628:	fyl2x
-    646c762a:	mov    %rcx,%rax
-    646c762d:	movq   $0x0,0x8(%rcx)
-    646c7635:	fstpt  (%rcx)
-    646c7637:	ret
-    646c7638:	jp     646c7601 <log2l+0x11>
-    646c763a:	fstp   %st(1)
-    646c763c:	fstp   %st(1)
-    646c763e:	mov    %rcx,%rax
-    646c7641:	movq   $0x0,0x8(%rcx)
-    646c7649:	fstpt  (%rcx)
-    646c764b:	ret
-    646c764c:	nop
-    646c764d:	nop
-    646c764e:	nop
-    646c764f:	nop
-
-00000000646c7650 <vfprintf>:
-    646c7650:	jmp    *0x6cf6(%rip)        # 646ce34c <__imp_vfprintf>
-    646c7656:	nop
-    646c7657:	nop
-
-00000000646c7658 <strncmp>:
-    646c7658:	jmp    *0x6ce6(%rip)        # 646ce344 <__imp_strncmp>
-    646c765e:	nop
-    646c765f:	nop
-
-00000000646c7660 <strlen>:
-    646c7660:	jmp    *0x6cd6(%rip)        # 646ce33c <__imp_strlen>
-    646c7666:	nop
-    646c7667:	nop
-
-00000000646c7668 <signal>:
-    646c7668:	jmp    *0x6cc6(%rip)        # 646ce334 <__imp_signal>
+    646c6fd6:	call   646c74e0 <exp2l>
+    646c6fdb:	test   %ebx,%ebx
+    646c6fdd:	fldt   0x50(%rsp)
+    646c6fe1:	fstpl  0x38(%rsp)
+    646c6fe5:	movsd  0x38(%rsp),%xmm6
+    646c6feb:	jns    646c6e0b <pow+0x10b>
+    646c6ff1:	mov    $0xffffffff,%edx
+    646c6ff6:	movq   %rbp,%xmm0
+    646c6ffb:	call   646c75b0 <ldexp>
+    646c7000:	mov    %rsi,%rdx
+    646c7003:	call   646c6c60 <internal_modf>
+    646c7008:	ucomisd %xmm7,%xmm0
+    646c700c:	jp     646c7014 <pow+0x314>
+    646c700e:	je     646c6e0b <pow+0x10b>
+    646c7014:	xorpd  0x23c4(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
+    646c701c:	jmp    646c6e0b <pow+0x10b>
+    646c7021:	test   %ebx,%ebx
+    646c7023:	js     646c721b <pow+0x51b>
+    646c7029:	movq   %rbp,%xmm5
+    646c702e:	ucomisd 0x23c2(%rip),%xmm5        # 646c93f8 <.rdata+0x58>
+    646c7036:	jp     646c703e <pow+0x33e>
+    646c7038:	je     646c7201 <pow+0x501>
+    646c703e:	lea    0x50(%rsp),%rbx
+    646c7043:	movq   %rdi,%xmm3
+    646c7048:	andpd  0x23c0(%rip),%xmm3        # 646c9410 <.rdata+0x70>
+    646c7050:	movsd  %xmm3,0x30(%rsp)
+    646c7056:	lea    0x40(%rsp),%rsi
+    646c705b:	fldl   0x30(%rsp)
+    646c705f:	mov    %rbx,%rcx
+    646c7062:	fstpt  0x40(%rsp)
+    646c7066:	mov    %rsi,%rdx
+    646c7069:	call   646c7680 <log2l>
+    646c706e:	mov    %rsi,%rdx
+    646c7071:	mov    %rbx,%rcx
+    646c7074:	fldt   0x50(%rsp)
+    646c7078:	mov    %rbp,0x30(%rsp)
+    646c707d:	fldl   0x30(%rsp)
+    646c7081:	fmulp  %st,%st(1)
+    646c7083:	fstpt  0x40(%rsp)
+    646c7087:	call   646c74e0 <exp2l>
+    646c708c:	fldt   0x50(%rsp)
+    646c7090:	fstpl  0x38(%rsp)
+    646c7094:	movsd  0x38(%rsp),%xmm6
+    646c709a:	jmp    646c6e0b <pow+0x10b>
+    646c709f:	nop
+    646c70a0:	lea    0x68(%rsp),%rbx
+    646c70a5:	movq   %rbp,%xmm0
+    646c70aa:	pxor   %xmm7,%xmm7
+    646c70ae:	mov    %rbx,%rdx
+    646c70b1:	call   646c6c60 <internal_modf>
+    646c70b6:	ucomisd %xmm7,%xmm0
+    646c70ba:	jp     646c70c2 <pow+0x3c2>
+    646c70bc:	je     646c71a1 <pow+0x4a1>
+    646c70c2:	test   %esi,%esi
+    646c70c4:	jns    646c6f02 <pow+0x202>
+    646c70ca:	btc    $0x3f,%rdi
+    646c70cf:	movq   %rdi,%xmm5
+    646c70d4:	divsd  %xmm5,%xmm2
+    646c70d8:	movapd %xmm2,%xmm6
+    646c70dc:	jmp    646c6e0b <pow+0x10b>
+    646c70e1:	lea    0x68(%rsp),%rbx
+    646c70e6:	movq   %rbp,%xmm0
+    646c70eb:	pxor   %xmm7,%xmm7
+    646c70ef:	mov    %rbx,%rdx
+    646c70f2:	call   646c6c60 <internal_modf>
+    646c70f7:	ucomisd %xmm7,%xmm0
+    646c70fb:	jp     646c70ff <pow+0x3ff>
+    646c70fd:	je     646c7121 <pow+0x421>
+    646c70ff:	test   %esi,%esi
+    646c7101:	movq   %rdi,%xmm6
+    646c7106:	xorpd  0x22d2(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
+    646c710e:	jns    646c6e0b <pow+0x10b>
+    646c7114:	divsd  %xmm6,%xmm2
+    646c7118:	movapd %xmm2,%xmm6
+    646c711c:	jmp    646c6e0b <pow+0x10b>
+    646c7121:	mov    $0xffffffff,%edx
+    646c7126:	movq   %rbp,%xmm0
+    646c712b:	call   646c75b0 <ldexp>
+    646c7130:	mov    %rbx,%rdx
+    646c7133:	call   646c6c60 <internal_modf>
+    646c7138:	mov    $0x0,%edx
+    646c713d:	ucomisd %xmm7,%xmm0
+    646c7141:	setnp  %al
+    646c7144:	cmovne %edx,%eax
+    646c7147:	mov    %esi,%edx
+    646c7149:	shr    $0x1f,%edx
+    646c714c:	test   %dl,%dl
+    646c714e:	je     646c7158 <pow+0x458>
+    646c7150:	test   %al,%al
+    646c7152:	jne    646c6f02 <pow+0x202>
+    646c7158:	mov    %esi,%edx
+    646c715a:	mov    $0x1,%r8d
+    646c7160:	not    %edx
+    646c7162:	shr    $0x1f,%edx
+    646c7165:	ucomisd %xmm7,%xmm0
+    646c7169:	setp   %cl
+    646c716c:	cmovne %r8d,%ecx
+    646c7170:	test   %cl,%cl
+    646c7172:	je     646c7178 <pow+0x478>
+    646c7174:	test   %dl,%dl
+    646c7176:	jne    646c7194 <pow+0x494>
+    646c7178:	test   %al,%al
+    646c717a:	je     646c7184 <pow+0x484>
+    646c717c:	test   %dl,%dl
+    646c717e:	jne    646c6e03 <pow+0x103>
+    646c7184:	test   %esi,%esi
+    646c7186:	js     646c71bc <pow+0x4bc>
+    646c7188:	ucomisd %xmm7,%xmm0
+    646c718c:	jp     646c7194 <pow+0x494>
+    646c718e:	je     646c6e03 <pow+0x103>
+    646c7194:	movsd  0x2224(%rip),%xmm6        # 646c93c0 <.rdata+0x20>
+    646c719c:	jmp    646c6e0b <pow+0x10b>
+    646c71a1:	mov    $0xffffffff,%edx
+    646c71a6:	movq   %rbp,%xmm0
+    646c71ab:	call   646c75b0 <ldexp>
+    646c71b0:	mov    %rbx,%rdx
+    646c71b3:	call   646c6c60 <internal_modf>
+    646c71b8:	test   %esi,%esi
+    646c71ba:	js     646c7188 <pow+0x488>
+    646c71bc:	ucomisd %xmm7,%xmm0
+    646c71c0:	jp     646c71c8 <pow+0x4c8>
+    646c71c2:	je     646c6f02 <pow+0x202>
+    646c71c8:	movsd  0x21e8(%rip),%xmm6        # 646c93b8 <.rdata+0x18>
+    646c71d0:	jmp    646c6e0b <pow+0x10b>
+    646c71d5:	movq   %rdi,%xmm5
+    646c71da:	xorpd  0x21fe(%rip),%xmm5        # 646c93e0 <.rdata+0x40>
+    646c71e2:	movq   %xmm5,%rax
+    646c71e7:	movq   %rdi,%xmm5
+    646c71ec:	ucomisd 0x21fc(%rip),%xmm5        # 646c93f0 <.rdata+0x50>
+    646c71f4:	jp     646c724f <pow+0x54f>
+    646c71f6:	jne    646c724f <pow+0x54f>
+    646c71f8:	movapd %xmm2,%xmm6
+    646c71fc:	jmp    646c6e0b <pow+0x10b>
+    646c7201:	mov    %rdi,0x30(%rsp)
+    646c7206:	fldl   0x30(%rsp)
+    646c720a:	fsqrt
+    646c720c:	fstpl  0x30(%rsp)
+    646c7210:	movsd  0x30(%rsp),%xmm6
+    646c7216:	jmp    646c6e0b <pow+0x10b>
+    646c721b:	call   646c7778 <_errno>
+    646c7220:	movsd  0x2180(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
+    646c7228:	movl   $0x21,(%rax)
+    646c722e:	jmp    646c6e7b <pow+0x17b>
+    646c7233:	movq   %rbp,%xmm3
+    646c7238:	movq   %rdi,%xmm0
+    646c723d:	cvttsd2si %xmm3,%edx
+    646c7241:	call   646c7260 <__powi>
+    646c7246:	movapd %xmm0,%xmm6
+    646c724a:	jmp    646c6e0b <pow+0x10b>
+    646c724f:	mov    %rax,%rdi
+    646c7252:	jmp    646c6f34 <pow+0x234>
+    646c7257:	nop
+    646c7258:	nop
+    646c7259:	nop
+    646c725a:	nop
+    646c725b:	nop
+    646c725c:	nop
+    646c725d:	nop
+    646c725e:	nop
+    646c725f:	nop
+
+00000000646c7260 <__powi>:
+    646c7260:	sub    $0x58,%rsp
+    646c7264:	movaps %xmm6,0x40(%rsp)
+    646c7269:	movsd  0x21c7(%rip),%xmm1        # 646c9438 <.rdata+0x18>
+    646c7271:	mov    $0x0,%r10d
+    646c7277:	movq   %xmm0,%r8
+    646c727c:	movq   %xmm0,%rax
+    646c7281:	shr    $0x20,%r8
+    646c7285:	mov    %r8d,%ecx
+    646c7288:	mov    %r8d,%r9d
+    646c728b:	and    $0xfffff,%ecx
+    646c7291:	and    $0x7ff00000,%r9d
+    646c7298:	or     %eax,%ecx
+    646c729a:	ucomisd %xmm1,%xmm0
+    646c729e:	mov    %r9d,%r11d
+    646c72a1:	setnp  %al
+    646c72a4:	cmovne %r10d,%eax
+    646c72a8:	test   %edx,%edx
+    646c72aa:	sete   %r10b
+    646c72ae:	or     %r10d,%eax
+    646c72b1:	or     %ecx,%r11d
+    646c72b4:	jne    646c72f0 <__powi+0x90>
+    646c72b6:	test   %al,%al
+    646c72b8:	movapd %xmm1,%xmm6
+    646c72bc:	jne    646c72e0 <__powi+0x80>
+    646c72be:	mov    %edx,%eax
+    646c72c0:	and    $0x1,%eax
+    646c72c3:	test   %edx,%edx
+    646c72c5:	js     646c73b5 <__powi+0x155>
+    646c72cb:	test   %eax,%eax
+    646c72cd:	pxor   %xmm6,%xmm6
+    646c72d1:	je     646c72e0 <__powi+0x80>
+    646c72d3:	test   %r8d,%r8d
+    646c72d6:	jns    646c72e0 <__powi+0x80>
+    646c72d8:	movsd  0x2160(%rip),%xmm6        # 646c9440 <.rdata+0x20>
+    646c72e0:	movapd %xmm6,%xmm0
+    646c72e4:	movaps 0x40(%rsp),%xmm6
+    646c72e9:	add    $0x58,%rsp
+    646c72ed:	ret
+    646c72ee:	xchg   %ax,%ax
+    646c72f0:	test   %r9d,%r9d
+    646c72f3:	jne    646c7360 <__powi+0x100>
+    646c72f5:	test   %al,%al
+    646c72f7:	movapd %xmm1,%xmm6
+    646c72fb:	jne    646c72e0 <__powi+0x80>
+    646c72fd:	mov    %edx,%eax
+    646c72ff:	movapd %xmm0,%xmm6
+    646c7303:	andpd  0x2155(%rip),%xmm6        # 646c9460 <.rdata+0x40>
+    646c730b:	and    $0x1,%eax
+    646c730e:	test   %edx,%edx
+    646c7310:	js     646c73a2 <__powi+0x142>
+    646c7316:	cmp    $0x1,%edx
+    646c7319:	je     646c7341 <__powi+0xe1>
+    646c731b:	test   $0x1,%dl
+    646c731e:	jne    646c7450 <__powi+0x1f0>
+    646c7324:	movapd %xmm6,%xmm0
+    646c7328:	shr    %edx
+    646c732a:	movapd %xmm1,%xmm6
+    646c732e:	xchg   %ax,%ax
+    646c7330:	mulsd  %xmm0,%xmm0
+    646c7334:	test   $0x1,%dl
+    646c7337:	je     646c733d <__powi+0xdd>
+    646c7339:	mulsd  %xmm0,%xmm6
+    646c733d:	shr    %edx
+    646c733f:	jne    646c7330 <__powi+0xd0>
+    646c7341:	shr    $0x1f,%r8d
+    646c7345:	test   %r8b,%r8b
+    646c7348:	je     646c72e0 <__powi+0x80>
+    646c734a:	test   %eax,%eax
+    646c734c:	je     646c72e0 <__powi+0x80>
+    646c734e:	xorpd  0x211a(%rip),%xmm6        # 646c9470 <.rdata+0x50>
+    646c7356:	jmp    646c72e0 <__powi+0x80>
+    646c7358:	nopl   0x0(%rax,%rax,1)
+    646c7360:	cmp    $0x7ff00000,%r9d
+    646c7367:	jne    646c72f5 <__powi+0x95>
+    646c7369:	test   %ecx,%ecx
+    646c736b:	jne    646c73e0 <__powi+0x180>
+    646c736d:	mov    %edx,%r9d
+    646c7370:	movapd %xmm1,%xmm6
+    646c7374:	and    $0x1,%r9d
+    646c7378:	test   %al,%al
+    646c737a:	jne    646c72e0 <__powi+0x80>
+    646c7380:	test   %r8d,%r8d
+    646c7383:	js     646c7470 <__powi+0x210>
+    646c7389:	test   %edx,%edx
+    646c738b:	movsd  0x20b5(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c7393:	jns    646c72e0 <__powi+0x80>
+    646c7399:	pxor   %xmm6,%xmm6
+    646c739d:	jmp    646c72e0 <__powi+0x80>
+    646c73a2:	movapd %xmm1,%xmm4
+    646c73a6:	neg    %edx
+    646c73a8:	divsd  %xmm6,%xmm4
+    646c73ac:	movapd %xmm4,%xmm6
+    646c73b0:	jmp    646c7316 <__powi+0xb6>
+    646c73b5:	test   %eax,%eax
+    646c73b7:	movsd  0x2089(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c73bf:	je     646c72e0 <__powi+0x80>
+    646c73c5:	test   %r8d,%r8d
+    646c73c8:	jns    646c72e0 <__powi+0x80>
+    646c73ce:	movsd  0x207a(%rip),%xmm6        # 646c9450 <.rdata+0x30>
+    646c73d6:	jmp    646c72e0 <__powi+0x80>
+    646c73db:	nopl   0x0(%rax,%rax,1)
+    646c73e0:	test   %al,%al
+    646c73e2:	movapd %xmm1,%xmm6
+    646c73e6:	jne    646c72e0 <__powi+0x80>
+    646c73ec:	test   %r8d,%r8d
+    646c73ef:	movsd  0x2039(%rip),%xmm6        # 646c9430 <.rdata+0x10>
+    646c73f7:	js     646c7460 <__powi+0x200>
+    646c73f9:	mov    %edx,0x3c(%rsp)
+    646c73fd:	movsd  %xmm0,0x30(%rsp)
+    646c7403:	call   646c7778 <_errno>
+    646c7408:	mov    0x3c(%rsp),%edx
+    646c740c:	pxor   %xmm3,%xmm3
+    646c7410:	mov    $0x1,%ecx
+    646c7415:	movsd  0x30(%rsp),%xmm0
+    646c741b:	movl   $0x21,(%rax)
+    646c7421:	movsd  %xmm6,0x20(%rsp)
+    646c7427:	movapd %xmm0,%xmm2
+    646c742b:	cvtsi2sd %edx,%xmm3
+    646c742f:	lea    0x1fea(%rip),%rdx        # 646c9420 <.rdata>
+    646c7436:	call   646c79f0 <__mingw_raise_matherr>
+    646c743b:	movapd %xmm6,%xmm0
+    646c743f:	movaps 0x40(%rsp),%xmm6
+    646c7444:	add    $0x58,%rsp
+    646c7448:	ret
+    646c7449:	nopl   0x0(%rax)
+    646c7450:	movapd %xmm6,%xmm1
+    646c7454:	jmp    646c7324 <__powi+0xc4>
+    646c7459:	nopl   0x0(%rax)
+    646c7460:	movsd  0x1fc0(%rip),%xmm6        # 646c9428 <.rdata+0x8>
+    646c7468:	jmp    646c73f9 <__powi+0x199>
+    646c746a:	nopw   0x0(%rax,%rax,1)
+    646c7470:	mov    %edx,%eax
+    646c7472:	not    %eax
+    646c7474:	mov    %eax,%ecx
+    646c7476:	and    $0x1,%ecx
+    646c7479:	test   %edx,%edx
+    646c747b:	jns    646c7489 <__powi+0x229>
+    646c747d:	test   %cl,%cl
+    646c747f:	pxor   %xmm6,%xmm6
+    646c7483:	jne    646c72e0 <__powi+0x80>
+    646c7489:	shr    $0x1f,%eax
+    646c748c:	test   $0x1,%dl
+    646c748f:	je     646c74a1 <__powi+0x241>
+    646c7491:	test   %al,%al
+    646c7493:	movsd  0x1fb5(%rip),%xmm6        # 646c9450 <.rdata+0x30>
+    646c749b:	jne    646c72e0 <__powi+0x80>
+    646c74a1:	test   %cl,%cl
+    646c74a3:	je     646c74b5 <__powi+0x255>
+    646c74a5:	test   %al,%al
+    646c74a7:	movsd  0x1f99(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c74af:	jne    646c72e0 <__powi+0x80>
+    646c74b5:	test   %edx,%edx
+    646c74b7:	js     646c74d0 <__powi+0x270>
+    646c74b9:	and    $0x1,%dl
+    646c74bc:	jne    646c73ce <__powi+0x16e>
+    646c74c2:	movsd  0x1f7e(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c74ca:	jmp    646c72e0 <__powi+0x80>
+    646c74cf:	nop
+    646c74d0:	test   %r9d,%r9d
+    646c74d3:	jne    646c72d8 <__powi+0x78>
+    646c74d9:	jmp    646c7399 <__powi+0x139>
+    646c74de:	nop
+    646c74df:	nop
+
+00000000646c74e0 <exp2l>:
+    646c74e0:	fldt   (%rdx)
+    646c74e2:	fxam
+    646c74e4:	fstsw  %ax
+    646c74e7:	mov    $0x45,%dh
+    646c74e9:	and    %ah,%dh
+    646c74eb:	cmp    $0x5,%dh
+    646c74ee:	je     646c752f <exp2l+0x4f>
+    646c74f0:	fld    %st(0)
+    646c74f2:	sub    $0x8,%rsp
+    646c74f6:	fnstcw 0x4(%rsp)
+    646c74fa:	movzwl 0x4(%rsp),%eax
+    646c74ff:	or     $0xc,%ah
+    646c7502:	mov    %ax,(%rsp)
+    646c7506:	fldcw  (%rsp)
+    646c7509:	frndint
+    646c750b:	fldcw  0x4(%rsp)
+    646c750f:	add    $0x8,%rsp
+    646c7513:	fsubr  %st,%st(1)
+    646c7515:	fxch   %st(1)
+    646c7517:	f2xm1
+    646c7519:	fld1
+    646c751b:	faddp  %st,%st(1)
+    646c751d:	fscale
+    646c751f:	fstp   %st(1)
+    646c7521:	mov    %rcx,%rax
+    646c7524:	movq   $0x0,0x8(%rcx)
+    646c752c:	fstpt  (%rcx)
+    646c752e:	ret
+    646c752f:	test   $0x200,%eax
+    646c7534:	je     646c753a <exp2l+0x5a>
+    646c7536:	fstp   %st(0)
+    646c7538:	fldz
+    646c753a:	mov    %rcx,%rax
+    646c753d:	movq   $0x0,0x8(%rcx)
+    646c7545:	fstpt  (%rcx)
+    646c7547:	ret
+    646c7548:	nop
+    646c7549:	nop
+    646c754a:	nop
+    646c754b:	nop
+    646c754c:	nop
+    646c754d:	nop
+    646c754e:	nop
+    646c754f:	nop
+
+00000000646c7550 <one>:
+    646c7550:	add    %al,(%rax)
+    646c7552:	add    %al,(%rax)
+    646c7554:	add    %al,(%rax)
+    646c7556:	lock (bad)
+
+00000000646c7558 <limit>:
+    646c7558:	pop    %rdx
+    646c755a:	cmc
+    646c755b:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c755f:	(bad)
+
+00000000646c7560 <__logl_internal>:
+    646c7560:	fldln2
+    646c7562:	fldt   (%rdx)
+    646c7564:	fld    %st(0)
+    646c7566:	fsubl  -0x1c(%rip)        # 646c7550 <one>
+    646c756c:	fld    %st(0)
+    646c756e:	fabs
+    646c7570:	fcompl -0x1e(%rip)        # 646c7558 <limit>
+    646c7576:	fnstsw %ax
+    646c7578:	and    $0x45,%ah
+    646c757b:	je     646c758f <__logl_internal+0x2f>
+    646c757d:	fstp   %st(1)
+    646c757f:	fyl2xp1
+    646c7581:	mov    %rcx,%rax
+    646c7584:	movq   $0x0,0x8(%rcx)
+    646c758c:	fstpt  (%rcx)
+    646c758e:	ret
+    646c758f:	fstp   %st(0)
+    646c7591:	fyl2x
+    646c7593:	mov    %rcx,%rax
+    646c7596:	movq   $0x0,0x8(%rcx)
+    646c759e:	fstpt  (%rcx)
+    646c75a0:	ret
+    646c75a1:	nop
+    646c75a2:	nop
+    646c75a3:	nop
+    646c75a4:	nop
+    646c75a5:	nop
+    646c75a6:	nop
+    646c75a7:	nop
+    646c75a8:	nop
+    646c75a9:	nop
+    646c75aa:	nop
+    646c75ab:	nop
+    646c75ac:	nop
+    646c75ad:	nop
+    646c75ae:	nop
+    646c75af:	nop
+
+00000000646c75b0 <ldexp>:
+    646c75b0:	push   %rbx
+    646c75b1:	sub    $0x30,%rsp
+    646c75b5:	movq   %xmm0,%rax
+    646c75ba:	movq   %xmm0,%rbx
+    646c75bf:	shr    $0x20,%rax
+    646c75c3:	mov    %eax,%r8d
+    646c75c6:	and    $0x7fffffff,%r8d
+    646c75cd:	or     %ebx,%r8d
+    646c75d0:	sete   %r8b
+    646c75d4:	and    $0x7ff00000,%eax
+    646c75d9:	sete   %cl
+    646c75dc:	or     %cl,%r8b
+    646c75df:	jne    646c75e8 <ldexp+0x38>
+    646c75e1:	cmp    $0x7ff00000,%eax
+    646c75e6:	je     646c7663 <ldexp+0xb3>
+    646c75e8:	movq   %rbx,%xmm1
+    646c75ed:	pxor   %xmm0,%xmm0
+    646c75f1:	ucomisd %xmm0,%xmm1
+    646c75f5:	jp     646c75f9 <ldexp+0x49>
+    646c75f7:	je     646c7663 <ldexp+0xb3>
+    646c75f9:	pxor   %xmm2,%xmm2
+    646c75fd:	cvtsi2sd %edx,%xmm2
+    646c7601:	mov    %rbx,0x20(%rsp)
+    646c7606:	fldl   0x20(%rsp)
+    646c760a:	movsd  %xmm2,0x28(%rsp)
+    646c7610:	fldl   0x28(%rsp)
+    646c7614:	fxch   %st(1)
+    646c7616:	fscale
+    646c7618:	fstp   %st(1)
+    646c761a:	fstpl  0x20(%rsp)
+    646c761e:	mov    0x20(%rsp),%rbx
+    646c7623:	mov    %rbx,%rax
+    646c7626:	shr    $0x20,%rax
+    646c762a:	mov    %eax,%ecx
+    646c762c:	and    $0x7fffffff,%ecx
+    646c7632:	or     %ebx,%ecx
+    646c7634:	sete   %cl
+    646c7637:	and    $0x7ff00000,%eax
+    646c763c:	sete   %dl
+    646c763f:	or     %dl,%cl
+    646c7641:	jne    646c764a <ldexp+0x9a>
+    646c7643:	cmp    $0x7ff00000,%eax
+    646c7648:	je     646c7658 <ldexp+0xa8>
+    646c764a:	movsd  0x20(%rsp),%xmm3
+    646c7650:	ucomisd %xmm0,%xmm3
+    646c7654:	jp     646c7663 <ldexp+0xb3>
+    646c7656:	jne    646c7663 <ldexp+0xb3>
+    646c7658:	call   646c7778 <_errno>
+    646c765d:	movl   $0x22,(%rax)
+    646c7663:	movq   %rbx,%xmm0
+    646c7668:	add    $0x30,%rsp
+    646c766c:	pop    %rbx
+    646c766d:	ret
     646c766e:	nop
     646c766f:	nop
 
-00000000646c7670 <printf>:
-    646c7670:	jmp    *0x6cae(%rip)        # 646ce324 <__imp_printf>
-    646c7676:	nop
-    646c7677:	nop
-
-00000000646c7678 <perror>:
-    646c7678:	jmp    *0x6c9e(%rip)        # 646ce31c <__imp_perror>
-    646c767e:	nop
-    646c767f:	nop
-
-00000000646c7680 <malloc>:
-    646c7680:	jmp    *0x6c8e(%rip)        # 646ce314 <__imp_malloc>
-    646c7686:	nop
-    646c7687:	nop
-
-00000000646c7688 <log10>:
-    646c7688:	jmp    *0x6c7e(%rip)        # 646ce30c <__imp_log10>
-    646c768e:	nop
-    646c768f:	nop
-
-00000000646c7690 <fwrite>:
-    646c7690:	jmp    *0x6c6e(%rip)        # 646ce304 <__imp_fwrite>
-    646c7696:	nop
-    646c7697:	nop
-
-00000000646c7698 <free>:
-    646c7698:	jmp    *0x6c5e(%rip)        # 646ce2fc <__imp_free>
-    646c769e:	nop
-    646c769f:	nop
-
-00000000646c76a0 <fprintf>:
-    646c76a0:	jmp    *0x6c4e(%rip)        # 646ce2f4 <__imp_fprintf>
-    646c76a6:	nop
-    646c76a7:	nop
-
-00000000646c76a8 <fopen>:
-    646c76a8:	jmp    *0x6c3e(%rip)        # 646ce2ec <__imp_fopen>
-    646c76ae:	nop
-    646c76af:	nop
-
-00000000646c76b0 <fclose>:
-    646c76b0:	jmp    *0x6c2e(%rip)        # 646ce2e4 <__imp_fclose>
-    646c76b6:	nop
-    646c76b7:	nop
-
-00000000646c76b8 <exit>:
-    646c76b8:	jmp    *0x6c1e(%rip)        # 646ce2dc <__imp_exit>
-    646c76be:	nop
-    646c76bf:	nop
-
-00000000646c76c0 <calloc>:
-    646c76c0:	jmp    *0x6c0e(%rip)        # 646ce2d4 <__imp_calloc>
-    646c76c6:	nop
-    646c76c7:	nop
-
-00000000646c76c8 <abort>:
-    646c76c8:	jmp    *0x6bfe(%rip)        # 646ce2cc <__imp_abort>
-    646c76ce:	nop
-    646c76cf:	nop
-
-00000000646c76d0 <_vsnprintf>:
-    646c76d0:	jmp    *0x6bee(%rip)        # 646ce2c4 <__imp__vsnprintf>
-    646c76d6:	nop
-    646c76d7:	nop
-
-00000000646c76d8 <_mkdir>:
-    646c76d8:	jmp    *0x6bd6(%rip)        # 646ce2b4 <__imp__mkdir>
+00000000646c7670 <one>:
+    646c7670:	add    %al,(%rax)
+    646c7672:	add    %al,(%rax)
+    646c7674:	add    %al,(%rax)
+    646c7676:	lock (bad)
+
+00000000646c7678 <limit>:
+    646c7678:	pop    %rdx
+    646c767a:	cmc
+    646c767b:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c767f:	(bad)
+
+00000000646c7680 <log2l>:
+    646c7680:	fldl   -0x16(%rip)        # 646c7670 <one>
+    646c7686:	fldt   (%rdx)
+    646c7688:	fxam
+    646c768a:	fnstsw %ax
+    646c768c:	fld    %st(0)
+    646c768e:	sahf
+    646c768f:	jb     646c76c8 <log2l+0x48>
+    646c7691:	fsub   %st(2),%st
+    646c7693:	fld    %st(0)
+    646c7695:	fabs
+    646c7697:	fcompl -0x25(%rip)        # 646c7678 <limit>
+    646c769d:	fnstsw %ax
+    646c769f:	and    $0x45,%ah
+    646c76a2:	je     646c76b6 <log2l+0x36>
+    646c76a4:	fstp   %st(1)
+    646c76a6:	fyl2xp1
+    646c76a8:	mov    %rcx,%rax
+    646c76ab:	movq   $0x0,0x8(%rcx)
+    646c76b3:	fstpt  (%rcx)
+    646c76b5:	ret
+    646c76b6:	fstp   %st(0)
+    646c76b8:	fyl2x
+    646c76ba:	mov    %rcx,%rax
+    646c76bd:	movq   $0x0,0x8(%rcx)
+    646c76c5:	fstpt  (%rcx)
+    646c76c7:	ret
+    646c76c8:	jp     646c7691 <log2l+0x11>
+    646c76ca:	fstp   %st(1)
+    646c76cc:	fstp   %st(1)
+    646c76ce:	mov    %rcx,%rax
+    646c76d1:	movq   $0x0,0x8(%rcx)
+    646c76d9:	fstpt  (%rcx)
+    646c76db:	ret
+    646c76dc:	nop
+    646c76dd:	nop
     646c76de:	nop
     646c76df:	nop
 
-00000000646c76e0 <_initterm>:
-    646c76e0:	jmp    *0x6bbe(%rip)        # 646ce2a4 <__imp__initterm>
+00000000646c76e0 <vfprintf>:
+    646c76e0:	jmp    *0x6c66(%rip)        # 646ce34c <__imp_vfprintf>
     646c76e6:	nop
     646c76e7:	nop
 
-00000000646c76e8 <_errno>:
-    646c76e8:	jmp    *0x6bae(%rip)        # 646ce29c <__imp__errno>
+00000000646c76e8 <strncmp>:
+    646c76e8:	jmp    *0x6c56(%rip)        # 646ce344 <__imp_strncmp>
     646c76ee:	nop
     646c76ef:	nop
 
-00000000646c76f0 <_amsg_exit>:
-    646c76f0:	jmp    *0x6b9e(%rip)        # 646ce294 <__imp__amsg_exit>
+00000000646c76f0 <strlen>:
+    646c76f0:	jmp    *0x6c46(%rip)        # 646ce33c <__imp_strlen>
     646c76f6:	nop
     646c76f7:	nop
-    646c76f8:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7700 <_initialize_onexit_table>:
-    646c7700:	test   %rcx,%rcx
-    646c7703:	je     646c771f <_initialize_onexit_table+0x1f>
-    646c7705:	xor    %eax,%eax
-    646c7707:	movq   $0x0,0x10(%rcx)
-    646c770f:	movq   $0x0,0x8(%rcx)
-    646c7717:	movq   $0x0,(%rcx)
-    646c771e:	ret
-    646c771f:	mov    $0xffffffff,%eax
-    646c7724:	ret
-    646c7725:	nop
-    646c7726:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7730 <_register_onexit_function>:
-    646c7730:	push   %rbp
-    646c7731:	push   %rdi
-    646c7732:	push   %rsi
-    646c7733:	push   %rbx
-    646c7734:	sub    $0x28,%rsp
-    646c7738:	test   %rcx,%rcx
-    646c773b:	mov    %rcx,%rbx
-    646c773e:	mov    %rdx,%rdi
-    646c7741:	je     646c77e0 <_register_onexit_function+0xb0>
-    646c7747:	mov    $0x8,%ecx
-    646c774c:	call   646c78a0 <_lock>
-    646c7751:	cmpq   $0x0,(%rbx)
-    646c7755:	je     646c77b4 <_register_onexit_function+0x84>
-    646c7757:	mov    0x8(%rbx),%rsi
-    646c775b:	mov    0x10(%rbx),%rax
-    646c775f:	cmp    %rsi,%rax
-    646c7762:	je     646c7784 <_register_onexit_function+0x54>
-    646c7764:	lea    0x8(%rsi),%rax
-    646c7768:	mov    $0x8,%ecx
-    646c776d:	mov    %rax,0x8(%rbx)
-    646c7771:	mov    %rdi,(%rsi)
-    646c7774:	call   646c7898 <_unlock>
-    646c7779:	xor    %eax,%eax
-    646c777b:	add    $0x28,%rsp
-    646c777f:	pop    %rbx
-    646c7780:	pop    %rsi
-    646c7781:	pop    %rdi
-    646c7782:	pop    %rbp
-    646c7783:	ret
-    646c7784:	mov    (%rbx),%rcx
-    646c7787:	sub    %rcx,%rsi
-    646c778a:	mov    %rsi,%rax
-    646c778d:	sar    $0x3,%rax
-    646c7791:	shl    $0x4,%rax
-    646c7795:	mov    %rax,%rdx
-    646c7798:	mov    %rax,%rbp
-    646c779b:	call   646c7890 <realloc>
-    646c77a0:	test   %rax,%rax
-    646c77a3:	je     646c77e7 <_register_onexit_function+0xb7>
-    646c77a5:	mov    %rax,(%rbx)
-    646c77a8:	add    %rax,%rsi
-    646c77ab:	add    %rbp,%rax
-    646c77ae:	mov    %rax,0x10(%rbx)
-    646c77b2:	jmp    646c7764 <_register_onexit_function+0x34>
-    646c77b4:	mov    $0x8,%edx
-    646c77b9:	mov    $0x20,%ecx
-    646c77be:	call   646c76c0 <calloc>
-    646c77c3:	test   %rax,%rax
-    646c77c6:	mov    %rax,%rsi
-    646c77c9:	mov    %rax,(%rbx)
-    646c77cc:	je     646c77e7 <_register_onexit_function+0xb7>
-    646c77ce:	mov    %rax,0x8(%rbx)
-    646c77d2:	lea    0x100(%rax),%rax
-    646c77d9:	mov    %rax,0x10(%rbx)
-    646c77dd:	jmp    646c775f <_register_onexit_function+0x2f>
-    646c77df:	nop
-    646c77e0:	mov    $0xffffffff,%eax
-    646c77e5:	jmp    646c777b <_register_onexit_function+0x4b>
-    646c77e7:	mov    $0x8,%ecx
-    646c77ec:	call   646c7898 <_unlock>
-    646c77f1:	mov    $0xffffffff,%eax
-    646c77f6:	jmp    646c777b <_register_onexit_function+0x4b>
-    646c77f8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7800 <_execute_onexit_table>:
-    646c7800:	push   %rdi
-    646c7801:	push   %rsi
-    646c7802:	push   %rbx
-    646c7803:	sub    $0x20,%rsp
-    646c7807:	mov    %rcx,%rdi
-    646c780a:	mov    $0x8,%ecx
-    646c780f:	call   646c78a0 <_lock>
-    646c7814:	mov    (%rdi),%rsi
-    646c7817:	mov    $0x8,%ecx
-    646c781c:	movq   $0x0,0x10(%rdi)
-    646c7824:	mov    0x8(%rdi),%rbx
-    646c7828:	movq   $0x0,(%rdi)
-    646c782f:	movq   $0x0,0x8(%rdi)
-    646c7837:	call   646c7898 <_unlock>
-    646c783c:	test   %rsi,%rsi
-    646c783f:	je     646c7865 <_execute_onexit_table+0x65>
-    646c7841:	sub    $0x8,%rbx
-    646c7845:	cmp    %rbx,%rsi
-    646c7848:	ja     646c785d <_execute_onexit_table+0x5d>
-    646c784a:	mov    (%rbx),%rax
-    646c784d:	test   %rax,%rax
-    646c7850:	je     646c7841 <_execute_onexit_table+0x41>
-    646c7852:	call   *%rax
-    646c7854:	sub    $0x8,%rbx
-    646c7858:	cmp    %rbx,%rsi
-    646c785b:	jbe    646c784a <_execute_onexit_table+0x4a>
-    646c785d:	mov    %rsi,%rcx
-    646c7860:	call   646c7698 <free>
-    646c7865:	xor    %eax,%eax
-    646c7867:	add    $0x20,%rsp
-    646c786b:	pop    %rbx
-    646c786c:	pop    %rsi
-    646c786d:	pop    %rdi
-    646c786e:	ret
+00000000646c76f8 <signal>:
+    646c76f8:	jmp    *0x6c36(%rip)        # 646ce334 <__imp_signal>
+    646c76fe:	nop
+    646c76ff:	nop
+
+00000000646c7700 <printf>:
+    646c7700:	jmp    *0x6c1e(%rip)        # 646ce324 <__imp_printf>
+    646c7706:	nop
+    646c7707:	nop
+
+00000000646c7708 <perror>:
+    646c7708:	jmp    *0x6c0e(%rip)        # 646ce31c <__imp_perror>
+    646c770e:	nop
+    646c770f:	nop
+
+00000000646c7710 <malloc>:
+    646c7710:	jmp    *0x6bfe(%rip)        # 646ce314 <__imp_malloc>
+    646c7716:	nop
+    646c7717:	nop
+
+00000000646c7718 <log10>:
+    646c7718:	jmp    *0x6bee(%rip)        # 646ce30c <__imp_log10>
+    646c771e:	nop
+    646c771f:	nop
+
+00000000646c7720 <fwrite>:
+    646c7720:	jmp    *0x6bde(%rip)        # 646ce304 <__imp_fwrite>
+    646c7726:	nop
+    646c7727:	nop
+
+00000000646c7728 <free>:
+    646c7728:	jmp    *0x6bce(%rip)        # 646ce2fc <__imp_free>
+    646c772e:	nop
+    646c772f:	nop
+
+00000000646c7730 <fprintf>:
+    646c7730:	jmp    *0x6bbe(%rip)        # 646ce2f4 <__imp_fprintf>
+    646c7736:	nop
+    646c7737:	nop
+
+00000000646c7738 <fopen>:
+    646c7738:	jmp    *0x6bae(%rip)        # 646ce2ec <__imp_fopen>
+    646c773e:	nop
+    646c773f:	nop
+
+00000000646c7740 <fclose>:
+    646c7740:	jmp    *0x6b9e(%rip)        # 646ce2e4 <__imp_fclose>
+    646c7746:	nop
+    646c7747:	nop
+
+00000000646c7748 <exit>:
+    646c7748:	jmp    *0x6b8e(%rip)        # 646ce2dc <__imp_exit>
+    646c774e:	nop
+    646c774f:	nop
+
+00000000646c7750 <calloc>:
+    646c7750:	jmp    *0x6b7e(%rip)        # 646ce2d4 <__imp_calloc>
+    646c7756:	nop
+    646c7757:	nop
+
+00000000646c7758 <abort>:
+    646c7758:	jmp    *0x6b6e(%rip)        # 646ce2cc <__imp_abort>
+    646c775e:	nop
+    646c775f:	nop
+
+00000000646c7760 <_vsnprintf>:
+    646c7760:	jmp    *0x6b5e(%rip)        # 646ce2c4 <__imp__vsnprintf>
+    646c7766:	nop
+    646c7767:	nop
+
+00000000646c7768 <_mkdir>:
+    646c7768:	jmp    *0x6b46(%rip)        # 646ce2b4 <__imp__mkdir>
+    646c776e:	nop
+    646c776f:	nop
+
+00000000646c7770 <_initterm>:
+    646c7770:	jmp    *0x6b2e(%rip)        # 646ce2a4 <__imp__initterm>
+    646c7776:	nop
+    646c7777:	nop
+
+00000000646c7778 <_errno>:
+    646c7778:	jmp    *0x6b1e(%rip)        # 646ce29c <__imp__errno>
+    646c777e:	nop
+    646c777f:	nop
+
+00000000646c7780 <_amsg_exit>:
+    646c7780:	jmp    *0x6b0e(%rip)        # 646ce294 <__imp__amsg_exit>
+    646c7786:	nop
+    646c7787:	nop
+    646c7788:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7790 <_initialize_onexit_table>:
+    646c7790:	test   %rcx,%rcx
+    646c7793:	je     646c77af <_initialize_onexit_table+0x1f>
+    646c7795:	xor    %eax,%eax
+    646c7797:	movq   $0x0,0x10(%rcx)
+    646c779f:	movq   $0x0,0x8(%rcx)
+    646c77a7:	movq   $0x0,(%rcx)
+    646c77ae:	ret
+    646c77af:	mov    $0xffffffff,%eax
+    646c77b4:	ret
+    646c77b5:	nop
+    646c77b6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c77c0 <_register_onexit_function>:
+    646c77c0:	push   %rbp
+    646c77c1:	push   %rdi
+    646c77c2:	push   %rsi
+    646c77c3:	push   %rbx
+    646c77c4:	sub    $0x28,%rsp
+    646c77c8:	test   %rcx,%rcx
+    646c77cb:	mov    %rcx,%rbx
+    646c77ce:	mov    %rdx,%rdi
+    646c77d1:	je     646c7870 <_register_onexit_function+0xb0>
+    646c77d7:	mov    $0x8,%ecx
+    646c77dc:	call   646c7930 <_lock>
+    646c77e1:	cmpq   $0x0,(%rbx)
+    646c77e5:	je     646c7844 <_register_onexit_function+0x84>
+    646c77e7:	mov    0x8(%rbx),%rsi
+    646c77eb:	mov    0x10(%rbx),%rax
+    646c77ef:	cmp    %rsi,%rax
+    646c77f2:	je     646c7814 <_register_onexit_function+0x54>
+    646c77f4:	lea    0x8(%rsi),%rax
+    646c77f8:	mov    $0x8,%ecx
+    646c77fd:	mov    %rax,0x8(%rbx)
+    646c7801:	mov    %rdi,(%rsi)
+    646c7804:	call   646c7928 <_unlock>
+    646c7809:	xor    %eax,%eax
+    646c780b:	add    $0x28,%rsp
+    646c780f:	pop    %rbx
+    646c7810:	pop    %rsi
+    646c7811:	pop    %rdi
+    646c7812:	pop    %rbp
+    646c7813:	ret
+    646c7814:	mov    (%rbx),%rcx
+    646c7817:	sub    %rcx,%rsi
+    646c781a:	mov    %rsi,%rax
+    646c781d:	sar    $0x3,%rax
+    646c7821:	shl    $0x4,%rax
+    646c7825:	mov    %rax,%rdx
+    646c7828:	mov    %rax,%rbp
+    646c782b:	call   646c7920 <realloc>
+    646c7830:	test   %rax,%rax
+    646c7833:	je     646c7877 <_register_onexit_function+0xb7>
+    646c7835:	mov    %rax,(%rbx)
+    646c7838:	add    %rax,%rsi
+    646c783b:	add    %rbp,%rax
+    646c783e:	mov    %rax,0x10(%rbx)
+    646c7842:	jmp    646c77f4 <_register_onexit_function+0x34>
+    646c7844:	mov    $0x8,%edx
+    646c7849:	mov    $0x20,%ecx
+    646c784e:	call   646c7750 <calloc>
+    646c7853:	test   %rax,%rax
+    646c7856:	mov    %rax,%rsi
+    646c7859:	mov    %rax,(%rbx)
+    646c785c:	je     646c7877 <_register_onexit_function+0xb7>
+    646c785e:	mov    %rax,0x8(%rbx)
+    646c7862:	lea    0x100(%rax),%rax
+    646c7869:	mov    %rax,0x10(%rbx)
+    646c786d:	jmp    646c77ef <_register_onexit_function+0x2f>
     646c786f:	nop
-
-00000000646c7870 <__acrt_iob_func>:
-    646c7870:	push   %rbx
-    646c7871:	sub    $0x20,%rsp
-    646c7875:	mov    %ecx,%ebx
-    646c7877:	call   646c78a8 <__iob_func>
-    646c787c:	mov    %ebx,%ecx
-    646c787e:	lea    (%rcx,%rcx,2),%rdx
-    646c7882:	shl    $0x4,%rdx
-    646c7886:	add    %rdx,%rax
-    646c7889:	add    $0x20,%rsp
-    646c788d:	pop    %rbx
-    646c788e:	ret
-    646c788f:	nop
-
-00000000646c7890 <realloc>:
-    646c7890:	jmp    *0x6a96(%rip)        # 646ce32c <__imp_realloc>
-    646c7896:	nop
-    646c7897:	nop
-
-00000000646c7898 <_unlock>:
-    646c7898:	jmp    *0x6a1e(%rip)        # 646ce2bc <__imp__unlock>
-    646c789e:	nop
-    646c789f:	nop
-
-00000000646c78a0 <_lock>:
-    646c78a0:	jmp    *0x6a06(%rip)        # 646ce2ac <__imp__lock>
-    646c78a6:	nop
-    646c78a7:	nop
-
-00000000646c78a8 <__iob_func>:
-    646c78a8:	jmp    *0x69d6(%rip)        # 646ce284 <__imp___iob_func>
-    646c78ae:	nop
-    646c78af:	nop
-
-00000000646c78b0 <VirtualQuery>:
-    646c78b0:	jmp    *0x69be(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c78b6:	nop
-    646c78b7:	nop
-
-00000000646c78b8 <VirtualProtect>:
-    646c78b8:	jmp    *0x69ae(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c78be:	nop
-    646c78bf:	nop
-
-00000000646c78c0 <UnhandledExceptionFilter>:
-    646c78c0:	jmp    *0x699e(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c78c6:	nop
-    646c78c7:	nop
-
-00000000646c78c8 <TlsGetValue>:
-    646c78c8:	jmp    *0x698e(%rip)        # 646ce25c <__imp_TlsGetValue>
-    646c78ce:	nop
-    646c78cf:	nop
-
-00000000646c78d0 <TerminateProcess>:
-    646c78d0:	jmp    *0x697e(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c78d6:	nop
-    646c78d7:	nop
-
-00000000646c78d8 <SetUnhandledExceptionFilter>:
-    646c78d8:	jmp    *0x6966(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c78de:	nop
-    646c78df:	nop
-
-00000000646c78e0 <RtlVirtualUnwind>:
-    646c78e0:	jmp    *0x6956(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c78e6:	nop
-    646c78e7:	nop
-
-00000000646c78e8 <RtlLookupFunctionEntry>:
-    646c78e8:	jmp    *0x6946(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c78ee:	nop
-    646c78ef:	nop
-
-00000000646c78f0 <RtlCaptureContext>:
-    646c78f0:	jmp    *0x6936(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c78f6:	nop
-    646c78f7:	nop
-
-00000000646c78f8 <RtlAddFunctionTable>:
-    646c78f8:	jmp    *0x6926(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c78fe:	nop
+    646c7870:	mov    $0xffffffff,%eax
+    646c7875:	jmp    646c780b <_register_onexit_function+0x4b>
+    646c7877:	mov    $0x8,%ecx
+    646c787c:	call   646c7928 <_unlock>
+    646c7881:	mov    $0xffffffff,%eax
+    646c7886:	jmp    646c780b <_register_onexit_function+0x4b>
+    646c7888:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7890 <_execute_onexit_table>:
+    646c7890:	push   %rdi
+    646c7891:	push   %rsi
+    646c7892:	push   %rbx
+    646c7893:	sub    $0x20,%rsp
+    646c7897:	mov    %rcx,%rdi
+    646c789a:	mov    $0x8,%ecx
+    646c789f:	call   646c7930 <_lock>
+    646c78a4:	mov    (%rdi),%rsi
+    646c78a7:	mov    $0x8,%ecx
+    646c78ac:	movq   $0x0,0x10(%rdi)
+    646c78b4:	mov    0x8(%rdi),%rbx
+    646c78b8:	movq   $0x0,(%rdi)
+    646c78bf:	movq   $0x0,0x8(%rdi)
+    646c78c7:	call   646c7928 <_unlock>
+    646c78cc:	test   %rsi,%rsi
+    646c78cf:	je     646c78f5 <_execute_onexit_table+0x65>
+    646c78d1:	sub    $0x8,%rbx
+    646c78d5:	cmp    %rbx,%rsi
+    646c78d8:	ja     646c78ed <_execute_onexit_table+0x5d>
+    646c78da:	mov    (%rbx),%rax
+    646c78dd:	test   %rax,%rax
+    646c78e0:	je     646c78d1 <_execute_onexit_table+0x41>
+    646c78e2:	call   *%rax
+    646c78e4:	sub    $0x8,%rbx
+    646c78e8:	cmp    %rbx,%rsi
+    646c78eb:	jbe    646c78da <_execute_onexit_table+0x4a>
+    646c78ed:	mov    %rsi,%rcx
+    646c78f0:	call   646c7728 <free>
+    646c78f5:	xor    %eax,%eax
+    646c78f7:	add    $0x20,%rsp
+    646c78fb:	pop    %rbx
+    646c78fc:	pop    %rsi
+    646c78fd:	pop    %rdi
+    646c78fe:	ret
     646c78ff:	nop
 
-00000000646c7900 <QueryPerformanceCounter>:
-    646c7900:	jmp    *0x6916(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c7906:	nop
-    646c7907:	nop
-
-00000000646c7908 <LeaveCriticalSection>:
-    646c7908:	jmp    *0x6906(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c790e:	nop
-    646c790f:	nop
-
-00000000646c7910 <InitializeCriticalSection>:
-    646c7910:	jmp    *0x68f6(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c7916:	nop
-    646c7917:	nop
-
-00000000646c7918 <GetTickCount>:
-    646c7918:	jmp    *0x68e6(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c791e:	nop
+00000000646c7900 <__acrt_iob_func>:
+    646c7900:	push   %rbx
+    646c7901:	sub    $0x20,%rsp
+    646c7905:	mov    %ecx,%ebx
+    646c7907:	call   646c7938 <__iob_func>
+    646c790c:	mov    %ebx,%ecx
+    646c790e:	lea    (%rcx,%rcx,2),%rdx
+    646c7912:	shl    $0x4,%rdx
+    646c7916:	add    %rdx,%rax
+    646c7919:	add    $0x20,%rsp
+    646c791d:	pop    %rbx
+    646c791e:	ret
     646c791f:	nop
 
-00000000646c7920 <GetSystemTimeAsFileTime>:
-    646c7920:	jmp    *0x68d6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+00000000646c7920 <realloc>:
+    646c7920:	jmp    *0x6a06(%rip)        # 646ce32c <__imp_realloc>
     646c7926:	nop
     646c7927:	nop
 
-00000000646c7928 <GetLastError>:
-    646c7928:	jmp    *0x68c6(%rip)        # 646ce1f4 <__imp_GetLastError>
+00000000646c7928 <_unlock>:
+    646c7928:	jmp    *0x698e(%rip)        # 646ce2bc <__imp__unlock>
     646c792e:	nop
     646c792f:	nop
 
-00000000646c7930 <GetCurrentThreadId>:
-    646c7930:	jmp    *0x68b6(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+00000000646c7930 <_lock>:
+    646c7930:	jmp    *0x6976(%rip)        # 646ce2ac <__imp__lock>
     646c7936:	nop
     646c7937:	nop
 
-00000000646c7938 <GetCurrentProcessId>:
-    646c7938:	jmp    *0x68a6(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+00000000646c7938 <__iob_func>:
+    646c7938:	jmp    *0x6946(%rip)        # 646ce284 <__imp___iob_func>
     646c793e:	nop
     646c793f:	nop
 
-00000000646c7940 <GetCurrentProcess>:
-    646c7940:	jmp    *0x6896(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+00000000646c7940 <VirtualQuery>:
+    646c7940:	jmp    *0x692e(%rip)        # 646ce274 <__imp_VirtualQuery>
     646c7946:	nop
     646c7947:	nop
 
-00000000646c7948 <EnterCriticalSection>:
-    646c7948:	jmp    *0x6886(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+00000000646c7948 <VirtualProtect>:
+    646c7948:	jmp    *0x691e(%rip)        # 646ce26c <__imp_VirtualProtect>
     646c794e:	nop
     646c794f:	nop
 
-00000000646c7950 <DeleteCriticalSection>:
-    646c7950:	jmp    *0x6876(%rip)        # 646ce1cc <__IAT_start__>
+00000000646c7950 <UnhandledExceptionFilter>:
+    646c7950:	jmp    *0x690e(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
     646c7956:	nop
     646c7957:	nop
-    646c7958:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7960 <__mingw_raise_matherr>:
-    646c7960:	sub    $0x58,%rsp
-    646c7964:	mov    0x5205(%rip),%rax        # 646ccb70 <stUserMathErr>
-    646c796b:	test   %rax,%rax
-    646c796e:	je     646c799c <__mingw_raise_matherr+0x3c>
-    646c7970:	movsd  0x80(%rsp),%xmm0
-    646c7979:	mov    %ecx,0x20(%rsp)
-    646c797d:	lea    0x20(%rsp),%rcx
-    646c7982:	mov    %rdx,0x28(%rsp)
-    646c7987:	movsd  %xmm2,0x30(%rsp)
-    646c798d:	movsd  %xmm3,0x38(%rsp)
-    646c7993:	movsd  %xmm0,0x40(%rsp)
-    646c7999:	call   *%rax
-    646c799b:	nop
-    646c799c:	add    $0x58,%rsp
-    646c79a0:	ret
-    646c79a1:	nopl   0x0(%rax,%rax,1)
-    646c79a6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c79b0 <__mingw_setusermatherr>:
-    646c79b0:	mov    %rcx,0x51b9(%rip)        # 646ccb70 <stUserMathErr>
-    646c79b7:	jmp    646c7ac0 <__setusermatherr>
-    646c79bc:	nopl   0x0(%rax)
-
-00000000646c79c0 <_matherr>:
-    646c79c0:	push   %rsi
-    646c79c1:	push   %rbx
-    646c79c2:	sub    $0x78,%rsp
-    646c79c6:	movaps %xmm6,0x40(%rsp)
-    646c79cb:	movaps %xmm7,0x50(%rsp)
-    646c79d0:	movaps %xmm8,0x60(%rsp)
-    646c79d6:	cmpl   $0x6,(%rcx)
-    646c79d9:	ja     646c7ab0 <_matherr+0xf0>
-    646c79df:	mov    (%rcx),%eax
-    646c79e1:	lea    0x1bbc(%rip),%rdx        # 646c95a4 <.rdata+0x124>
-    646c79e8:	movslq (%rdx,%rax,4),%rax
-    646c79ec:	add    %rdx,%rax
-    646c79ef:	jmp    *%rax
-    646c79f1:	lea    0x1a88(%rip),%rbx        # 646c9480 <.rdata>
-    646c79f8:	mov    0x8(%rcx),%rsi
-    646c79fc:	movsd  0x20(%rcx),%xmm8
-    646c7a02:	movsd  0x18(%rcx),%xmm7
-    646c7a07:	movsd  0x10(%rcx),%xmm6
-    646c7a0c:	mov    $0x2,%ecx
-    646c7a11:	call   646c7870 <__acrt_iob_func>
-    646c7a16:	movsd  %xmm8,0x30(%rsp)
-    646c7a1d:	mov    %rsi,%r9
-    646c7a20:	mov    %rbx,%r8
-    646c7a23:	movsd  %xmm7,0x28(%rsp)
-    646c7a29:	lea    0x1b48(%rip),%rdx        # 646c9578 <.rdata+0xf8>
-    646c7a30:	mov    %rax,%rcx
-    646c7a33:	movsd  %xmm6,0x20(%rsp)
-    646c7a39:	call   646c76a0 <fprintf>
-    646c7a3e:	nop
-    646c7a3f:	movaps 0x40(%rsp),%xmm6
-    646c7a44:	xor    %eax,%eax
-    646c7a46:	movaps 0x50(%rsp),%xmm7
-    646c7a4b:	movaps 0x60(%rsp),%xmm8
-    646c7a51:	add    $0x78,%rsp
-    646c7a55:	pop    %rbx
-    646c7a56:	pop    %rsi
-    646c7a57:	ret
-    646c7a58:	nopl   0x0(%rax,%rax,1)
-    646c7a60:	lea    0x1a38(%rip),%rbx        # 646c949f <.rdata+0x1f>
-    646c7a67:	jmp    646c79f8 <_matherr+0x38>
-    646c7a69:	nopl   0x0(%rax)
-    646c7a70:	lea    0x1a49(%rip),%rbx        # 646c94c0 <.rdata+0x40>
-    646c7a77:	jmp    646c79f8 <_matherr+0x38>
-    646c7a7c:	nopl   0x0(%rax)
-    646c7a80:	lea    0x1aa9(%rip),%rbx        # 646c9530 <.rdata+0xb0>
-    646c7a87:	jmp    646c79f8 <_matherr+0x38>
-    646c7a8c:	nopl   0x0(%rax)
-    646c7a90:	lea    0x1a71(%rip),%rbx        # 646c9508 <.rdata+0x88>
-    646c7a97:	jmp    646c79f8 <_matherr+0x38>
-    646c7a9c:	nopl   0x0(%rax)
-    646c7aa0:	lea    0x1a39(%rip),%rbx        # 646c94e0 <.rdata+0x60>
-    646c7aa7:	jmp    646c79f8 <_matherr+0x38>
-    646c7aac:	nopl   0x0(%rax)
-    646c7ab0:	lea    0x1aaf(%rip),%rbx        # 646c9566 <.rdata+0xe6>
-    646c7ab7:	jmp    646c79f8 <_matherr+0x38>
-    646c7abc:	nop
-    646c7abd:	nop
-    646c7abe:	nop
-    646c7abf:	nop
-
-00000000646c7ac0 <__setusermatherr>:
-    646c7ac0:	jmp    *0x67c6(%rip)        # 646ce28c <__imp___setusermatherr>
-    646c7ac6:	nop
-    646c7ac7:	nop
-    646c7ac8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7ad0 <__report_error>:
-    646c7ad0:	push   %rsi
-    646c7ad1:	push   %rbx
-    646c7ad2:	sub    $0x38,%rsp
-    646c7ad6:	lea    0x58(%rsp),%rax
-    646c7adb:	mov    %rcx,%rbx
-    646c7ade:	mov    $0x2,%ecx
-    646c7ae3:	mov    %rdx,0x58(%rsp)
-    646c7ae8:	mov    %r8,0x60(%rsp)
-    646c7aed:	mov    %r9,0x68(%rsp)
-    646c7af2:	mov    %rax,0x28(%rsp)
-    646c7af7:	call   646c7870 <__acrt_iob_func>
-    646c7afc:	mov    $0x1b,%r8d
-    646c7b02:	mov    $0x1,%edx
-    646c7b07:	lea    0x16d2(%rip),%rcx        # 646c91e0 <.rdata>
-    646c7b0e:	mov    %rax,%r9
-    646c7b11:	call   646c7690 <fwrite>
-    646c7b16:	mov    0x28(%rsp),%rsi
-    646c7b1b:	mov    $0x2,%ecx
-    646c7b20:	call   646c7870 <__acrt_iob_func>
-    646c7b25:	mov    %rbx,%rdx
-    646c7b28:	mov    %rax,%rcx
-    646c7b2b:	mov    %rsi,%r8
-    646c7b2e:	call   646c7650 <vfprintf>
-    646c7b33:	call   646c76c8 <abort>
-    646c7b38:	nop
-    646c7b39:	nop
-    646c7b3a:	nop
-    646c7b3b:	nop
-    646c7b3c:	nop
-    646c7b3d:	nop
-    646c7b3e:	nop
-    646c7b3f:	nop
-
-00000000646c7b40 <register_frame_ctor>:
-    646c7b40:	jmp    646c1390 <__gcc_register_frame>
-    646c7b45:	nop
-    646c7b46:	nop
-    646c7b47:	nop
-    646c7b48:	nop
-    646c7b49:	nop
-    646c7b4a:	nop
-    646c7b4b:	nop
+00000000646c7958 <TlsGetValue>:
+    646c7958:	jmp    *0x68fe(%rip)        # 646ce25c <__imp_TlsGetValue>
+    646c795e:	nop
+    646c795f:	nop
+
+00000000646c7960 <TerminateProcess>:
+    646c7960:	jmp    *0x68ee(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c7966:	nop
+    646c7967:	nop
+
+00000000646c7968 <SetUnhandledExceptionFilter>:
+    646c7968:	jmp    *0x68d6(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c796e:	nop
+    646c796f:	nop
+
+00000000646c7970 <RtlVirtualUnwind>:
+    646c7970:	jmp    *0x68c6(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c7976:	nop
+    646c7977:	nop
+
+00000000646c7978 <RtlLookupFunctionEntry>:
+    646c7978:	jmp    *0x68b6(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c797e:	nop
+    646c797f:	nop
+
+00000000646c7980 <RtlCaptureContext>:
+    646c7980:	jmp    *0x68a6(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c7986:	nop
+    646c7987:	nop
+
+00000000646c7988 <RtlAddFunctionTable>:
+    646c7988:	jmp    *0x6896(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c798e:	nop
+    646c798f:	nop
+
+00000000646c7990 <QueryPerformanceCounter>:
+    646c7990:	jmp    *0x6886(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c7996:	nop
+    646c7997:	nop
+
+00000000646c7998 <LeaveCriticalSection>:
+    646c7998:	jmp    *0x6876(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c799e:	nop
+    646c799f:	nop
+
+00000000646c79a0 <InitializeCriticalSection>:
+    646c79a0:	jmp    *0x6866(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c79a6:	nop
+    646c79a7:	nop
+
+00000000646c79a8 <GetTickCount>:
+    646c79a8:	jmp    *0x6856(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c79ae:	nop
+    646c79af:	nop
+
+00000000646c79b0 <GetSystemTimeAsFileTime>:
+    646c79b0:	jmp    *0x6846(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c79b6:	nop
+    646c79b7:	nop
+
+00000000646c79b8 <GetLastError>:
+    646c79b8:	jmp    *0x6836(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c79be:	nop
+    646c79bf:	nop
+
+00000000646c79c0 <GetCurrentThreadId>:
+    646c79c0:	jmp    *0x6826(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c79c6:	nop
+    646c79c7:	nop
+
+00000000646c79c8 <GetCurrentProcessId>:
+    646c79c8:	jmp    *0x6816(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c79ce:	nop
+    646c79cf:	nop
+
+00000000646c79d0 <GetCurrentProcess>:
+    646c79d0:	jmp    *0x6806(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c79d6:	nop
+    646c79d7:	nop
+
+00000000646c79d8 <EnterCriticalSection>:
+    646c79d8:	jmp    *0x67f6(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c79de:	nop
+    646c79df:	nop
+
+00000000646c79e0 <DeleteCriticalSection>:
+    646c79e0:	jmp    *0x67e6(%rip)        # 646ce1cc <__IAT_start__>
+    646c79e6:	nop
+    646c79e7:	nop
+    646c79e8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c79f0 <__mingw_raise_matherr>:
+    646c79f0:	sub    $0x58,%rsp
+    646c79f4:	mov    0x5175(%rip),%rax        # 646ccb70 <stUserMathErr>
+    646c79fb:	test   %rax,%rax
+    646c79fe:	je     646c7a2c <__mingw_raise_matherr+0x3c>
+    646c7a00:	movsd  0x80(%rsp),%xmm0
+    646c7a09:	mov    %ecx,0x20(%rsp)
+    646c7a0d:	lea    0x20(%rsp),%rcx
+    646c7a12:	mov    %rdx,0x28(%rsp)
+    646c7a17:	movsd  %xmm2,0x30(%rsp)
+    646c7a1d:	movsd  %xmm3,0x38(%rsp)
+    646c7a23:	movsd  %xmm0,0x40(%rsp)
+    646c7a29:	call   *%rax
+    646c7a2b:	nop
+    646c7a2c:	add    $0x58,%rsp
+    646c7a30:	ret
+    646c7a31:	nopl   0x0(%rax,%rax,1)
+    646c7a36:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7a40 <__mingw_setusermatherr>:
+    646c7a40:	mov    %rcx,0x5129(%rip)        # 646ccb70 <stUserMathErr>
+    646c7a47:	jmp    646c7b50 <__setusermatherr>
+    646c7a4c:	nopl   0x0(%rax)
+
+00000000646c7a50 <_matherr>:
+    646c7a50:	push   %rsi
+    646c7a51:	push   %rbx
+    646c7a52:	sub    $0x78,%rsp
+    646c7a56:	movaps %xmm6,0x40(%rsp)
+    646c7a5b:	movaps %xmm7,0x50(%rsp)
+    646c7a60:	movaps %xmm8,0x60(%rsp)
+    646c7a66:	cmpl   $0x6,(%rcx)
+    646c7a69:	ja     646c7b40 <_matherr+0xf0>
+    646c7a6f:	mov    (%rcx),%eax
+    646c7a71:	lea    0x1b2c(%rip),%rdx        # 646c95a4 <.rdata+0x124>
+    646c7a78:	movslq (%rdx,%rax,4),%rax
+    646c7a7c:	add    %rdx,%rax
+    646c7a7f:	jmp    *%rax
+    646c7a81:	lea    0x19f8(%rip),%rbx        # 646c9480 <.rdata>
+    646c7a88:	mov    0x8(%rcx),%rsi
+    646c7a8c:	movsd  0x20(%rcx),%xmm8
+    646c7a92:	movsd  0x18(%rcx),%xmm7
+    646c7a97:	movsd  0x10(%rcx),%xmm6
+    646c7a9c:	mov    $0x2,%ecx
+    646c7aa1:	call   646c7900 <__acrt_iob_func>
+    646c7aa6:	movsd  %xmm8,0x30(%rsp)
+    646c7aad:	mov    %rsi,%r9
+    646c7ab0:	mov    %rbx,%r8
+    646c7ab3:	movsd  %xmm7,0x28(%rsp)
+    646c7ab9:	lea    0x1ab8(%rip),%rdx        # 646c9578 <.rdata+0xf8>
+    646c7ac0:	mov    %rax,%rcx
+    646c7ac3:	movsd  %xmm6,0x20(%rsp)
+    646c7ac9:	call   646c7730 <fprintf>
+    646c7ace:	nop
+    646c7acf:	movaps 0x40(%rsp),%xmm6
+    646c7ad4:	xor    %eax,%eax
+    646c7ad6:	movaps 0x50(%rsp),%xmm7
+    646c7adb:	movaps 0x60(%rsp),%xmm8
+    646c7ae1:	add    $0x78,%rsp
+    646c7ae5:	pop    %rbx
+    646c7ae6:	pop    %rsi
+    646c7ae7:	ret
+    646c7ae8:	nopl   0x0(%rax,%rax,1)
+    646c7af0:	lea    0x19a8(%rip),%rbx        # 646c949f <.rdata+0x1f>
+    646c7af7:	jmp    646c7a88 <_matherr+0x38>
+    646c7af9:	nopl   0x0(%rax)
+    646c7b00:	lea    0x19b9(%rip),%rbx        # 646c94c0 <.rdata+0x40>
+    646c7b07:	jmp    646c7a88 <_matherr+0x38>
+    646c7b0c:	nopl   0x0(%rax)
+    646c7b10:	lea    0x1a19(%rip),%rbx        # 646c9530 <.rdata+0xb0>
+    646c7b17:	jmp    646c7a88 <_matherr+0x38>
+    646c7b1c:	nopl   0x0(%rax)
+    646c7b20:	lea    0x19e1(%rip),%rbx        # 646c9508 <.rdata+0x88>
+    646c7b27:	jmp    646c7a88 <_matherr+0x38>
+    646c7b2c:	nopl   0x0(%rax)
+    646c7b30:	lea    0x19a9(%rip),%rbx        # 646c94e0 <.rdata+0x60>
+    646c7b37:	jmp    646c7a88 <_matherr+0x38>
+    646c7b3c:	nopl   0x0(%rax)
+    646c7b40:	lea    0x1a1f(%rip),%rbx        # 646c9566 <.rdata+0xe6>
+    646c7b47:	jmp    646c7a88 <_matherr+0x38>
     646c7b4c:	nop
     646c7b4d:	nop
     646c7b4e:	nop
     646c7b4f:	nop
 
-00000000646c7b50 <__CTOR_LIST__>:
-    646c7b50:	(bad)
-    646c7b51:	(bad)
-    646c7b52:	(bad)
-    646c7b53:	(bad)
-    646c7b54:	(bad)
-    646c7b55:	(bad)
-    646c7b56:	(bad)
-    646c7b57:	incl   0x7b(%rax)
-
-00000000646c7b58 <.ctors.65535>:
-    646c7b58:	rex jnp 646c7bc7 <__DTOR_LIST__+0x5f>
-    646c7b5b:	add    %al,%fs:(%rax)
-	...
-
-00000000646c7b68 <__DTOR_LIST__>:
-    646c7b68:	(bad)
-    646c7b69:	(bad)
-    646c7b6a:	(bad)
-    646c7b6b:	(bad)
-    646c7b6c:	(bad)
-    646c7b6d:	(bad)
-    646c7b6e:	(bad)
-    646c7b6f:	incl   (%rax)
-    646c7b71:	add    %al,(%rax)
-    646c7b73:	add    %al,(%rax)
-    646c7b75:	add    %al,(%rax)
+00000000646c7b50 <__setusermatherr>:
+    646c7b50:	jmp    *0x6736(%rip)        # 646ce28c <__imp___setusermatherr>
+    646c7b56:	nop
+    646c7b57:	nop
+    646c7b58:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7b60 <__report_error>:
+    646c7b60:	push   %rsi
+    646c7b61:	push   %rbx
+    646c7b62:	sub    $0x38,%rsp
+    646c7b66:	lea    0x58(%rsp),%rax
+    646c7b6b:	mov    %rcx,%rbx
+    646c7b6e:	mov    $0x2,%ecx
+    646c7b73:	mov    %rdx,0x58(%rsp)
+    646c7b78:	mov    %r8,0x60(%rsp)
+    646c7b7d:	mov    %r9,0x68(%rsp)
+    646c7b82:	mov    %rax,0x28(%rsp)
+    646c7b87:	call   646c7900 <__acrt_iob_func>
+    646c7b8c:	mov    $0x1b,%r8d
+    646c7b92:	mov    $0x1,%edx
+    646c7b97:	lea    0x1642(%rip),%rcx        # 646c91e0 <.rdata>
+    646c7b9e:	mov    %rax,%r9
+    646c7ba1:	call   646c7720 <fwrite>
+    646c7ba6:	mov    0x28(%rsp),%rsi
+    646c7bab:	mov    $0x2,%ecx
+    646c7bb0:	call   646c7900 <__acrt_iob_func>
+    646c7bb5:	mov    %rbx,%rdx
+    646c7bb8:	mov    %rax,%rcx
+    646c7bbb:	mov    %rsi,%r8
+    646c7bbe:	call   646c76e0 <vfprintf>
+    646c7bc3:	call   646c7758 <abort>
+    646c7bc8:	nop
+    646c7bc9:	nop
+    646c7bca:	nop
+    646c7bcb:	nop
+    646c7bcc:	nop
+    646c7bcd:	nop
+    646c7bce:	nop
+    646c7bcf:	nop
+
+00000000646c7bd0 <register_frame_ctor>:
+    646c7bd0:	jmp    646c1390 <__gcc_register_frame>
+    646c7bd5:	nop
+    646c7bd6:	nop
+    646c7bd7:	nop
+    646c7bd8:	nop
+    646c7bd9:	nop
+    646c7bda:	nop
+    646c7bdb:	nop
+    646c7bdc:	nop
+    646c7bdd:	nop
+    646c7bde:	nop
+    646c7bdf:	nop
+
+00000000646c7be0 <__CTOR_LIST__>:
+    646c7be0:	(bad)
+    646c7be1:	(bad)
+    646c7be2:	(bad)
+    646c7be3:	(bad)
+    646c7be4:	(bad)
+    646c7be5:	(bad)
+    646c7be6:	(bad)
+    646c7be7:	call   *%rax
+
+00000000646c7be8 <.ctors.65535>:
+    646c7be8:	sarb   0x6c(%rbx)
+    646c7beb:	add    %al,%fs:(%rax)
+	...
+
+00000000646c7bf8 <__DTOR_LIST__>:
+    646c7bf8:	(bad)
+    646c7bf9:	(bad)
+    646c7bfa:	(bad)
+    646c7bfb:	(bad)
+    646c7bfc:	(bad)
+    646c7bfd:	(bad)
+    646c7bfe:	(bad)
+    646c7bff:	incl   (%rax)
+    646c7c01:	add    %al,(%rax)
+    646c7c03:	add    %al,(%rax)
+    646c7c05:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000000646c8000 <__data_start__>:
-    646c8000:	jo     646c807d <__imp___acrt_iob_func+0xd>
-    646c8002:	insb   (%dx),%es:(%rdi)
-    646c8003:	add    %al,%fs:(%rax)
+    646c8000:	add    %bh,0x64(%rsp,%rbp,2)
 	...
 
 00000000646c8010 <__native_vcclrit_reason>:
     646c8010:	(bad)
     646c8011:	(bad)
     646c8012:	(bad)
     646c8013:	(bad)
@@ -10492,31 +10548,32 @@
     646c8044:	add    %al,(%rax)
     646c8046:	stos   %al,%es:(%rdi)
     646c8047:	mov    $0x3fff,%eax
     646c804c:	add    %al,(%rax)
 	...
 
 00000000646c8050 <__imp__execute_onexit_table>:
-    646c8050:	add    %bh,0x6c(%rax)
+    646c8050:	nop
+    646c8051:	js     646c80bf <__data_end__+0x1f>
     646c8053:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8058 <__imp__register_onexit_function>:
-    646c8058:	xor    %dh,0x6c(%rdi)
-    646c805b:	add    %al,%fs:(%rax)
+    646c8058:	shlb   $0x64,0x6c(%rdi)
+    646c805c:	add    %al,(%rax)
 	...
 
 00000000646c8060 <__imp__initialize_onexit_table>:
-    646c8060:	add    %dh,0x6c(%rdi)
+    646c8060:	nop
+    646c8061:	ja     646c80cf <__data_end__+0x2f>
     646c8063:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8070 <__imp___acrt_iob_func>:
-    646c8070:	jo     646c80ea <__data_end__+0x4a>
-    646c8072:	insb   (%dx),%es:(%rdi)
+    646c8070:	add    %bh,0x6c(%rcx)
     646c8073:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8080 <__security_cookie>:
     646c8080:	xor    0x2b992ddf(%rdx),%ah
 	...
 
@@ -10700,20 +10757,18 @@
     646c916d:	add    %al,(%rax)
 	...
 
 00000000646c9170 <GS_ExceptionPointers>:
     646c9170:	add    $0x6c,%bh
     646c9173:	add    %al,%fs:(%rax)
     646c9176:	add    %al,(%rax)
-    646c9178:	movabs 0x9000000000646cc2,%al
+    646c9178:	movabs 0x2000000000646cc2,%al
 
 00000000646c9180 <__dyn_tls_init_callback>:
-    646c9180:	nop
-    646c9181:	push   %rsp
-    646c9182:	insb   (%dx),%es:(%rdi)
+    646c9180:	and    %dl,0x6c(%rbp)
     646c9183:	add    %al,%fs:(%rax)
 	...
 
 00000000646c91a0 <_tls_used>:
     646c91a0:	add    %al,(%rax)
     646c91a2:	insl   (%dx),%es:(%rdi)
     646c91a3:	add    %al,%fs:(%rax)
@@ -11126,39 +11181,34 @@
     646c9591:	and    $0x20202967,%eax
     646c9596:	sub    %dh,0x65(%rdx)
     646c9599:	je     646c9611 <.refptr.__image_base__+0x1>
     646c959b:	(bad)
     646c959c:	insb   (%dx),%es:(%rdi)
     646c959d:	cmp    $0xa296725,%eax
     646c95a2:	add    %al,(%rax)
-    646c95a4:	or     $0xe5,%al
-    646c95a6:	(bad)
-    646c95a7:	decl   -0x1c(%rbp)
+    646c95a4:	pushf
+    646c95a5:	in     $0xff,%eax
+    646c95a7:	(bad)
+    646c95a8:	fucom  %st(4)
     646c95aa:	(bad)
-    646c95ab:	(bad)
-    646c95ac:	mov    $0xccffffe4,%esp
-    646c95b1:	in     $0xff,%al
-    646c95b3:	(bad)
-    646c95b4:	fsub   %st,%st(4)
-    646c95b6:	(bad)
+    646c95ab:	decl   -0x1(%rbp,%riz,8)
+    646c95af:	lcall  *-0x1(%rbp,%riz,8)
+    646c95b3:	ljmp   *-0x1(%rbp,%riz,8)
     646c95b7:	(bad)
-    646c95b8:	in     (%dx),%al
-    646c95b9:	in     $0xff,%al
-    646c95bb:	(bad)
-    646c95bc:	cld
-    646c95bd:	in     $0xff,%al
-    646c95bf:	jmp    *(%rax)
+    646c95b8:	jl     646c959f <.rdata+0x11f>
+    646c95ba:	(bad)
+    646c95bb:	decl   -0x7fdf0001(%rbp,%riz,8)
 
 00000000646c95c0 <.refptr._CRT_MT>:
     646c95c0:	and    %al,0x646c(%rax)
 	...
 
 00000000646c95d0 <.refptr.__CTOR_LIST__>:
-    646c95d0:	push   %rax
-    646c95d1:	jnp    646c963f <.refptr.__native_startup_lock+0xf>
+    646c95d0:	loopne 646c964d <.refptr.__native_startup_state+0xd>
+    646c95d2:	insb   (%dx),%es:(%rdi)
     646c95d3:	add    %al,%fs:(%rax)
 	...
 
 00000000646c95e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
     646c95e0:	loopne 646c957a <.rdata+0xfa>
     646c95e2:	insb   (%dx),%es:(%rdi)
     646c95e3:	add    %al,%fs:(%rax)
@@ -11740,25 +11790,26 @@
     646ca23a:	add    %al,(%rax)
     646ca23c:	adc    $0xb2,%al
     646ca23e:	add    %al,(%rax)
     646ca240:	pop    %rbp
     646ca241:	xor    (%rax),%al
     646ca243:	add    %bh,0x1c000034(%rcx)
     646ca249:	mov    $0x0,%dl
-    646ca24b:	add    %bh,-0x38ffffcc(%rcx)
+    646ca24b:	add    %bh,-0x2fffffcc(%rcx)
     646ca251:	cmp    %al,(%rax)
     646ca253:	add    %ch,(%rax)
     646ca255:	mov    $0x0,%dl
-    646ca257:	add    %al,%bh
+    646ca257:	add    %dl,%al
     646ca259:	cmp    %al,(%rax)
-    646ca25b:	add    %bh,0x3a(%rbx)
-    646ca25e:	add    %al,(%rax)
-    646ca260:	cmp    %dh,0x3a7b0000(%rdx)
+    646ca25b:	add    %al,-0x4dc80000(%rdx,%rdi,1)
+    646ca262:	add    %al,(%rax)
+    646ca264:	test   %bh,(%rdx)
     646ca266:	add    %al,(%rax)
     646ca268:	(bad)
+    646ca269:	cmp    (%rax),%eax
     646ca26b:	add    %al,0x0(%rdx,%rsi,4)
 	...
 
 00000000646ca270 <.pdata>:
     646ca270:	sarb   (%rbx)
     646ca272:	add    %al,(%rax)
     646ca274:	sbb    (%rax,%rax,1),%bh
@@ -11831,348 +11882,340 @@
     646ca320:	cld
     646ca321:	mov    $0x0,%dl
     646ca323:	add    %dl,%ch
     646ca325:	rex.WRB add %r8b,(%r8)
     646ca328:	cmp    %ecx,0x0(%rsi)
     646ca32b:	add    %cl,(%rax)
     646ca32d:	mov    $0x0,%bl
-	...
-
-00000000646ca330 <.pdata>:
-    646ca330:	rex
+    646ca32f:	add    %bh,(%rcx)
     646ca331:	rex.WRX add %r8b,(%rax)
-    646ca334:	mov    $0x50,%dh
-    646ca336:	add    %al,(%rax)
+    646ca334:	(bad)
+    646ca335:	rex.WRX add %r8b,(%rax)
     646ca338:	adc    $0xb3,%al
-    646ca33a:	add    %al,(%rax)
-    646ca33c:	mov    $0x50,%dh
-    646ca33e:	add    %al,(%rax)
-    646ca340:	sahf
-    646ca341:	push   %rcx
-    646ca342:	add    %al,(%rax)
-    646ca344:	and    $0xb3,%al
 	...
 
-00000000646ca348 <.pdata>:
-    646ca348:	mov    $0x51,%al
+00000000646ca33c <.pdata>:
+    646ca33c:	rorb   0x0(%rsi)
+    646ca33f:	add    %al,0x51(%rsi)
+    646ca342:	add    %al,(%rax)
+    646ca344:	and    %dh,0x51460000(%rbx)
     646ca34a:	add    %al,(%rax)
-    646ca34c:	in     $0x51,%eax
+    646ca34c:	cs push %rdx
     646ca34e:	add    %al,(%rax)
-    646ca350:	xor    %dh,0x51f00000(%rbx)
+    646ca350:	xor    %dh,0x52400000(%rbx)
+
+00000000646ca354 <.pdata>:
+    646ca354:	rex push %rdx
     646ca356:	add    %al,(%rax)
-    646ca358:	push   %rsi
-    646ca359:	push   %rdx
+    646ca358:	jne    646ca3ac <.pdata+0x1c>
     646ca35a:	add    %al,(%rax)
-    646ca35c:	cmp    %dh,0x52600000(%rbx)
-    646ca362:	add    %al,(%rax)
-    646ca364:	jg     646ca3b8 <.pdata+0x10>
+    646ca35c:	cmp    $0xb3,%al
+    646ca35e:	add    %al,(%rax)
+    646ca360:	adcb   $0x0,0x0(%rdx)
+    646ca364:	out    %al,$0x52
     646ca366:	add    %al,(%rax)
     646ca368:	rex.R mov $0x0,%bl
+    646ca36b:	add    %dh,%al
+    646ca36d:	push   %rdx
+    646ca36e:	add    %al,(%rax)
+    646ca370:	rcpps  (%rax),%xmm0
+    646ca373:	add    %dl,-0x4d(%rax)
 	...
 
-00000000646ca36c <.pdata>:
-    646ca36c:	adcb   $0x0,0x0(%rdx)
-    646ca370:	push   %rsi
-    646ca371:	push   %rbx
-    646ca372:	add    %al,(%rax)
-    646ca374:	rex.W mov $0x0,%bl
-    646ca377:	add    %ah,0x53(%rax)
-    646ca37a:	add    %al,(%rax)
-    646ca37c:	pop    %rax
-    646ca37d:	push   %rsp
+00000000646ca378 <.pdata>:
+    646ca378:	adc    %dl,0x0(%rbx)
+    646ca37b:	add    %ah,%dh
+    646ca37d:	push   %rbx
     646ca37e:	add    %al,(%rax)
-    646ca380:	pop    %rax
+    646ca380:	push   %rsp
     646ca381:	mov    $0x0,%bl
+    646ca383:	add    %dh,%al
+    646ca385:	push   %rbx
+    646ca386:	add    %al,(%rax)
+    646ca388:	call   c86ca3e1 <.debug_str+0x63ff23e1>
+    646ca38d:	mov    $0x0,%bl
 	...
 
-00000000646ca384 <.pdata>:
-    646ca384:	(bad)
-    646ca385:	push   %rsp
-    646ca386:	add    %al,(%rax)
-    646ca388:	(bad)
-    646ca389:	push   %rsp
-    646ca38a:	add    %al,(%rax)
-    646ca38c:	push   $0xffffffff900000b3
-    646ca391:	push   %rsp
+00000000646ca390 <.pdata>:
+    646ca390:	lock push %rsp
     646ca392:	add    %al,(%rax)
-    646ca394:	add    0x0(%rbp),%edx
-    646ca397:	add    %dh,-0x4d(%rax)
+    646ca394:	(bad)
+    646ca395:	push   %rbp
+    646ca396:	add    %al,(%rax)
+    646ca398:	je     646ca34d <.pdata+0x11>
     646ca39a:	add    %al,(%rax)
-    646ca39c:	adc    %dl,0x0(%rbp)
-    646ca39f:	add    %dl,(%rbx)
-    646ca3a1:	push   %rbp
-    646ca3a2:	add    %al,(%rax)
-    646ca3a4:	jl     646ca359 <.pdata+0x11>
-	...
-
-00000000646ca3a8 <.pdata>:
-    646ca3a8:	and    %dl,0x0(%rbp)
-    646ca3ab:	add    %ah,-0x4c800000(,%rdx,2)
-    646ca3b2:	add    %al,(%rax)
-    646ca3b4:	xor    %dl,0x0(%rbp)
-    646ca3b7:	add    %dh,-0x4c7c0000(,%rdx,2)
-	...
-
-00000000646ca3c0 <.pdata.unlikely>:
-    646ca3c0:	rex push %rbp
+    646ca39c:	and    %dl,0x0(%rbp)
+    646ca39f:	add    %dl,0x7c000055(%rbx)
+    646ca3a5:	mov    $0x0,%bl
+    646ca3a7:	add    %ah,-0x5cffffab(%rax)
+    646ca3ad:	push   %rbp
+    646ca3ae:	add    %al,(%rax)
+    646ca3b0:	mov    %dh,0x55b00000(%rbx)
+
+00000000646ca3b4 <.pdata>:
+    646ca3b4:	mov    $0x55,%al
+    646ca3b6:	add    %al,(%rax)
+    646ca3b8:	mov    $0x55,%ah
+    646ca3ba:	add    %al,(%rax)
+    646ca3bc:	mov    %?,0x55c00000(%rbx)
     646ca3c2:	add    %al,(%rax)
-    646ca3c4:	or     $0x94000057,%eax
+    646ca3c4:	(bad)
+    646ca3c5:	push   %rbp
+    646ca3c6:	add    %al,(%rax)
+    646ca3c8:	nop
     646ca3c9:	mov    $0x0,%bl
 	...
 
-00000000646ca3cc <.pdata>:
-    646ca3cc:	adc    %dl,0x0(%rdi)
-    646ca3cf:	add    %cl,%bl
-    646ca3d1:	pop    %rcx
-    646ca3d2:	add    %al,(%rax)
-    646ca3d4:	movsb  %ds:(%rsi),%es:(%rdi)
+00000000646ca3cc <.pdata.unlikely>:
+    646ca3cc:	rclb   0x0(%rbp)
+    646ca3cf:	add    %bl,-0x5fffffa9(%rbp)
     646ca3d5:	mov    $0x0,%bl
-    646ca3d7:	add    %dl,%al
-    646ca3d9:	pop    %rcx
-    646ca3da:	add    %al,(%rax)
-    646ca3dc:	jo     646ca439 <.pdata+0x1>
-    646ca3de:	add    %al,(%rax)
-    646ca3e0:	mov    $0x700000b3,%esp
+	...
 
-00000000646ca3e4 <.pdata>:
-    646ca3e4:	jo     646ca441 <.pdata+0x9>
+00000000646ca3d8 <.pdata>:
+    646ca3d8:	movabs 0xb000005a5b000057,%al
+    646ca3e1:	mov    $0x0,%bl
+    646ca3e3:	add    %ah,0x5a(%rax)
     646ca3e6:	add    %al,(%rax)
-    646ca3e8:	pop    %rsp
-    646ca3e9:	pop    %rsp
-    646ca3ea:	add    %al,(%rax)
-    646ca3ec:	(bad)
-    646ca3ed:	mov    $0x0,%bl
-    646ca3ef:	add    %ah,0x5c(%rax)
-    646ca3f2:	add    %al,(%rax)
-    646ca3f4:	rex.RXB pop %r14
+    646ca3e8:	add    %bl,0x0(%rax,%rax,1)
+    646ca3ec:	enter  $0xb3,$0x0
+
+00000000646ca3f0 <.pdata>:
+    646ca3f0:	add    %bl,0x0(%rax,%rax,1)
+    646ca3f4:	in     (%dx),%al
+    646ca3f5:	pop    %rsp
     646ca3f6:	add    %al,(%rax)
-    646ca3f8:	(bad)
-    646ca3f9:	mov    $0x0,%bl
-    646ca3fb:	add    %dl,0x5e(%rax)
+    646ca3f8:	shlb   0x5cf00000(%rbx)
     646ca3fe:	add    %al,(%rax)
-    646ca400:	mov    $0xdc00005e,%edx
-    646ca405:	mov    $0x0,%bl
-	...
-
-00000000646ca408 <.pdata>:
-    646ca408:	rcrb   $0x0,0x0(%rsi)
-    646ca40c:	(bad)
-    646ca40d:	pop    %rdi
+    646ca400:	xlat   %ds:(%rbx)
+    646ca401:	pop    %rsi
+    646ca402:	add    %al,(%rax)
+    646ca404:	loopne 646ca3b9 <.pdata+0x5>
+    646ca406:	add    %al,(%rax)
+    646ca408:	loopne 646ca468 <.pdata+0x24>
+    646ca40a:	add    %al,(%rax)
+    646ca40c:	rex.WX pop %rdi
     646ca40e:	add    %al,(%rax)
-    646ca410:	in     (%dx),%al
-    646ca411:	mov    $0x0,%bl
-    646ca413:	add    %al,0x5f(%rax)
+    646ca410:	call   b46ca4c8 <.debug_str+0x4fff24c8>
+
+00000000646ca414 <.pdata>:
+    646ca414:	push   %rax
+    646ca415:	pop    %rdi
     646ca416:	add    %al,(%rax)
-    646ca418:	loopne 646ca479 <.pdata+0x41>
+    646ca418:	iret
+    646ca419:	pop    %rdi
     646ca41a:	add    %al,(%rax)
-    646ca41c:	cld
+    646ca41c:	clc
     646ca41d:	mov    $0x0,%bl
-    646ca41f:	add    %ah,%al
+    646ca41f:	add    %dl,%al
     646ca421:	pop    %rdi
     646ca422:	add    %al,(%rax)
-    646ca424:	mov    $0x4000060,%edx
-    646ca429:	mov    $0x0,%ah
-    646ca42b:	add    %al,%al
-    646ca42d:	(bad)
-    646ca42e:	add    %al,(%rax)
-    646ca430:	fisubs 0x0(%rax)
-    646ca433:	add    %cl,(%rsp,%rsi,4)
-	...
-
-00000000646ca438 <.pdata>:
-    646ca438:	loopne 646ca49a <.pdata+0x62>
-    646ca43a:	add    %al,(%rax)
-    646ca43c:	repnz (bad)
+    646ca424:	jo     646ca486 <.pdata+0x42>
+    646ca426:	add    %al,(%rax)
+    646ca428:	or     %dh,0x607000(%rax,%rax,1)
+    646ca42f:	add    %cl,0x61(%rdx)
+    646ca432:	add    %al,(%rax)
+    646ca434:	adc    %dh,0x615000(%rax,%rax,1)
+    646ca43b:	add    %ch,0x61(%rsi)
     646ca43e:	add    %al,(%rax)
-    646ca440:	adc    %dh,0x610000(%rax,%rax,1)
-    646ca447:	add    %al,0x0(%rcx,%riz,2)
-    646ca44b:	add    %dl,(%rsp,%rsi,4)
+    646ca440:	sbb    %dh,0x617000(%rax,%rax,1)
+
+00000000646ca444 <.pdata>:
+    646ca444:	jo     646ca4a7 <.pdata+0x63>
+    646ca446:	add    %al,(%rax)
+    646ca448:	(bad)
+    646ca449:	(bad)
+    646ca44a:	add    %al,(%rax)
+    646ca44c:	sbb    $0xb4,%al
     646ca44e:	add    %al,(%rax)
-    646ca450:	push   %rax
+    646ca450:	nop
     646ca451:	(bad)
     646ca452:	add    %al,(%rax)
-    646ca454:	frstor 0x0(%rcx)
-    646ca457:	add    %bl,(%rax)
-    646ca459:	mov    $0x0,%ah
-    646ca45b:	add    %ah,%al
-    646ca45d:	(bad)
-    646ca45e:	add    %al,(%rax)
-    646ca460:	push   %rsp
-    646ca461:	(bad)
+    646ca454:	(bad)
+    646ca455:	(bad)
+    646ca456:	add    %al,(%rax)
+    646ca458:	and    %dh,0x61e000(%rax,%rax,1)
+    646ca45f:	add    %ch,0x62(%rbp)
     646ca462:	add    %al,(%rax)
     646ca464:	and    $0xb4,%al
     646ca466:	add    %al,(%rax)
-    646ca468:	(bad)
-    646ca469:	(bad)
+    646ca468:	jo     646ca4cc <.pdata+0x4>
     646ca46a:	add    %al,(%rax)
-    646ca46c:	sahf
-    646ca46d:	(bad)
+    646ca46c:	in     $0x62,%al
     646ca46e:	add    %al,(%rax)
-    646ca470:	sub    $0xb4,%al
-    646ca472:	add    %al,(%rax)
-    646ca474:	movabs 0x340000630f000062,%al
+    646ca470:	xor    %dh,0x62f000(%rax,%rax,1)
+    646ca477:	add    %ch,(%rsi)
+    646ca479:	movsxd (%rax),%eax
+    646ca47b:	add    %bh,(%rax)
     646ca47d:	mov    $0x0,%ah
-    646ca47f:	add    %dl,(%rax)
+    646ca47f:	add    %dh,(%rax)
     646ca481:	movsxd (%rax),%eax
-    646ca483:	add    %al,0x63(%rdi)
-    646ca486:	add    %al,(%rax)
-    646ca488:	cmp    $0xb4,%al
-    646ca48a:	add    %al,(%rax)
-    646ca48c:	push   %rax
-    646ca48d:	movsxd (%rax),%eax
-    646ca48f:	add    %ah,%cl
+    646ca483:	add    %bl,0x40000063(%rdi)
+    646ca489:	mov    $0x0,%ah
+    646ca48b:	add    %ah,-0x28ffff9d(%rax)
     646ca491:	movsxd (%rax),%eax
-    646ca493:	add    %al,0x0(%rsp,%rsi,4)
-    646ca497:	add    %dh,%al
-    646ca499:	movsxd (%rax),%eax
-    646ca49b:	add    %dl,0x4c000064(%rsi)
+    646ca493:	add    %cl,-0x4c(%rax)
+    646ca496:	add    %al,(%rax)
+    646ca498:	loopne 646ca4fd <.pdata+0x5>
+    646ca49a:	add    %al,(%rax)
+    646ca49c:	jno    646ca502 <.pdata+0xa>
+    646ca49e:	add    %al,(%rax)
+    646ca4a0:	push   %rax
     646ca4a1:	mov    $0x0,%ah
-    646ca4a3:	add    %ah,-0x5cffff9c(%rax)
-    646ca4a9:	add    %al,%fs:(%rax)
-    646ca4ac:	push   %rsp
+    646ca4a3:	add    %al,0x26000064(%rax)
+    646ca4a9:	add    %al,%gs:(%rax)
+    646ca4ac:	pop    %rax
     646ca4ad:	mov    $0x0,%ah
-	...
-
-00000000646ca4b0 <.pdata>:
-    646ca4b0:	lock add %al,%fs:(%rax)
-    646ca4b4:	mulb   0x0(%rax,%rax,1)
-    646ca4b8:	pop    %rax
-    646ca4b9:	mov    $0x0,%ah
+    646ca4af:	add    %dh,(%rax)
+    646ca4b1:	add    %al,%gs:(%rax)
+    646ca4b4:	xor    0x0(%rbp),%esp
+    646ca4b7:	add    %ah,-0x4c(%rax)
 	...
 
 00000000646ca4bc <.pdata>:
-    646ca4bc:	add    %ah,0x0(%rbp)
-    646ca4bf:	add    %al,(%rsi)
-    646ca4c1:	add    %al,%gs:(%rax)
-    646ca4c4:	pop    %rsp
-    646ca4c5:	mov    $0x0,%ah
+    646ca4bc:	andb   $0x0,0x0(%rbp)
+    646ca4c0:	xchg   %ah,0x0(%rbp)
+    646ca4c3:	add    %ah,0x0(%rsp,%rsi,4)
 	...
 
 00000000646ca4c8 <.pdata>:
-    646ca4c8:	adc    %ah,0x0(%rbp)
-    646ca4cb:	add    %ah,0x0(%rbp,%riz,2)
-    646ca4cf:	add    %ah,-0x4c(%rax)
-	...
+    646ca4c8:	nop
+    646ca4c9:	add    %al,%gs:(%rax)
+    646ca4cc:	xchg   %eax,%esi
+    646ca4cd:	add    %al,%gs:(%rax)
+    646ca4d0:	push   $0xffffffffa00000b4
 
 00000000646ca4d4 <.pdata>:
-    646ca4d4:	jo     646ca53b <.pdata+0x13>
-    646ca4d6:	add    %al,(%rax)
-    646ca4d8:	xchg   %eax,%esi
-    646ca4d9:	data16 add %al,(%rax)
-    646ca4dc:	fs mov $0x0,%ah
+    646ca4d4:	movabs 0x6c000065f4000065,%al
+    646ca4dd:	mov    $0x0,%ah
 	...
 
 00000000646ca4e0 <.pdata>:
-    646ca4e0:	movabs 0x70000066a5000066,%al
-    646ca4e9:	mov    $0x0,%ah
+    646ca4e0:	add    %ah,0x0(%rsi)
+    646ca4e3:	add    %ah,(%rsi)
+    646ca4e5:	add    %al,(%eax)
+    646ca4e8:	jo     646ca49e <.pdata+0x5a>
 	...
 
 00000000646ca4ec <.pdata>:
-    646ca4ec:	mov    $0x66,%al
-    646ca4ee:	add    %al,(%rax)
-    646ca4f0:	xchg   %esp,0x0(%rdi)
-    646ca4f3:	add    %dh,0x0(%rsp,%rsi,4)
+    646ca4ec:	xor    %ah,0x0(%rdi)
+    646ca4ef:	add    %dh,0x7c000067(%rip)        # e06ca55c <.debug_str+0x7bff255c>
+    646ca4f5:	mov    $0x0,%ah
 	...
 
 00000000646ca4f8 <.pdata>:
-    646ca4f8:	nop
+    646ca4f8:	rex
     646ca4f9:	add    %al,(%eax)
-    646ca4fc:	test   %ch,0x0(%rax)
-    646ca4ff:	add    %bh,-0x4c(%rax)
+    646ca4fc:	(bad)
+    646ca4fd:	push   $0xffffffffb4800000
 	...
 
 00000000646ca504 <.pdata>:
-    646ca504:	shrb   $0x0,0x0(%rax)
-    646ca508:	movsb  %ds:(%rsi),%es:(%rdi)
-    646ca509:	push   $0x0
-    646ca50b:	add    %al,0x6ab00000(%rsp,%rsi,4)
+    646ca504:	and    %ch,0x0(%rax)
+    646ca507:	add    %dl,(%rcx,%rbp,2)
+    646ca50a:	add    %al,(%rax)
+    646ca50c:	test   %dh,0x695000(%rax,%rax,1)
 
 00000000646ca510 <.pdata>:
-    646ca510:	mov    $0x6a,%al
-    646ca512:	add    %al,(%rax)
-    646ca514:	shrb   0x0(%rbx)
-    646ca517:	add    %dl,-0x2fffff4c(%rax)
+    646ca510:	push   %rax
+    646ca511:	imul   $0x6b3400,(%rax),%eax
+    646ca517:	add    %dl,0x400000b4(%rax)
 
 00000000646ca51c <.pdata>:
-    646ca51c:	shrb   0x0(%rbx)
-    646ca51f:	add    %ah,0x6c(%rsi)
+    646ca51c:	rex imul $0x0,(%rax),%eax
+    646ca520:	(bad)
+    646ca521:	insb   (%dx),%es:(%rdi)
     646ca522:	add    %al,(%rax)
     646ca524:	pushf
     646ca525:	mov    $0x0,%ah
 	...
 
 00000000646ca528 <.pdata>:
-    646ca528:	jo     646ca596 <.pdata+0xe>
+    646ca528:	(bad)
+    646ca529:	insb   (%dx),%es:(%rdi)
     646ca52a:	add    %al,(%rax)
-    646ca52c:	(bad)
-    646ca52d:	jno    646ca52f <.pdata+0x7>
-    646ca52f:	add    %ah,0x71d00000(%rsp,%rsi,4)
-    646ca536:	add    %al,(%rax)
-    646ca538:	rex.WRX je 646ca53b <.pdata+0x13>
-    646ca53b:	add    %al,%al
-    646ca53d:	mov    $0x0,%ah
+    646ca52c:	imulb  0x0(%rax,%rax,1)
+    646ca530:	test   $0xb4,%al
 	...
 
-00000000646ca540 <.pdata>:
-    646ca540:	and    %dh,0x0(%rbp)
+00000000646ca534 <.pdata>:
+    646ca534:	add    %ch,0x0(%rbp)
+    646ca537:	add    %dl,0x72(%rdi)
+    646ca53a:	add    %al,(%rax)
+    646ca53c:	mov    $0xb4,%al
+    646ca53e:	add    %al,(%rax)
+    646ca540:	(bad)
+    646ca541:	jb     646ca543 <.pdata+0xf>
     646ca543:	add    %bl,%dh
-    646ca545:	jne    646ca547 <.pdata+0x7>
+    646ca545:	je     646ca547 <.pdata+0x13>
     646ca547:	add    %cl,%ah
     646ca549:	mov    $0x0,%ah
 	...
 
 00000000646ca54c <.pdata>:
-    646ca54c:	add    %dh,0x0(%rdi)
-    646ca54f:	add    %ah,-0x2bffff89(%rip)        # 386ca5cc <__size_of_stack_reserve__+0x384ca5cc>
+    646ca54c:	mov    $0x75,%al
+    646ca54e:	add    %al,(%rax)
+    646ca550:	outsb  %ds:(%rsi),(%dx)
+    646ca551:	jbe    646ca553 <.pdata+0x7>
+    646ca553:	add    %bl,%al
     646ca555:	mov    $0x0,%ah
 	...
 
 00000000646ca558 <.pdata>:
-    646ca558:	xor    %dh,0x0(%rdi)
-    646ca55b:	add    %bh,%al
-    646ca55d:	ja     646ca55f <.pdata+0x7>
-    646ca55f:	add    %bl,%al
+    646ca558:	nop
+    646ca559:	ja     646ca55b <.pdata+0x3>
+    646ca55b:	add    %dh,-0x1fffff89(%rbp)
     646ca561:	mov    $0x0,%ah
-    646ca563:	add    %al,(%rax)
-    646ca565:	js     646ca567 <.pdata+0xf>
-    646ca567:	add    %ch,0x78(%rdi)
-    646ca56a:	add    %al,(%rax)
-    646ca56c:	call   d46ca625 <.debug_str+0x6fff2625>
-    646ca571:	js     646ca573 <.pdata+0x1b>
-    646ca573:	add    %cl,-0xbffff88(%rdi)
-    646ca579:	mov    $0x0,%ah
 	...
 
-00000000646ca57c <.pdata>:
-    646ca57c:	(bad)
-    646ca57d:	jns    646ca57f <.pdata+0x3>
-    646ca57f:	add    %ah,-0x3ffff87(%rcx)
-    646ca585:	mov    $0x0,%ah
+00000000646ca564 <.pdata>:
+    646ca564:	shlb   $0x0,0x0(%rdi)
+    646ca568:	mov    %bh,0x0(%rax)
+    646ca56b:	add    %ah,%ah
+    646ca56d:	mov    $0x0,%ah
+    646ca56f:	add    %dl,-0xffff88(%rax)
+    646ca575:	js     646ca577 <.pdata+0x13>
+    646ca577:	add    %dh,%ah
+    646ca579:	mov    $0x0,%ah
+    646ca57b:	add    %al,(%rax)
+    646ca57d:	jns    646ca57f <.pdata+0x1b>
+    646ca57f:	add    %bl,(%rdi)
+    646ca581:	jns    646ca583 <.pdata+0x1f>
+    646ca583:	add    %al,(%rax)
+    646ca585:	mov    $0x0,%ch
 	...
 
 00000000646ca588 <.pdata>:
-    646ca588:	mov    $0x79,%al
-    646ca58a:	add    %al,(%rax)
-    646ca58c:	mov    $0x4000079,%esp
+    646ca588:	lock jns 646ca58b <.pdata+0x3>
+    646ca58b:	add    %dh,(%rcx)
+    646ca58d:	jp     646ca58f <.pdata+0x7>
+    646ca58f:	add    %cl,(%rax)
     646ca591:	mov    $0x0,%ch
-    646ca593:	add    %al,%al
-    646ca595:	jns    646ca597 <.pdata+0xf>
-    646ca597:	add    %bh,-0x4af80000(%rdx,%rdi,2)
-    646ca59e:	add    %al,(%rax)
-    646ca5a0:	sarb   0x0(%rdx)
-    646ca5a3:	add    %bh,(%rcx)
-    646ca5a5:	jnp    646ca5a7 <.pdata+0x1f>
-    646ca5a7:	add    %cl,0x400000b3(%rax)
-
-00000000646ca5ac <.pdata.startup>:
-    646ca5ac:	rex jnp 646ca5af <.pdata.startup+0x3>
-    646ca5af:	add    %al,0x7b(%rbp)
-    646ca5b2:	add    %al,(%rax)
-    646ca5b4:	.byte 0x20
-    646ca5b5:	mov    $0x0,%ch
+	...
+
+00000000646ca594 <.pdata>:
+    646ca594:	rex jp 646ca597 <.pdata+0x3>
+    646ca597:	add    %cl,0x0(%rdx,%rdi,2)
+    646ca59b:	add    %dl,(%rax)
+    646ca59d:	mov    $0x0,%ch
+    646ca59f:	add    %dl,0x7a(%rax)
+    646ca5a2:	add    %al,(%rax)
+    646ca5a4:	rex.WR jnp 646ca5a7 <.pdata+0x13>
+    646ca5a7:	add    %dl,0x7b600000(,%rsi,4)
+    646ca5ae:	add    %al,(%rax)
+    646ca5b0:	leave
+    646ca5b1:	jnp    646ca5b3 <.pdata+0x1f>
+    646ca5b3:	add    %dl,0x7bd00000(%rbx,%rsi,4)
+
+00000000646ca5b8 <.pdata.startup>:
+    646ca5b8:	sarb   0x0(%rbx)
+    646ca5bb:	add    %dl,%ch
+    646ca5bd:	jnp    646ca5bf <.pdata.startup+0x7>
+    646ca5bf:	.byte 0x0
+    646ca5c0:	sub    $0xb5,%al
 	...
 
 Disassembly of section .xdata:
 
 00000000646cb000 <.xdata>:
     646cb000:	add    %eax,(%rax)
     646cb002:	add    %al,(%rax)
@@ -12457,289 +12500,293 @@
     646cb2fd:	or     %al,(%rbx)
     646cb2ff:	add    $0x3045208,%eax
     646cb304:	add    %edx,0x0(%rax)
     646cb307:	add    %al,(%rcx)
     646cb309:	or     %al,(%rbx)
     646cb30b:	add    $0x3045208,%eax
     646cb310:	add    %edx,0x0(%rax)
+    646cb313:	add    %al,(%rcx)
+    646cb315:	or     %al,(%rbx)
+    646cb317:	add    $0x3045208,%eax
+    646cb31c:	add    %edx,0x0(%rax)
+	...
+
+00000000646cb320 <.xdata>:
+    646cb320:	add    %edx,(%rcx)
+    646cb322:	add    $0x9031185,%eax
+    646cb327:	add    %edx,(%rdi)
+    646cb329:	add    %al,(%rdx)
+    646cb32b:	xor    %al,(%rcx)
+    646cb32d:	push   %rax
+    646cb32e:	add    %al,(%rax)
+    646cb330:	add    %ecx,(%rax)
+    646cb332:	add    0x3047208(%rip),%eax        # 67712540 <.debug_str+0x303a540>
+    646cb338:	add    %edx,0x0(%rax)
+	...
+
+00000000646cb33c <.xdata>:
+    646cb33c:	add    %eax,(%rcx,%rax,1)
+    646cb33f:	add    %al,(%rdx,%rax,2)
+    646cb342:	add    %al,(%rax)
+    646cb344:	add    %eax,(%rsi)
+    646cb346:	add    (%rax),%eax
+    646cb348:	(bad)
+    646cb349:	rex.X add (%rax),%sil
+    646cb34c:	add    %esp,0x0(%rax)
+    646cb34f:	add    %al,(%rcx)
+    646cb351:	add    %al,(%rax)
+	...
+
+00000000646cb354 <.xdata>:
+    646cb354:	add    %ecx,(%rdx)
+    646cb356:	(bad)
+    646cb357:	add    %cl,(%rdx)
+    646cb359:	push   %rdx
+    646cb35a:	(bad)
+    646cb35b:	xor    %al,0x3700460(%rip)        # 67dcb7c1 <.debug_str+0x36f37c1>
+    646cb361:	push   %rax
+    646cb362:	add    %al,%al
+    646cb364:	add    %ecx,(%rdx)
+    646cb366:	add    $0x6d20a05,%eax
+    646cb36b:	add    (%rbx),%eax
+    646cb36d:	xor    %al,(%rdx)
+    646cb36f:	(bad)
+    646cb370:	add    %edx,0x0(%rax)
+	...
+
+00000000646cb374 <.xdata>:
+    646cb374:	add    %eax,(%rcx,%rax,1)
+    646cb377:	add    %al,(%rdx,%rax,2)
+    646cb37a:	add    %al,(%rax)
+    646cb37c:	add    %eax,(%rsi)
+    646cb37e:	add    (%rax),%eax
+    646cb380:	(bad)
+    646cb381:	rex.X add (%rax),%sil
+    646cb384:	add    %esp,0x0(%rax)
+    646cb387:	add    %al,(%rcx)
+    646cb389:	add    %al,(%rax)
+	...
+
+00000000646cb38c <.xdata>:
+    646cb38c:	add    %eax,(%rax)
+    646cb38e:	add    %al,(%rax)
+    646cb390:	add    %eax,(%rax)
+	...
+
+00000000646cb394 <.xdata.unlikely>:
+    646cb394:	add    %eax,(%rsi)
+    646cb396:	add    (%rax),%eax
+    646cb398:	(bad)
+    646cb399:	(bad)
+    646cb39b:	xor    %al,(%rcx)
+    646cb39d:	(bad)
+	...
+
+00000000646cb3a0 <.xdata>:
+    646cb3a0:	add    %ecx,(%rdx)
+    646cb3a2:	(bad)
+    646cb3a3:	add    %cl,(%rdx)
+    646cb3a5:	xchg   %eax,%edx
+    646cb3a6:	(bad)
+    646cb3a7:	xor    %al,0x3700460(%rip)        # 67dcb80d <.debug_str+0x36f380d>
+    646cb3ad:	push   %rax
+    646cb3ae:	add    %al,%al
+    646cb3b0:	add    %ebx,(%rax)
+    646cb3b2:	or     0x62100318(%rbp),%al
+    646cb3b8:	or     $0x30,%al
+    646cb3ba:	or     0xa(%rax),%esp
+    646cb3bd:	jo     646cb3c8 <.xdata>
+    646cb3bf:	rolb   $0xd0,(%rdi)
+    646cb3c2:	add    $0x1f003e0,%eax
+    646cb3c7:	push   %rax
+
+00000000646cb3c8 <.xdata>:
+    646cb3c8:	add    %eax,(%rcx,%rax,1)
+    646cb3cb:	add    %al,(%rdx,%rax,2)
+    646cb3ce:	add    %al,(%rax)
+    646cb3d0:	add    %ecx,(%rdx)
+    646cb3d2:	(bad)
+    646cb3d3:	add    %cl,(%rdx)
+    646cb3d5:	xor    (%rsi),%al
+    646cb3d7:	xor    %al,0x3700460(%rip)        # 67dcb83d <.debug_str+0x36f383d>
+    646cb3dd:	push   %rax
+    646cb3de:	add    %al,%al
+    646cb3e0:	add    %eax,0x32050002(%rip)        # 9671b3e8 <.debug_str+0x320433e8>
+    646cb3e6:	add    %esi,(%rax)
+
+00000000646cb3e8 <.xdata>:
+    646cb3e8:	add    %ecx,(%rax)
+    646cb3ea:	add    $0x4420800,%eax
+    646cb3ef:	xor    %al,(%rbx)
+    646cb3f1:	(bad)
+    646cb3f2:	add    0x1(%rax),%dh
+    646cb3f5:	push   %rax
+    646cb3f6:	add    %al,(%rax)
+    646cb3f8:	add    %ecx,(%rax)
+    646cb3fa:	add    $0x4420800,%eax
+    646cb3ff:	xor    %al,(%rbx)
+    646cb401:	(bad)
+    646cb402:	add    0x1(%rax),%dh
+    646cb405:	push   %rax
+    646cb406:	add    %al,(%rax)
+    646cb408:	add    %eax,0x32050002(%rip)        # 9671b410 <.debug_str+0x32043410>
+    646cb40e:	add    %esi,(%rax)
+    646cb410:	add    %eax,0x32050002(%rip)        # 9671b418 <.debug_str+0x32043418>
+    646cb416:	add    %esi,(%rax)
+
+00000000646cb418 <.xdata>:
+    646cb418:	add    %eax,(%rax)
+    646cb41a:	add    %al,(%rax)
+    646cb41c:	add    %eax,(%rax)
+    646cb41e:	add    %al,(%rax)
+    646cb420:	add    %eax,(%rax)
+    646cb422:	add    %al,(%rax)
+    646cb424:	add    %eax,(%rdi)
+    646cb426:	add    $0x0,%al
+    646cb428:	(bad)
+    646cb429:	xor    (%rbx),%al
+    646cb42b:	xor    %al,(%rdx)
+    646cb42d:	(bad)
+    646cb42e:	add    %esi,0x1(%rax)
+    646cb431:	add    $0x1,%al
+    646cb433:	add    %al,(%rdx,%rax,2)
+    646cb436:	add    %al,(%rax)
+    646cb438:	add    %eax,(%rcx,%rax,1)
+    646cb43b:	add    %al,(%rdx,%rax,2)
+    646cb43e:	add    %al,(%rax)
+    646cb440:	add    %eax,(%rcx,%rax,1)
+    646cb443:	add    %al,(%rdx,%rax,2)
+    646cb446:	add    %al,(%rax)
+    646cb448:	add    %eax,(%rcx,%rax,1)
+    646cb44b:	add    %al,(%rdx,%rax,2)
+    646cb44e:	add    %al,(%rax)
+    646cb450:	add    %eax,(%rcx,%rax,1)
+    646cb453:	add    %al,(%rdx,%rax,2)
+    646cb456:	add    %al,(%rax)
+    646cb458:	add    %eax,(%rcx,%rax,1)
+    646cb45b:	add    %al,(%rdx,%rax,2)
 	...
 
-00000000646cb314 <.xdata>:
-    646cb314:	add    %edx,(%rcx)
-    646cb316:	add    $0x9031185,%eax
-    646cb31b:	add    %edx,(%rdi)
-    646cb31d:	add    %al,(%rdx)
-    646cb31f:	xor    %al,(%rcx)
-    646cb321:	push   %rax
-    646cb322:	add    %al,(%rax)
-    646cb324:	add    %ecx,(%rax)
-    646cb326:	add    0x3047208(%rip),%eax        # 67712534 <.debug_str+0x303a534>
-    646cb32c:	add    %edx,0x0(%rax)
-	...
-
-00000000646cb330 <.xdata>:
-    646cb330:	add    %eax,(%rcx,%rax,1)
-    646cb333:	add    %al,(%rdx,%rax,2)
-    646cb336:	add    %al,(%rax)
-    646cb338:	add    %eax,(%rsi)
-    646cb33a:	add    (%rax),%eax
-    646cb33c:	(bad)
-    646cb33d:	rex.X add (%rax),%sil
-    646cb340:	add    %esp,0x0(%rax)
-    646cb343:	add    %al,(%rcx)
-    646cb345:	add    %al,(%rax)
-	...
-
-00000000646cb348 <.xdata>:
-    646cb348:	add    %ecx,(%rdx)
-    646cb34a:	(bad)
-    646cb34b:	add    %cl,(%rdx)
-    646cb34d:	push   %rdx
-    646cb34e:	(bad)
-    646cb34f:	xor    %al,0x3700460(%rip)        # 67dcb7b5 <.debug_str+0x36f37b5>
-    646cb355:	push   %rax
-    646cb356:	add    %al,%al
-    646cb358:	add    %ecx,(%rdx)
-    646cb35a:	add    $0x6d20a05,%eax
-    646cb35f:	add    (%rbx),%eax
-    646cb361:	xor    %al,(%rdx)
-    646cb363:	(bad)
-    646cb364:	add    %edx,0x0(%rax)
-	...
-
-00000000646cb368 <.xdata>:
-    646cb368:	add    %eax,(%rcx,%rax,1)
-    646cb36b:	add    %al,(%rdx,%rax,2)
-    646cb36e:	add    %al,(%rax)
-    646cb370:	add    %eax,(%rsi)
-    646cb372:	add    (%rax),%eax
-    646cb374:	(bad)
-    646cb375:	rex.X add (%rax),%sil
-    646cb378:	add    %esp,0x0(%rax)
-    646cb37b:	add    %al,(%rcx)
-    646cb37d:	add    %al,(%rax)
-	...
-
-00000000646cb380 <.xdata>:
-    646cb380:	add    %eax,(%rax)
-    646cb382:	add    %al,(%rax)
-    646cb384:	add    %eax,(%rax)
-	...
-
-00000000646cb388 <.xdata.unlikely>:
-    646cb388:	add    %eax,(%rsi)
-    646cb38a:	add    (%rax),%eax
-    646cb38c:	(bad)
-    646cb38d:	(bad)
-    646cb38f:	xor    %al,(%rcx)
-    646cb391:	(bad)
-	...
-
-00000000646cb394 <.xdata>:
-    646cb394:	add    %ecx,(%rdx)
-    646cb396:	(bad)
-    646cb397:	add    %cl,(%rdx)
-    646cb399:	xchg   %eax,%edx
-    646cb39a:	(bad)
-    646cb39b:	xor    %al,0x3700460(%rip)        # 67dcb801 <.debug_str+0x36f3801>
-    646cb3a1:	push   %rax
-    646cb3a2:	add    %al,%al
-    646cb3a4:	add    %ebx,(%rax)
-    646cb3a6:	or     0x62100318(%rbp),%al
-    646cb3ac:	or     $0x30,%al
-    646cb3ae:	or     0xa(%rax),%esp
-    646cb3b1:	jo     646cb3bc <.xdata>
-    646cb3b3:	rolb   $0xd0,(%rdi)
-    646cb3b6:	add    $0x1f003e0,%eax
-    646cb3bb:	push   %rax
-
-00000000646cb3bc <.xdata>:
-    646cb3bc:	add    %eax,(%rcx,%rax,1)
-    646cb3bf:	add    %al,(%rdx,%rax,2)
-    646cb3c2:	add    %al,(%rax)
-    646cb3c4:	add    %ecx,(%rdx)
-    646cb3c6:	(bad)
-    646cb3c7:	add    %cl,(%rdx)
-    646cb3c9:	xor    (%rsi),%al
-    646cb3cb:	xor    %al,0x3700460(%rip)        # 67dcb831 <.debug_str+0x36f3831>
-    646cb3d1:	push   %rax
-    646cb3d2:	add    %al,%al
-    646cb3d4:	add    %eax,0x32050002(%rip)        # 9671b3dc <.debug_str+0x320433dc>
-    646cb3da:	add    %esi,(%rax)
-
-00000000646cb3dc <.xdata>:
-    646cb3dc:	add    %ecx,(%rax)
-    646cb3de:	add    $0x4420800,%eax
-    646cb3e3:	xor    %al,(%rbx)
-    646cb3e5:	(bad)
-    646cb3e6:	add    0x1(%rax),%dh
-    646cb3e9:	push   %rax
-    646cb3ea:	add    %al,(%rax)
-    646cb3ec:	add    %ecx,(%rax)
-    646cb3ee:	add    $0x4420800,%eax
-    646cb3f3:	xor    %al,(%rbx)
-    646cb3f5:	(bad)
-    646cb3f6:	add    0x1(%rax),%dh
-    646cb3f9:	push   %rax
-    646cb3fa:	add    %al,(%rax)
-    646cb3fc:	add    %eax,0x32050002(%rip)        # 9671b404 <.debug_str+0x32043404>
-    646cb402:	add    %esi,(%rax)
-    646cb404:	add    %eax,0x32050002(%rip)        # 9671b40c <.debug_str+0x3204340c>
-    646cb40a:	add    %esi,(%rax)
-
-00000000646cb40c <.xdata>:
-    646cb40c:	add    %eax,(%rax)
-    646cb40e:	add    %al,(%rax)
-    646cb410:	add    %eax,(%rax)
-    646cb412:	add    %al,(%rax)
-    646cb414:	add    %eax,(%rax)
-    646cb416:	add    %al,(%rax)
-    646cb418:	add    %eax,(%rdi)
-    646cb41a:	add    $0x0,%al
-    646cb41c:	(bad)
-    646cb41d:	xor    (%rbx),%al
-    646cb41f:	xor    %al,(%rdx)
-    646cb421:	(bad)
-    646cb422:	add    %esi,0x1(%rax)
-    646cb425:	add    $0x1,%al
-    646cb427:	add    %al,(%rdx,%rax,2)
-    646cb42a:	add    %al,(%rax)
-    646cb42c:	add    %eax,(%rcx,%rax,1)
-    646cb42f:	add    %al,(%rdx,%rax,2)
-    646cb432:	add    %al,(%rax)
-    646cb434:	add    %eax,(%rcx,%rax,1)
-    646cb437:	add    %al,(%rdx,%rax,2)
-    646cb43a:	add    %al,(%rax)
-    646cb43c:	add    %eax,(%rcx,%rax,1)
-    646cb43f:	add    %al,(%rdx,%rax,2)
-    646cb442:	add    %al,(%rax)
-    646cb444:	add    %eax,(%rcx,%rax,1)
-    646cb447:	add    %al,(%rdx,%rax,2)
-    646cb44a:	add    %al,(%rax)
-    646cb44c:	add    %eax,(%rcx,%rax,1)
-    646cb44f:	add    %al,(%rdx,%rax,2)
-	...
-
-00000000646cb454 <.xdata>:
-    646cb454:	add    %eax,(%rax)
+00000000646cb460 <.xdata>:
+    646cb460:	add    %eax,(%rax)
 	...
 
-00000000646cb458 <.xdata>:
-    646cb458:	add    %eax,(%rax)
+00000000646cb464 <.xdata>:
+    646cb464:	add    %eax,(%rax)
 	...
 
-00000000646cb45c <.xdata>:
-    646cb45c:	add    %eax,(%rax)
+00000000646cb468 <.xdata>:
+    646cb468:	add    %eax,(%rax)
 	...
 
-00000000646cb460 <.xdata>:
-    646cb460:	add    %eax,(%rax)
+00000000646cb46c <.xdata>:
+    646cb46c:	add    %eax,(%rax)
 	...
 
-00000000646cb464 <.xdata>:
-    646cb464:	add    %ecx,(%rdx)
-    646cb466:	add    $0x0,%al
-    646cb468:	or     0x4(%rax),%ch
-    646cb46b:	add    %al,0x1300192(%rip)        # 659cb603 <.debug_str+0x12f3603>
-
 00000000646cb470 <.xdata>:
-    646cb470:	add    %eax,(%rax)
-	...
+    646cb470:	add    %ecx,(%rdx)
+    646cb472:	add    $0x0,%al
+    646cb474:	or     0x4(%rax),%ch
+    646cb477:	add    %al,0x1300192(%rip)        # 659cb60f <.debug_str+0x12f360f>
 
-00000000646cb474 <.xdata>:
-    646cb474:	add    %eax,(%rax)
+00000000646cb47c <.xdata>:
+    646cb47c:	add    %eax,(%rax)
 	...
 
-00000000646cb478 <.xdata>:
-    646cb478:	add    %ecx,(%rdx)
-    646cb47a:	add    $0x0,%al
-    646cb47c:	or     0x6(%rax),%ch
-    646cb47f:	add    %al,0x13001d2(%rip)        # 659cb657 <.debug_str+0x12f3657>
+00000000646cb480 <.xdata>:
+    646cb480:	add    %eax,(%rax)
+	...
 
 00000000646cb484 <.xdata>:
     646cb484:	add    %ecx,(%rdx)
     646cb486:	add    $0x0,%al
-    646cb488:	or     0x4(%rax),%ch
-    646cb48b:	add    %al,0x1300192(%rip)        # 659cb623 <.debug_str+0x12f3623>
+    646cb488:	or     0x6(%rax),%ch
+    646cb48b:	add    %al,0x13001d2(%rip)        # 659cb663 <.debug_str+0x12f3663>
 
 00000000646cb490 <.xdata>:
     646cb490:	add    %ecx,(%rdx)
     646cb492:	add    $0x0,%al
-    646cb494:	or     0x6(%rax),%ch
-    646cb497:	add    %al,0x13001d2(%rip)        # 659cb66f <.debug_str+0x12f366f>
+    646cb494:	or     0x4(%rax),%ch
+    646cb497:	add    %al,0x1300192(%rip)        # 659cb62f <.debug_str+0x12f362f>
 
 00000000646cb49c <.xdata>:
-    646cb49c:	add    %eax,(%rcx,%rax,1)
-    646cb49f:	add    %al,(%rdx,%riz,1)
-    646cb4a2:	add    %al,(%rax)
-    646cb4a4:	add    %ebx,(%rdx)
-    646cb4a6:	or     (%rax),%eax
-    646cb4a8:	sbb    0x8(%rax),%bh
-    646cb4ab:	add    %dl,(%rdx)
-    646cb4ad:	push   $0x10d0007
-    646cb4b2:	adc    (%rax),%al
-    646cb4b4:	(bad)
-    646cb4b5:	xor    %al,0x3700460(%rip)        # 67dcb91b <.debug_str+0x36f391b>
-    646cb4bb:	push   %rax
-    646cb4bc:	add    %al,%al
-	...
-
-00000000646cb4c0 <.xdata>:
-    646cb4c0:	add    %ecx,(%rcx)
-    646cb4c2:	add    (%rax),%eax
-    646cb4c4:	or     %ebp,0x4(%rax)
-    646cb4c7:	add    %al,(%rdx,%riz,4)
+    646cb49c:	add    %ecx,(%rdx)
+    646cb49e:	add    $0x0,%al
+    646cb4a0:	or     0x6(%rax),%ch
+    646cb4a3:	add    %al,0x13001d2(%rip)        # 659cb67b <.debug_str+0x12f367b>
+
+00000000646cb4a8 <.xdata>:
+    646cb4a8:	add    %eax,(%rcx,%rax,1)
+    646cb4ab:	add    %al,(%rdx,%riz,1)
+    646cb4ae:	add    %al,(%rax)
+    646cb4b0:	add    %ebx,(%rdx)
+    646cb4b2:	or     (%rax),%eax
+    646cb4b4:	sbb    0x8(%rax),%bh
+    646cb4b7:	add    %dl,(%rdx)
+    646cb4b9:	push   $0x10d0007
+    646cb4be:	adc    (%rax),%al
+    646cb4c0:	(bad)
+    646cb4c1:	xor    %al,0x3700460(%rip)        # 67dcb927 <.debug_str+0x36f3927>
+    646cb4c7:	push   %rax
+    646cb4c8:	add    %al,%al
 	...
 
 00000000646cb4cc <.xdata>:
-    646cb4cc:	add    %eax,0x52050002(%rip)        # b671b4d4 <.debug_str+0x520434d4>
-    646cb4d2:	add    %esi,(%rax)
-
-00000000646cb4d4 <.xdata>:
-    646cb4d4:	add    %eax,(%rax)
-    646cb4d6:	add    %al,(%rax)
-    646cb4d8:	add    %ecx,(%rax)
-    646cb4da:	add    $0x4420800,%eax
-    646cb4df:	xor    %al,(%rbx)
-    646cb4e1:	(bad)
-    646cb4e2:	add    0x1(%rax),%dh
-    646cb4e5:	push   %rax
-    646cb4e6:	add    %al,(%rax)
-    646cb4e8:	add    %eax,(%rdi)
-    646cb4ea:	add    $0x0,%al
-    646cb4ec:	(bad)
-    646cb4ed:	xor    (%rbx),%al
-    646cb4ef:	xor    %al,(%rdx)
-    646cb4f1:	(bad)
-    646cb4f2:	add    %esi,0x1(%rax)
-
-00000000646cb4f4 <.xdata>:
-    646cb4f4:	add    %eax,0x32050002(%rip)        # 9671b4fc <.debug_str+0x320434fc>
-    646cb4fa:	add    %esi,(%rax)
-
-00000000646cb4fc <.xdata>:
-    646cb4fc:	add    %eax,(%rcx,%rax,1)
-    646cb4ff:	add    %al,(%rdx,%riz,4)
-    646cb502:	add    %al,(%rax)
-    646cb504:	add    %eax,(%rax)
-    646cb506:	add    %al,(%rax)
-    646cb508:	add    %edx,(%rsi)
-    646cb50a:	or     %eax,(%rax)
-    646cb50c:	(bad)
-    646cb50d:	mov    %al,(%rsi)
-    646cb50f:	add    %dl,(%rax)
-    646cb511:	js     646cb518 <.xdata+0x1c>
-    646cb513:	add    %cl,(%rbx)
-    646cb515:	push   $0xffffffffe2060004
-    646cb51a:	add    (%rax),%dh
-    646cb51c:	add    %esp,0x0(%rax)
+    646cb4cc:	add    %ecx,(%rcx)
+    646cb4ce:	add    (%rax),%eax
+    646cb4d0:	or     %ebp,0x4(%rax)
+    646cb4d3:	add    %al,(%rdx,%riz,4)
+	...
+
+00000000646cb4d8 <.xdata>:
+    646cb4d8:	add    %eax,0x52050002(%rip)        # b671b4e0 <.debug_str+0x520434e0>
+    646cb4de:	add    %esi,(%rax)
+
+00000000646cb4e0 <.xdata>:
+    646cb4e0:	add    %eax,(%rax)
+    646cb4e2:	add    %al,(%rax)
+    646cb4e4:	add    %ecx,(%rax)
+    646cb4e6:	add    $0x4420800,%eax
+    646cb4eb:	xor    %al,(%rbx)
+    646cb4ed:	(bad)
+    646cb4ee:	add    0x1(%rax),%dh
+    646cb4f1:	push   %rax
+    646cb4f2:	add    %al,(%rax)
+    646cb4f4:	add    %eax,(%rdi)
+    646cb4f6:	add    $0x0,%al
+    646cb4f8:	(bad)
+    646cb4f9:	xor    (%rbx),%al
+    646cb4fb:	xor    %al,(%rdx)
+    646cb4fd:	(bad)
+    646cb4fe:	add    %esi,0x1(%rax)
+
+00000000646cb500 <.xdata>:
+    646cb500:	add    %eax,0x32050002(%rip)        # 9671b508 <.debug_str+0x32043508>
+    646cb506:	add    %esi,(%rax)
+
+00000000646cb508 <.xdata>:
+    646cb508:	add    %eax,(%rcx,%rax,1)
+    646cb50b:	add    %al,(%rdx,%riz,4)
+    646cb50e:	add    %al,(%rax)
+    646cb510:	add    %eax,(%rax)
+    646cb512:	add    %al,(%rax)
+    646cb514:	add    %edx,(%rsi)
+    646cb516:	or     %eax,(%rax)
+    646cb518:	(bad)
+    646cb519:	mov    %al,(%rsi)
+    646cb51b:	add    %dl,(%rax)
+    646cb51d:	js     646cb524 <.xdata+0x1c>
+    646cb51f:	add    %cl,(%rbx)
+    646cb521:	push   $0xffffffffe2060004
+    646cb526:	add    (%rax),%dh
+    646cb528:	add    %esp,0x0(%rax)
 	...
 
-00000000646cb520 <.xdata.startup>:
-    646cb520:	add    %eax,(%rax)
+00000000646cb52c <.xdata.startup>:
+    646cb52c:	add    %eax,(%rax)
 	...
 
 Disassembly of section .bss:
 
 00000000646cc000 <__bss_start__>:
 	...
 
@@ -12892,33 +12939,37 @@
 	...
 
 Disassembly of section .edata:
 
 00000000646cd000 <.edata>:
     646cd000:	add    %al,(%rax)
     646cd002:	add    %al,(%rax)
-    646cd004:	ss loope 646cd07c <.edata+0x7c>
-    646cd007:	add    %al,%fs:(%rax)
+    646cd004:	rex.RXB (bad)
+    646cd006:	jg     646cd06c <.edata+0x6c>
+    646cd008:	add    %al,(%rax)
     646cd00a:	add    %al,(%rax)
-    646cd00c:	mov    %dl,%dl
-    646cd00e:	add    %al,(%rax)
-    646cd010:	add    %eax,(%rax)
-    646cd012:	add    %al,(%rax)
-    646cd014:	cmp    $0x3d000000,%eax
+    646cd00c:	xchg   %eax,%esp
+    646cd00d:	rolb   %cl,(%rax)
+    646cd00f:	add    %al,(%rcx)
+    646cd011:	add    %al,(%rax)
+    646cd013:	add    %bh,(%rsi)
+    646cd015:	add    %al,(%rax)
+    646cd017:	add    %bh,(%rsi)
     646cd019:	add    %al,(%rax)
     646cd01b:	add    %ch,(%rax)
     646cd01d:	rolb   (%rax)
-    646cd01f:	add    %bl,(%rcx,%rdx,8)
-    646cd022:	add    %al,(%rax)
-    646cd024:	adc    %dl,%dl
-    646cd026:	add    %al,(%rax)
-    646cd028:	sub    %eax,0x0(%rbx)
-    646cd02b:	add    %ah,%dl
-    646cd02d:	sbb    %al,(%rax)
-    646cd02f:	add    %al,(%rdi,%rdx,1)
+    646cd01f:	add    %ah,(%rax)
+    646cd021:	roll   (%rax)
+    646cd023:	add    %bl,(%rax)
+    646cd025:	rolb   %cl,(%rax)
+    646cd027:	add    %ch,(%rcx)
+    646cd029:	rex.XB add %al,(%r8)
+    646cd02c:	loop   646cd046 <.edata+0x46>
+    646cd02e:	add    %al,(%rax)
+    646cd030:	add    $0x17,%al
     646cd032:	add    %al,(%rax)
     646cd034:	mov    $0x13,%al
     646cd036:	add    %al,(%rax)
     646cd038:	rex.XB adc $0x278e0000,%eax
     646cd03e:	add    %al,(%rax)
     646cd040:	push   %rdx
     646cd041:	(bad)
@@ -12962,21 +13013,21 @@
     646cd094:	cs sub %eax,(%rax)
     646cd097:	add    %cl,0x0(%rcx,%rbp,1)
     646cd09b:	add    %ah,(%rdi,%rbp,1)
     646cd09e:	add    %al,(%rax)
     646cd0a0:	cs xor %al,(%rax)
     646cd0a3:	add    %al,%al
     646cd0a5:	cs add %al,(%rax)
-    646cd0a8:	addl   $0x38c700,0x0(%rbx)
-    646cd0af:	add    %bh,0x3a(%rbx)
-    646cd0b2:	add    %al,(%rax)
-    646cd0b4:	pop    %rbp
-    646cd0b5:	xor    (%rax),%al
-    646cd0b7:	add    %bl,0x1a00003f(%rax)
-    646cd0bd:	cmp    $0x0,%al
+    646cd0a8:	addl   $0x38d000,0x0(%rbx)
+    646cd0af:	add    %al,0x325d0000(%rdx,%rdi,1)
+    646cd0b6:	add    %al,(%rax)
+    646cd0b8:	cwtl
+    646cd0b9:	(bad)
+    646cd0ba:	add    %al,(%rax)
+    646cd0bc:	sbb    (%rax,%rax,1),%bh
     646cd0bf:	add    %dl,-0x51ffffbc(%rax)
     646cd0c5:	sub    (%rax),%al
     646cd0c7:	add    %bl,0x2d(%rsi)
     646cd0ca:	add    %al,(%rax)
     646cd0cc:	mov    $0x2d,%dl
     646cd0ce:	add    %al,(%rax)
     646cd0d0:	stos   %al,%es:(%rdi)
@@ -12988,692 +13039,698 @@
     646cd0dc:	xor    %ch,(%rdx)
     646cd0de:	add    %al,(%rax)
     646cd0e0:	(bad)
     646cd0e1:	cs add %al,(%rax)
     646cd0e4:	(bad)
     646cd0e5:	rex.WRB add %r8b,(%r8)
     646cd0e8:	fldl   0x0(%rbx)
-    646cd0eb:	add    %dl,%ch
-    646cd0ed:	rex.WRB add %r8b,(%r8)
-    646cd0f0:	rolb   0x0(%rsi)
-    646cd0f3:	add    %al,0x31000031(%rax)
-    646cd0f9:	xor    (%rax),%al
-    646cd0fb:	add    %bl,(%rdi)
-    646cd0fd:	add    %r8b,(%r8)
-    646cd100:	addb   $0x0,0x0(%rdi)
-    646cd104:	out    %al,$0x47
-    646cd106:	add    %al,(%rax)
-    646cd108:	or     0x0(%rax,%rax,1),%cl
-    646cd10c:	mov    $0x90000034,%ecx
-    646cd111:	rex.WR add %r8b,(%rax)
-    646cd114:	mov    $0x50,%dh
-    646cd116:	add    %al,(%rax)
-    646cd118:	rex
-    646cd119:	rex.WRX add %r8b,(%rax)
-    646cd11c:	xchg   %eax,%edi
-    646cd11d:	rolb   %cl,(%rax)
-    646cd11f:	add    %bl,-0x4effff2e(%rsi)
+    646cd0eb:	add    %bh,(%rcx)
+    646cd0ed:	rex.WRX add %r8b,(%rax)
+    646cd0f0:	(bad)
+    646cd0f1:	rex.WRB add %r8b,(%r8)
+    646cd0f4:	rolb   0x0(%rsi)
+    646cd0f7:	add    %al,0x31000031(%rax)
+    646cd0fd:	xor    (%rax),%al
+    646cd0ff:	add    %bl,(%rdi)
+    646cd101:	add    %r8b,(%r8)
+    646cd104:	addb   $0x0,0x0(%rdi)
+    646cd108:	out    %al,$0x47
+    646cd10a:	add    %al,(%rax)
+    646cd10c:	or     0x0(%rax,%rax,1),%cl
+    646cd110:	mov    $0x90000034,%ecx
+    646cd115:	rex.WR add %r8b,(%rax)
+    646cd118:	rex.RX push %rcx
+    646cd11a:	add    %al,(%rax)
+    646cd11c:	rorb   0x0(%rsi)
+    646cd11f:	add    %ah,-0x57ffff2e(%rcx)
     646cd125:	rolb   %cl,(%rax)
-    646cd127:	add    %al,%bl
-    646cd129:	rolb   %cl,(%rax)
-    646cd12b:	add    %dl,%bl
+    646cd127:	add    %bh,-0x32ffff2e(%rbx)
     646cd12d:	rolb   %cl,(%rax)
-    646cd12f:	add    %ch,%cl
+    646cd12f:	add    %bl,%ch
     646cd131:	rolb   %cl,(%rax)
-    646cd133:	add    %bh,%ch
+    646cd133:	add    %dh,%bl
     646cd135:	rolb   %cl,(%rax)
-    646cd137:	add    %dl,(%rax)
+    646cd137:	add    %al,(%rdi)
     646cd139:	roll   %cl,(%rax)
-    646cd13b:	add    %ah,(%rcx)
+    646cd13b:	add    %bl,(%rdx)
     646cd13d:	roll   %cl,(%rax)
-    646cd13f:	add    %bh,(%rax)
+    646cd13f:	add    %ch,(%rbx)
     646cd141:	roll   %cl,(%rax)
-    646cd143:	add    %cl,-0x2d(%rbx)
+    646cd143:	add    %al,-0x2d(%rdx)
     646cd146:	add    %al,(%rax)
-    646cd148:	pop    %rbp
+    646cd148:	push   %rbp
     646cd149:	roll   %cl,(%rax)
-    646cd14b:	add    %ch,-0x2d(%rbp)
+    646cd14b:	add    %ah,-0x2d(%rdi)
     646cd14e:	add    %al,(%rax)
-    646cd150:	adc    $0x0,%ebx
-    646cd153:	add    %dl,-0x57ffff2d(%rsi)
-    646cd159:	roll   %cl,(%rax)
-    646cd15b:	add    %bh,-0x31ffff2d(%rax)
+    646cd150:	ja     646cd125 <.edata+0x125>
+    646cd152:	add    %al,(%rax)
+    646cd154:	(bad)
+    646cd155:	roll   %cl,(%rax)
+    646cd157:	add    %ah,-0x4dffff2d(%rax)
+    646cd15d:	roll   %cl,(%rax)
+    646cd15f:	add    %al,%dl
     646cd161:	roll   %cl,(%rax)
-    646cd163:	add    %ah,%cl
+    646cd163:	add    %bl,%al
     646cd165:	roll   %cl,(%rax)
-    646cd167:	add    %dh,%bl
+    646cd167:	add    %ch,%bl
     646cd169:	roll   %cl,(%rax)
-    646cd16b:	add    %al,(%rbx)
-    646cd16d:	(bad)
-    646cd16e:	add    %al,(%rax)
-    646cd170:	adc    $0xd4,%al
-    646cd172:	add    %al,(%rax)
-    646cd174:	(bad)
+    646cd16b:	add    %bh,%ch
+    646cd16d:	roll   %cl,(%rax)
+    646cd16f:	add    %cl,0x1e0000d4(%rip)        # 826cd249 <.debug_str+0x1dff5249>
     646cd175:	(bad)
     646cd176:	add    %al,(%rax)
-    646cd178:	cmp    %edx,%esp
+    646cd178:	xor    %edx,%esp
     646cd17a:	add    %al,(%rax)
-    646cd17c:	rex.WB (bad)
+    646cd17c:	rex.XB (bad)
     646cd17e:	add    %al,(%rax)
-    646cd180:	pop    %rdi
+    646cd180:	push   %rbx
     646cd181:	(bad)
     646cd182:	add    %al,(%rax)
-    646cd184:	outsb  %ds:(%rsi),(%dx)
-    646cd185:	(bad)
-    646cd186:	add    %al,(%rax)
-    646cd188:	jl     646cd15e <.edata+0x15e>
+    646cd184:	imul   $0xd4780000,%esp,%edx
     646cd18a:	add    %al,(%rax)
-    646cd18c:	mov    %dl,%ah
+    646cd18c:	xchg   %dl,%ah
     646cd18e:	add    %al,(%rax)
-    646cd190:	xchg   %eax,%ebp
+    646cd190:	xchg   %eax,%edx
     646cd191:	(bad)
     646cd192:	add    %al,(%rax)
     646cd194:	lahf
     646cd195:	(bad)
     646cd196:	add    %al,(%rax)
-    646cd198:	stos   %eax,%es:(%rdi)
-    646cd199:	(bad)
-    646cd19a:	add    %al,(%rax)
-    646cd19c:	mov    $0xc30000d4,%edx
+    646cd198:	test   $0xb50000d4,%eax
+    646cd19d:	(bad)
+    646cd19e:	add    %al,(%rax)
+    646cd1a0:	(bad)
     646cd1a1:	(bad)
     646cd1a2:	add    %al,(%rax)
-    646cd1a4:	rcl    %esp
+    646cd1a4:	int    $0xd4
     646cd1a6:	add    %al,(%rax)
-    646cd1a8:	jrcxz  646cd17e <.edata+0x17e>
+    646cd1a8:	fcmovnbe %st(4),%st
     646cd1aa:	add    %al,(%rax)
-    646cd1ac:	not    %esp
+    646cd1ac:	in     (%dx),%eax
+    646cd1ad:	(bad)
     646cd1ae:	add    %al,(%rax)
-    646cd1b0:	or     %dl,%ch
+    646cd1b0:	add    %edx,%ebp
     646cd1b2:	add    %al,(%rax)
-    646cd1b4:	sbb    %ch,%dl
+    646cd1b4:	adc    %ch,%dl
     646cd1b6:	add    %al,(%rax)
-    646cd1b8:	and    $0x360000d5,%eax
+    646cd1b8:	and    $0xd5,%al
+    646cd1ba:	add    %al,(%rax)
+    646cd1bc:	(bad)
     646cd1bd:	(bad)
     646cd1be:	add    %al,(%rax)
-    646cd1c0:	rex.WB (bad)
+    646cd1c0:	rex (bad)
     646cd1c2:	add    %al,(%rax)
-    646cd1c4:	(bad)
+    646cd1c4:	push   %rbx
+    646cd1c5:	(bad)
     646cd1c6:	add    %al,(%rax)
-    646cd1c8:	je     646cd19f <.edata+0x19f>
+    646cd1c8:	insb   (%dx),%es:(%rdi)
+    646cd1c9:	(bad)
     646cd1ca:	add    %al,(%rax)
-    646cd1cc:	mov    %ss,%ebp
+    646cd1cc:	jle    646cd1a3 <.edata+0x1a3>
     646cd1ce:	add    %al,(%rax)
-    646cd1d0:	movsb  %ds:(%rsi),%es:(%rdi)
+    646cd1d0:	xchg   %eax,%esi
     646cd1d1:	(bad)
     646cd1d2:	add    %al,(%rax)
-    646cd1d4:	mov    $0xd5,%cl
+    646cd1d4:	scas   %es:(%rdi),%al
+    646cd1d5:	(bad)
     646cd1d6:	add    %al,(%rax)
-    646cd1d8:	(bad)
-    646cd1d9:	(bad)
-    646cd1da:	add    %al,(%rax)
-    646cd1dc:	rcl    %cl,%ebp
+    646cd1d8:	mov    $0xd10000d5,%ebx
+    646cd1dd:	(bad)
     646cd1de:	add    %al,(%rax)
-    646cd1e0:	(bad)
+    646cd1e0:	fst    %st(5)
     646cd1e2:	add    %al,(%rax)
-    646cd1e4:	in     $0xd5,%eax
+    646cd1e4:	jrcxz  646cd1bb <.edata+0x1bb>
     646cd1e6:	add    %al,(%rax)
-    646cd1e8:	lock (bad)
+    646cd1e8:	int1
+    646cd1e9:	(bad)
     646cd1ea:	add    %al,(%rax)
-    646cd1ec:	add    $0xd6,%al
+    646cd1ec:	std
+    646cd1ed:	(bad)
     646cd1ee:	add    %al,(%rax)
-    646cd1f0:	sbb    %dh,%dl
+    646cd1f0:	or     %dl,%dh
     646cd1f2:	add    %al,(%rax)
-    646cd1f4:	(bad)
-    646cd1f5:	(bad)
+    646cd1f4:	sbb    $0xd6,%al
     646cd1f6:	add    %al,(%rax)
     646cd1f8:	xor    %dh,%dl
     646cd1fa:	add    %al,(%rax)
-    646cd1fc:	cmp    $0xd6,%al
+    646cd1fc:	(bad)
+    646cd1fd:	(bad)
     646cd1fe:	add    %al,(%rax)
-    646cd200:	rex.WB (bad)
+    646cd200:	rex.WX (bad)
     646cd202:	add    %al,(%rax)
-    646cd204:	pop    %rax
+    646cd204:	push   %rsp
     646cd205:	(bad)
     646cd206:	add    %al,(%rax)
     646cd208:	(bad)
     646cd209:	(bad)
     646cd20a:	add    %al,(%rax)
-    646cd20c:	push   $0xffffffffffffffd6
+    646cd20c:	jo     646cd1e4 <.edata+0x1e4>
     646cd20e:	add    %al,(%rax)
-    646cd210:	add    %al,(%rax)
-    646cd212:	add    %eax,(%rax)
-    646cd214:	add    (%rax),%al
-    646cd216:	add    (%rax),%eax
-    646cd218:	add    $0x0,%al
-    646cd21a:	add    $0x7000600,%eax
-    646cd21f:	add    %cl,(%rax)
-    646cd221:	add    %cl,(%rcx)
-    646cd223:	add    %cl,(%rdx)
-    646cd225:	add    %cl,(%rbx)
-    646cd227:	add    %cl,(%rax,%rax,1)
-    646cd22a:	or     $0xf000e00,%eax
-    646cd22f:	add    %dl,(%rax)
-    646cd231:	add    %dl,(%rcx)
-    646cd233:	add    %dl,(%rdx)
-    646cd235:	add    %dl,(%rbx)
-    646cd237:	add    %dl,(%rax,%rax,1)
-    646cd23a:	adc    $0x17001600,%eax
-    646cd23f:	add    %bl,(%rax)
-    646cd241:	add    %bl,(%rcx)
-    646cd243:	add    %bl,(%rdx)
-    646cd245:	add    %bl,(%rbx)
-    646cd247:	add    %bl,(%rax,%rax,1)
-    646cd24a:	sbb    $0x1f001e00,%eax
-    646cd24f:	add    %ah,(%rax)
-    646cd251:	add    %ah,(%rcx)
-    646cd253:	add    %ah,(%rdx)
-    646cd255:	add    %ah,(%rbx)
-    646cd257:	add    %ah,(%rax,%rax,1)
-    646cd25a:	and    $0x27002600,%eax
-    646cd25f:	add    %ch,(%rax)
-    646cd261:	add    %ch,(%rcx)
-    646cd263:	add    %ch,(%rdx)
-    646cd265:	add    %ch,(%rbx)
-    646cd267:	add    %ch,(%rax,%rax,1)
-    646cd26a:	sub    $0x2f002e00,%eax
-    646cd26f:	add    %dh,(%rax)
-    646cd271:	add    %dh,(%rcx)
-    646cd273:	add    %dh,(%rdx)
-    646cd275:	add    %dh,(%rbx)
-    646cd277:	add    %dh,(%rax,%rax,1)
-    646cd27a:	xor    $0x37003600,%eax
-    646cd27f:	add    %bh,(%rax)
-    646cd281:	add    %bh,(%rcx)
-    646cd283:	add    %bh,(%rdx)
-    646cd285:	add    %bh,(%rbx)
-    646cd287:	add    %bh,(%rax,%rax,1)
-    646cd28a:	jne    646cd2ef <.edata+0x2ef>
-    646cd28c:	pop    %rdi
-    646cd28d:	jae    646cd2f6 <.edata+0x2f6>
-    646cd28f:	jae    646cd2fa <.edata+0x2fa>
-    646cd291:	insl   (%dx),%es:(%rdi)
-    646cd292:	cs fs insb (%dx),%es:(%rdi)
-    646cd295:	insb   (%dx),%es:(%rdi)
-    646cd296:	add    %ah,0x72(%rcx)
-    646cd299:	(bad)
-    646cd29a:	outsb  %ds:(%rsi),(%dx)
-    646cd29b:	add    %ah,%gs:0x5f(%ebx)
-    646cd2a0:	(bad)
-    646cd2a1:	jb     646cd315 <.edata+0x315>
+    646cd210:	jns    646cd1e8 <.edata+0x1e8>
+    646cd212:	add    %al,(%rax)
+    646cd214:	(bad)
+    646cd215:	(bad)
+    646cd216:	add    %al,(%rax)
+    646cd218:	add    %al,(%rax)
+    646cd21a:	add    %eax,(%rax)
+    646cd21c:	add    (%rax),%al
+    646cd21e:	add    (%rax),%eax
+    646cd220:	add    $0x0,%al
+    646cd222:	add    $0x7000600,%eax
+    646cd227:	add    %cl,(%rax)
+    646cd229:	add    %cl,(%rcx)
+    646cd22b:	add    %cl,(%rdx)
+    646cd22d:	add    %cl,(%rbx)
+    646cd22f:	add    %cl,(%rax,%rax,1)
+    646cd232:	or     $0xf000e00,%eax
+    646cd237:	add    %dl,(%rax)
+    646cd239:	add    %dl,(%rcx)
+    646cd23b:	add    %dl,(%rdx)
+    646cd23d:	add    %dl,(%rbx)
+    646cd23f:	add    %dl,(%rax,%rax,1)
+    646cd242:	adc    $0x17001600,%eax
+    646cd247:	add    %bl,(%rax)
+    646cd249:	add    %bl,(%rcx)
+    646cd24b:	add    %bl,(%rdx)
+    646cd24d:	add    %bl,(%rbx)
+    646cd24f:	add    %bl,(%rax,%rax,1)
+    646cd252:	sbb    $0x1f001e00,%eax
+    646cd257:	add    %ah,(%rax)
+    646cd259:	add    %ah,(%rcx)
+    646cd25b:	add    %ah,(%rdx)
+    646cd25d:	add    %ah,(%rbx)
+    646cd25f:	add    %ah,(%rax,%rax,1)
+    646cd262:	and    $0x27002600,%eax
+    646cd267:	add    %ch,(%rax)
+    646cd269:	add    %ch,(%rcx)
+    646cd26b:	add    %ch,(%rdx)
+    646cd26d:	add    %ch,(%rbx)
+    646cd26f:	add    %ch,(%rax,%rax,1)
+    646cd272:	sub    $0x2f002e00,%eax
+    646cd277:	add    %dh,(%rax)
+    646cd279:	add    %dh,(%rcx)
+    646cd27b:	add    %dh,(%rdx)
+    646cd27d:	add    %dh,(%rbx)
+    646cd27f:	add    %dh,(%rax,%rax,1)
+    646cd282:	xor    $0x37003600,%eax
+    646cd287:	add    %bh,(%rax)
+    646cd289:	add    %bh,(%rcx)
+    646cd28b:	add    %bh,(%rdx)
+    646cd28d:	add    %bh,(%rbx)
+    646cd28f:	add    %bh,(%rax,%rax,1)
+    646cd292:	cmp    $0x5f637500,%eax
+    646cd297:	jae    646cd300 <.edata+0x300>
+    646cd299:	jae    646cd304 <.edata+0x304>
+    646cd29b:	insl   (%dx),%es:(%rdi)
+    646cd29c:	cs fs insb (%dx),%es:(%rdi)
+    646cd29f:	insb   (%dx),%es:(%rdi)
+    646cd2a0:	add    %ah,0x72(%rcx)
     646cd2a3:	(bad)
-    646cd2a4:	jns    646cd305 <.edata+0x305>
-    646cd2a6:	insl   (%dx),%es:(%rdi)
-    646cd2a7:	(bad)
-    646cd2a8:	js     646cd309 <.edata+0x309>
-    646cd2aa:	outsl  %fs:(%rsi),(%dx)
-    646cd2ac:	jne    646cd310 <.edata+0x310>
-    646cd2ae:	insb   (%dx),%es:(%rdi)
-    646cd2af:	add    %ah,%gs:0x5f(%rbx)
-    646cd2b3:	(bad)
-    646cd2b4:	jb     646cd328 <.edata+0x328>
-    646cd2b6:	(bad)
-    646cd2b7:	jns    646cd318 <.edata+0x318>
-    646cd2b9:	insl   (%dx),%es:(%rdi)
-    646cd2ba:	(bad)
-    646cd2bb:	js     646cd31c <.edata+0x31c>
-    646cd2bd:	data16 insb (%dx),%es:(%rdi)
-    646cd2bf:	outsl  %ds:(%rsi),(%dx)
+    646cd2a4:	outsb  %ds:(%rsi),(%dx)
+    646cd2a5:	add    %ah,%gs:0x5f(%ebx)
+    646cd2aa:	(bad)
+    646cd2ab:	jb     646cd31f <.edata+0x31f>
+    646cd2ad:	(bad)
+    646cd2ae:	jns    646cd30f <.edata+0x30f>
+    646cd2b0:	insl   (%dx),%es:(%rdi)
+    646cd2b1:	(bad)
+    646cd2b2:	js     646cd313 <.edata+0x313>
+    646cd2b4:	outsl  %fs:(%rsi),(%dx)
+    646cd2b6:	jne    646cd31a <.edata+0x31a>
+    646cd2b8:	insb   (%dx),%es:(%rdi)
+    646cd2b9:	add    %ah,%gs:0x5f(%rbx)
+    646cd2bd:	(bad)
+    646cd2be:	jb     646cd332 <.edata+0x332>
     646cd2c0:	(bad)
-    646cd2c1:	je     646cd2c3 <.edata+0x2c3>
-    646cd2c3:	movsxd 0x61(%rdi),%ebx
-    646cd2c6:	jb     646cd33a <.edata+0x33a>
-    646cd2c8:	(bad)
-    646cd2c9:	jns    646cd32a <.edata+0x32a>
-    646cd2cb:	insl   (%dx),%es:(%rdi)
-    646cd2cc:	(bad)
-    646cd2cd:	js     646cd32e <.edata+0x32e>
-    646cd2cf:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd2d6:	jb     646cd34a <.edata+0x34a>
-    646cd2d8:	(bad)
-    646cd2d9:	jns    646cd33a <.edata+0x33a>
-    646cd2db:	insl   (%dx),%es:(%rdi)
-    646cd2dc:	(bad)
-    646cd2dd:	js     646cd33e <.edata+0x33e>
-    646cd2df:	insb   (%dx),%es:(%rdi)
-    646cd2e0:	outsl  %ds:(%rsi),(%dx)
-    646cd2e1:	outsb  %ds:(%rsi),(%dx)
-    646cd2e2:	addr32 pop %rdi
-    646cd2e4:	insb   (%dx),%es:(%rdi)
-    646cd2e5:	outsl  %ds:(%rsi),(%dx)
-    646cd2e6:	outsb  %ds:(%rsi),(%dx)
-    646cd2e7:	add    %ah,0x5f(%ebx)
-    646cd2eb:	(bad)
-    646cd2ec:	jb     646cd360 <.edata+0x360>
-    646cd2ee:	(bad)
-    646cd2ef:	jns    646cd350 <.edata+0x350>
-    646cd2f1:	insl   (%dx),%es:(%rdi)
-    646cd2f2:	gs (bad)
-    646cd2f4:	outsb  %ds:(%rsi),(%dx)
-    646cd2f5:	pop    %rdi
-    646cd2f6:	outsl  %fs:(%rsi),(%dx)
-    646cd2f8:	jne    646cd35c <.edata+0x35c>
-    646cd2fa:	insb   (%dx),%es:(%rdi)
-    646cd2fb:	add    %ah,%gs:0x5f(%rbx)
-    646cd2ff:	(bad)
-    646cd300:	jb     646cd374 <.edata+0x374>
-    646cd302:	(bad)
-    646cd303:	jns    646cd364 <.edata+0x364>
-    646cd305:	insl   (%dx),%es:(%rdi)
-    646cd306:	gs (bad)
-    646cd308:	outsb  %ds:(%rsi),(%dx)
-    646cd309:	pop    %rdi
-    646cd30a:	data16 insb (%dx),%es:(%rdi)
-    646cd30c:	outsl  %ds:(%rsi),(%dx)
-    646cd30d:	(bad)
-    646cd30e:	je     646cd310 <.edata+0x310>
-    646cd310:	movsxd 0x61(%rdi),%ebx
-    646cd313:	jb     646cd387 <.edata+0x387>
-    646cd315:	(bad)
-    646cd316:	jns    646cd377 <.edata+0x377>
-    646cd318:	insl   (%dx),%es:(%rdi)
-    646cd319:	gs (bad)
-    646cd31b:	outsb  %ds:(%rsi),(%dx)
-    646cd31c:	pop    %rdi
-    646cd31d:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd324:	jb     646cd398 <.edata+0x398>
-    646cd326:	(bad)
-    646cd327:	jns    646cd388 <.edata+0x388>
-    646cd329:	insl   (%dx),%es:(%rdi)
-    646cd32a:	gs (bad)
-    646cd32c:	outsb  %ds:(%rsi),(%dx)
-    646cd32d:	pop    %rdi
-    646cd32e:	insb   (%dx),%es:(%rdi)
-    646cd32f:	outsl  %ds:(%rsi),(%dx)
-    646cd330:	outsb  %ds:(%rsi),(%dx)
-    646cd331:	addr32 pop %rdi
-    646cd333:	insb   (%dx),%es:(%rdi)
-    646cd334:	outsl  %ds:(%rsi),(%dx)
-    646cd335:	outsb  %ds:(%rsi),(%dx)
-    646cd336:	add    %ah,0x5f(%ebx)
-    646cd33a:	(bad)
-    646cd33b:	jb     646cd3af <.edata+0x3af>
-    646cd33d:	(bad)
-    646cd33e:	jns    646cd39f <.edata+0x39f>
-    646cd340:	insl   (%dx),%es:(%rdi)
-    646cd341:	imul   $0x62756f64,0x5f(%rsi),%ebp
-    646cd348:	insb   (%dx),%es:(%rdi)
-    646cd349:	add    %ah,%gs:0x5f(%rbx)
-    646cd34d:	(bad)
-    646cd34e:	jb     646cd3c2 <.edata+0x3c2>
-    646cd350:	(bad)
-    646cd351:	jns    646cd3b2 <.edata+0x3b2>
-    646cd353:	insl   (%dx),%es:(%rdi)
-    646cd354:	imul   $0x616f6c66,0x5f(%rsi),%ebp
-    646cd35b:	je     646cd35d <.edata+0x35d>
-    646cd35d:	movsxd 0x61(%rdi),%ebx
-    646cd360:	jb     646cd3d4 <.edata+0x3d4>
-    646cd362:	(bad)
-    646cd363:	jns    646cd3c4 <.edata+0x3c4>
-    646cd365:	insl   (%dx),%es:(%rdi)
-    646cd366:	imul   $0x746e69,0x5f(%rsi),%ebp
-    646cd36d:	movsxd 0x61(%rdi),%ebx
-    646cd370:	jb     646cd3e4 <.edata+0x3e4>
-    646cd372:	(bad)
-    646cd373:	jns    646cd3d4 <.edata+0x3d4>
-    646cd375:	insl   (%dx),%es:(%rdi)
-    646cd376:	imul   $0x676e6f6c,0x5f(%rsi),%ebp
-    646cd37d:	pop    %rdi
-    646cd37e:	insb   (%dx),%es:(%rdi)
-    646cd37f:	outsl  %ds:(%rsi),(%dx)
-    646cd380:	outsb  %ds:(%rsi),(%dx)
-    646cd381:	add    %ah,0x5f(%ebx)
-    646cd385:	(bad)
-    646cd386:	jb     646cd3fa <.edata+0x3fa>
-    646cd388:	(bad)
-    646cd389:	jns    646cd3ea <.edata+0x3ea>
-    646cd38b:	jae    646cd401 <.edata+0x401>
-    646cd38d:	fs pop %rdi
-    646cd38f:	outsl  %fs:(%rsi),(%dx)
-    646cd391:	jne    646cd3f5 <.edata+0x3f5>
-    646cd393:	insb   (%dx),%es:(%rdi)
-    646cd394:	add    %ah,%gs:0x5f(%rbx)
-    646cd398:	(bad)
-    646cd399:	jb     646cd40d <.edata+0x40d>
-    646cd39b:	(bad)
-    646cd39c:	jns    646cd3fd <.edata+0x3fd>
-    646cd39e:	jae    646cd414 <.edata+0x414>
-    646cd3a0:	fs pop %rdi
-    646cd3a2:	data16 insb (%dx),%es:(%rdi)
-    646cd3a4:	outsl  %ds:(%rsi),(%dx)
+    646cd2c1:	jns    646cd322 <.edata+0x322>
+    646cd2c3:	insl   (%dx),%es:(%rdi)
+    646cd2c4:	(bad)
+    646cd2c5:	js     646cd326 <.edata+0x326>
+    646cd2c7:	data16 insb (%dx),%es:(%rdi)
+    646cd2c9:	outsl  %ds:(%rsi),(%dx)
+    646cd2ca:	(bad)
+    646cd2cb:	je     646cd2cd <.edata+0x2cd>
+    646cd2cd:	movsxd 0x61(%rdi),%ebx
+    646cd2d0:	jb     646cd344 <.edata+0x344>
+    646cd2d2:	(bad)
+    646cd2d3:	jns    646cd334 <.edata+0x334>
+    646cd2d5:	insl   (%dx),%es:(%rdi)
+    646cd2d6:	(bad)
+    646cd2d7:	js     646cd338 <.edata+0x338>
+    646cd2d9:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd2e0:	jb     646cd354 <.edata+0x354>
+    646cd2e2:	(bad)
+    646cd2e3:	jns    646cd344 <.edata+0x344>
+    646cd2e5:	insl   (%dx),%es:(%rdi)
+    646cd2e6:	(bad)
+    646cd2e7:	js     646cd348 <.edata+0x348>
+    646cd2e9:	insb   (%dx),%es:(%rdi)
+    646cd2ea:	outsl  %ds:(%rsi),(%dx)
+    646cd2eb:	outsb  %ds:(%rsi),(%dx)
+    646cd2ec:	addr32 pop %rdi
+    646cd2ee:	insb   (%dx),%es:(%rdi)
+    646cd2ef:	outsl  %ds:(%rsi),(%dx)
+    646cd2f0:	outsb  %ds:(%rsi),(%dx)
+    646cd2f1:	add    %ah,0x5f(%ebx)
+    646cd2f5:	(bad)
+    646cd2f6:	jb     646cd36a <.edata+0x36a>
+    646cd2f8:	(bad)
+    646cd2f9:	jns    646cd35a <.edata+0x35a>
+    646cd2fb:	insl   (%dx),%es:(%rdi)
+    646cd2fc:	gs (bad)
+    646cd2fe:	outsb  %ds:(%rsi),(%dx)
+    646cd2ff:	pop    %rdi
+    646cd300:	outsl  %fs:(%rsi),(%dx)
+    646cd302:	jne    646cd366 <.edata+0x366>
+    646cd304:	insb   (%dx),%es:(%rdi)
+    646cd305:	add    %ah,%gs:0x5f(%rbx)
+    646cd309:	(bad)
+    646cd30a:	jb     646cd37e <.edata+0x37e>
+    646cd30c:	(bad)
+    646cd30d:	jns    646cd36e <.edata+0x36e>
+    646cd30f:	insl   (%dx),%es:(%rdi)
+    646cd310:	gs (bad)
+    646cd312:	outsb  %ds:(%rsi),(%dx)
+    646cd313:	pop    %rdi
+    646cd314:	data16 insb (%dx),%es:(%rdi)
+    646cd316:	outsl  %ds:(%rsi),(%dx)
+    646cd317:	(bad)
+    646cd318:	je     646cd31a <.edata+0x31a>
+    646cd31a:	movsxd 0x61(%rdi),%ebx
+    646cd31d:	jb     646cd391 <.edata+0x391>
+    646cd31f:	(bad)
+    646cd320:	jns    646cd381 <.edata+0x381>
+    646cd322:	insl   (%dx),%es:(%rdi)
+    646cd323:	gs (bad)
+    646cd325:	outsb  %ds:(%rsi),(%dx)
+    646cd326:	pop    %rdi
+    646cd327:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd32e:	jb     646cd3a2 <.edata+0x3a2>
+    646cd330:	(bad)
+    646cd331:	jns    646cd392 <.edata+0x392>
+    646cd333:	insl   (%dx),%es:(%rdi)
+    646cd334:	gs (bad)
+    646cd336:	outsb  %ds:(%rsi),(%dx)
+    646cd337:	pop    %rdi
+    646cd338:	insb   (%dx),%es:(%rdi)
+    646cd339:	outsl  %ds:(%rsi),(%dx)
+    646cd33a:	outsb  %ds:(%rsi),(%dx)
+    646cd33b:	addr32 pop %rdi
+    646cd33d:	insb   (%dx),%es:(%rdi)
+    646cd33e:	outsl  %ds:(%rsi),(%dx)
+    646cd33f:	outsb  %ds:(%rsi),(%dx)
+    646cd340:	add    %ah,0x5f(%ebx)
+    646cd344:	(bad)
+    646cd345:	jb     646cd3b9 <.edata+0x3b9>
+    646cd347:	(bad)
+    646cd348:	jns    646cd3a9 <.edata+0x3a9>
+    646cd34a:	insl   (%dx),%es:(%rdi)
+    646cd34b:	imul   $0x62756f64,0x5f(%rsi),%ebp
+    646cd352:	insb   (%dx),%es:(%rdi)
+    646cd353:	add    %ah,%gs:0x5f(%rbx)
+    646cd357:	(bad)
+    646cd358:	jb     646cd3cc <.edata+0x3cc>
+    646cd35a:	(bad)
+    646cd35b:	jns    646cd3bc <.edata+0x3bc>
+    646cd35d:	insl   (%dx),%es:(%rdi)
+    646cd35e:	imul   $0x616f6c66,0x5f(%rsi),%ebp
+    646cd365:	je     646cd367 <.edata+0x367>
+    646cd367:	movsxd 0x61(%rdi),%ebx
+    646cd36a:	jb     646cd3de <.edata+0x3de>
+    646cd36c:	(bad)
+    646cd36d:	jns    646cd3ce <.edata+0x3ce>
+    646cd36f:	insl   (%dx),%es:(%rdi)
+    646cd370:	imul   $0x746e69,0x5f(%rsi),%ebp
+    646cd377:	movsxd 0x61(%rdi),%ebx
+    646cd37a:	jb     646cd3ee <.edata+0x3ee>
+    646cd37c:	(bad)
+    646cd37d:	jns    646cd3de <.edata+0x3de>
+    646cd37f:	insl   (%dx),%es:(%rdi)
+    646cd380:	imul   $0x676e6f6c,0x5f(%rsi),%ebp
+    646cd387:	pop    %rdi
+    646cd388:	insb   (%dx),%es:(%rdi)
+    646cd389:	outsl  %ds:(%rsi),(%dx)
+    646cd38a:	outsb  %ds:(%rsi),(%dx)
+    646cd38b:	add    %ah,0x5f(%ebx)
+    646cd38f:	(bad)
+    646cd390:	jb     646cd404 <.edata+0x404>
+    646cd392:	(bad)
+    646cd393:	jns    646cd3f4 <.edata+0x3f4>
+    646cd395:	jae    646cd40b <.edata+0x40b>
+    646cd397:	fs pop %rdi
+    646cd399:	outsl  %fs:(%rsi),(%dx)
+    646cd39b:	jne    646cd3ff <.edata+0x3ff>
+    646cd39d:	insb   (%dx),%es:(%rdi)
+    646cd39e:	add    %ah,%gs:0x5f(%rbx)
+    646cd3a2:	(bad)
+    646cd3a3:	jb     646cd417 <.edata+0x417>
     646cd3a5:	(bad)
-    646cd3a6:	je     646cd3a8 <.edata+0x3a8>
-    646cd3a8:	movsxd 0x61(%rdi),%ebx
-    646cd3ab:	jb     646cd41f <.edata+0x41f>
-    646cd3ad:	(bad)
-    646cd3ae:	jns    646cd40f <.edata+0x40f>
-    646cd3b0:	jae    646cd426 <.edata+0x426>
-    646cd3b2:	fs pop %rdi
-    646cd3b4:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd3bb:	jb     646cd42f <.edata+0x42f>
-    646cd3bd:	(bad)
-    646cd3be:	jns    646cd41f <.edata+0x41f>
-    646cd3c0:	jae    646cd436 <.edata+0x436>
-    646cd3c2:	fs pop %rdi
-    646cd3c4:	insb   (%dx),%es:(%rdi)
-    646cd3c5:	outsl  %ds:(%rsi),(%dx)
-    646cd3c6:	outsb  %ds:(%rsi),(%dx)
-    646cd3c7:	addr32 pop %rdi
-    646cd3c9:	insb   (%dx),%es:(%rdi)
-    646cd3ca:	outsl  %ds:(%rsi),(%dx)
-    646cd3cb:	outsb  %ds:(%rsi),(%dx)
-    646cd3cc:	add    %ah,0x5f(%ebx)
-    646cd3d0:	(bad)
-    646cd3d1:	jb     646cd445 <.edata+0x445>
-    646cd3d3:	(bad)
-    646cd3d4:	jns    646cd435 <.edata+0x435>
-    646cd3d6:	jae    646cd44d <.edata+0x44d>
-    646cd3d8:	insl   (%dx),%es:(%rdi)
-    646cd3d9:	pop    %rdi
-    646cd3da:	outsl  %fs:(%rsi),(%dx)
-    646cd3dc:	jne    646cd440 <.edata+0x440>
-    646cd3de:	insb   (%dx),%es:(%rdi)
-    646cd3df:	add    %ah,%gs:0x5f(%rbx)
-    646cd3e3:	(bad)
-    646cd3e4:	jb     646cd458 <.edata+0x458>
-    646cd3e6:	(bad)
-    646cd3e7:	jns    646cd448 <.edata+0x448>
-    646cd3e9:	jae    646cd460 <.edata+0x460>
-    646cd3eb:	insl   (%dx),%es:(%rdi)
-    646cd3ec:	pop    %rdi
-    646cd3ed:	data16 insb (%dx),%es:(%rdi)
-    646cd3ef:	outsl  %ds:(%rsi),(%dx)
+    646cd3a6:	jns    646cd407 <.edata+0x407>
+    646cd3a8:	jae    646cd41e <.edata+0x41e>
+    646cd3aa:	fs pop %rdi
+    646cd3ac:	data16 insb (%dx),%es:(%rdi)
+    646cd3ae:	outsl  %ds:(%rsi),(%dx)
+    646cd3af:	(bad)
+    646cd3b0:	je     646cd3b2 <.edata+0x3b2>
+    646cd3b2:	movsxd 0x61(%rdi),%ebx
+    646cd3b5:	jb     646cd429 <.edata+0x429>
+    646cd3b7:	(bad)
+    646cd3b8:	jns    646cd419 <.edata+0x419>
+    646cd3ba:	jae    646cd430 <.edata+0x430>
+    646cd3bc:	fs pop %rdi
+    646cd3be:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd3c5:	jb     646cd439 <.edata+0x439>
+    646cd3c7:	(bad)
+    646cd3c8:	jns    646cd429 <.edata+0x429>
+    646cd3ca:	jae    646cd440 <.edata+0x440>
+    646cd3cc:	fs pop %rdi
+    646cd3ce:	insb   (%dx),%es:(%rdi)
+    646cd3cf:	outsl  %ds:(%rsi),(%dx)
+    646cd3d0:	outsb  %ds:(%rsi),(%dx)
+    646cd3d1:	addr32 pop %rdi
+    646cd3d3:	insb   (%dx),%es:(%rdi)
+    646cd3d4:	outsl  %ds:(%rsi),(%dx)
+    646cd3d5:	outsb  %ds:(%rsi),(%dx)
+    646cd3d6:	add    %ah,0x5f(%ebx)
+    646cd3da:	(bad)
+    646cd3db:	jb     646cd44f <.edata+0x44f>
+    646cd3dd:	(bad)
+    646cd3de:	jns    646cd43f <.edata+0x43f>
+    646cd3e0:	jae    646cd457 <.edata+0x457>
+    646cd3e2:	insl   (%dx),%es:(%rdi)
+    646cd3e3:	pop    %rdi
+    646cd3e4:	outsl  %fs:(%rsi),(%dx)
+    646cd3e6:	jne    646cd44a <.edata+0x44a>
+    646cd3e8:	insb   (%dx),%es:(%rdi)
+    646cd3e9:	add    %ah,%gs:0x5f(%rbx)
+    646cd3ed:	(bad)
+    646cd3ee:	jb     646cd462 <.edata+0x462>
     646cd3f0:	(bad)
-    646cd3f1:	je     646cd3f3 <.edata+0x3f3>
-    646cd3f3:	movsxd 0x61(%rdi),%ebx
-    646cd3f6:	jb     646cd46a <.edata+0x46a>
-    646cd3f8:	(bad)
-    646cd3f9:	jns    646cd45a <.edata+0x45a>
-    646cd3fb:	jae    646cd472 <.edata+0x472>
-    646cd3fd:	insl   (%dx),%es:(%rdi)
-    646cd3fe:	pop    %rdi
-    646cd3ff:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd406:	jb     646cd47a <.edata+0x47a>
-    646cd408:	(bad)
-    646cd409:	jns    646cd46a <.edata+0x46a>
-    646cd40b:	jae    646cd482 <.edata+0x482>
-    646cd40d:	insl   (%dx),%es:(%rdi)
-    646cd40e:	pop    %rdi
-    646cd40f:	insb   (%dx),%es:(%rdi)
-    646cd410:	outsl  %ds:(%rsi),(%dx)
-    646cd411:	outsb  %ds:(%rsi),(%dx)
-    646cd412:	add    %ah,0x5f(%ebx)
-    646cd416:	(bad)
-    646cd417:	jb     646cd48b <.edata+0x48b>
-    646cd419:	(bad)
-    646cd41a:	jns    646cd47b <.edata+0x47b>
-    646cd41c:	jbe    646cd47f <.edata+0x47f>
-    646cd41e:	jb     646cd47f <.edata+0x47f>
-    646cd420:	outsl  %fs:(%rsi),(%dx)
-    646cd422:	jne    646cd486 <.edata+0x486>
-    646cd424:	insb   (%dx),%es:(%rdi)
-    646cd425:	add    %ah,%gs:0x5f(%rbx)
-    646cd429:	(bad)
-    646cd42a:	jb     646cd49e <.edata+0x49e>
-    646cd42c:	(bad)
-    646cd42d:	jns    646cd48e <.edata+0x48e>
-    646cd42f:	jbe    646cd492 <.edata+0x492>
-    646cd431:	jb     646cd492 <.edata+0x492>
-    646cd433:	data16 insb (%dx),%es:(%rdi)
-    646cd435:	outsl  %ds:(%rsi),(%dx)
+    646cd3f1:	jns    646cd452 <.edata+0x452>
+    646cd3f3:	jae    646cd46a <.edata+0x46a>
+    646cd3f5:	insl   (%dx),%es:(%rdi)
+    646cd3f6:	pop    %rdi
+    646cd3f7:	data16 insb (%dx),%es:(%rdi)
+    646cd3f9:	outsl  %ds:(%rsi),(%dx)
+    646cd3fa:	(bad)
+    646cd3fb:	je     646cd3fd <.edata+0x3fd>
+    646cd3fd:	movsxd 0x61(%rdi),%ebx
+    646cd400:	jb     646cd474 <.edata+0x474>
+    646cd402:	(bad)
+    646cd403:	jns    646cd464 <.edata+0x464>
+    646cd405:	jae    646cd47c <.edata+0x47c>
+    646cd407:	insl   (%dx),%es:(%rdi)
+    646cd408:	pop    %rdi
+    646cd409:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd410:	jb     646cd484 <.edata+0x484>
+    646cd412:	(bad)
+    646cd413:	jns    646cd474 <.edata+0x474>
+    646cd415:	jae    646cd48c <.edata+0x48c>
+    646cd417:	insl   (%dx),%es:(%rdi)
+    646cd418:	pop    %rdi
+    646cd419:	insb   (%dx),%es:(%rdi)
+    646cd41a:	outsl  %ds:(%rsi),(%dx)
+    646cd41b:	outsb  %ds:(%rsi),(%dx)
+    646cd41c:	add    %ah,0x5f(%ebx)
+    646cd420:	(bad)
+    646cd421:	jb     646cd495 <.edata+0x495>
+    646cd423:	(bad)
+    646cd424:	jns    646cd485 <.edata+0x485>
+    646cd426:	jbe    646cd489 <.edata+0x489>
+    646cd428:	jb     646cd489 <.edata+0x489>
+    646cd42a:	outsl  %fs:(%rsi),(%dx)
+    646cd42c:	jne    646cd490 <.edata+0x490>
+    646cd42e:	insb   (%dx),%es:(%rdi)
+    646cd42f:	add    %ah,%gs:0x5f(%rbx)
+    646cd433:	(bad)
+    646cd434:	jb     646cd4a8 <.edata+0x4a8>
     646cd436:	(bad)
-    646cd437:	je     646cd439 <.edata+0x439>
-    646cd439:	movsxd 0x61(%rdi),%ebx
-    646cd43c:	jb     646cd4b0 <.edata+0x4b0>
-    646cd43e:	(bad)
-    646cd43f:	jns    646cd4a0 <.edata+0x4a0>
-    646cd441:	jbe    646cd4a4 <.edata+0x4a4>
-    646cd443:	jb     646cd4a4 <.edata+0x4a4>
-    646cd445:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd44c:	jb     646cd4c0 <.edata+0x4c0>
-    646cd44e:	(bad)
-    646cd44f:	jns    646cd4b0 <.edata+0x4b0>
-    646cd451:	jbe    646cd4b4 <.edata+0x4b4>
-    646cd453:	jb     646cd4b4 <.edata+0x4b4>
-    646cd455:	insb   (%dx),%es:(%rdi)
-    646cd456:	outsl  %ds:(%rsi),(%dx)
-    646cd457:	outsb  %ds:(%rsi),(%dx)
-    646cd458:	addr32 pop %rdi
-    646cd45a:	insb   (%dx),%es:(%rdi)
-    646cd45b:	outsl  %ds:(%rsi),(%dx)
-    646cd45c:	outsb  %ds:(%rsi),(%dx)
-    646cd45d:	add    %ah,0x6d(%ebx)
-    646cd461:	jo     646cd4c9 <.edata+0x4c9>
-    646cd463:	jne    646cd4d3 <.edata+0x4d3>
-    646cd465:	movsxd 0x64(%rdi),%ebx
-    646cd468:	outsl  %ds:(%rsi),(%dx)
-    646cd469:	jne    646cd4cd <.edata+0x4cd>
-    646cd46b:	insb   (%dx),%es:(%rdi)
-    646cd46c:	add    %ah,%gs:0x6d(%rbx)
-    646cd470:	jo     646cd4d8 <.edata+0x4d8>
-    646cd472:	jne    646cd4e2 <.edata+0x4e2>
-    646cd474:	movsxd 0x66(%rdi),%ebx
-    646cd477:	insb   (%dx),%es:(%rdi)
-    646cd478:	outsl  %ds:(%rsi),(%dx)
-    646cd479:	(bad)
-    646cd47a:	je     646cd47c <.edata+0x47c>
-    646cd47c:	movsxd 0x70(%rbp),%ebp
-    646cd47f:	data16 jne 646cd4f0 <.edata+0x4f0>
-    646cd482:	movsxd 0x69(%rdi),%ebx
-    646cd485:	outsb  %ds:(%rsi),(%dx)
-    646cd486:	je     646cd488 <.edata+0x488>
-    646cd488:	movsxd 0x70(%rbp),%ebp
-    646cd48b:	data16 jne 646cd4fc <.edata+0x4fc>
-    646cd48e:	movsxd 0x6c(%rdi),%ebx
-    646cd491:	outsl  %ds:(%rsi),(%dx)
-    646cd492:	outsb  %ds:(%rsi),(%dx)
-    646cd493:	add    %ah,0x6f(%ebx)
-    646cd497:	jbe    646cd4f8 <.edata+0x4f8>
-    646cd499:	insl   (%dx),%es:(%rdi)
-    646cd49a:	outsl  %ds:(%rsi),(%dx)
-    646cd49b:	fs gs insb (%dx),%es:(%rdi)
-    646cd49e:	add    %ah,0x6f(%rbx)
+    646cd437:	jns    646cd498 <.edata+0x498>
+    646cd439:	jbe    646cd49c <.edata+0x49c>
+    646cd43b:	jb     646cd49c <.edata+0x49c>
+    646cd43d:	data16 insb (%dx),%es:(%rdi)
+    646cd43f:	outsl  %ds:(%rsi),(%dx)
+    646cd440:	(bad)
+    646cd441:	je     646cd443 <.edata+0x443>
+    646cd443:	movsxd 0x61(%rdi),%ebx
+    646cd446:	jb     646cd4ba <.edata+0x4ba>
+    646cd448:	(bad)
+    646cd449:	jns    646cd4aa <.edata+0x4aa>
+    646cd44b:	jbe    646cd4ae <.edata+0x4ae>
+    646cd44d:	jb     646cd4ae <.edata+0x4ae>
+    646cd44f:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd456:	jb     646cd4ca <.edata+0x4ca>
+    646cd458:	(bad)
+    646cd459:	jns    646cd4ba <.edata+0x4ba>
+    646cd45b:	jbe    646cd4be <.edata+0x4be>
+    646cd45d:	jb     646cd4be <.edata+0x4be>
+    646cd45f:	insb   (%dx),%es:(%rdi)
+    646cd460:	outsl  %ds:(%rsi),(%dx)
+    646cd461:	outsb  %ds:(%rsi),(%dx)
+    646cd462:	addr32 pop %rdi
+    646cd464:	insb   (%dx),%es:(%rdi)
+    646cd465:	outsl  %ds:(%rsi),(%dx)
+    646cd466:	outsb  %ds:(%rsi),(%dx)
+    646cd467:	add    %ah,0x6d(%ebx)
+    646cd46b:	jo     646cd4d3 <.edata+0x4d3>
+    646cd46d:	jne    646cd4dd <.edata+0x4dd>
+    646cd46f:	movsxd 0x64(%rdi),%ebx
+    646cd472:	outsl  %ds:(%rsi),(%dx)
+    646cd473:	jne    646cd4d7 <.edata+0x4d7>
+    646cd475:	insb   (%dx),%es:(%rdi)
+    646cd476:	add    %ah,%gs:0x6d(%rbx)
+    646cd47a:	jo     646cd4e2 <.edata+0x4e2>
+    646cd47c:	jne    646cd4ec <.edata+0x4ec>
+    646cd47e:	movsxd 0x66(%rdi),%ebx
+    646cd481:	insb   (%dx),%es:(%rdi)
+    646cd482:	outsl  %ds:(%rsi),(%dx)
+    646cd483:	(bad)
+    646cd484:	je     646cd486 <.edata+0x486>
+    646cd486:	movsxd 0x70(%rbp),%ebp
+    646cd489:	data16 jne 646cd4fa <.edata+0x4fa>
+    646cd48c:	movsxd 0x69(%rdi),%ebx
+    646cd48f:	outsb  %ds:(%rsi),(%dx)
+    646cd490:	je     646cd492 <.edata+0x492>
+    646cd492:	movsxd 0x70(%rbp),%ebp
+    646cd495:	data16 jne 646cd506 <.edata+0x506>
+    646cd498:	movsxd 0x6c(%rdi),%ebx
+    646cd49b:	outsl  %ds:(%rsi),(%dx)
+    646cd49c:	outsb  %ds:(%rsi),(%dx)
+    646cd49d:	add    %ah,0x6f(%ebx)
     646cd4a1:	jbe    646cd502 <.edata+0x502>
     646cd4a3:	insl   (%dx),%es:(%rdi)
     646cd4a4:	outsl  %ds:(%rsi),(%dx)
     646cd4a5:	fs gs insb (%dx),%es:(%rdi)
-    646cd4a8:	xor    0x63(%rax,%rax,1),%ah
-    646cd4ac:	outsl  %ds:(%rsi),(%dx)
-    646cd4ad:	jbe    646cd50e <.edata+0x50e>
-    646cd4af:	insl   (%dx),%es:(%rdi)
-    646cd4b0:	outsl  %ds:(%rsi),(%dx)
-    646cd4b1:	fs gs insb (%dx),%es:(%rdi)
-    646cd4b4:	pop    %rdi
-    646cd4b5:	imul   $0x5f640074,0x69(%rsi),%ebp
-    646cd4bc:	(bad)
-    646cd4bd:	jb     646cd520 <.edata+0x520>
-    646cd4bf:	outsb  %ds:(%rsi),(%dx)
-    646cd4c0:	add    %ah,%gs:0x69(%esi)
-    646cd4c5:	outsb  %ds:(%rsi),(%dx)
-    646cd4c6:	fs pop %rdi
-    646cd4c8:	outsb  %ds:(%rsi),(%dx)
-    646cd4c9:	imul   $0x726f62,%gs:0x68(%rdi),%esp
-    646cd4d1:	imul   $0x67,0x69(%rdx),%esi
-    646cd4d5:	gs pop %rdi
-    646cd4d7:	insl   (%dx),%es:(%rdi)
-    646cd4d8:	gs insl (%dx),%es:(%rdi)
-    646cd4da:	outsl  %ds:(%rsi),(%dx)
-    646cd4db:	jb     646cd556 <.edata+0x556>
-    646cd4dd:	pop    %rdi
-    646cd4de:	data16 jb 646cd546 <.edata+0x546>
-    646cd4e1:	add    %ch,%gs:0x72(%rbx)
-    646cd4e5:	imul   $0x7261705f,0x65(%rdi),%esp
-    646cd4ec:	(bad)
-    646cd4ed:	insl   (%dx),%es:(%rdi)
-    646cd4ee:	pop    %rdi
-    646cd4ef:	jae    646cd556 <.edata+0x556>
-    646cd4f1:	je     646cd567 <.edata+0x567>
-    646cd4f3:	imul   $0x5f756c00,0x67(%rsi),%ebp
-    646cd4fa:	fs movsxd %gs:0x6d(%rdi),%ebp
-    646cd4ff:	jo     646cd570 <.edata+0x570>
-    646cd501:	jae    646cd56c <.edata+0x56c>
-    646cd503:	je     646cd56e <.edata+0x56e>
-    646cd505:	outsl  %ds:(%rsi),(%dx)
-    646cd506:	outsb  %ds:(%rsi),(%dx)
-    646cd507:	add    %ch,0x5f(%rbp,%rsi,2)
-    646cd50b:	imul   $0x65737265,0x76(%rsi),%ebp
-    646cd512:	pop    %rdi
-    646cd513:	jae    646cd584 <.edata+0x584>
-    646cd515:	insb   (%dx),%es:(%rdi)
-    646cd516:	jbe    646cd57d <.edata+0x57d>
-    646cd518:	jb     646cd51a <.edata+0x51a>
-    646cd51a:	insl   (%dx),%es:(%rdi)
-    646cd51b:	(bad)
-    646cd51c:	je     646cd590 <.edata+0x590>
-    646cd51e:	imul   $0x6d726f,0x66(%rax),%edi
-    646cd525:	insl   (%dx),%es:(%rdi)
-    646cd526:	je     646cd559 <.edata+0x559>
-    646cd528:	cmp    %edi,(%rcx)
-    646cd52a:	xor    (%rdi),%esi
-    646cd52c:	pop    %rdi
-    646cd52d:	outsb  %gs:(%esi),(%dx)
-    646cd530:	gs jb  646cd594 <.edata+0x594>
-    646cd533:	je     646cd59a <.edata+0x59a>
-    646cd535:	add    %ch,0x74(%rbp)
-    646cd538:	xor    %edi,(%rcx)
-    646cd53a:	cmp    %esi,(%rbx)
-    646cd53c:	(bad)
-    646cd53d:	pop    %rdi
-    646cd53e:	addr32 gs je 646cd5a1 <.edata+0x5a1>
-    646cd542:	outsl  %fs:(%rsi),(%dx)
-    646cd544:	jne    646cd5a8 <.edata+0x5a8>
-    646cd546:	insb   (%dx),%es:(%rdi)
-    646cd547:	add    %ch,%gs:0x74(%rbp)
-    646cd54b:	xor    %edi,(%rcx)
-    646cd54d:	cmp    %esi,(%rbx)
-    646cd54f:	(bad)
-    646cd550:	pop    %rdi
-    646cd551:	addr32 gs je 646cd5b4 <.edata+0x5b4>
-    646cd555:	outsl  %fs:(%rsi),(%dx)
-    646cd557:	jne    646cd5bb <.edata+0x5bb>
-    646cd559:	insb   (%dx),%es:(%rdi)
-    646cd55a:	gs pop %rdi
-    646cd55c:	jb     646cd5bf <.edata+0x5bf>
-    646cd55e:	outsb  %ds:(%rsi),(%dx)
-    646cd55f:	add    %ch,%gs:0x74(%ebp)
-    646cd564:	xor    %edi,(%rcx)
-    646cd566:	cmp    %esi,(%rbx)
-    646cd568:	(bad)
-    646cd569:	pop    %rdi
-    646cd56a:	addr32 gs je 646cd5cd <.edata+0x5cd>
-    646cd56e:	data16 insb (%dx),%es:(%rdi)
-    646cd570:	outsl  %ds:(%rsi),(%dx)
-    646cd571:	(bad)
-    646cd572:	je     646cd574 <.edata+0x574>
-    646cd574:	insl   (%dx),%es:(%rdi)
-    646cd575:	je     646cd5a8 <.edata+0x5a8>
-    646cd577:	cmp    %edi,(%rcx)
-    646cd579:	xor    (%rdi),%esi
-    646cd57b:	pop    %rdi
-    646cd57c:	addr32 gs je 646cd5df <.edata+0x5df>
-    646cd580:	data16 insb (%dx),%es:(%rdi)
-    646cd582:	outsl  %ds:(%rsi),(%dx)
-    646cd583:	(bad)
-    646cd584:	je     646cd5e5 <.edata+0x5e5>
-    646cd586:	jb     646cd5e9 <.edata+0x5e9>
-    646cd588:	outsb  %ds:(%rsi),(%dx)
-    646cd589:	add    %ch,%gs:0x74(%ebp)
-    646cd58e:	xor    %edi,(%rcx)
-    646cd590:	cmp    %esi,(%rbx)
-    646cd592:	(bad)
-    646cd593:	pop    %rdi
-    646cd594:	addr32 gs je 646cd5f7 <.edata+0x5f7>
-    646cd598:	imul   $0x725f3233,0x74(%rsi),%ebp
-    646cd59f:	(bad)
-    646cd5a0:	outsb  %ds:(%rsi),(%dx)
-    646cd5a1:	add    %ch,%gs:0x74(%ebp)
-    646cd5a6:	xor    %edi,(%rcx)
-    646cd5a8:	cmp    %esi,(%rbx)
-    646cd5aa:	(bad)
-    646cd5ab:	pop    %rdi
-    646cd5ac:	imul   $0x746d0074,0x69(%rsi),%ebp
-    646cd5b3:	xor    %edi,(%rcx)
-    646cd5b5:	cmp    %esi,(%rbx)
-    646cd5b7:	(bad)
-    646cd5b8:	pop    %rdi
-    646cd5b9:	jb     646cd61c <.edata+0x61c>
-    646cd5bb:	outsb  %ds:(%rsi),(%dx)
-    646cd5bc:	outsl  %fs:(%rsi),(%dx)
-    646cd5be:	insl   (%dx),%es:(%rdi)
-    646cd5bf:	pop    %rdi
-    646cd5c0:	outsb  %ds:(%rsi),(%dx)
-    646cd5c1:	outsl  %ds:(%rsi),(%dx)
-    646cd5c2:	jb     646cd631 <.edata+0x631>
-    646cd5c4:	(bad)
-    646cd5c5:	insb   (%dx),%es:(%rdi)
-    646cd5c6:	add    %dh,0x61(%rax)
-    646cd5c9:	jb     646cd63f <.edata+0x63f>
-    646cd5cb:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
-    646cd5d3:	jo     646cd639 <.edata+0x639>
-    646cd5d5:	imul   $0x69757100,0x74(%rbx),%esi
-    646cd5dc:	movsxd 0x73(%rbx),%ebp
-    646cd5df:	outsl  %ds:(%rsi),(%dx)
-    646cd5e0:	jb     646cd656 <.edata+0x656>
-    646cd5e2:	xor    0x72(%rax,%rax,1),%ah
-    646cd5e6:	(bad)
-    646cd5e7:	outsb  %ds:(%rsi),(%dx)
-    646cd5e8:	outsl  %fs:(%rsi),(%dx)
-    646cd5ea:	insl   (%dx),%es:(%rdi)
-    646cd5eb:	jo     646cd64e <.edata+0x64e>
-    646cd5ed:	je     646cd657 <.edata+0x657>
-    646cd5ef:	add    %dh,0x61(%rbx)
-    646cd5f2:	insl   (%dx),%es:(%rdi)
-    646cd5f3:	jo     646cd661 <.edata+0x661>
-    646cd5f5:	imul   $0x6174735f,0x67(%rsi),%ebp
-    646cd5fc:	je     646cd663 <.edata+0x663>
-    646cd5fe:	pop    %rdi
-    646cd5ff:	imul   $0x61730074,0x69(%rsi),%ebp
-    646cd606:	insl   (%dx),%es:(%rdi)
-    646cd607:	jo     646cd675 <__bss_end__+0xae5>
-    646cd609:	imul   $0x6174735f,0x67(%rsi),%ebp
-    646cd610:	je     646cd677 <__bss_end__+0xae7>
-    646cd612:	pop    %rdi
-    646cd613:	jne    646cd685 <__bss_end__+0xaf5>
-    646cd615:	fs (bad)
-    646cd617:	je     646cd67e <__bss_end__+0xaee>
-    646cd619:	add    %dh,0x61(%rbx)
-    646cd61c:	jbe    646cd683 <__bss_end__+0xaf3>
-    646cd61e:	pop    %rdi
-    646cd61f:	xor    %esp,0x72(%rcx,%riz,2)
-    646cd623:	jb     646cd686 <__bss_end__+0xaf6>
-    646cd625:	jns    646cd627 <.edata+0x627>
-    646cd627:	jae    646cd690 <__bss_end__+0xb00>
-    646cd629:	jae    646cd694 <__bss_end__+0xb04>
-    646cd62b:	insl   (%dx),%es:(%rdi)
-    646cd62c:	pop    %rdi
-    646cd62d:	imul   $0x67730074,0x69(%rsi),%ebp
-    646cd634:	jae    646cd69f <__bss_end__+0xb0f>
-    646cd636:	insl   (%dx),%es:(%rdi)
-    646cd637:	pop    %rdi
-    646cd638:	jb     646cd6af <__bss_end__+0xb1f>
-    646cd63a:	outsb  %ds:(%rsi),(%dx)
-    646cd63b:	add    %dh,0x67(%rbx)
-    646cd63e:	jae    646cd6a9 <__bss_end__+0xb19>
-    646cd640:	insl   (%dx),%es:(%rdi)
-    646cd641:	pop    %rdi
-    646cd642:	je     646cd6a3 <__bss_end__+0xb13>
-    646cd644:	data16 jb 646cd6ac <__bss_end__+0xb1c>
-    646cd647:	add    %dh,%gs:0x69(%rbx)
-    646cd64b:	insl   (%dx),%es:(%rdi)
-    646cd64c:	jo     646cd6ba <__bss_end__+0xb2a>
-    646cd64e:	gs pop %rdi
-    646cd650:	imul   $0x67,0x69(%rdx),%esi
-    646cd654:	imul   $0x61777300,0x67(%rsi),%ebp
-    646cd65b:	jo     646cd6cf <__bss_end__+0xb3f>
-    646cd65d:	outsl  %ds:(%rsi),(%dx)
-    646cd65e:	ja     646cd6d3 <__bss_end__+0xb43>
-    646cd660:	add    %dh,0x61(%rsi)
-    646cd663:	jb     646cd6ce <__bss_end__+0xb3e>
-    646cd665:	(bad)
-    646cd666:	outsb  %ds:(%rsi),(%dx)
-    646cd667:	movsxd 0x0(%rbp),%esp
-    646cd66a:	jbe    646cd6cd <__bss_end__+0xb3d>
-    646cd66c:	jb     646cd6d7 <__bss_end__+0xb47>
-    646cd66e:	outsl  %ds:(%rsi),(%dx)
-    646cd66f:	addr32 jb 646cd6d3 <__bss_end__+0xb43>
-    646cd672:	insl   (%dx),%es:(%rdi)
+    646cd4a8:	add    %ah,0x6f(%rbx)
+    646cd4ab:	jbe    646cd50c <.edata+0x50c>
+    646cd4ad:	insl   (%dx),%es:(%rdi)
+    646cd4ae:	outsl  %ds:(%rsi),(%dx)
+    646cd4af:	fs gs insb (%dx),%es:(%rdi)
+    646cd4b2:	xor    0x63(%rax,%rax,1),%ah
+    646cd4b6:	outsl  %ds:(%rsi),(%dx)
+    646cd4b7:	jbe    646cd518 <.edata+0x518>
+    646cd4b9:	insl   (%dx),%es:(%rdi)
+    646cd4ba:	outsl  %ds:(%rsi),(%dx)
+    646cd4bb:	fs gs insb (%dx),%es:(%rdi)
+    646cd4be:	pop    %rdi
+    646cd4bf:	imul   $0x5f640074,0x69(%rsi),%ebp
+    646cd4c6:	(bad)
+    646cd4c7:	jb     646cd52a <.edata+0x52a>
+    646cd4c9:	outsb  %ds:(%rsi),(%dx)
+    646cd4ca:	add    %ah,%gs:0x69(%esi)
+    646cd4cf:	outsb  %ds:(%rsi),(%dx)
+    646cd4d0:	fs pop %rdi
+    646cd4d2:	outsb  %ds:(%rsi),(%dx)
+    646cd4d3:	imul   $0x726f62,%gs:0x68(%rdi),%esp
+    646cd4db:	imul   $0x67,0x69(%rdx),%esi
+    646cd4df:	gs pop %rdi
+    646cd4e1:	insl   (%dx),%es:(%rdi)
+    646cd4e2:	gs insl (%dx),%es:(%rdi)
+    646cd4e4:	outsl  %ds:(%rsi),(%dx)
+    646cd4e5:	jb     646cd560 <.edata+0x560>
+    646cd4e7:	pop    %rdi
+    646cd4e8:	data16 jb 646cd550 <.edata+0x550>
+    646cd4eb:	add    %ch,%gs:0x72(%rbx)
+    646cd4ef:	imul   $0x7261705f,0x65(%rdi),%esp
+    646cd4f6:	(bad)
+    646cd4f7:	insl   (%dx),%es:(%rdi)
+    646cd4f8:	pop    %rdi
+    646cd4f9:	jae    646cd560 <.edata+0x560>
+    646cd4fb:	je     646cd571 <.edata+0x571>
+    646cd4fd:	imul   $0x5f756c00,0x67(%rsi),%ebp
+    646cd504:	fs movsxd %gs:0x6d(%rdi),%ebp
+    646cd509:	jo     646cd57a <.edata+0x57a>
+    646cd50b:	jae    646cd576 <.edata+0x576>
+    646cd50d:	je     646cd578 <.edata+0x578>
+    646cd50f:	outsl  %ds:(%rsi),(%dx)
+    646cd510:	outsb  %ds:(%rsi),(%dx)
+    646cd511:	add    %ch,0x5f(%rbp,%rsi,2)
+    646cd515:	imul   $0x65737265,0x76(%rsi),%ebp
+    646cd51c:	pop    %rdi
+    646cd51d:	jae    646cd58e <.edata+0x58e>
+    646cd51f:	insb   (%dx),%es:(%rdi)
+    646cd520:	jbe    646cd587 <.edata+0x587>
+    646cd522:	jb     646cd524 <.edata+0x524>
+    646cd524:	insl   (%dx),%es:(%rdi)
+    646cd525:	(bad)
+    646cd526:	je     646cd59a <.edata+0x59a>
+    646cd528:	imul   $0x6d726f,0x66(%rax),%edi
+    646cd52f:	insl   (%dx),%es:(%rdi)
+    646cd530:	je     646cd563 <.edata+0x563>
+    646cd532:	cmp    %edi,(%rcx)
+    646cd534:	xor    (%rdi),%esi
+    646cd536:	pop    %rdi
+    646cd537:	outsb  %gs:(%esi),(%dx)
+    646cd53a:	gs jb  646cd59e <.edata+0x59e>
+    646cd53d:	je     646cd5a4 <.edata+0x5a4>
+    646cd53f:	add    %ch,0x74(%rbp)
+    646cd542:	xor    %edi,(%rcx)
+    646cd544:	cmp    %esi,(%rbx)
+    646cd546:	(bad)
+    646cd547:	pop    %rdi
+    646cd548:	addr32 gs je 646cd5ab <.edata+0x5ab>
+    646cd54c:	outsl  %fs:(%rsi),(%dx)
+    646cd54e:	jne    646cd5b2 <.edata+0x5b2>
+    646cd550:	insb   (%dx),%es:(%rdi)
+    646cd551:	add    %ch,%gs:0x74(%rbp)
+    646cd555:	xor    %edi,(%rcx)
+    646cd557:	cmp    %esi,(%rbx)
+    646cd559:	(bad)
+    646cd55a:	pop    %rdi
+    646cd55b:	addr32 gs je 646cd5be <.edata+0x5be>
+    646cd55f:	outsl  %fs:(%rsi),(%dx)
+    646cd561:	jne    646cd5c5 <.edata+0x5c5>
+    646cd563:	insb   (%dx),%es:(%rdi)
+    646cd564:	gs pop %rdi
+    646cd566:	jb     646cd5c9 <.edata+0x5c9>
+    646cd568:	outsb  %ds:(%rsi),(%dx)
+    646cd569:	add    %ch,%gs:0x74(%ebp)
+    646cd56e:	xor    %edi,(%rcx)
+    646cd570:	cmp    %esi,(%rbx)
+    646cd572:	(bad)
+    646cd573:	pop    %rdi
+    646cd574:	addr32 gs je 646cd5d7 <.edata+0x5d7>
+    646cd578:	data16 insb (%dx),%es:(%rdi)
+    646cd57a:	outsl  %ds:(%rsi),(%dx)
+    646cd57b:	(bad)
+    646cd57c:	je     646cd57e <.edata+0x57e>
+    646cd57e:	insl   (%dx),%es:(%rdi)
+    646cd57f:	je     646cd5b2 <.edata+0x5b2>
+    646cd581:	cmp    %edi,(%rcx)
+    646cd583:	xor    (%rdi),%esi
+    646cd585:	pop    %rdi
+    646cd586:	addr32 gs je 646cd5e9 <.edata+0x5e9>
+    646cd58a:	data16 insb (%dx),%es:(%rdi)
+    646cd58c:	outsl  %ds:(%rsi),(%dx)
+    646cd58d:	(bad)
+    646cd58e:	je     646cd5ef <.edata+0x5ef>
+    646cd590:	jb     646cd5f3 <.edata+0x5f3>
+    646cd592:	outsb  %ds:(%rsi),(%dx)
+    646cd593:	add    %ch,%gs:0x74(%ebp)
+    646cd598:	xor    %edi,(%rcx)
+    646cd59a:	cmp    %esi,(%rbx)
+    646cd59c:	(bad)
+    646cd59d:	pop    %rdi
+    646cd59e:	addr32 gs je 646cd601 <.edata+0x601>
+    646cd5a2:	imul   $0x725f3233,0x74(%rsi),%ebp
+    646cd5a9:	(bad)
+    646cd5aa:	outsb  %ds:(%rsi),(%dx)
+    646cd5ab:	add    %ch,%gs:0x74(%ebp)
+    646cd5b0:	xor    %edi,(%rcx)
+    646cd5b2:	cmp    %esi,(%rbx)
+    646cd5b4:	(bad)
+    646cd5b5:	pop    %rdi
+    646cd5b6:	imul   $0x746d0074,0x69(%rsi),%ebp
+    646cd5bd:	xor    %edi,(%rcx)
+    646cd5bf:	cmp    %esi,(%rbx)
+    646cd5c1:	(bad)
+    646cd5c2:	pop    %rdi
+    646cd5c3:	jb     646cd626 <.edata+0x626>
+    646cd5c5:	outsb  %ds:(%rsi),(%dx)
+    646cd5c6:	outsl  %fs:(%rsi),(%dx)
+    646cd5c8:	insl   (%dx),%es:(%rdi)
+    646cd5c9:	pop    %rdi
+    646cd5ca:	outsb  %ds:(%rsi),(%dx)
+    646cd5cb:	outsl  %ds:(%rsi),(%dx)
+    646cd5cc:	jb     646cd63b <.edata+0x63b>
+    646cd5ce:	(bad)
+    646cd5cf:	insb   (%dx),%es:(%rdi)
+    646cd5d0:	add    %dh,0x61(%rax)
+    646cd5d3:	jb     646cd649 <.edata+0x649>
+    646cd5d5:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
+    646cd5dd:	jo     646cd643 <.edata+0x643>
+    646cd5df:	imul   $0x69757100,0x74(%rbx),%esi
+    646cd5e6:	movsxd 0x73(%rbx),%ebp
+    646cd5e9:	gs insb (%dx),%es:(%rdi)
+    646cd5eb:	movsxd %gs:0x64(%rdx,%rsi,1),%esi
+    646cd5f0:	add    %dh,0x75(%rcx)
+    646cd5f3:	imul   $0x74726f73,0x6b(%rbx),%esp
+    646cd5fa:	xor    0x72(%rax,%rax,1),%ah
+    646cd5fe:	(bad)
+    646cd5ff:	outsb  %ds:(%rsi),(%dx)
+    646cd600:	outsl  %fs:(%rsi),(%dx)
+    646cd602:	insl   (%dx),%es:(%rdi)
+    646cd603:	jo     646cd666 <.edata+0x666>
+    646cd605:	je     646cd66f <.edata+0x66f>
+    646cd607:	add    %dh,0x61(%rbx)
+    646cd60a:	insl   (%dx),%es:(%rdi)
+    646cd60b:	jo     646cd679 <.edata+0x679>
+    646cd60d:	imul   $0x6174735f,0x67(%rsi),%ebp
+    646cd614:	je     646cd67b <.edata+0x67b>
+    646cd616:	pop    %rdi
+    646cd617:	imul   $0x61730074,0x69(%rsi),%ebp
+    646cd61e:	insl   (%dx),%es:(%rdi)
+    646cd61f:	jo     646cd68d <__bss_end__+0xafd>
+    646cd621:	imul   $0x6174735f,0x67(%rsi),%ebp
+    646cd628:	je     646cd68f <__bss_end__+0xaff>
+    646cd62a:	pop    %rdi
+    646cd62b:	jne    646cd69d <__bss_end__+0xb0d>
+    646cd62d:	fs (bad)
+    646cd62f:	je     646cd696 <__bss_end__+0xb06>
+    646cd631:	add    %dh,0x61(%rbx)
+    646cd634:	jbe    646cd69b <__bss_end__+0xb0b>
+    646cd636:	pop    %rdi
+    646cd637:	xor    %esp,0x72(%rcx,%riz,2)
+    646cd63b:	jb     646cd69e <__bss_end__+0xb0e>
+    646cd63d:	jns    646cd63f <.edata+0x63f>
+    646cd63f:	jae    646cd6a8 <__bss_end__+0xb18>
+    646cd641:	jae    646cd6ac <__bss_end__+0xb1c>
+    646cd643:	insl   (%dx),%es:(%rdi)
+    646cd644:	pop    %rdi
+    646cd645:	imul   $0x67730074,0x69(%rsi),%ebp
+    646cd64c:	jae    646cd6b7 <__bss_end__+0xb27>
+    646cd64e:	insl   (%dx),%es:(%rdi)
+    646cd64f:	pop    %rdi
+    646cd650:	jb     646cd6c7 <__bss_end__+0xb37>
+    646cd652:	outsb  %ds:(%rsi),(%dx)
+    646cd653:	add    %dh,0x67(%rbx)
+    646cd656:	jae    646cd6c1 <__bss_end__+0xb31>
+    646cd658:	insl   (%dx),%es:(%rdi)
+    646cd659:	pop    %rdi
+    646cd65a:	je     646cd6bb <__bss_end__+0xb2b>
+    646cd65c:	data16 jb 646cd6c4 <__bss_end__+0xb34>
+    646cd65f:	add    %dh,%gs:0x69(%rbx)
+    646cd663:	insl   (%dx),%es:(%rdi)
+    646cd664:	jo     646cd6d2 <__bss_end__+0xb42>
+    646cd666:	gs pop %rdi
+    646cd668:	imul   $0x67,0x69(%rdx),%esi
+    646cd66c:	imul   $0x61777300,0x67(%rsi),%ebp
+    646cd673:	jo     646cd6e7 <__bss_end__+0xb57>
+    646cd675:	outsl  %ds:(%rsi),(%dx)
+    646cd676:	ja     646cd6eb <__bss_end__+0xb5b>
+    646cd678:	add    %dh,0x61(%rsi)
+    646cd67b:	jb     646cd6e6 <__bss_end__+0xb56>
+    646cd67d:	(bad)
+    646cd67e:	outsb  %ds:(%rsi),(%dx)
+    646cd67f:	movsxd 0x0(%rbp),%esp
+    646cd682:	jbe    646cd6e5 <__bss_end__+0xb55>
+    646cd684:	jb     646cd6ef <__bss_end__+0xb5f>
+    646cd686:	outsl  %ds:(%rsi),(%dx)
+    646cd687:	addr32 jb 646cd6eb <__bss_end__+0xb5b>
+    646cd68a:	insl   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .idata:
 
 00000000646ce000 <_head_lib64_libkernel32_a>:
     646ce000:	cmp    $0xe0,%al
 	...
@@ -14956,23 +15013,20 @@
 00000000646cf020 <__xi_z>:
 	...
 
 00000000646cf028 <___crt_xi_end__>:
 	...
 
 00000000646cf030 <__xl_c>:
-    646cf030:	nop
-    646cf031:	push   %rsp
-    646cf032:	insb   (%dx),%es:(%rdi)
+    646cf030:	and    %dl,0x6c(%rbp)
     646cf033:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf038 <__xl_d>:
-    646cf038:	(bad)
-    646cf039:	push   %rsp
+    646cf038:	lock push %rsp
     646cf03a:	insb   (%dx),%es:(%rdi)
     646cf03b:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf040 <__xl_z>:
 	...
 
@@ -14992,18 +15046,17 @@
 
 Disassembly of section .reloc:
 
 00000000646d1000 <.reloc>:
     646d1000:	add    %dh,0x0(%rax)
     646d1003:	add    %cl,(%rax,%rax,1)
     646d1006:	add    %al,(%rax)
-    646d1008:	pop    %rax
-    646d1009:	stos   %eax,%es:(%rdi)
-    646d100a:	add    %al,(%rax)
-    646d100c:	add    %al,0x140000(%rax)
+    646d1008:	call   646d10b8 <___tls_end__+0x10a8>
+    646d100d:	addb   $0x0,(%rax)
+    646d1010:	adc    $0x0,%al
     646d1012:	add    %al,(%rax)
     646d1014:	add    %ah,-0x5fa75fb0(%rax)
     646d101a:	(bad)
     646d101b:	movabs 0x90000000a070,%al
     646d1024:	xor    $0x0,%al
     646d1026:	add    %al,(%rax)
     646d1028:	jo     646d0fcb <___tls_end__+0xfbb>
@@ -15030,16 +15083,16 @@
     646d2002:	add    %al,(%rax)
     646d2004:	add    (%rax),%al
     646d2006:	add    %al,(%rax)
     646d2008:	add    %al,(%rax)
     646d200a:	or     %al,(%rax)
     646d200c:	add    %al,(%rax)
     646d200e:	add    %al,(%rax)
-    646d2010:	mov    $0x64,%al
-    646d2012:	insb   (%dx),%es:(%rdi)
+    646d2010:	rex
+    646d2011:	gs insb (%dx),%es:(%rdi)
     646d2013:	add    %al,%fs:(%rax)
     646d2016:	add    %al,(%rax)
     646d2018:	xor    (%rax),%al
 	...
 
 00000000646d2030 <.debug_aranges>:
     646d2030:	sbb    $0x0,%al
@@ -15056,19 +15109,19 @@
     646d3002:	add    %al,(%rax)
     646d3004:	add    (%rax),%al
     646d3006:	add    %al,(%rax)
     646d3008:	add    %al,(%rax)
     646d300a:	or     %al,(%rcx)
     646d300c:	add    %al,(%rax)
     646d300e:	add    %al,(%rax)
-    646d3010:	mov    $0x64,%al
-    646d3012:	insb   (%dx),%es:(%rdi)
+    646d3010:	rex
+    646d3011:	gs insb (%dx),%es:(%rdi)
     646d3013:	add    %al,%fs:(%rax)
     646d3016:	add    %al,(%rax)
-    646d3018:	loop   646d307e <.debug_info+0x50>
+    646d3018:	jb     646d307f <.debug_info+0x51>
     646d301a:	insb   (%dx),%es:(%rdi)
     646d301b:	add    %al,%fs:(%rax)
     646d301e:	add    %al,(%rax)
     646d3020:	add    %al,(%rax)
     646d3022:	add    %al,(%rax)
     646d3024:	cmp    %eax,(%rax)
     646d3026:	add    %al,(%rax)
@@ -19185,23 +19238,23 @@
     646d4ed8:	pop    %rdi
     646d4ed9:	add    %cl,(%rax,%rsi,1)
     646d4edc:	adc    %edi,0x0(%rsi,%rbx,1)
     646d4ee0:	add    %bl,(%rax)
     646d4ee2:	xchg   %ebx,(%rsi)
     646d4ee4:	add    %al,(%rax)
     646d4ee6:	or     $0x90a0939,%eax
-    646d4eeb:	add    0x7b(%rax),%edx
-    646d4eee:	insb   (%dx),%es:(%rdi)
+    646d4eeb:	add    %eax,%esp
+    646d4eed:	jnp    646d4f5b <.debug_info+0x1f2d>
     646d4eef:	add    %al,%fs:(%rax)
     646d4ef2:	add    %al,(%rax)
     646d4ef4:	sbb    %bl,0xd00001e(%rbp)
     646d4efa:	cmp    (%rcx),%cl
     646d4efc:	or     (%rcx),%cl
-    646d4efe:	add    0x7b(%rax),%ebp
-    646d4f01:	insb   (%dx),%es:(%rdi)
+    646d4efe:	add    %eax,%edi
+    646d4f00:	jnp    646d4f6e <.debug_info+0x1f40>
     646d4f02:	add    %al,%fs:(%rax)
     646d4f05:	add    %al,(%rax)
 	...
 
 Disassembly of section .debug_abbrev:
 
 00000000646d5000 <.debug_abbrev>:
@@ -19375,16 +19428,16 @@
     646d604f:	ja     646d60ba <.debug_line+0x3f>
     646d6051:	outsb  %ds:(%rsi),(%dx)
     646d6052:	cs push %rbx
     646d6054:	add    %al,(%rcx)
     646d6056:	add    %al,(%rax)
     646d6058:	add    %al,(%rax)
     646d605a:	or     %eax,(%rdx)
-    646d605c:	mov    $0x64,%al
-    646d605e:	insb   (%dx),%es:(%rdi)
+    646d605c:	rex
+    646d605d:	gs insb (%dx),%es:(%rdi)
     646d605f:	add    %al,%fs:(%rax)
     646d6062:	add    %al,(%rax)
     646d6064:	add    %esp,%esi
     646d6066:	add    %al,(%rcx)
     646d6068:	and    (%rdx),%ah
     646d606a:	addr32 pop %rcx
     646d606c:	xor    %dh,0x4b(%rbp)
@@ -19548,16 +19601,16 @@
     646d700d:	or     $0x7,%al
     646d700f:	or     %ah,0x1(%rax)
     646d7015:	add    %al,(%rax)
     646d7017:	add    %ch,(%rax,%rax,1)
     646d701a:	add    %al,(%rax)
     646d701c:	add    %al,(%rax)
     646d701e:	add    %al,(%rax)
-    646d7020:	mov    $0x64,%al
-    646d7022:	insb   (%dx),%es:(%rdi)
+    646d7020:	rex
+    646d7021:	gs insb (%dx),%es:(%rdi)
     646d7023:	add    %al,%fs:(%rax)
     646d7026:	add    %al,(%rax)
     646d7028:	xor    (%rax),%al
     646d702a:	add    %al,(%rax)
     646d702c:	add    %al,(%rax)
     646d702e:	add    %al,(%rax)
     646d7030:	rex.B (bad)
```

### Comparing `uc_sgsim-1.2.2/uc_sgsim/cov_model/base.py` & `uc_sgsim-1.2.3/uc_sgsim/cov_model/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/cov_model/model.py` & `uc_sgsim-1.2.3/uc_sgsim/cov_model/model.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/krige/base.py` & `uc_sgsim-1.2.3/uc_sgsim/krige/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/krige/kriging.py` & `uc_sgsim-1.2.3/uc_sgsim/krige/kriging.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/plot/base.py` & `uc_sgsim-1.2.3/uc_sgsim/plot/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/plot/plot.py` & `uc_sgsim-1.2.3/uc_sgsim/plot/plot.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim/random_field.py` & `uc_sgsim-1.2.3/uc_sgsim/random_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import numpy as np
 from uc_sgsim.exception import VariogramDoesNotCompute
 from uc_sgsim.utils import save_as_multiple_file, save_as_one_file
 from uc_sgsim.cov_model.base import CovModel
 
 
 class RandomField:
-    def __init__(self, x: int, model: CovModel, realization_number: int):
-        self.__model = model
+    def __init__(self, x: int, realization_number: int):
         self.__realization_number = realization_number
-        self.__bandwidth_step = model.bandwidth_step
-        self.__bandwidth = model.bandwidth
-        self.__create_grid(x)
+        self._create_grid(x)
 
-    def __create_grid(self, x: int, y: int = 0) -> None:
+    def _create_grid(self, x: int, y: int = 0) -> None:
         self.__x = range(x)
         self.__y = range(y)
         self.__x_size = len(self.__x)
         self.__y_size = len(self.__y)
         self.random_field = np.empty([self.__realization_number, self.__x_size])
         self.variogram = 0
 
@@ -33,33 +30,21 @@
         return self.__y
 
     @property
     def y_size(self) -> int:
         return self.__y_size
 
     @property
-    def model(self) -> CovModel:
-        return self.__model
-
-    @property
     def realization_number(self) -> int:
         return self.__realization_number
 
     @realization_number.setter
     def realization_number(self, val: int):
         self.__realization_number = val
 
-    @property
-    def bandwidth(self) -> np.array:
-        return self.__bandwidth
-
-    @property
-    def bandwidth_step(self) -> int:
-        return self.__bandwidth_step
-
     def save_random_field(
         self,
         path: str,
         file_type: str = 'csv',
         save_single: bool = False,
     ) -> None:
         digit = int(np.log10(self.realization_number))
@@ -102,7 +87,32 @@
                     len(self.bandwidth),
                     self.variogram,
                     file_type,
                     'Variogram',
                 )
         else:
             save_as_one_file(path, self.variogram)
+
+
+class SgsimField(RandomField):
+    def __init__(
+        self,
+        x: int,
+        realization_number: int,
+        model: CovModel,
+    ):
+        super().__init__(x, realization_number)
+        self.__model = model
+        self.__bandwidth_step = model.bandwidth_step
+        self.__bandwidth = model.bandwidth
+
+    @property
+    def model(self) -> CovModel:
+        return self.__model
+
+    @property
+    def bandwidth(self) -> np.array:
+        return self.__bandwidth
+
+    @property
+    def bandwidth_step(self) -> int:
+        return self.__bandwidth_step
```

### Comparing `uc_sgsim-1.2.2/uc_sgsim/sgsim.py` & `uc_sgsim-1.2.3/uc_sgsim/sgsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 from ctypes import CDLL, POINTER, c_double, c_int
 from multiprocessing import Pool
 
 import numpy as np
 from uc_sgsim.exception import VariogramDoesNotCompute
 from uc_sgsim.krige import SimpleKrige
-from uc_sgsim.random_field import RandomField
+from uc_sgsim.random_field import SgsimField
 from uc_sgsim.plot.plot import Visualize
 from uc_sgsim.cov_model.base import CovModel
 from uc_sgsim.utils import CovModelStructure, SgsimStructure
 
 BASE_DIR = Path(__file__).resolve().parent
 
 
-class UCSgsim(RandomField):
+class UCSgsim(SgsimField):
     def __init__(
         self,
         x: int,
         model: CovModel,
         realization_number: int,
         krige_method: str = 'SimpleKrige',
     ):
```

### Comparing `uc_sgsim-1.2.2/uc_sgsim/utils.py` & `uc_sgsim-1.2.3/uc_sgsim/utils.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.2/uc_sgsim.egg-info/PKG-INFO` & `uc_sgsim-1.2.3/uc_sgsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: uc-sgsim
-Version: 1.2.2
+Version: 1.2.3
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
@@ -124,28 +128,28 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
-    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
+    sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
     sgsim_c.mean_plot('ALL')  # Plot mean
     sgsim_c.variance_plot()  # Plot variance
     sgsim_c.cdf_plot(x_location=10)  # CDF
     sgsim_c.hist_plot(x_location=10)  # Hist
     sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim_c.vario_plot()
+    sgsim.variogram_plot()
     # Save random_field and variogram
     sgsim_c.save_random_field('randomfields.csv', save_single=True)
     sgsim_c.save_variogram('variograms.csv', save_single=True)
 
     # show figure
     plt.show()
 ```
```

### Comparing `uc_sgsim-1.2.2/uc_sgsim.egg-info/SOURCES.txt` & `uc_sgsim-1.2.3/uc_sgsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

