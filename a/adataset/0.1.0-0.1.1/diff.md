# Comparing `tmp/adataset-0.1.0.tar.gz` & `tmp/adataset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adataset-0.1.0.tar", last modified: Wed Jan 18 10:50:02 2023, max compression
+gzip compressed data, was "adataset-0.1.1.tar", last modified: Sat Jun 10 11:50:55 2023, max compression
```

## Comparing `adataset-0.1.0.tar` & `adataset-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.957413 adataset-0.1.0/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-01-18 10:50:02.957283 adataset-0.1.0/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-01-18 10:42:59.000000 adataset-0.1.0/README.md
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.953968 adataset-0.1.0/adataset/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-01-18 03:39:48.000000 adataset-0.1.0/adataset/__init__.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.953288 adataset-0.1.0/adataset/calibration_meta/
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.954194 adataset-0.1.0/adataset/calibration_meta/camera_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.954328 adataset-0.1.0/adataset/calibration_meta/gnss_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.954453 adataset-0.1.0/adataset/calibration_meta/radar_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.954575 adataset-0.1.0/adataset/calibration_meta/vehicle_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.954795 adataset-0.1.0/adataset/calibration_meta/velodyne_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/velodyne_params/lidar_height.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.955775 adataset-0.1.0/adataset/kitti/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-01-18 08:37:20.000000 adataset-0.1.0/adataset/kitti/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)    10884 2023-01-18 10:24:42.000000 adataset-0.1.0/adataset/kitti/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/kitti/common.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4037 2023-01-18 08:44:16.000000 adataset-0.1.0/adataset/kitti/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     5406 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/kitti/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-01-18 06:50:05.000000 adataset-0.1.0/adataset/kitti/kitti.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/kitti/pcd_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/kitti/proj_helper.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/kitti/sensor.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-01-18 08:40:40.000000 adataset-0.1.0/adataset/main.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.956472 adataset-0.1.0/adataset/nuscenes/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-01-18 08:37:25.000000 adataset-0.1.0/adataset/nuscenes/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     9030 2023-01-18 09:31:04.000000 adataset-0.1.0/adataset/nuscenes/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3950 2023-01-18 08:43:08.000000 adataset-0.1.0/adataset/nuscenes/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4825 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/nuscenes/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/nuscenes/nuscenes.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2022-12-27 01:38:59.000000 adataset-0.1.0/adataset/nuscenes/pcd_converter.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-01-18 10:50:02.957133 adataset-0.1.0/adataset.egg-info/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1219 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/SOURCES.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/dependency_links.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/entry_points.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/requires.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-01-18 10:50:02.000000 adataset-0.1.0/adataset.egg-info/top_level.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-01-18 10:50:02.957453 adataset-0.1.0/setup.cfg
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-01-18 10:29:28.000000 adataset-0.1.0/setup.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.498804 adataset-0.1.1/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-10 11:50:55.498561 adataset-0.1.1/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-05-20 04:47:09.000000 adataset-0.1.1/README.md
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.475995 adataset-0.1.1/adataset/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/__init__.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.470794 adataset-0.1.1/adataset/calibration_meta/
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.477464 adataset-0.1.1/adataset/calibration_meta/camera_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.477940 adataset-0.1.1/adataset/calibration_meta/gnss_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.478409 adataset-0.1.1/adataset/calibration_meta/radar_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.478943 adataset-0.1.1/adataset/calibration_meta/vehicle_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.480285 adataset-0.1.1/adataset/calibration_meta/velodyne_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/velodyne_params/lidar_height.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.487923 adataset-0.1.1/adataset/kitti/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12153 2023-06-10 11:44:42.000000 adataset-0.1.1/adataset/kitti/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/common.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3707 2023-06-10 11:46:05.000000 adataset-0.1.1/adataset/kitti/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 11:44:59.000000 adataset-0.1.1/adataset/kitti/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/kitti.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1892 2023-06-10 11:45:15.000000 adataset-0.1.1/adataset/kitti/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/pcd_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/proj_helper.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/sensor.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/main.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.493162 adataset-0.1.1/adataset/nuscenes/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12194 2023-06-10 11:48:19.000000 adataset-0.1.1/adataset/nuscenes/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3956 2023-06-10 11:33:09.000000 adataset-0.1.1/adataset/nuscenes/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 10:39:20.000000 adataset-0.1.1/adataset/nuscenes/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/nuscenes.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     2363 2023-06-10 11:09:08.000000 adataset-0.1.1/adataset/nuscenes/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/pcd_converter.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.498263 adataset-0.1.1/adataset.egg-info/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1276 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/entry_points.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/requires.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/top_level.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-06-10 11:50:55.498877 adataset-0.1.1/setup.cfg
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-06-10 09:41:03.000000 adataset-0.1.1/setup.py
```

### Comparing `adataset-0.1.0/PKG-INFO` & `adataset-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.0/README.md` & `adataset-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/calibration_meta/camera_params/camera_intrinsics.yaml` & `adataset-0.1.1/adataset/calibration_meta/camera_params/camera_intrinsics.yaml`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/kitti/calibration_converter.py` & `adataset-0.1.1/adataset/kitti/calibration_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 import yaml
 import numpy as np
 import pkgutil
 
 from pathlib import Path
 
 from adataset.kitti.geometry import Euler, rotation_matrix_to_euler
-
+from adataset.kitti.params import (
+  apollo2kitti_lidar,
+  apollo2kitti_camera,
+  apollo2kitti_imu,
+  kitti2apollo_lidar,
+  kitti2apollo_camera,
+)
 
 CALIBRATION_META_ROOT = 'calibration_meta'
 # Lidar meta
 VELODYNE_PARAMS_PATH = 'velodyne_params'
 LIDAR_NOVATEL_EXTRINSICS = 'lidar_novatel_extrinsics.yaml'
 # Camera meta
 CAMERA_PARAMS_PATH ='camera_params'
@@ -41,14 +47,21 @@
 
 # Frame ID
 CAMERA_FRAME_ID = 'velodyne64'
 RADAR_FRAME_ID = 'novatel'
 LIDAR_FRAME_ID = 'novatel'
 
 
+def _matrix_padding4x4(r_array):
+  transform = np.empty((4, 4))
+  transform[:3,:3] = r_array.reshape((3, 3))
+  transform[:3, 3] = [0, 0, 0]
+  transform[3, :]  = [0, 0, 0, 1]
+  return transform
+
 def load_yaml(file_path):
   """Read content from yaml
 
   Args:
       file_path (str): yaml file
 
   Returns:
@@ -193,15 +206,22 @@
 def process_calib_imu_to_velo(dataset_path, calibration_file_path):
   absolute_path = os.path.join(dataset_path, 'calib_imu_to_velo.txt')
   calibrated_sensor = dict()
   with open(absolute_path, 'r') as f:
     lines = f.readlines()
     r = lines[1].lstrip('R:').split()
     r_array = np.array(r, dtype=np.float32)
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array.reshape((3, 3)))
+    # Apollo coordinate system conversion
+    # k_imu * imu2lidar = k_lidar
+    # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
+    transform = _matrix_padding4x4(r_array)
+    imu_to_velo = apollo2kitti_imu @ transform @ kitti2apollo_lidar
+    r_array = imu_to_velo[:3,:3]
+
+    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
 
     t = lines[2].lstrip('T:').split()
     calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
 
   gen_velodyne_params('velodyne64', calibrated_sensor, calibration_file_path)
@@ -226,15 +246,23 @@
     calibrated_sensor['K'] = np.array(k, dtype=np.float32).tolist()
 
     d = lines[2][len('S_00:'):].strip().split()
     calibrated_sensor['D'] = np.array(d, dtype=np.float32).tolist()
 
     r = lines[3][len('S_00:'):].strip().split()
     r_array = np.array(r, dtype=np.float32)
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array.reshape((3, 3)))
+    # Todo(zero): Need to generate cam to cam external parameters
+    # Apollo coordinate system conversion
+    # k_cam * cam2cam = k_cam
+    # apollo_camera * apollo2k_camera * cam2cam = apollo_camera * apollo2k_camera
+    transform = _matrix_padding4x4(r_array)
+    cam_to_cam = apollo2kitti_camera @ transform @ kitti2apollo_camera
+    r_array = cam_to_cam[:3,:3]
+
+    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
 
     t = lines[4][len('S_00:'):].strip().split()
     calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
 
     s_rect = lines[5][len('S_rect_01:'):].strip().split()
@@ -251,15 +279,22 @@
 def process_calib_velo_to_cam(dataset_path, calibration_file_path):
   absolute_path = os.path.join(dataset_path, 'calib_velo_to_cam.txt')
   calibrated_sensor = dict()
   with open(absolute_path, 'r') as f:
     lines = f.readlines()
     r = lines[1].lstrip('R:').split()
     r_array = np.array(r, dtype=np.float32)
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array.reshape((3, 3)))
+    # Apollo coordinate system conversion
+    # k_lidar * lidar2cam = k_camera
+    # apollo_lidar * apollo2k_lidar * lidar2cam = apollo_camera * apollo2k_camera
+    transform = _matrix_padding4x4(r_array)
+    velo_to_cam = apollo2kitti_lidar @ transform @ kitti2apollo_camera
+    r_array = velo_to_cam[:3,:3]
+
+    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
 
     t = lines[2].lstrip('T:').split()
     calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
 
   gen_camera_extrinsics('camera', calibrated_sensor, calibration_file_path)
```

### Comparing `adataset-0.1.0/adataset/kitti/common.py` & `adataset-0.1.1/adataset/kitti/common.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/kitti/dataset_converter.py` & `adataset-0.1.1/adataset/kitti/dataset_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,44 +14,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###############################################################################
 '''Generate apollo record file by kitti raw sensor data.'''
 
 import logging
-import numpy as np
 
 from cyber_record.record import Record
 from record_msg.builder import (
   ImageBuilder,
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
 from adataset.kitti.kitti import KITTISchema, KITTI
-from adataset.kitti.geometry import Quaternion
+from adataset.kitti.geometry import Quaternion, Euler, rotation_matrix_to_euler
+from adataset.kitti.params import (
+  kitti2apollo_lidar,
+  kitti2apollo_imu
+)
 
 
 LOCALIZATION_TOPIC = '/apollo/localization/pose'
 TF_TOPIC= '/tf'
 
 
-# Need to convert to apollo coordinate system
-imu_to_velo = np.array(
-    [[ 9.999976e-01, 7.553071e-04,-2.035826e-03,-8.086759e-01],
-     [-7.854027e-04, 9.998898e-01,-1.482298e-02, 3.195559e-01],
-     [ 2.024406e-03, 1.482454e-02, 9.998881e-01,-7.997231e-01],
-     [ 0.0000000, 0.0000000, 0.0000000, 1.0000000]])
-
-kitti_to_apollo = np.array([[ 0.0000000, 1.0000000, 0.0000000, 0.0000000],
-                            [-1.0000000, 0.0000000, 0.0000000, 0.0000000],
-                            [ 0.0000000, 0.0000000, 1.0000000, 0.0000000],
-                            [ 0.0000000, 0.0000000, 0.0000000, 1.0000000]])
-
-LIDAR_TRANSFORM = np.matmul(np.linalg.inv(imu_to_velo), kitti_to_apollo)
-
 def dataset_to_record(kitti, record_root_path):
   """Construct record message and save it as record
 
   Args:
       kitti (_type_): kitti
       record_root_path (str): record file saved path
   """
@@ -67,15 +56,15 @@
       pb_msg = None
       # There're mix gray and rgb image files, so we just choose rgb image
       if c == 'image_02' or c == 'image_03':
         # KITTI image types: 'gray', 'bgr8'
         pb_msg = image_builder.build(f, 'camera', 'bgr8', t)
         channel_name = "/apollo/sensor/camera/{}/image".format(c)
       elif c.startswith('velodyne'):
-        pb_msg = pc_builder.build_nuscenes(f, 'velodyne', t, LIDAR_TRANSFORM)
+        pb_msg = pc_builder.build_nuscenes(f, 'velodyne', t, kitti2apollo_lidar)
         channel_name = "/apollo/sensor/{}/compensator/PointCloud2".format(c)
 
       if pb_msg:
         record.write(channel_name, pb_msg, int(t*1e9))
 
       if ego_pose:
         rotation = ego_pose.rotation
@@ -83,16 +72,21 @@
         heading = quat.to_euler().yaw
 
         pb_msg = localization_builder.build(
           ego_pose.translation, ego_pose.rotation, heading, t)
         if pb_msg:
           record.write(LOCALIZATION_TOPIC, pb_msg, int(t*1e9))
 
+        # Apollo coordinate system conversion
+        r_array = kitti2apollo_imu[:3,:3]
+        roll, pitch, yaw = rotation_matrix_to_euler(r_array)
+        kitti2apollo_q = Euler(roll, pitch, yaw).to_quaternion()
+        quat = quat * kitti2apollo_q
         pb_msg = transform_builder.build('world', 'localization',
-          ego_pose.translation, ego_pose.rotation, t)
+          ego_pose.translation, [quat.w, quat.x, quat.y, quat.z], t)
         if pb_msg:
           record.write(TF_TOPIC, pb_msg, int(t*1e9))
 
 
 def convert_dataset(dataset_path, record_path):
   """Generate apollo record file by KITTI dataset
```

### Comparing `adataset-0.1.0/adataset/kitti/geometry.py` & `adataset-0.1.1/adataset/kitti/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,7 +142,10 @@
 
   def __mul__(self, other):
     w = self.w * other.w - self.x * other.x - self.y * other.y - self.z * other.z
     x = self.w * other.x + self.x * other.w + self.y * other.z - self.z * other.y
     y = self.w * other.y - self.x * other.z + self.y * other.w + self.z * other.x
     z = self.w * other.z + self.x * other.y - self.y * other.x + self.z * other.w
     return Quaternion(w, x, y, z)
+
+  def __str__(self) -> str:
+    return "w: {}, x: {}, y: {}, z: {}".format(self.w, self.x, self.y, self.z)
```

### Comparing `adataset-0.1.0/adataset/kitti/kitti.py` & `adataset-0.1.1/adataset/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/kitti/pcd_converter.py` & `adataset-0.1.1/adataset/kitti/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/kitti/proj_helper.py` & `adataset-0.1.1/adataset/kitti/proj_helper.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/kitti/sensor.py` & `adataset-0.1.1/adataset/kitti/sensor.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/main.py` & `adataset-0.1.1/adataset/main.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/nuscenes/calibration_converter.py` & `adataset-0.1.1/adataset/nuscenes/calibration_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,33 @@
 # limitations under the License.
 ###############################################################################
 '''Generate apollo calibration files by nuscenes calibration data.'''
 
 import os
 import yaml
 import pkgutil
+import numpy as np
 
 from itertools import chain
 from pathlib import Path
 
 from adataset.nuscenes.nuscenes import NuScenesSchema, NuScenesHelper, NuScenes
-
+from adataset.nuscenes.geometry import (
+  Euler,
+  Quaternion,
+  euler_to_rotation_matrix,
+  rotation_matrix_to_euler
+)
+from adataset.nuscenes.params import (
+  apollo2nuscenes_lidar,
+  apollo2nuscenes_imu,
+  nuscenes2apollo_camera,
+  nuscenes2apollo_lidar,
+  nuscenes2apollo_radar,
+)
 
 CALIBRATION_META_ROOT = 'calibration_meta'
 # Lidar meta
 VELODYNE_PARAMS_PATH = 'velodyne_params'
 LIDAR_NOVATEL_EXTRINSICS = 'lidar_novatel_extrinsics.yaml'
 # Camera meta
 CAMERA_PARAMS_PATH ='camera_params'
@@ -40,14 +53,20 @@
 RADAR_EXTRINSICS = 'radar_extrinsics.yaml'
 
 # Frame ID
 CAMERA_FRAME_ID = 'novatel'
 RADAR_FRAME_ID = 'novatel'
 LIDAR_FRAME_ID = 'novatel'
 
+def _construct_transform(r, t):
+  transform = np.empty((4, 4))
+  transform[:3,:3] = r
+  transform[:3, 3] = t
+  transform[3, :]  = [0, 0, 0, 1]
+  return transform
 
 def load_yaml(file_path):
   """Read content from yaml
 
   Args:
       file_path (str): yaml file
 
@@ -174,28 +193,87 @@
   file_path = os.path.join(calibration_file_path, VELODYNE_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   lidar_novatel_extrinsics = os.path.join(file_path, file_name)
   save_yaml(lidar_novatel_extrinsics, lidar_extrinsics)
 
 
+def process_calib_imu_to_velo(channel, calibrated_sensor, calibration_file_path):
+  qw, qx, qy, qz = calibrated_sensor['rotation']
+  q = Quaternion(qw, qx, qy, qz)
+  euler = q.to_euler()
+  r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
+  # Apollo coordinate system conversion
+  # k_imu * imu2lidar = k_lidar
+  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
+  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  imu_to_velo = apollo2nuscenes_imu @ transform @ nuscenes2apollo_lidar
+  r_matrix = imu_to_velo[:3,:3]
+
+  roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
+  q = Euler(roll, pitch, yaw).to_quaternion()
+  calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+
+  calibrated_sensor['translation'] = imu_to_velo[:3, 3].tolist()
+  gen_velodyne_params(channel, calibrated_sensor, calibration_file_path)
+
+def process_calib_velo_to_cam(channel, calibrated_sensor, calibration_file_path):
+  qw, qx, qy, qz = calibrated_sensor['rotation']
+  q = Quaternion(qw, qx, qy, qz)
+  euler = q.to_euler()
+  r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
+  # Apollo coordinate system conversion
+  # k_imu * imu2lidar = k_lidar
+  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
+  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  velo_to_cam = apollo2nuscenes_lidar @ transform @ nuscenes2apollo_camera
+  r_matrix = velo_to_cam[:3,:3]
+
+  roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
+  q = Euler(roll, pitch, yaw).to_quaternion()
+  calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+
+  calibrated_sensor['translation'] = velo_to_cam[:3, 3].tolist()
+  gen_radar_params(channel, calibrated_sensor, calibration_file_path)
+
+
+def process_calib_velo_to_radar(channel, calibrated_sensor, calibration_file_path):
+  qw, qx, qy, qz = calibrated_sensor['rotation']
+  q = Quaternion(qw, qx, qy, qz)
+  euler = q.to_euler()
+  r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
+  # Apollo coordinate system conversion
+  # k_imu * imu2lidar = k_lidar
+  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
+  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  velo_to_radar = apollo2nuscenes_lidar @ transform @ nuscenes2apollo_radar
+  r_matrix = velo_to_radar[:3,:3]
+
+  roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
+  q = Euler(roll, pitch, yaw).to_quaternion()
+  calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+
+  calibrated_sensor['translation'] = velo_to_radar[:3, 3].tolist()
+  gen_radar_params(channel, calibrated_sensor, calibration_file_path)
+
+
 def gen_sensor_calibration(calibrations, calibration_file_path):
   """Generate camera/radar/lidar extrinsic file and camera intrinsic file
 
   Args:
       calibrations (dict): nuscenes calibrated_sensor json objects
       calibration_file_path (str): saved path
   """
   for channel, calibrated_sensor in calibrations.items():
     if channel.startswith('CAM'):
-      gen_camera_params(channel, calibrated_sensor, calibration_file_path)
+      process_calib_imu_to_velo(channel, calibrated_sensor, calibration_file_path)
     elif channel.startswith('LIDAR'):
-      gen_velodyne_params(channel, calibrated_sensor, calibration_file_path)
+      process_calib_velo_to_cam(channel, calibrated_sensor, calibration_file_path)
     elif channel.startswith('RADAR'):
-      gen_radar_params(channel, calibrated_sensor, calibration_file_path)
+      process_calib_velo_to_radar(channel, calibrated_sensor, calibration_file_path)
     else:
       print("Unsupported sensor: {}".format(channel))
 
 
 def dataset_to_calibration(nuscenes, calibration_root_path):
   """Generate sensor calibration
```

### Comparing `adataset-0.1.0/adataset/nuscenes/dataset_converter.py` & `adataset-0.1.1/adataset/nuscenes/dataset_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###############################################################################
 '''Generate apollo record file by nuscenes raw sensor data.'''
 
 import os
 import logging
-import numpy as np
 
 from cyber_record.record import Record
 from record_msg.builder import (
   ImageBuilder,
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
 from adataset.nuscenes.nuscenes import NuScenesSchema, NuScenesHelper, NuScenes
-from adataset.nuscenes.geometry import Quaternion
-
+from adataset.nuscenes.geometry import (
+  Euler,
+  Quaternion,
+  rotation_matrix_to_euler
+)
+from adataset.nuscenes.params import (
+  nuscenes2apollo_lidar,
+  nuscenes2apollo_imu,
+)
 
 LOCALIZATION_TOPIC = '/apollo/localization/pose'
 TF_TOPIC= '/tf'
 
 
-# Need to convert to apollo coordinate system, for nuscenes is 90 degrees
-LIDAR_TRANSFORM = np.array([[ 0.0020333, 0.9997041, 0.0242417, 0.9437130],
-                            [-0.9999805, 0.0021757,-0.0058486, 0.0000000],
-                            [-0.0058997,-0.0242294, 0.9996890, 1.8402300],
-                            [ 0.0000000, 0.0000000, 0.0000000, 1.0000000]])
-
 def dataset_to_record(nuscenes, record_root_path):
   """Construct record message and save it as record
 
   Args:
       nuscenes (_type_): nuscenes(one scene)
       record_root_path (str): record file saved path
   """
@@ -60,15 +60,15 @@
     for c, f, ego_pose, calibrated_sensor, t in nuscenes:
       logging.debug("{}, {}, {}, {}".format(c, f, ego_pose, t))
       pb_msg = None
       if c.startswith('CAM'):
         pb_msg = image_builder.build(f, 'camera', 'rgb8', t/1e6)
         channel_name = "/apollo/sensor/camera/{}/image".format(c)
       elif c.startswith('LIDAR'):
-        pb_msg = pc_builder.build_nuscenes(f, 'velodyne', t/1e6, LIDAR_TRANSFORM)
+        pb_msg = pc_builder.build_nuscenes(f, 'velodyne', t/1e6, nuscenes2apollo_lidar)
         channel_name = "/apollo/sensor/{}/compensator/PointCloud2".format(c)
 
       if pb_msg:
         record.write(channel_name, pb_msg, t*1000)
 
       rotation = ego_pose['rotation']
       quat = Quaternion(rotation[0], rotation[1], rotation[2], rotation[3])
@@ -76,16 +76,21 @@
 
       ego_pose_t = ego_pose['timestamp']
       pb_msg = localization_builder.build(
         ego_pose['translation'], ego_pose['rotation'], heading, ego_pose_t/1e6)
       if pb_msg:
         record.write(LOCALIZATION_TOPIC, pb_msg, ego_pose_t*1000)
 
+      # Apollo coordinate system conversion
+      r_matrix = nuscenes2apollo_imu[:3,:3]
+      roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
+      nuscenes2apollo_q = Euler(roll, pitch, yaw).to_quaternion()
+      quat = quat * nuscenes2apollo_q
       pb_msg = transform_builder.build('world', 'localization',
-        ego_pose['translation'], ego_pose['rotation'], ego_pose_t/1e6)
+        ego_pose['translation'], [quat.w, quat.x, quat.y, quat.z], ego_pose_t/1e6)
       if pb_msg:
         record.write(TF_TOPIC, pb_msg, ego_pose_t*1000)
 
 def convert_dataset(dataset_path, record_path):
   """Generate apollo record file by nuscenes dataset
 
   Args:
```

### Comparing `adataset-0.1.0/adataset/nuscenes/geometry.py` & `adataset-0.1.1/adataset/nuscenes/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # limitations under the License.
 ###############################################################################
 
 import math
 import numpy as np
 
 
-def rotation_matrix(theta1, theta2, theta3, order='xyz'):
+def euler_to_rotation_matrix(theta1, theta2, theta3, order='xyz'):
   c1 = np.cos(theta1)
   s1 = np.sin(theta1)
   c2 = np.cos(theta2)
   s2 = np.sin(theta2)
   c3 = np.cos(theta3)
   s3 = np.sin(theta3)
 
@@ -74,14 +74,35 @@
                       [-s2, c2*s3, c2*c3]])
   elif order=='zxy':
     matrix = np.array([[c1*c3-s1*s2*s3, -c2*s1, c1*s3+c3*s1*s2],
                       [c3*s1+c1*s2*s3, c1*c2, s1*s3-c1*c3*s2],
                       [-c2*s3, s2, c2*c3]])
   return matrix
 
+def is_rotation_matrix(R) :
+  Rt = np.transpose(R)
+  should_be_identity = np.dot(Rt, R)
+  I = np.identity(3, dtype = R.dtype)
+  n = np.linalg.norm(I - should_be_identity)
+  return n < 1e-6
+
+def rotation_matrix_to_euler(R) :
+  assert(is_rotation_matrix(R))
+  sy = math.sqrt(R[0,0] * R[0,0] +  R[1,0] * R[1,0])
+  singular = sy < 1e-6
+  if not singular :
+    x = math.atan2(R[2,1] , R[2,2])
+    y = math.atan2(-R[2,0], sy)
+    z = math.atan2(R[1,0], R[0,0])
+  else :
+    x = math.atan2(-R[1,2], R[1,1])
+    y = math.atan2(-R[2,0], sy)
+    z = 0
+  return np.array([x, y, z])
+
 
 class Euler(object):
   def __init__(self, roll, pitch, yaw) -> None:
     self.roll = roll
     self.pitch = pitch
     self.yaw = yaw
 
@@ -121,7 +142,10 @@
 
   def __mul__(self, other):
     w = self.w * other.w - self.x * other.x - self.y * other.y - self.z * other.z
     x = self.w * other.x + self.x * other.w + self.y * other.z - self.z * other.y
     y = self.w * other.y - self.x * other.z + self.y * other.w + self.z * other.x
     z = self.w * other.z + self.x * other.y - self.y * other.x + self.z * other.w
     return Quaternion(w, x, y, z)
+
+  def __str__(self) -> str:
+    return "w: {}, x: {}, y: {}, z: {}".format(self.w, self.x, self.y, self.z)
```

### Comparing `adataset-0.1.0/adataset/nuscenes/nuscenes.py` & `adataset-0.1.1/adataset/nuscenes/nuscenes.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset/nuscenes/pcd_converter.py` & `adataset-0.1.1/adataset/nuscenes/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.0/adataset.egg-info/PKG-INFO` & `adataset-0.1.1/adataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.0/adataset.egg-info/SOURCES.txt` & `adataset-0.1.1/adataset.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 ./adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
 ./adataset/kitti/__init__.py
 ./adataset/kitti/calibration_converter.py
 ./adataset/kitti/common.py
 ./adataset/kitti/dataset_converter.py
 ./adataset/kitti/geometry.py
 ./adataset/kitti/kitti.py
+./adataset/kitti/params.py
 ./adataset/kitti/pcd_converter.py
 ./adataset/kitti/proj_helper.py
 ./adataset/kitti/sensor.py
 ./adataset/nuscenes/__init__.py
 ./adataset/nuscenes/calibration_converter.py
 ./adataset/nuscenes/dataset_converter.py
 ./adataset/nuscenes/geometry.py
 ./adataset/nuscenes/nuscenes.py
+./adataset/nuscenes/params.py
 ./adataset/nuscenes/pcd_converter.py
 adataset.egg-info/PKG-INFO
 adataset.egg-info/SOURCES.txt
 adataset.egg-info/dependency_links.txt
 adataset.egg-info/entry_points.txt
 adataset.egg-info/requires.txt
 adataset.egg-info/top_level.txt
```

### Comparing `adataset-0.1.0/setup.py` & `adataset-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adataset",
-    version="0.1.0",
+    version="0.1.1",
     author="apollo-team",
     author_email="apollo-support@baidu.com",
     description="Dataset conversion to Apollo record tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset",
     project_urls={
```

