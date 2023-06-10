# Comparing `tmp/iman-0.0.8.tar.gz` & `tmp/iman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iman-0.0.8.tar", last modified: Wed Oct 26 08:41:58 2022, max compression
+gzip compressed data, was "dist\iman-0.0.9.tar", last modified: Wed Oct 26 09:01:02 2022, max compression
```

## Comparing `iman-0.0.8.tar` & `iman-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-26 08:41:58.000000 iman-0.0.8/
--rw-rw-rw-   0        0        0     1794 2022-10-26 08:41:58.000000 iman-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-26 08:41:58.000000 iman-0.0.8/iman/
--rw-rw-rw-   0        0        0    11046 2022-10-25 11:17:35.000000 iman-0.0.8/iman/Audio.py
--rw-rw-rw-   0        0        0     3956 2022-10-26 08:41:15.000000 iman-0.0.8/iman/__init__.py
--rw-rw-rw-   0        0        0      843 2022-10-25 11:17:47.000000 iman-0.0.8/iman/info.py
--rw-rw-rw-   0        0        0     2440 2022-10-26 08:38:23.000000 iman-0.0.8/iman/metrics.py
--rw-rw-rw-   0        0        0      329 2022-10-25 11:18:01.000000 iman-0.0.8/iman/tsne.py
--rw-rw-rw-   0        0        0     7118 2022-10-26 06:01:06.000000 iman-0.0.8/iman/xvector.py
-drwxrwxrwx   0        0        0        0 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/
--rw-rw-rw-   0        0        0     1794 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-10-26 08:41:58.000000 iman-0.0.8/iman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-26 08:41:58.000000 iman-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2197 2022-10-26 08:41:03.000000 iman-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman/
+-rw-rw-rw-   0        0        0    11046 2022-10-25 11:17:35.000000 iman-0.0.9/iman/Audio.py
+-rw-rw-rw-   0        0        0     3963 2022-10-26 08:59:53.000000 iman-0.0.9/iman/__init__.py
+-rw-rw-rw-   0        0        0      843 2022-10-25 11:17:47.000000 iman-0.0.9/iman/info.py
+-rw-rw-rw-   0        0        0     2440 2022-10-26 08:38:23.000000 iman-0.0.9/iman/metrics.py
+-rw-rw-rw-   0        0        0      329 2022-10-25 11:18:01.000000 iman-0.0.9/iman/tsne.py
+-rw-rw-rw-   0        0        0     7143 2022-10-26 08:59:26.000000 iman-0.0.9/iman/xvector.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-26 09:01:02.000000 iman-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2022-10-26 09:00:03.000000 iman-0.0.9/setup.py
```

### Comparing `iman-0.0.8/PKG-INFO` & `iman-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
@@ -61,11 +61,11 @@
 6-wer_list(ref_list , hyp_list)
 7-cer_list(ref_list , hyp_list)
 
 from iman import tsne:
 1-plot(fea , label)
 
 from iman import xvector:
-1-xvec,lda_xvec,gender = get(filename , model_path , model_name , model_speaker_num)
+1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))
```

### Comparing `iman-0.0.8/iman/Audio.py` & `iman-0.0.9/iman/Audio.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.8/iman/__init__.py` & `iman-0.0.9/iman/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 import time
 from glob import glob as gf
 import os
 import numpy as np
 
 def help():
-   print('from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model_path , model_name , model_speaker_num)\n\n')
+   print('from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))\n\n')
 
    
 def clear():
     if os.name == 'nt':
         _ = os.system('cls')  
     else:
         _ = os.system('clear')
```

### Comparing `iman-0.0.8/iman/info.py` & `iman-0.0.9/iman/info.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.8/iman/metrics.py` & `iman-0.0.9/iman/metrics.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.8/iman/xvector.py` & `iman-0.0.9/iman/xvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,20 +191,23 @@
   return modelxvec
 
 def get_xvec(feat, modelxvec ,batch_size):
  
   xvec,gender = modelxvec.predict(feat, batch_size = batch_size,verbose=1,use_multiprocessing=True)
   return xvec,gender
 
-def get(filename , model_path , model_name , model_speaker_num):
-   model = get_model(model_path , model_name , model_speaker_num)
+
+def model(model_path , model_name , model_speaker_num):
+    return get_model(model_path , model_name , model_speaker_num)
+
+def get(filename , _model):
    sample_rate=8000
    data =Audio.Read(filename , sample_rate)
    fea = get_fea_file(data , sample_rate)
-   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), model, batch_size=1)
+   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), _model, batch_size=1)
    xvec_lda = apply_lda(xvec, PJ(model_path, 'meanvec.npy'), PJ(model_path, 'lda.job'))
    gender='male'
    if (a[0][0]>=a[0][1]):
        gender='female'
    return(np.squeeze(xvec),np.squeeze(xvec_lda),gender)
```

### Comparing `iman-0.0.8/iman.egg-info/PKG-INFO` & `iman-0.0.9/iman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
@@ -61,11 +61,11 @@
 6-wer_list(ref_list , hyp_list)
 7-cer_list(ref_list , hyp_list)
 
 from iman import tsne:
 1-plot(fea , label)
 
 from iman import xvector:
-1-xvec,lda_xvec,gender = get(filename , model_path , model_name , model_speaker_num)
+1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))
```

### Comparing `iman-0.0.8/setup.py` & `iman-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
         # the name must match the folder name 'verysimplemodule'
         name="iman", 
-        version='0.0.8',
+        version='0.0.9',
         author="Iman Sarraf",
         author_email="imansarraf@gmail.com",
         description='Python package for daily Tasks',
-        long_description='from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model_path , model_name , model_speaker_num)\n\n',
+        long_description='from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))\n\n',
         packages=find_packages(),
         
         # add any additional packages that 
         # needs to be installed along with your package.
         install_requires=['scipy','numpy','six','matplotlib'], 
         
         keywords=['python', 'iman'],
```

