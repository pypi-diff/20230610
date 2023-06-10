# Comparing `tmp/pypaz-0.1.9.tar.gz` & `tmp/pypaz-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaz-0.1.9.tar", last modified: Fri Aug  5 09:44:43 2022, max compression
+gzip compressed data, was "pypaz-0.2.4.tar", last modified: Sat Jun 10 13:40:05 2023, max compression
```

## Comparing `pypaz-0.1.9.tar` & `pypaz-0.2.4.tar`

### file list

```diff
@@ -1,120 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.249374 pypaz-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-08-05 09:44:32.000000 pypaz-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-05 09:44:43.249374 pypaz-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17703 2022-08-05 09:44:32.000000 pypaz-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.241374 pypaz-0.1.9/paz/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.241374 pypaz-0.1.9/paz/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/abstract/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/abstract/processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/abstract/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/applications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.241374 pypaz-0.1.9/paz/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/angles.py
--rw-r--r--   0 runner    (1001) docker     (121)    20265 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/boxes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/camera.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.241374 pypaz-0.1.9/paz/backend/groups/
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/groups/SE3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/groups/SO3.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/groups/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/heatmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/backend/image/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15694 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/image/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     8825 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/image/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/image/opencv_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/image/tensorflow_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    16787 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/munkres.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     7016 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/backend/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/CMU_poanoptic.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/fat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/fer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/ferplus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/open_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7232 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9726 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/evaluation/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/classification/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/classification/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/detection/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/detection/haar_cascade.py
--rw-r--r--   0 runner    (1001) docker     (121)     9842 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/detection/ssd300.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/detection/ssd512.py
--rw-r--r--   0 runner    (1001) docker     (121)     5617 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/detection/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/keypoint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7003 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/detnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/iknet.py
--rw-r--r--   0 runner    (1001) docker     (121)     5620 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/keypointnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/keypoint/projector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3942 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12512 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/pose_estimation/higher_hrnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11568 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/models/segmentation/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/optimization/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.245374 pypaz-0.1.9/paz/optimization/losses/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10769 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/keypointnet_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/multi_box_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.249374 pypaz-0.1.9/paz/optimization/losses/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/segmentation/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/segmentation/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/segmentation/jaccard_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/optimization/losses/segmentation/weighted_reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.249374 pypaz-0.1.9/paz/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/angles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)    19676 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    17039 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    21422 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/pose.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/pipelines/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.249374 pypaz-0.1.9/paz/processors/
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/angles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)    12498 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)    21600 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/geometric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    18296 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (121)    15481 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     7006 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     8212 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/munkres.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/pose.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14863 2022-08-05 09:44:32.000000 pypaz-0.1.9/paz/processors/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 09:44:43.249374 pypaz-0.1.9/pypaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-05 09:44:43.000000 pypaz-0.1.9/pypaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-08-05 09:44:43.000000 pypaz-0.1.9/pypaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 09:44:43.000000 pypaz-0.1.9/pypaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-05 09:44:43.000000 pypaz-0.1.9/pypaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-05 09:44:43.000000 pypaz-0.1.9/pypaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 09:44:43.249374 pypaz-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-05 09:44:32.000000 pypaz-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-10 13:39:55.000000 pypaz-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-10 13:40:05.403826 pypaz-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-10 13:39:55.000000 pypaz-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/applications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/backend/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/SE3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/SO3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/heatmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/backend/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/opencv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/tensorflow_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23479 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/munkres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/CMU_poanoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/fer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/ferplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/human36m.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/omniglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/open_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/evaluation/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/protonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/detection/efficientdet/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/haar_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/ssd300.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/ssd512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/detnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/iknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/keypointnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/simplebaselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/pose_estimation/higher_hrnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/segmentation/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/keypointnet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/multi_box_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/losses/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/jaccard_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/weighted_reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34146 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21416 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18276 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/munkres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/pypaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:40:05.403826 pypaz-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-10 13:39:55.000000 pypaz-0.2.4/setup.py
```

### Comparing `pypaz-0.1.9/LICENSE` & `pypaz-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/README.md` & `pypaz-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 # (PAZ) Perception for Autonomous Systems
 [![Unit testing](https://github.com/oarriaga/paz/actions/workflows/python-package.yml/badge.svg)](https://github.com/oarriaga/paz/actions/workflows/python-package.yml)
 [![PyPI upload](https://github.com/oarriaga/paz/actions/workflows/python-publish.yml/badge.svg)](https://github.com/oarriaga/paz/actions/workflows/python-publish.yml)
 [![Publish Website](https://github.com/oarriaga/paz/actions/workflows/publish-website.yml/badge.svg)](https://github.com/oarriaga/paz/actions/workflows/publish-website.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/pypaz?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/pypaz)
 
 Hierarchical perception library in Python.
 
 ## Selected examples:
 PAZ is used in the following examples (links to **real-time demos** and training scripts):
 
 | [Probabilistic 2D keypoints](https://github.com/oarriaga/paz/tree/master/examples/probabilistic_keypoint_estimation)| [6D head-pose estimation](https://github.com/oarriaga/paz/tree/master/examples/pose_estimation)  | [Object detection](https://github.com/oarriaga/paz/tree/master/examples/object_detection)|
 |---------------------------|--------------------------| ------------------|
 |<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/probabilistic_keypoints.png" width="425"> | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/head_pose.png" width="440">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/object_detection.png" width="430">|
 
 | [Emotion classifier](https://github.com/oarriaga/paz/tree/master/examples/face_classification) | [2D keypoint estimation](https://github.com/oarriaga/paz/tree/master/examples/keypoint_estimation)   | [Mask-RCNN (in-progress)](https://github.com/oarriaga/paz/tree/mask_rcnn/examples/mask_rcnn)  |
 |---------------------------|--------------------------| -----------------------|
 |<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/emotion.gif" width="250">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/keypoints.png" width="410">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/mask.png" width="400">|
 
-|[Semantic segmentation](https://github.com/oarriaga/paz/tree/master/examples/semantic_segmentation) | [Hand pose estimation](https://github.com/oarriaga/paz/tree/master/examples/minimal_hand) |  [Human pose estimation](https://github.com/oarriaga/paz/tree/master/examples/human_pose_estimation_2D) |
+|[Semantic segmentation](https://github.com/oarriaga/paz/tree/master/examples/semantic_segmentation) | [Hand pose estimation](https://github.com/oarriaga/paz/tree/master/examples/hand_pose_estimation) |  [2D Human pose estimation](https://github.com/oarriaga/paz/tree/master/examples/human_pose_estimation_2D) |
 |---------------------------|-----------------------|-----------------|
 | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/semantic_segmentation.png" width="325">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/minimal_hand_example.jpg" width="330"> |<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/human_pose.gif" width="250"> | 
 
-| [3D keypoint discovery](https://github.com/oarriaga/paz/tree/master/examples/discovery_of_latent_keypoints)     | [Hand closure detection](https://github.com/oarriaga/paz/tree/master/examples/minimal_hand)  | [6D pose estimation](https://github.com/oarriaga/paz/tree/master/examples/pix2pose) |
+| [3D keypoint discovery](https://github.com/oarriaga/paz/tree/master/examples/discovery_of_latent_keypoints)     | [Hand closure detection](https://github.com/oarriaga/paz/tree/master/examples/hand_pose_estimation)  | [6D pose estimation](https://github.com/oarriaga/paz/tree/master/examples/pix2pose) |
 |---------------------------|-----------------------| --------------------------|
 |<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/discovery_keypoints.png" width="335"> | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/hand_closure_detection.gif" width="250">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/pix2pose_example.jpg" width="330"> |
 
 | [Implicit orientation](https://github.com/oarriaga/paz/tree/master/examples/implicit_orientation_learning)  | [Attention (STNs)](https://github.com/oarriaga/paz/tree/master/examples/spatial_transfomer_networks) | [Haar Cascade detector](https://github.com/oarriaga/paz/tree/master/examples/haar_cascade_detectors) |
 |---------------------------|-----------------------|-----------------|
 |<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/implicit_pose.png" width="335">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/attention.png" width="340"> | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/haar_cascades.png" width="330"> |
 
-| [Eigenfaces](https://github.com/oarriaga/paz/blob/master/examples/eigenfaces) | | |
+| [Eigenfaces](https://github.com/oarriaga/paz/blob/master/examples/eigenfaces) |[Prototypical Networks](https://github.com/oarriaga/paz/tree/master/examples/prototypical_networks) | [3D Human pose estimation](https://github.com/oarriaga/paz/blob/master/examples/human_pose_estimation_3D) |
 |---------------------------|-----------------------|-----------------|
-|<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/eigenfaces.png" width="325">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/your_example_here.png" width="330">  | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/blank.png" width="330">
+|<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/eigenfaces.png" width="325">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/protonets.png" width="330">  | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/human_pose3D.gif" width="250"> |
+
+
+| | | |
+|---------------------------|-----------------------|-----------------|
+|<img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/your_example_here.png" width="330">| <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/blank.png" width="330"> | <img src="https://raw.githubusercontent.com/oarriaga/altamira-data/master/images/blank.png" width="330"> |
 
 
 All models can be re-trained with your own data (except for Mask-RCNN, we are working on it [here](https://github.com/oarriaga/paz/tree/mask_rcnn)).
 
 ## Table of Contents
 <!--ts-->
 * [Examples](#selected-examples)
@@ -185,28 +191,32 @@
 ### Models
 
 The following models are implemented in PAZ and they can be trained with your own data:
 
 | Task (link to implementation)    |Model (link to paper)  |
 |---------------------------:|-----------------------| 
 |[Object detection](https://github.com/oarriaga/paz/blob/master/paz/models/detection/ssd300.py)|[SSD-300](https://arxiv.org/abs/1512.02325)|
-|[Object detection](https://github.com/oarriaga/paz/blob/master/paz/models/detection/ssd512.py)|[SSD-512](https://arxiv.org/abs/1512.02325)|                
+|[Object detection](https://github.com/oarriaga/paz/blob/master/paz/models/detection/ssd512.py)|[SSD-512](https://arxiv.org/abs/1512.02325)|
 |[Probabilistic keypoint est.](https://github.com/oarriaga/paz/blob/master/examples/probabilistic_keypoint_estimation/model.py) |[Gaussian Mixture CNN](https://www.robots.ox.ac.uk/~vgg/publications/2018/Neumann18a/)   |
 |[Detection and Segmentation](https://github.com/oarriaga/paz/tree/mask_rcnn/examples/mask_rcnn)  |[MaskRCNN (in progress)](https://arxiv.org/abs/1703.06870) |
 |[Keypoint estimation](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/hrnet.py)|[HRNet](https://arxiv.org/abs/1908.07919)|
-|[Semantic segmentation](https://github.com/oarriaga/paz/blob/master/paz/models/segmentation/unet.py)|[U-NET](https://arxiv.org/abs/1505.04597)|      
+|[Semantic segmentation](https://github.com/oarriaga/paz/blob/master/paz/models/segmentation/unet.py)|[U-NET](https://arxiv.org/abs/1505.04597)|
 |[6D Pose estimation](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/keypointnet.py)          |[Pix2Pose](https://arxiv.org/abs/1908.07433)          |
 |[Implicit orientation](https://github.com/oarriaga/paz/blob/master/examples/implicit_orientation_learning/model.py)        |[AutoEncoder](https://arxiv.org/abs/1902.01275)            |
 |[Emotion classification](https://github.com/oarriaga/paz/blob/master/paz/models/classification/xception.py)       |[MiniXception](https://arxiv.org/abs/1710.07557)           |
 |[Discovery of Keypoints](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/keypointnet.py)      |[KeypointNet](https://arxiv.org/abs/1807.03146)            |
 |[Keypoint estimation](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/keypointnet.py)  |[KeypointNet2D](https://arxiv.org/abs/1807.03146)|
 |[Attention](https://github.com/oarriaga/paz/blob/master/examples/spatial_transfomer_networks/STN.py)                   |[Spatial Transformers](https://arxiv.org/abs/1506.02025)   |
 |[Object detection](https://github.com/oarriaga/paz/blob/master/paz/models/detection/haar_cascade.py)            |[HaarCascades](https://link.springer.com/article/10.1023/B:VISI.0000013087.49260.fb)  |
-|[Human pose estimation](https://github.com/oarriaga/paz/blob/master/paz/models/pose_estimation/higher_hrnet.py)            |[HigherHRNet](https://arxiv.org/abs/1908.10357)  |
-|[Hand pose estimation](https://github.com/oarriaga/paz/blob/refactor_readme/paz/models/keypoint/detnet.py)            |[DetNet](https://vcai.mpi-inf.mpg.de/projects/2020-cvpr-hands/)  |
+|[2D Human pose estimation](https://github.com/oarriaga/paz/blob/master/paz/models/pose_estimation/higher_hrnet.py)            |[HigherHRNet](https://arxiv.org/abs/1908.10357)  |
+|[3D Human pose estimation](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/simplebaselines.py) | [Simple Baseline](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/simplebaselines.py) |
+|[Hand pose estimation](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/detnet.py)            |[DetNet](https://vcai.mpi-inf.mpg.de/projects/2020-cvpr-hands/)  |
+|[Hand closure classification](https://github.com/oarriaga/paz/blob/master/paz/models/keypoint/iknet.py)            |[IKNet](https://vcai.mpi-inf.mpg.de/projects/2020-cvpr-hands/)  |
+|[Hand detection](https://github.com/oarriaga/paz/blob/master/paz/models/detection/ssd512.py)            |[SSD512](https://arxiv.org/abs/1512.02325)|
+|[Few-shot classification](https://github.com/oarriaga/paz/blob/master/paz/models/classification/protonet.py)| [Prototypical Networks](https://arxiv.org/abs/1703.05175)|
 
 
 ## Motivation
 Even though there are multiple high-level computer vision libraries in different deep learning frameworks, I felt there was not a consolidated deep learning library for robot-perception in my framework of choice (Keras).
 
 As a final remark, I would like to mention, that I feel that we might tend to forget the great effort and emotional status behind every (open-source) project.
 I feel it's easy to blurry a company name with the individuals behind their work, and we forget that there is someone feeling our criticism and our praise.
```

### Comparing `pypaz-0.1.9/paz/abstract/loader.py` & `pypaz-0.2.4/paz/abstract/loader.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/abstract/messages.py` & `pypaz-0.2.4/paz/abstract/messages.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/abstract/processor.py` & `pypaz-0.2.4/paz/abstract/processor.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/abstract/sequence.py` & `pypaz-0.2.4/paz/abstract/sequence.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/applications.py` & `pypaz-0.2.4/paz/applications.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,28 @@
 from .pipelines import SSD512YCBVideo
 from .pipelines import SSD300FAT
 from .pipelines import DetectMiniXceptionFER
 from .pipelines import MiniXceptionFER
 from .pipelines import FaceKeypointNet2D32
 from .pipelines import HeadPoseKeypointNet2D32
 from .pipelines import HaarCascadeFrontalFace
+from .pipelines import EFFICIENTDETD0COCO
+from .pipelines import EFFICIENTDETD1COCO
+from .pipelines import EFFICIENTDETD2COCO
+from .pipelines import EFFICIENTDETD3COCO
+from .pipelines import EFFICIENTDETD4COCO
+from .pipelines import EFFICIENTDETD5COCO
+from .pipelines import EFFICIENTDETD6COCO
+from .pipelines import EFFICIENTDETD7COCO
+from .pipelines import EFFICIENTDETD0VOC
 
 from .pipelines import SinglePowerDrillPIX2POSE6D
 from .pipelines import MultiPowerDrillPIX2POSE6D
 from .pipelines import PIX2POSEPowerDrill
 from .pipelines import PIX2YCBTools6D
 
 from .pipelines import HigherHRNetHumanPose2D
 from .pipelines import DetNetHandKeypoints
 from .pipelines import MinimalHandPoseEstimation
 from .pipelines import DetectMinimalHand
+from .pipelines import ClassifyHandClosure
+from .pipelines import SSD512MinimalHandPose
```

### Comparing `pypaz-0.1.9/paz/backend/angles.py` & `pypaz-0.2.4/paz/backend/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/boxes.py` & `pypaz-0.2.4/paz/backend/boxes.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     x_max = center_x + (W / 2.0)
     y_min = center_y - (H / 2.0)
     y_max = center_y + (H / 2.0)
     return np.concatenate([x_min, y_min, x_max, y_max], axis=1)
 
 
 def encode(matched, priors, variances=[0.1, 0.1, 0.2, 0.2]):
-    """Encode the variances from the priorbox layers into the ground truth boxes
-    we have matched (based on jaccard overlap) with the prior boxes.
+    """Encode the variances from the priorbox layers into the ground truth
+    boxes we have matched (based on jaccard overlap) with the prior boxes.
 
     # Arguments
         matched: Numpy array of shape `(num_priors, 4)` with boxes in
             point-form.
         priors: Numpy array of shape `(num_priors, 4)` with boxes in
             center-form.
         variances: (list[float]) Variances of priorboxes
@@ -312,45 +312,188 @@
         intersec_over_union_mask = intersec_over_union <= iou_thresh
         remaining_sorted_box_indices = remaining_sorted_box_indices[
             intersec_over_union_mask]
 
     return selected_indices.astype(int), num_selected_boxes
 
 
-def nms_per_class(box_data, nms_thresh=.45, conf_thresh=0.01, top_k=200):
-    """Applies non-maximum-suppression per class.
-    # Arguments
-        box_data: Numpy array of shape `(num_prior_boxes, 4 + num_classes)`.
-        nsm_thresh: Float. Non-maximum suppression threshold.
-        conf_thresh: Float. Filter scores with a lower confidence value before
-            performing non-maximum supression.
-        top_k: Integer. Maximum number of boxes per class outputted by nms.
-
-    Returns
-        Numpy array of shape `(num_classes, top_k, 5)`.
+def nms_per_class(box_data, nms_thresh=.45, epsilon=0.01, top_k=200):
+    """Applies non maximum suppression per class.
+    This function takes all the detections from the detector which
+    consists of boxes and their corresponding class scores to which it
+    applies non maximum suppression for every class independently and
+    then combines the result.
+
+    # Arguments
+        box_data: Array of shape `(num_nms_boxes, 4 + num_classes)`
+            containing the box coordinates as well as the predicted
+            scores of all the classes for all non suppressed boxes.
+        nms_thresh: Float, Non-maximum suppression threshold.
+        epsilon: Float, Filter scores with a lower confidence
+            value before performing non-maximum supression.
+        top_k: Int, Maximum number of boxes per class outputted by nms.
+
+    # Returns
+        Tuple: Containing an array non suppressed boxes of shape
+            `(num_nms_boxes, 4 + num_classes)` and an array
+            of corresponding class labels of shape `(num_nms_boxes, )`.
     """
-    decoded_boxes, class_predictions = box_data[:, :4], box_data[:, 4:]
+    decoded_boxes = box_data[:, :4]
+    class_predictions = box_data[:, 4:]
     num_classes = class_predictions.shape[1]
-    output = np.zeros((num_classes, top_k, 5))
-
-    # skip the background class (start counter in 1)
-    for class_arg in range(1, num_classes):
-        conf_mask = class_predictions[:, class_arg] >= conf_thresh
-        scores = class_predictions[:, class_arg][conf_mask]
-        if len(scores) == 0:
-            continue
-        boxes = decoded_boxes[conf_mask]
-        indices, count = apply_non_max_suppression(
-            boxes, scores, nms_thresh, top_k)
-        scores = np.expand_dims(scores, -1)
+    nms_boxes = np.array([], dtype=float).reshape(0, box_data.shape[1])
+    class_labels = np.array([], dtype=np.int)
+    args = (decoded_boxes, class_predictions, epsilon, nms_thresh, top_k)
+    for class_arg in range(num_classes):
+        nms_boxes, class_labels = _nms_per_class(
+            nms_boxes, class_labels, class_arg, *args)
+    return nms_boxes, class_labels
+
+
+def _nms_per_class(nms_boxes, class_labels, class_arg, decoded_boxes,
+                   class_predictions, epsilon, nms_thresh, top_k):
+    """Applies non maximum suppression for a given class.
+    This function takes all the detections that belong only to the given
+    single class and applies non maximum suppression for that class
+    alone and returns the resulting non suppressed boxes.
+
+    # Arguments
+        nms_boxes: Array of shape `(num_boxes, 4 + num_classes)`.
+        class_labels: Array of shape `(num_boxes, )`.
+        class_arg: Int, class index.
+        decoded_boxes: Array of shape `(num_prior_boxes, 4)`
+            containing the box coordinates of all the
+            non suppressed boxes.
+        class_predictions: Array of shape
+            `(num_nms_boxes, num_classes)` containing the predicted
+            scores of all the classes for all the non suppressed boxes.
+        epsilon: Float, Filter scores with a lower confidence
+            value before performing non-maximum supression.
+        nms_thresh: Float, Non-maximum suppression threshold.
+        top_k: Int, Maximum number of boxes per class outputted by nms.
+
+    # Returns
+        Tuple: Containing an array non suppressed boxes per class of
+            shape `(num_nms_boxes_per_class, 4 + num_classes) and an
+            array corresponding class labels of shape
+            `(num_nms_boxes_per_class, )`.
+    """
+    scores, mask = pre_filter_nms(class_arg, class_predictions, epsilon)
+
+    if len(scores) != 0:
+        boxes = decoded_boxes[mask]
+        selected = apply_non_max_suppression(boxes, scores, nms_thresh, top_k)
+        indices, count = selected
         selected_indices = indices[:count]
-        selections = np.concatenate(
-            (boxes[selected_indices], scores[selected_indices]), axis=1)
-        output[class_arg, :count, :] = selections
-    return output
+        selected_boxes = boxes[selected_indices]
+        selected_classes = class_predictions[mask][selected_indices]
+        selections = np.concatenate((selected_boxes, selected_classes), axis=1)
+        nms_boxes = np.concatenate((nms_boxes, selections), axis=0)
+        class_label = np.repeat(class_arg, count)
+        class_labels = np.append(class_labels, class_label)
+    return nms_boxes, class_labels
+
+
+def pre_filter_nms(class_arg, class_predictions, epsilon):
+    """Applies score filtering.
+    This function takes all the predicted scores of a given class and
+    filters out all the predictions less than the given `epsilon` value.
+
+    # Arguments
+        class_arg: Int, class index.
+        class_predictions: Array of shape
+            `(num_nms_boxes, num_classes)` containing the predicted
+            scores of all the classes for all the non suppressed boxes.
+        epsilon: Float, threshold value for score filtering.
+
+    # Returns
+        Tuple: Containing an array filtered scores of shape
+            `(num_pre_filtered_boxes, )` and an array filter mask of
+            shape `(num_prior_boxes, )`.
+    """
+    mask = class_predictions[:, class_arg] >= epsilon
+    scores = class_predictions[:, class_arg][mask]
+    return scores, mask
+
+
+def merge_nms_box_with_class(box_data, class_labels):
+    """Merges box coordinates with their corresponding class
+    defined by `class_labels` which is decided by best box geometry
+    by non maximum suppression (and not by the best scoring class)
+    into a single output.
+    This function retains only the predicted score of the class to
+    which the box belongs to and sets the scores of all the remaining
+    classes to zero, thereby combining box and class information in a
+    single variable.
+
+    # Arguments
+        box_data: Array of shape `(num_nms_boxes, 4 + num_classes)`
+            containing the box coordinates as well as the predicted
+            scores of all the classes for all non suppressed boxes.
+        class_labels: Array of shape `(num_nms_boxes, )` that contains
+            the indices of the class whose score is to be retained.
+
+    # Returns
+        boxes: Array of shape `(num_nms_boxes, 4 + num_classes)`,
+            containing coordinates of non supressed boxes along with
+            scores of the class to which the box belongs. The scores of
+            the other classes are zeros.
+    """
+    decoded_boxes = box_data[:, :4]
+    class_predictions = box_data[:, 4:]
+    retained_class_score = suppress_other_class_scores(
+        class_predictions, class_labels)
+    box_data = np.concatenate((decoded_boxes, retained_class_score), axis=1)
+    return box_data
+
+
+def suppress_other_class_scores(class_predictions, class_labels):
+    """Retains the score of class in `class_labels` and
+    sets other class scores to zero.
+
+    # Arguments
+        class_predictions: Array of shape
+            `(num_nms_boxes, num_classes)` containing the predicted
+            scores of all the classes for all the non suppressed boxes.
+        class_labels: Array of shape `(num_nms_boxes, )` that contains
+            the indices of the class whose score is to be retained.
+
+    # Returns
+        retained_class_score: Array of shape
+            `(num_nms_boxes, num_classes)` that consists of score at
+            only those location specified by 'class_labels' and zero
+            at other class locations.
+
+    # Note
+        This approach retains the scores of that class in
+        `class_predictions` defined by `class_labels` by generating
+        a boolean mask `score_suppress_mask` with elements True at the
+        locations where the score in `class_predictions` is to be
+        retained and False wherever the class score is to be suppressed.
+        This approach of retaining/suppressing scores does not make use
+        of for loop, if-else condition and direct value assignment
+        to arrays.
+    """
+    num_nms_boxes, num_classes = class_predictions.shape
+    class_indices = np.arange(num_classes)
+    class_indices = np.expand_dims(class_indices, axis=0)
+    class_indices = np.repeat(class_indices, num_nms_boxes, axis=0)
+    class_labels = np.expand_dims(class_labels, axis=1)
+    class_labels = np.repeat(class_labels, num_classes, axis=1)
+    """
+    The difference of class_indices and class_labels contains zero
+    at those locations of the result where the score is to be retained
+    whose boolean value is False while others being True. This
+    difference obtained as a boolean array gives a negative mask which
+    when inverted gives the score_suppress_mask.
+    """
+    negative_mask = np.array(class_indices - class_labels, dtype=bool)
+    score_suppress_mask = np.logical_not(negative_mask)
+    retained_class_score = np.multiply(class_predictions, score_suppress_mask)
+    return retained_class_score
 
 
 def to_one_hot(class_indices, num_classes):
     """ Transform from class index to one-hot encoded vector.
 
     # Arguments
         class_indices: Numpy array. One dimensional array specifying
@@ -363,15 +506,16 @@
     one_hot_vectors = np.zeros((len(class_indices), num_classes))
     for vector_arg, class_args in enumerate(class_indices):
         one_hot_vectors[vector_arg, class_args] = 1.0
     return one_hot_vectors
 
 
 def make_box_square(box):
-    """Makes box coordinates square with sides equal to the longest original side.
+    """Makes box coordinates square with sides equal to the longest
+        original side.
 
     # Arguments
         box: Numpy array with shape `(4)` with point corner coordinates.
 
     # Returns
         returns: List of box coordinates ints.
     """
@@ -438,15 +582,15 @@
         x_max = width
     if y_max > height:
         y_max = height
     return x_min, y_min, x_max, y_max
 
 
 def denormalize_box(box, image_shape):
-    """Scales corner box coordinates from normalized values to image dimensions.
+    """Scales corner box coordinates from normalized values to image dimensions
 
     # Arguments
         box: Numpy array containing corner box coordinates.
         image_shape: List of integers with (height, width).
 
     # Returns
         returns: box corner coordinates in image dimensions
@@ -515,7 +659,66 @@
     # Returns
         Left-down-bottom corner (x_min, y_min, z_min) and right-up-top
             (x_max, y_max, z_max) corner.
     """
     XYZ_min = np.min(points3D, axis=0)
     XYZ_max = np.max(points3D, axis=0)
     return XYZ_min, XYZ_max
+
+
+def filter_boxes(boxes, conf_thresh):
+    """Filters given boxes based on scores.
+
+    # Arguments
+        boxes: Array of shape `(num_nms_boxes, 4 + num_classes)`.
+        conf_thresh: Float, Filter boxes with a confidence value
+            lower than this.
+
+    # Returns
+        confident_boxes: Array of shape
+            `(num_filtered_boxes, 4 + num_classes)`.
+    """
+    class_predictions = boxes[:, 4:]
+    class_scores = np.max(class_predictions, axis=1)
+    confidence_mask = class_scores >= conf_thresh
+    confident_boxes = boxes[confidence_mask]
+    return confident_boxes
+
+
+def scale_box(predictions, image_scales):
+    """
+    # Arguments
+        predictions: Array of shape `(num_boxes, num_classes+N)`
+            model predictions.
+        image_scales: Array of shape `()`, scale value of boxes.
+
+    # Returns
+        predictions: Array of shape `(num_boxes, num_classes+N)`
+            model predictions.
+    """
+    boxes = predictions[:, :4]
+    scales = image_scales[np.newaxis][np.newaxis]
+    boxes = boxes * scales
+    predictions = np.concatenate([boxes, predictions[:, 4:]], 1)
+    return predictions
+
+
+def change_box_coordinates(outputs):
+    """Converts box coordinates format from (y_min, x_min, y_max, x_max)
+    to (x_min, y_min, x_max, y_max).
+
+    # Arguments
+        outputs: Tensor, model output.
+
+    # Returns
+        outputs: Array, Processed outputs by merging the features
+            at all levels. Each row corresponds to box coordinate
+            offsets and sigmoid of the class logits.
+    """
+    outputs = outputs[0]
+    boxes, classes = outputs[:, :4], outputs[:, 4:]
+    s1, s2, s3, s4 = np.hsplit(boxes, 4)
+    boxes = np.concatenate([s2, s1, s4, s3], axis=1)
+    boxes = boxes[np.newaxis]
+    classes = classes[np.newaxis]
+    outputs = np.concatenate([boxes, classes], axis=2)
+    return outputs
```

### Comparing `pypaz-0.1.9/paz/backend/camera.py` & `pypaz-0.2.4/paz/backend/camera.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,24 @@
 
         focal_length = (width / 2) * (1 / np.tan(np.deg2rad(HFOV / 2.0)))
         intrinsics = np.array([[focal_length, 0, width / 2.0],
                                [0, focal_length, height / 2.0],
                                [0, 0, 1.0]])
         self.intrinsics = intrinsics
 
+    def take_photo(self):
+        """Starts camera, reads buffer and returns an image.
+        """
+        self.start()
+        image = self.read()
+        # all pipelines start with RGB
+        image = convert_color_space(image, BGR2RGB)
+        self.stop()
+        return image
+
 
 class VideoPlayer(object):
     """Performs visualization inferences in a real-time video.
 
     # Properties
         image_size: List of two integers. Output size of the displayed image.
         pipeline: Function. Should take RGB image as input and it should
@@ -227,15 +237,15 @@
         fourCC = cv2.VideoWriter_fourcc(*fourCC)
         writer = cv2.VideoWriter(name, fourCC, fps, self.image_size)
 
         video = cv2.VideoCapture(video_file_path)
         if (video.isOpened() is False):
             print("Error opening video  file")
 
-        while(video.isOpened()):
+        while video.isOpened():
             is_frame_received, frame = video.read()
             if not is_frame_received:
                 print("Frame not received. Exiting ...")
                 break
             if is_frame_received is True:
                 output = self.pipeline(frame)
                 if output is None:
```

### Comparing `pypaz-0.1.9/paz/backend/groups/SE3.py` & `pypaz-0.2.4/paz/backend/groups/SE3.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/groups/SO3.py` & `pypaz-0.2.4/paz/backend/groups/SO3.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/groups/quaternion.py` & `pypaz-0.2.4/paz/backend/groups/quaternion.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/heatmaps.py` & `pypaz-0.2.4/paz/backend/heatmaps.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/image/draw.py` & `pypaz-0.2.4/paz/backend/image/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,37 +285,40 @@
 
 def make_mosaic(images, shape, border=0):
     """ Creates an image mosaic.
 
     # Arguments
         images: Numpy array of shape (num_images, height, width, num_channels)
         shape: List of two integers indicating the mosaic shape.
-            Shape must satisfy: shape[0] * shape[1] == len(images).
         border: Integer indicating the border per image.
 
     # Returns
         A numpy array containing all images.
+
+    # Exceptions
+        Shape must satisfy `len(images) > shape[0] * shape[1]`
     """
-    num_images = len(images)
+    num_images, H, W, num_channels = images.shape
     num_rows, num_cols = shape
-    H, W, num_channels = images.shape[1:]
-    mosaic = np.ma.masked_all(
-        (num_rows * H + (num_rows - 1) * border,
-         num_cols * W + (num_cols - 1) * border, num_channels),
-        dtype=np.float32)
+    if num_images > (num_rows * num_cols):
+        raise ValueError('Number of images is bigger than shape')
+
+    total_rows = (num_rows * H) + ((num_rows - 1) * border)
+    total_cols = (num_cols * W) + ((num_cols - 1) * border)
+    mosaic = np.ones((total_rows, total_cols, num_channels))
+
     padded_H = H + border
     padded_W = W + border
-    for image_arg in range(num_images):
+
+    for image_arg, image in enumerate(images):
         row = int(np.floor(image_arg / num_cols))
         col = image_arg % num_cols
-        image = images[image_arg]
-        image_shape = image.shape
-        mosaic[row * padded_H:row * padded_H + image_shape[0],
-               col * padded_W:col * padded_W + image_shape[1], :] = image
-    return mosaic.astype('uint8')
+        mosaic[row * padded_H:row * padded_H + H,
+               col * padded_W:col * padded_W + W, :] = image
+    return mosaic
 
 
 def draw_points2D(image, points2D, colors):
     """Draws a pixel for all points2D in UV space using only numpy.
 
     # Arguments
         image: Array (H, W).
```

### Comparing `pypaz-0.1.9/paz/backend/image/image.py` & `pypaz-0.2.4/paz/backend/image/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 
 from .opencv_image import (convert_color_space, gaussian_image_blur,
-                           median_image_blur, warp_affine, RGB2HSV, HSV2RGB)
+                           median_image_blur, warp_affine, resize_image,
+                           RGB2HSV, HSV2RGB)
 
 
 def cast_image(image, dtype):
     """Casts an image into a different type
 
     # Arguments
         image: Numpy array.
@@ -318,7 +319,35 @@
     # Returns
         scaling factor: Numpy array of size 2
     '''
     H, W = image.shape[:2]
     H_scale = H / shape[0]
     W_scale = W / shape[1]
     return np.array([W_scale * scale, H_scale * scale])
+
+
+def scale_resize(image, image_size):
+    """Resizes and crops image by returning the scales to original
+    image.
+
+    Args:
+        image: Numpy array, raw image.
+        image_size: Int, size of the image.
+
+    Returns:
+        Tuple: output_image, image_scale.
+    """
+    H, W = image.shape[0], image.shape[1]
+    image_scale_x = image_size / W
+    image_scale_y = image_size / H
+    image_scale = min(image_scale_x, image_scale_y)
+    scaled_H = int(H * image_scale)
+    scaled_W = int(W * image_scale)
+    scaled_image = resize_image(image, (scaled_W, scaled_H))
+    scaled_image = scaled_image[:image_size, :image_size, :]
+    output_image = np.zeros((image_size, image_size, image.shape[2]))
+    output_image[:scaled_image.shape[0],
+                 :scaled_image.shape[1],
+                 :scaled_image.shape[2]] = scaled_image
+    image_scale = np.array(1 / image_scale)
+    output_image = output_image[np.newaxis]
+    return output_image, image_scale
```

### Comparing `pypaz-0.1.9/paz/backend/image/opencv_image.py` & `pypaz-0.2.4/paz/backend/image/opencv_image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/image/tensorflow_image.py` & `pypaz-0.2.4/paz/backend/image/tensorflow_image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/keypoints.py` & `pypaz-0.2.4/paz/backend/keypoints.py`

 * *Files 27% similar despite different names*

```diff
@@ -101,28 +101,14 @@
     image_shape = np.array([width, height])
     points2D = points2D + 1.0          # [-1, 1], [-1, 1] -> [2, 0], [0, 2]
     points2D = points2D / 2.0          # [2 , 0], [0 , 2] -> [1, 0], [0, 1]
     points2D = points2D * image_shape  # [1 , 0], [0 , 1] -> [W, 0], [0, H]
     return points2D
 
 
-"""
-def denormalize_keypoints(keypoints, height, width):
-    for keypoint_arg, keypoint in enumerate(keypoints):
-        x, y = keypoint[:2]
-        # transform key-point coordinates to image coordinates
-        x = (min(max(x, -1), 1) * width / 2 + width / 2) - 0.5
-        # flip since the image coordinates for y are flipped
-        y = height - 0.5 - (min(max(y, -1), 1) * height / 2 + height / 2)
-        x, y = int(round(x)), int(round(y))
-        keypoints[keypoint_arg][:2] = [x, y]
-    return keypoints
-"""
-
-
 def cascade_classifier(path):
     """OpenCV Cascade classifier.
 
     # Arguments
         path: String. Path to default openCV XML format.
 
     # Returns
@@ -498,7 +484,224 @@
 def uv_to_vu(keypoints):
     """Flips the uv coordinates to vu.
 
     # Arguments
         keypoints: Array.
     """
     return keypoints[:, ::-1]
+
+
+def standardize(data, mean, scale):
+    """it takes the data the mean and the standard deviation
+       and returns the standardized data
+
+    # Arguments
+        data: nxd matrix to normalize
+        mean: Array of means
+        scale: standard deviation
+
+    # Returns
+        standardized poses2D
+    # """
+    return np.divide((data - mean), scale)
+
+
+def destandardize(data, mean, scale):
+    """it takes the standardized data the mean and the standard
+       deviation and returns the destandardized data
+
+    # Arguments
+        data: nxd matrix to unnormalize
+        mean: Array of means
+        scale: standard deviation
+
+    # Returns
+        destandardized poses3D
+    """
+    return (data * scale) + mean
+
+
+def initialize_translation(joints2D, camera_intrinsics, ratio):
+    """Computes initial 3D translation of root joint
+
+    # Arguments
+        joints2D: 2D root joint from HigherHRNet
+        camera_intrinsics: camera intrinsic parameters
+        ratio: ration of sum of 3D bones to 2D bones
+
+    # Returns
+        Array of initial estimate of the global position
+        of the root joint in 3D
+    """
+    focal_length = camera_intrinsics[0, 0]
+    image_center_x = camera_intrinsics[0, 2]
+    image_center_y = camera_intrinsics[1, 2]
+    z = focal_length * ratio
+    x = (joints2D[:, 0] - image_center_x) * ratio
+    y = (joints2D[:, 1] - image_center_y) * ratio
+    translation = np.array((x, y, z))
+    return translation.flatten()
+
+
+def solve_least_squares(solver, compute_joints_distance,
+                        initial_joints_translation, joints3D,
+                        poses2D, camera_intrinsics):
+    """ Solve the least squares
+
+    # Arguments
+        solver: from scipy.optimize import least_squares
+        compute_joints_distance: global_pose.compute_joints_distance
+        initial_root_translation: initial 3D translation of root joint
+        joints3D: 16 moving joints in 3D
+        poses2d: 2D poses
+        camera_intrinsics: camera intrinsic parameters
+
+    Returns
+        optimal translation of root joint for each person
+    """
+    joints_translation = solver(
+        compute_joints_distance, initial_joints_translation, verbose=0,
+        args=(joints3D, poses2D, camera_intrinsics))
+    joints_translation = np.reshape(joints_translation.x, (-1, 3))
+    return joints_translation
+
+
+def get_bones_length(poses2D, poses3D):
+    """Computes sum of bone lengths in 3D
+
+    #Arguments
+        poses3D: array of predicted poses in 3D (Nx16x3)
+        poses2D: array of poses in 2D    (Nx32)
+
+    #Returns
+        sum_bones2D: sum of length of all bones in the 3D skeleton
+        sum_bones3D: sum of length of all bones in the 3D skeleton
+    """
+    sum_bones2D = 0
+    sum_bones3D = np.zeros(poses3D.shape[0])
+    start_joints = np.arange(0, 15)
+    end_joints = np.arange(1, 16)
+    for person in poses2D:
+        bone_length = np.linalg.norm(person[start_joints] -
+                                     person[end_joints])
+        sum_bones2D = sum_bones2D + bone_length
+    for person in poses3D:
+        bone_length = np.linalg.norm(person[start_joints] -
+                                     person[end_joints])
+        sum_bones3D = sum_bones3D + bone_length
+    return sum_bones2D, sum_bones3D
+
+
+def compute_reprojection_error(initial_translation, keypoints3D,
+                               keypoints2D, camera_intrinsics):
+    """compute distance between each person joints
+
+    # Arguments
+        initial_translation: initial guess of position of joint
+        keypoints3D: 3D keypoints to be optimized (Nx16x3)
+        keypoints2D: 2D keypoints (Nx32)
+        camera_inrinsics: camera intrinsic parameters
+
+    # Returns
+        person_sum: sum of L2 distances between each joint per person
+    """
+    initial_translation = np.reshape(initial_translation, (-1, 3))
+    new_poses3D = np.zeros((keypoints3D.shape))
+    for person in range(len(initial_translation)):
+        new_poses3D[person] = (keypoints3D[person] +
+                               initial_translation[person])
+    new_poses3D = new_poses3D.reshape((-1, 3))
+    rotation = np.identity(3)
+    translation = np.zeros((3,))
+    project2D = project_to_image(rotation, translation, new_poses3D,
+                                 camera_intrinsics)
+    joints_distance = np.linalg.norm(np.ravel(keypoints2D) -
+                                     np.ravel(project2D))
+
+    return np.sum(joints_distance)
+
+
+def merge_into_mean(keypoints2D, args_to_mean):
+    """merge keypoints and take the mean
+
+    # Arguments:
+             keypoints2D: keypoints2D (Nx17x2)
+             args_to_mean: dict of joint indices
+
+    # Returns:
+             keypoints2D: keypoints2D after merging
+            """
+    for point, joints_indices in args_to_mean.items():
+        keypoints2D[:, point] = (keypoints2D[:, joints_indices[0]] +
+                                 keypoints2D[:, joints_indices[1]]) / 2
+    return keypoints2D
+
+
+def filter_keypoints(keypoints, args_to_joints):
+    """filter keypoints.
+
+    # Arguments
+        keypoints: points in camera coordinates
+        args_to_joints: Array of joints indices
+
+    # Returns
+        filtered keypoints
+    # """
+    return keypoints[:, args_to_joints, :]
+
+
+def filter_keypoints3D(keypoints3D, args_to_joints3D):
+    """Selects 16 moving joints (Neck/Nose excluded) from 32 predicted
+       joints in 3D
+
+    # Arguments
+        keypoints3D: Nx96 points in camera coordinates
+        args_to_joints3D: list of indices
+
+    # Returns
+        filtered_joints_3D: Nx48 points (moving joints)
+    """
+    keypoints_num = len(keypoints3D)
+    keypoints3D = np.reshape(keypoints3D, [keypoints_num, 32, 3])
+    joints3D = filter_keypoints(keypoints3D, args_to_joints3D)
+    return joints3D
+
+
+def filter_keypoints2D(keypoints2D, args_to_mean, h36m_to_coco_joints2D):
+    """Selects 16 moving joints (Neck/Nose excluded) from 17 predicted
+       joints in 2D
+
+    # Arguments
+        keypoints3D: Nx17x2 points in camera coordinates
+        args_to_mean: keypoints indices
+        h36m_to_coco_joints2D: human36m dataset list of joints indices
+
+    # Returns
+        joints2D: Nx32 points (moving joints)
+    """
+    joints2D = filter_keypoints(keypoints2D, h36m_to_coco_joints2D)
+    joints2D = np.reshape(joints2D, [joints2D.shape[0], -1])
+    return joints2D
+
+
+def compute_optimized_pose3D(keypoints3D, joint_translation,
+                             camera_intrinsics):
+    """Compute the optimized 3D pose
+
+    # Arguments
+        keypoints3D: 3D keypoints
+        joint_translation: np array joints translation
+        camera_intrinsics: camera intrinsics parameters
+
+    # Returns
+        optimized_poses3D: np array of optimized posed3D
+    """
+    optimized_poses3D = []
+    for person in range(keypoints3D.shape[0]):
+        keypoints3D[person] = keypoints3D[person] + joint_translation[person]
+        rotation = np.identity(3)
+        translation = np.zeros((3,))
+        points = project_to_image(rotation, translation,
+                                  keypoints3D[person].reshape((-1, 3)),
+                                  camera_intrinsics)
+        optimized_poses3D.append(np.reshape(points, [1, 64]))
+    return np.array(optimized_poses3D)
```

### Comparing `pypaz-0.1.9/paz/backend/munkres.py` & `pypaz-0.2.4/paz/backend/munkres.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 def get_cover_matrix(shape):
     """Returns the initialized row and column cover matrix.
 
     # Arguments
         shape: Tuple. Shape of the cover matrix.
     """
-    row_covered = np.zeros(shape, dtype=bool)
-    col_covered = np.zeros(shape, dtype=bool)
+    row_covered = np.zeros(shape, dtype='bool')
+    col_covered = np.zeros(shape, dtype='bool')
     return row_covered, col_covered
 
 
 def find_uncovered_zero(n, cost_matrix, row_covered, col_covered, i0, j0):
     row = -1
     col = -1
     done = False
```

### Comparing `pypaz-0.1.9/paz/backend/render.py` & `pypaz-0.2.4/paz/backend/render.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/backend/standard.py` & `pypaz-0.2.4/paz/backend/standard.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import tensorflow as tf
 
 
 def append_values(dictionary, lists, keys):
     """Append dictionary values to lists
 
     # Arguments
         dictionary: dict
@@ -245,7 +246,28 @@
 
     image = pad_matrix(image, pool_size, strides, padding)
     H, W = image.shape[:2]
     for y in range(0, H - pool_size + 1, strides):
         for x in range(0, W - pool_size + 1, strides):
             max_image[y][x] = np.max(image[y:y + pool_size, x:x + pool_size])
     return max_image
+
+
+def predict(x, model, preprocess=None, postprocess=None):
+    """Preprocess, predict and postprocess input.
+    # Arguments
+        x: Input to model
+        model: Callable i.e. Keras model.
+        preprocess: Callable, used for preprocessing input x.
+        postprocess: Callable, used for postprocessing output of model.
+
+    # Note
+        If model outputs a tf.Tensor is converted automatically to numpy array.
+    """
+    if preprocess is not None:
+        x = preprocess(x)
+    y = model(x)
+    if isinstance(y, tf.Tensor):
+        y = y.numpy()
+    if postprocess is not None:
+        y = postprocess(y)
+    return y
```

### Comparing `pypaz-0.1.9/paz/datasets/CMU_poanoptic.py` & `pypaz-0.2.4/paz/datasets/CMU_poanoptic.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/cityscapes.py` & `pypaz-0.2.4/paz/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/coco.py` & `pypaz-0.2.4/paz/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/fat.py` & `pypaz-0.2.4/paz/datasets/fat.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/fer.py` & `pypaz-0.2.4/paz/datasets/fer.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/ferplus.py` & `pypaz-0.2.4/paz/datasets/ferplus.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/open_images.py` & `pypaz-0.2.4/paz/datasets/open_images.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/shapes.py` & `pypaz-0.2.4/paz/datasets/shapes.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/datasets/utils.py` & `pypaz-0.2.4/paz/datasets/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,14 +35,34 @@
                        'hot dog', 'pizza', 'donut', 'cake', 'chair', 'couch',
                        'potted plant', 'bed', 'dining table', 'toilet',
                        'tv', 'laptop', 'mouse', 'remote', 'keyboard',
                        'cell phone', 'microwave', 'oven', 'toaster',
                        'sink', 'refrigerator', 'book', 'clock', 'vase',
                        'scissors', 'teddy bear', 'hair drier', 'toothbrush']
 
+    elif dataset_name == 'COCO_EFFICIENTDET':
+        class_names = ['person', 'bicycle', 'car', 'motorcycle',
+                       'airplane', 'bus', 'train', 'truck', 'boat',
+                       'traffic light', 'fire hydrant', '0', 'stop sign',
+                       'parking meter', 'bench', 'bird', 'cat', 'dog', 'horse',
+                       'sheep', 'cow', 'elephant', 'bear', 'zebra', 'giraffe',
+                       '0', 'backpack', 'umbrella', '0', '0', 'handbag', 'tie',
+                       'suitcase', 'frisbee', 'skis', 'snowboard',
+                       'sports ball', 'kite', 'baseball bat', 'baseball glove',
+                       'skateboard', 'surfboard', 'tennis racket', 'bottle',
+                       '0', 'wine glass', 'cup', 'fork', 'knife', 'spoon',
+                       'bowl', 'banana', 'apple', 'sandwich', 'orange',
+                       'broccoli', 'carrot', 'hot dog', 'pizza', 'donut',
+                       'cake', 'chair', 'couch', 'potted plant', 'bed', '0',
+                       'dining table', '0', '0', 'toilet', '0', 'tv', 'laptop',
+                       'mouse', 'remote', 'keyboard', 'cell phone',
+                       'microwave', 'oven', 'toaster', 'sink', 'refrigerator',
+                       '0', 'book', 'clock', 'vase', 'scissors', 'teddy bear',
+                       'hair drier', 'toothbrush']
+
     elif dataset_name == 'YCBVideo':
         class_names = ['background', '037_scissors', '008_pudding_box',
                        '024_bowl', '005_tomato_soup_can', '007_tuna_fish_can',
                        '010_potted_meat_can', '061_foam_brick', '011_banana',
                        '035_power_drill', '004_sugar_box', '019_pitcher_base',
                        '006_mustard_bottle', '036_wood_block',
                        '009_gelatin_box', '051_large_clamp',
```

### Comparing `pypaz-0.1.9/paz/datasets/voc.py` & `pypaz-0.2.4/paz/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/evaluation/detection.py` & `pypaz-0.2.4/paz/evaluation/detection.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/__init__.py` & `pypaz-0.2.4/paz/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from .detection import SSD300
 from .detection import SSD512
 from .detection import HaarCascadeDetector
+from .detection import EFFICIENTDETD0
+from .detection import EFFICIENTDETD1
+from .detection import EFFICIENTDETD2
+from .detection import EFFICIENTDETD3
+from .detection import EFFICIENTDETD4
+from .detection import EFFICIENTDETD5
+from .detection import EFFICIENTDETD6
+from .detection import EFFICIENTDETD7
+from .keypoint.simplebaselines import SimpleBaseline
 from .keypoint.projector import Projector
 from .keypoint.keypointnet import KeypointNet
 from .keypoint.keypointnet import KeypointNetShared
 from .keypoint.keypointnet import KeypointNet2D
 from .keypoint.hrnet import HRNetResidual
 from .keypoint.hrnet import HRNetDense
 from .keypoint.detnet import DetNet
 from .keypoint.iknet import IKNet
 from .classification import build_xception
 from .classification import MiniXception
+from .classification import ProtoEmbedding
+from .classification import ProtoNet
 from .segmentation import UNET
 from .segmentation import UNET_VGG16
 from .segmentation import UNET_VGG19
 from .segmentation import UNET_RESNET50
 from .pose_estimation import HigherHRNet
```

### Comparing `pypaz-0.1.9/paz/models/classification/xception.py` & `pypaz-0.2.4/paz/models/classification/xception.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/detection/haar_cascade.py` & `pypaz-0.2.4/paz/models/detection/haar_cascade.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.url = WEIGHT_PATH + self.name
         self.path = get_file(self.name, self.url, cache_subdir='paz/models')
         self.model = cv2.CascadeClassifier(self.path)
         self.class_arg = class_arg
         self.scale = scale
         self.neighbors = neighbors
 
-    def predict(self, gray_image):
+    def __call__(self, gray_image):
         """ Detects faces from gray images.
 
         # Arguments
             gray_image: Numpy array of shape ``(H, W, 2)``.
 
         # Returns
             Numpy array of shape ``(num_boxes, 4)``.
```

### Comparing `pypaz-0.1.9/paz/models/detection/ssd300.py` & `pypaz-0.2.4/paz/models/detection/ssd300.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,10 +193,10 @@
         model_filename = '_'.join(['-'.join(model_filename), 'weights.hdf5'])
         weights_path = get_file(model_filename, WEIGHT_PATH + model_filename,
                                 cache_subdir='paz/models')
         print('Loading %s model weights' % weights_path)
         finetunning_model_names = ['SSD300-VGG-None_weights.hdf5',
                                    'SSD300-VOC-None_weights.hdf5']
         by_name = True if model_filename in finetunning_model_names else False
-        model.load_weights(weights_path, by_name)
+        model.load_weights(weights_path, by_name=by_name)
     model.prior_boxes = create_prior_boxes('VOC')
     return model
```

### Comparing `pypaz-0.1.9/paz/models/detection/ssd512.py` & `pypaz-0.2.4/paz/models/detection/ssd512.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/detection/utils.py` & `pypaz-0.2.4/paz/models/detection/utils.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/keypoint/detnet.py` & `pypaz-0.2.4/paz/models/keypoint/detnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/keypoint/hrnet.py` & `pypaz-0.2.4/paz/models/keypoint/hrnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/keypoint/iknet.py` & `pypaz-0.2.4/paz/models/keypoint/iknet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/keypoint/keypointnet.py` & `pypaz-0.2.4/paz/models/keypoint/keypointnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/keypoint/projector.py` & `pypaz-0.2.4/paz/models/keypoint/projector.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/layers.py` & `pypaz-0.2.4/paz/models/layers.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/pose_estimation/higher_hrnet.py` & `pypaz-0.2.4/paz/models/pose_estimation/higher_hrnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/models/segmentation/unet.py` & `pypaz-0.2.4/paz/models/segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/callbacks.py` & `pypaz-0.2.4/paz/optimization/callbacks.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/keypointnet_loss.py` & `pypaz-0.2.4/paz/optimization/losses/keypointnet_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/multi_box_loss.py` & `pypaz-0.2.4/paz/optimization/losses/multi_box_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/segmentation/dice_loss.py` & `pypaz-0.2.4/paz/optimization/losses/segmentation/dice_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/segmentation/focal_loss.py` & `pypaz-0.2.4/paz/optimization/losses/segmentation/focal_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/segmentation/jaccard_loss.py` & `pypaz-0.2.4/paz/optimization/losses/segmentation/jaccard_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/optimization/losses/segmentation/weighted_reconstruction.py` & `pypaz-0.2.4/paz/optimization/losses/segmentation/weighted_reconstruction.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/pipelines/__init__.py` & `pypaz-0.2.4/paz/pipelines/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,30 +16,48 @@
 from .detection import SSD300FAT
 from .detection import DetectHaarCascade
 from .detection import HaarCascadeFrontalFace
 from .detection import DetectMiniXceptionFER
 from .detection import DetectKeypoints2D
 from .detection import DetectFaceKeypointNet2D32
 from .detection import SSD512HandDetection
+from .detection import SSD512MinimalHandPose
+from .detection import SSDPreprocess
+from .detection import SSDPostprocess
+from .detection import DetectSingleShotEfficientDet
+from .detection import EfficientDetPreprocess
+from .detection import EfficientDetPostprocess
+from .detection import EFFICIENTDETD0COCO
+from .detection import EFFICIENTDETD1COCO
+from .detection import EFFICIENTDETD2COCO
+from .detection import EFFICIENTDETD3COCO
+from .detection import EFFICIENTDETD4COCO
+from .detection import EFFICIENTDETD5COCO
+from .detection import EFFICIENTDETD6COCO
+from .detection import EFFICIENTDETD7COCO
+from .detection import EFFICIENTDETD0VOC
 
 from .keypoints import KeypointNetSharedAugmentation
 from .keypoints import KeypointNetInference
 from .keypoints import EstimateKeypoints2D
 from .keypoints import FaceKeypointNet2D32
 from .keypoints import GetKeypoints
 from .keypoints import TransformKeypoints
 from .keypoints import HigherHRNetHumanPose2D
 from .keypoints import DetNetHandKeypoints
 from .keypoints import MinimalHandPoseEstimation
 from .keypoints import DetectMinimalHand
+from .keypoints import EstimateHumanPose3D
+from .keypoints import EstimateHumanPose
 
 from .renderer import RenderTwoViews
 from .renderer import RandomizeRenderedImage
 
 from .classification import MiniXceptionFER
+from .classification import ClassifyHandClosure
 
 from .pose import EstimatePoseKeypoints
 from .pose import HeadPoseKeypointNet2D32
 from .pose import SingleInstancePIX2POSE6D
 from .pose import MultiInstancePIX2POSE6D
 from .pose import MultiInstanceMultiClassPIX2POSE6D
 from .pose import SinglePowerDrillPIX2POSE6D
```

### Comparing `pypaz-0.1.9/paz/pipelines/angles.py` & `pypaz-0.2.4/paz/pipelines/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/pipelines/classification.py` & `pypaz-0.2.4/paz/pipelines/classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..abstract import SequentialProcessor
 from .. import processors as pr
 from . import PreprocessImage
 from ..models.classification import MiniXception
 from ..datasets import get_class_names
+from .keypoints import MinimalHandPoseEstimation
 
 
 # neutral, happiness, surprise, sadness, anger, disgust, fear, contempt
 EMOTION_COLORS = [[255, 0, 0], [45, 90, 45], [255, 0, 255], [255, 255, 0],
                   [0, 0, 255], [0, 255, 255], [0, 255, 0]]
 
 
@@ -41,7 +42,36 @@
         preprocess.insert(0, pr.ConvertColorSpace(pr.RGB2GRAY))
         preprocess.add(pr.ExpandDims(0))
         preprocess.add(pr.ExpandDims(-1))
         self.add(pr.Predict(self.classifier, preprocess))
         self.add(pr.CopyDomain([0], [1]))
         self.add(pr.ControlMap(pr.ToClassName(self.class_names), [0], [0]))
         self.add(pr.WrapOutput(['class_name', 'scores']))
+
+
+class ClassifyHandClosure(SequentialProcessor):
+    """Pipeline to classify minimal hand closure status.
+
+    # Example
+        ``` python
+        from paz.pipelines import ClassifyHandClosure
+
+        classify = ClassifyHandClosure()
+
+        # apply directly to an image (numpy-array)
+        inference = classify(image)
+        ```
+
+     # Returns
+        A function that takes an RGB image and outputs an image with class
+        status drawn on it.
+    """
+    def __init__(self, draw=True, right_hand=False):
+        super(ClassifyHandClosure, self).__init__()
+        self.add(MinimalHandPoseEstimation(draw, right_hand))
+        self.add(pr.UnpackDictionary(['image', 'relative_angles']))
+        self.add(pr.ControlMap(pr.IsHandOpen(), [1], [1]))
+        self.add(pr.ControlMap(pr.BooleanToTextMessage('OPEN', 'CLOSE'),
+                               [1], [1]))
+        if draw:
+            self.add(pr.ControlMap(pr.DrawText(), [0, 1], [0], {1: 1}))
+        self.add(pr.WrapOutput(['image', 'status']))
```

### Comparing `pypaz-0.1.9/paz/pipelines/detection.py` & `pypaz-0.2.4/paz/pipelines/pose.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,518 +1,470 @@
 import numpy as np
-
-from paz.models.detection.haar_cascade import WEIGHT_PATH
+from tensorflow.keras.utils import get_file
 
 from .. import processors as pr
-from ..abstract import SequentialProcessor, Processor
-from ..models import SSD512, SSD300, HaarCascadeDetector
-from ..datasets import get_class_names
+from ..abstract import Processor, SequentialProcessor, Pose6D
+from ..models import UNET_VGG16
+from ..backend.image.draw import draw_points2D, points3D_to_RGB
+from ..backend.standard import append_lists
+from ..backend.keypoints import (
+    translate_points2D_origin, denormalize_keypoints2D)
 
-from .image import AugmentImage, PreprocessImage
-from .classification import MiniXceptionFER
+from .masks import Pix2Points
+from .detection import HaarCascadeFrontalFace
 from .keypoints import FaceKeypointNet2D32
+from .detection import SSD300FAT, PostprocessBoxes2D
 
 
-class AugmentBoxes(SequentialProcessor):
-    """Perform data augmentation with bounding boxes.
+class EstimatePoseKeypoints(Processor):
+    def __init__(self, detect, estimate_keypoints, camera, offsets,
+                 model_points, class_to_dimensions, radius=3, thickness=1):
+        """Pose estimation pipeline using keypoints.
 
-    # Arguments
-        mean: List of three elements used to fill empty image spaces.
-    """
-    def __init__(self, mean=pr.BGR_IMAGENET_MEAN):
-        super(AugmentBoxes, self).__init__()
-        self.add(pr.ToImageBoxCoordinates())
-        self.add(pr.Expand(mean=mean))
-        self.add(pr.RandomSampleCrop())
-        self.add(pr.RandomFlipBoxesLeftRight())
-        self.add(pr.ToNormalizedBoxCoordinates())
+        # Arguments
+            detect: Function that outputs a dictionary with a key
+                ``boxes2D`` having a list of ``Box2D`` messages.
+            estimate_keypoints: Function that outputs a dictionary
+                with a key ``keypoints`` with numpy array as value
+            camera: Instance of ``paz.backend.camera.Camera`` with
+                camera intrinsics.
+            offsets: List of floats indicating the scaled offset to
+                be added to the ``Box2D`` coordinates.
+            model_points: Numpy array of shape ``(num_keypoints, 3)``
+                indicating the 3D coordinates of the predicted keypoints
+                from the ``esimate_keypoints`` function.
+            class_to_dimensions: Dictionary with keys being the class labels
+                of the predicted ``Box2D`` messages and the values a list of
+                three integers indicating the width, height and depth of the
+                object e.g. {'PowerDrill': [30, 20, 10]}.
+            radius: Int. radius of keypoint to be drawn.
+            thickness: Int. thickness of 3D box.
+
+        # Returns
+            A function that takes an RGB image and outputs the following
+            inferences as keys of a dictionary:
+                ``image``, ``boxes2D``, ``keypoints`` and ``poses6D``.
 
+        """
+        super(EstimatePoseKeypoints, self).__init__()
+        self.num_keypoints = estimate_keypoints.num_keypoints
+        self.detect = detect
+        self.estimate_keypoints = estimate_keypoints
+        self.square = SequentialProcessor()
+        self.square.add(pr.SquareBoxes2D())
+        self.square.add(pr.OffsetBoxes2D(offsets))
+        self.clip = pr.ClipBoxes2D()
+        self.crop = pr.CropBoxes2D()
+        self.change_coordinates = pr.ChangeKeypointsCoordinateSystem()
+        self.solve_PNP = pr.SolvePNP(model_points, camera)
+        self.draw_keypoints = pr.DrawKeypoints2D(self.num_keypoints, radius)
+        self.draw_box = pr.DrawBoxes3D(camera, class_to_dimensions,
+                                       thickness=thickness)
+        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'keypoints', 'poses6D'])
 
-class PreprocessBoxes(SequentialProcessor):
-    """Preprocess bounding boxes
+    def call(self, image):
+        boxes2D = self.detect(image)['boxes2D']
+        boxes2D = self.square(boxes2D)
+        boxes2D = self.clip(image, boxes2D)
+        cropped_images = self.crop(image, boxes2D)
+        poses6D, keypoints2D = [], []
+        for cropped_image, box2D in zip(cropped_images, boxes2D):
+            keypoints = self.estimate_keypoints(cropped_image)['keypoints']
+            keypoints = self.change_coordinates(keypoints, box2D)
+            pose6D = self.solve_PNP(keypoints)
+            image = self.draw_keypoints(image, keypoints)
+            image = self.draw_box(image, pose6D)
+            keypoints2D.append(keypoints)
+            poses6D.append(pose6D)
+        return self.wrap(image, boxes2D, keypoints2D, poses6D)
 
-    # Arguments
-        num_classes: Int.
-        prior_boxes: Numpy array of shape ``[num_boxes, 4]`` containing
-            prior/default bounding boxes.
-        IOU: Float. Intersection over union used to match boxes.
-        variances: List of two floats indicating variances to be encoded
-            for encoding bounding boxes.
-    """
-    def __init__(self, num_classes, prior_boxes, IOU, variances):
-        super(PreprocessBoxes, self).__init__()
-        self.add(pr.MatchBoxes(prior_boxes, IOU),)
-        self.add(pr.EncodeBoxes(prior_boxes, variances))
-        self.add(pr.BoxClassToOneHotVector(num_classes))
 
+class HeadPoseKeypointNet2D32(EstimatePoseKeypoints):
+    """Head pose estimation pipeline using a ``HaarCascade`` face detector
+        and a pre-trained ``KeypointNet2D`` estimation model.
 
-class AugmentDetection(SequentialProcessor):
-    """Augment boxes and images for object detection.
+        # Arguments
+            camera: Instance of ``paz.backend.camera.Camera`` with
+                camera intrinsics.
+            offsets: List of floats indicating the scaled offset to
+                be added to the ``Box2D`` coordinates.
+            radius: Int. radius of keypoint to be drawn.
+
+        # Example
+            ``` python
+            from paz.pipelines import HeadPoseKeypointNet2D32
+
+            estimate_pose = HeadPoseKeypointNet2D32()
+
+            # apply directly to an image (numpy-array)
+            inferences = estimate_pose(image)
+            ```
+
+        # Returns
+            A function that takes an RGB image and outputs the following
+            inferences as keys of a dictionary:
+                ``image``, ``boxes2D``, ``keypoints`` and ``poses6D``.
+        """
+    def __init__(self, camera, offsets=[0, 0], radius=5, thickness=2):
+        detect = HaarCascadeFrontalFace(draw=False)
+        estimate_keypoints = FaceKeypointNet2D32(draw=False)
+        """
+                               4--------1
+                              /|       /|
+                             / |      / |
+                            3--------2  |
+                            |  8_____|__5
+                            | /      | /
+                            |/       |/
+                            7--------6
+
+                   Z (depth)
+                  /
+                 /_____X (width)
+                 |
+                 |
+                 Y (height)
+        """
+        KEYPOINTS3D = np.array([
+            [-220, 1138, 678],  # left--center-eye
+            [+220, 1138, 678],  # right-center-eye
+            [-131, 1107, 676],  # left--eye close to nose
+            [-294, 1123, 610],  # left--eye close to ear
+            [+131, 1107, 676],  # right-eye close to nose
+            [+294, 1123, 610],  # right-eye close to ear
+            [-106, 1224, 758],  # left--eyebrow close to nose
+            [-375, 1208, 585],  # left--eyebrow close to ear
+            [+106, 1224, 758],  # right-eyebrow close to nose
+            [+375, 1208, 585],  # right-eyebrow close to ear
+            [0.0, 919, 909],  # nose
+            [-183, 683, 691],  # lefty-lip
+            [+183, 683, 691],  # right-lip
+            [0.0, 754, 826],  # up---lip
+            [0.0, 645, 815],  # down-lip
+        ])
+        KEYPOINTS3D = KEYPOINTS3D - np.mean(KEYPOINTS3D, axis=0)
+        super(HeadPoseKeypointNet2D32, self).__init__(
+            detect, estimate_keypoints, camera, offsets,
+            KEYPOINTS3D, {None: [900, 1200, 800]}, radius, thickness)
+
+
+class SingleInstancePIX2POSE6D(Processor):
+    """Predicts a single pose6D from an image. Optionally if a box2D message is
+        given it translates the predicted points2D to new origin located at
+        box2D top-left corner.
+
+    # Arguments
+        model: Keras segmentation model.
+        object_sizes: Array (3) determining the (width, height, depth)
+        camera: PAZ Camera with intrinsic matrix.
+        epsilon: Float. Values below this value would be replaced by 0.
+        resize: Boolean. If True RGB mask is resized before computing PnP.
+        class_name: Str indicating object name.
+        draw: Boolean. If True drawing functions are applied to output image.
 
-    # Arguments
-        prior_boxes: Numpy array of shape ``[num_boxes, 4]`` containing
-            prior/default bounding boxes.
-        split: Flag from `paz.processors.TRAIN`, ``paz.processors.VAL``
-            or ``paz.processors.TEST``. Certain transformations would take
-            place depending on the flag.
-        num_classes: Int.
-        size: Int. Image size.
-        mean: List of three elements indicating the per channel mean.
-        IOU: Float. Intersection over union used to match boxes.
-        variances: List of two floats indicating variances to be encoded
-            for encoding bounding boxes.
+    # Returns
+        Dictionary with inferred points2D, points3D, pose6D and image.
     """
-    def __init__(self, prior_boxes, split=pr.TRAIN, num_classes=21, size=300,
-                 mean=pr.BGR_IMAGENET_MEAN, IOU=.5,
-                 variances=[0.1, 0.1, 0.2, 0.2]):
-        super(AugmentDetection, self).__init__()
-        # image processors
-        self.augment_image = AugmentImage()
-        # self.augment_image.add(pr.ConvertColorSpace(pr.RGB2BGR))
-        self.preprocess_image = PreprocessImage((size, size), mean)
-        self.preprocess_image.insert(0, pr.ConvertColorSpace(pr.RGB2BGR))
-
-        # box processors
-        self.augment_boxes = AugmentBoxes()
-        args = (num_classes, prior_boxes, IOU, variances)
-        self.preprocess_boxes = PreprocessBoxes(*args)
-
-        # pipeline
-        self.add(pr.UnpackDictionary(['image', 'boxes']))
-        self.add(pr.ControlMap(pr.LoadImage(), [0], [0]))
-        if split == pr.TRAIN:
-            self.add(pr.ControlMap(self.augment_image, [0], [0]))
-            self.add(pr.ControlMap(self.augment_boxes, [0, 1], [0, 1]))
-        self.add(pr.ControlMap(self.preprocess_image, [0], [0]))
-        self.add(pr.ControlMap(self.preprocess_boxes, [1], [1]))
-        self.add(pr.SequenceWrapper(
-            {0: {'image': [size, size, 3]}},
-            {1: {'boxes': [len(prior_boxes), 4 + num_classes]}}))
-
-
-class PostprocessBoxes2D(SequentialProcessor):
-    """Filters, squares and offsets 2D bounding boxes
+    def __init__(self, model, object_sizes, camera,
+                 epsilon=0.15, resize=False, class_name=None, draw=True):
+        super(SingleInstancePIX2POSE6D, self).__init__()
+        self.camera = camera
+        self.pix2points = Pix2Points(model, object_sizes, epsilon, resize)
+        self.solvePnP = pr.SolveChangingObjectPnPRANSAC(self.camera.intrinsics)
+        self.draw_pose6D = pr.DrawPose6D(object_sizes, self.camera.intrinsics)
+        self.wrap = pr.WrapOutput(['image', 'points2D', 'points3D', 'pose6D'])
+        self.class_name = str(class_name)
+        self.object_sizes = object_sizes
+        self.draw = draw
 
-    # Arguments
-        valid_names: List of strings containing class names to keep.
+    def call(self, image, box2D=None):
+        inferences = self.pix2points(image)
+        points2D = inferences['points2D']
+        points3D = inferences['points3D']
+        points2D = denormalize_keypoints2D(points2D, *image.shape[:2])
+        if box2D is not None:
+            points2D = translate_points2D_origin(points2D, box2D.coordinates)
+            self.class_name = box2D.class_name
+        pose6D = None
+        if len(points3D) > self.solvePnP.MIN_REQUIRED_POINTS:
+            success, R, T = self.solvePnP(points3D, points2D)
+            if success:
+                pose6D = Pose6D.from_rotation_vector(R, T, self.class_name)
+        if (self.draw and (box2D is None) and (pose6D is not None)):
+            colors = points3D_to_RGB(points3D, self.object_sizes)
+            image = draw_points2D(image, points2D, colors)
+            image = self.draw_pose6D(image, pose6D)
+        inferences = self.wrap(image, points2D, points3D, pose6D)
+        return inferences
+
+
+class MultiInstancePIX2POSE6D(Processor):
+    """Predicts poses6D of multiple instances the same object from an image.
+
+    # Arguments
+        estimate_pose: Function that takes as input an image and outputs a
+            dictionary with points2D, points3D and pose6D messages e.g
+            SingleInstancePIX2POSE6D
         offsets: List of length two containing floats e.g. (x_scale, y_scale)
-    """
-    def __init__(self, offsets, valid_names=None):
-        super(PostprocessBoxes2D, self).__init__()
-        if valid_names is not None:
-            self.add(pr.FilterClassBoxes2D(valid_names))
-        self.add(pr.SquareBoxes2D())
-        self.add(pr.OffsetBoxes2D(offsets))
-
-
-class DetectSingleShot(Processor):
-    """Single-shot object detection prediction.
+        camera: PAZ Camera with intrinsic matrix.
+        draw: Boolean. If True drawing functions are applied to output image.
 
-    # Arguments
-        model: Keras model.
-        class_names: List of strings indicating the class names.
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        mean: List of three elements indicating the per channel mean.
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
+    # Returns
+        Dictionary with inferred boxes2D, poses6D and image.
     """
-    def __init__(self, model, class_names, score_thresh, nms_thresh,
-                 mean=pr.BGR_IMAGENET_MEAN, variances=[0.1, 0.1, 0.2, 0.2],
-                 draw=True):
-        self.model = model
-        self.class_names = class_names
-        self.score_thresh = score_thresh
-        self.nms_thresh = nms_thresh
-        self.variances = variances
+    def __init__(self, estimate_pose, offsets, camera=None, draw=True):
+        super(MultiInstancePIX2POSE6D, self).__init__()
         self.draw = draw
+        self.estimate_pose = estimate_pose
+        self.object_sizes = self.estimate_pose.object_sizes
+        self.camera = self.estimate_pose.camera if camera is None else camera
+        valid_names = [self.estimate_pose.class_name]
+        self.postprocess_boxes = PostprocessBoxes2D(offsets, valid_names)
 
-        super(DetectSingleShot, self).__init__()
-        preprocessing = SequentialProcessor(
-            [pr.ResizeImage(self.model.input_shape[1:3]),
-             pr.ConvertColorSpace(pr.RGB2BGR),
-             pr.SubtractMeanImage(mean),
-             pr.CastImage(float),
-             pr.ExpandDims(axis=0)])
-        postprocessing = SequentialProcessor(
-            [pr.Squeeze(axis=None),
-             pr.DecodeBoxes(self.model.prior_boxes, self.variances),
-             pr.NonMaximumSuppressionPerClass(self.nms_thresh),
-             pr.FilterBoxes(self.class_names, self.score_thresh)])
-        self.predict = pr.Predict(self.model, preprocessing, postprocessing)
-
-        self.denormalize = pr.DenormalizeBoxes2D()
-        self.draw_boxes2D = pr.DrawBoxes2D(self.class_names)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D'])
+        self.append_values = pr.AppendValues(
+            ['pose6D', 'points2D', 'points3D'])
+        self.clip = pr.ClipBoxes2D()
+        self.crop = pr.CropBoxes2D()
+        self.draw_RGBmask = pr.DrawRGBMasks(self.object_sizes)
+        self.draw_boxes2D = pr.DrawBoxes2D(valid_names, colors=[[0, 255, 0]])
+        self.draw_poses6D = pr.DrawPoses6D(
+            self.object_sizes, camera.intrinsics)
+        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'poses6D'])
 
-    def call(self, image):
-        boxes2D = self.predict(image)
-        boxes2D = self.denormalize(image, boxes2D)
+    def call(self, image, boxes2D):
+        boxes2D = self.postprocess_boxes(boxes2D)
+        boxes2D = self.clip(image, boxes2D)
+        cropped_images = self.crop(image, boxes2D)
+        poses6D, points2D, points3D = [], [], []
+        for crop, box2D in zip(cropped_images, boxes2D):
+            inferences = self.estimate_pose(crop, box2D)
+            self.append_values(inferences, [poses6D, points2D, points3D])
         if self.draw:
             image = self.draw_boxes2D(image, boxes2D)
-        return self.wrap(image, boxes2D)
-
-
-class SSD512COCO(DetectSingleShot):
-    """Single-shot inference pipeline with SSD512 trained on COCO.
-
-    # Arguments
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
-
-    # Example
-        ``` python
-        from paz.pipelines import SSD512COCO
-
-        detect = SSD512COCO()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
-     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-    # Reference
-        - [SSD: Single Shot MultiBox
-            Detector](https://arxiv.org/abs/1512.02325)
-    """
-    def __init__(self, score_thresh=0.60, nms_thresh=0.45, draw=True):
-        model = SSD512()
-        names = get_class_names('COCO')
-        super(SSD512COCO, self).__init__(
-            model, names, score_thresh, nms_thresh, draw=draw)
+            image = self.draw_RGBmask(image, points2D, points3D)
+            image = self.draw_poses6D(image, poses6D)
+        return self.wrap(image, boxes2D, poses6D)
 
 
-class SSD512YCBVideo(DetectSingleShot):
-    """Single-shot inference pipeline with SSD512 trained on YCBVideo.
+class SinglePowerDrillPIX2POSE6D(SingleInstancePIX2POSE6D):
+    """Predicts the pose6D of the YCB 035_power_drill object from an image.
+        Optionally if a box2D message is given it translates the predicted
+        points2D to new origin located at box2D top-left corner.
 
     # Arguments
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
-
-    # Example
-        ``` python
-        from paz.pipelines import SSD512YCBVideo
-
-        detect = SSD512YCBVideo()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
+        camera: PAZ Camera with intrinsic matrix.
+        epsilon: Float. Values below this value would be replaced by 0.
+        resize: Boolean. If True RGB mask is resized before computing PnP.
+        draw: Boolean. If True drawing functions are applied to output image.
 
     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-
+        Dictionary with inferred points2D, points3D, pose6D and image.
     """
-    def __init__(self, score_thresh=0.60, nms_thresh=0.45, draw=True):
-        names = get_class_names('YCBVideo')
-        model = SSD512(head_weights='YCBVideo', num_classes=len(names))
-        super(SSD512YCBVideo, self).__init__(
-            model, names, score_thresh, nms_thresh, draw=draw)
-
-
-class SSD300VOC(DetectSingleShot):
-    """Single-shot inference pipeline with SSD300 trained on VOC.
+    def __init__(self, camera, epsilon=0.15, resize=False, draw=True):
+        model = UNET_VGG16(3, (128, 128, 3))
+        URL = ('https://github.com/oarriaga/altamira-data/'
+               'releases/download/v0.13/')
+        name = 'UNET-VGG16_POWERDRILL_weights.hdf5'
+        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
+        print('Loading %s model weights' % weights_path)
+        model.load_weights(weights_path)
+        object_sizes = np.array([1840, 1870, 520]) / 10000
+        class_name = '035_power_drill'
+        super(SinglePowerDrillPIX2POSE6D, self).__init__(
+            model, object_sizes, camera, epsilon, resize, class_name, draw)
+
+
+class MultiPowerDrillPIX2POSE6D(MultiInstancePIX2POSE6D):
+    """Predicts poses6D of multiple instances the YCB 035_power_drill object
+        from an image.
 
     # Arguments
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
-
-    # Example
-        ``` python
-        from paz.pipelines import SSD300VOC
-
-        detect = SSD300VOC()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
-
-    # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-    # Reference
-        - [SSD: Single Shot MultiBox
-            Detector](https://arxiv.org/abs/1512.02325)
-    """
-    def __init__(self, score_thresh=0.60, nms_thresh=0.45, draw=True):
-        model = SSD300()
-        names = get_class_names('VOC')
-        super(SSD300VOC, self).__init__(
-            model, names, score_thresh, nms_thresh, draw=draw)
-
-
-class SSD300FAT(DetectSingleShot):
-    """Single-shot inference pipeline with SSD300 trained on FAT.
-
-    # Arguments
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
+        camera: PAZ Camera with intrinsic matrix.
+        offsets: List of length two containing floats e.g. (x_scale, y_scale)
+        epsilon: Float. Values below this value would be replaced by 0.
+        resize: Boolean. If True RGB mask is resized before computing PnP.
+        draw: Boolean. If True drawing functions are applied to output image.
 
-    # Example
-        ``` python
-        from paz.pipelines import SSD300FAT
-
-        detect = SSD300FAT()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
+        Dictionary with inferred boxes2D, poses6D and image.
     """
-    def __init__(self, score_thresh=0.60, nms_thresh=0.45, draw=True):
-        model = SSD300(22, 'FAT', 'FAT')
-        names = get_class_names('FAT')
-        super(SSD300FAT, self).__init__(
-            model, names, score_thresh, nms_thresh, draw=draw)
+    def __init__(self, camera, offsets, epsilon=0.15, resize=False, draw=True):
+        estimate_pose = SinglePowerDrillPIX2POSE6D(
+            camera, epsilon, resize, draw=False)
+        super(MultiPowerDrillPIX2POSE6D, self).__init__(
+            estimate_pose, offsets, camera, draw)
 
 
-class DetectHaarCascade(Processor):
-    """HaarCascade prediction pipeline/function from RGB-image.
+class PIX2POSEPowerDrill(Processor):
+    """PIX2POSE inference pipeline with SSD300 trained on FAT and UNET-VGG16
+        trained with domain randomization for the YCB object 035_power_drill.
 
     # Arguments
-        detector: An instantiated ``HaarCascadeDetector`` model.
-        offsets: List of two elements. Each element must be between [0, 1].
-        class_names: List of strings.
+        score_thresh: Float between [0, 1] for object detector.
+        nms_thresh: Float between [0, 1] indicating the non-maximum supression.
+        offsets: List of length two containing floats e.g. (x_scale, y_scale)
+        epsilon: Float. Values below this value would be replaced by 0.
         draw: Boolean. If ``True`` prediction are drawn in the returned image.
 
     # Returns
-        A function for predicting bounding box detections.
+        Dictionary with inferred boxes2D, poses6D and image.
     """
-    def __init__(self, detector, class_names=None, colors=None, draw=True):
-        super(DetectHaarCascade, self).__init__()
-        self.detector = detector
-        self.class_names = class_names
-        self.colors = colors
-        self.draw = draw
-        RGB2GRAY = pr.ConvertColorSpace(pr.RGB2GRAY)
-        postprocess = SequentialProcessor()
-        postprocess.add(pr.ToBoxes2D(self.class_names))
-        self.predict = pr.Predict(self.detector, RGB2GRAY, postprocess)
-        self.draw_boxes2D = pr.DrawBoxes2D(self.class_names, self.colors)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D'])
+    def __init__(self, camera, score_thresh=0.50, nms_thresh=0.45,
+                 offsets=[0.5, 0.5], epsilon=0.15, resize=False, draw=True):
+        self.detect = SSD300FAT(score_thresh, nms_thresh, draw=False)
+        self.estimate_pose = MultiPowerDrillPIX2POSE6D(
+            camera, offsets, epsilon, resize, draw)
 
     def call(self, image):
-        boxes2D = self.predict(image)
-        if self.draw:
-            image = self.draw_boxes2D(image, boxes2D)
-        return self.wrap(image, boxes2D)
+        return self.estimate_pose(image, self.detect(image)['boxes2D'])
 
 
-class HaarCascadeFrontalFace(DetectHaarCascade):
-    """HaarCascade pipeline for detecting frontal faces
+class MultiInstanceMultiClassPIX2POSE6D(Processor):
+    """Predicts poses6D of multiple instances of multiple objects from an image
 
     # Arguments
-        class_name: String indicating the class name.
-        color: List indicating the RGB color e.g. ``[0, 255, 0]``.
-        draw: Boolean. If ``False`` the bounding boxes are not drawn.
-
-    # Example
-        ``` python
-        from paz.pipelines import HaarCascadeFrontalFace
-
-        detect = HaarCascadeFrontalFace()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
-    # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-    """
-    def __init__(self, class_name='Face', color=[0, 255, 0], draw=True):
-        self.model = HaarCascadeDetector('frontalface_default', class_arg=0)
-        super(HaarCascadeFrontalFace, self).__init__(
-            self.model, [class_name], [color], draw)
-
-
-EMOTION_COLORS = [[255, 0, 0], [45, 90, 45], [255, 0, 255], [255, 255, 0],
-                  [0, 0, 255], [0, 255, 255], [0, 255, 0]]
-
-
-class DetectMiniXceptionFER(Processor):
-    """Emotion classification and detection pipeline.
-
-    # Returns
-        Dictionary with ``image`` and ``boxes2D``.
-
-    # Example
-        ``` python
-        from paz.pipelines import DetectMiniXceptionFER
-
-        detect = DetectMiniXceptionFER()
+        detect: Function that takes as input an image and outputs a dictionary
+            containing Boxes2D messages.
+        name_to_model: Dictionary with class name as key and as value a
+            Keras segmentation model.
+        name_to_size: Dictionary with class name as key and as value the
+            object sizes.
+        camera: PAZ Camera with intrinsic matrix.
+        offsets: List of length two containing floats e.g. (x_scale, y_scale)
+        epsilon: Float. Values below this value would be replaced by 0.
+        resize: Boolean. If True RGB mask is resized before computing PnP.
+        draw: Boolean. If True drawing functions are applied to output image.
 
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-    # References
-       - [Real-time Convolutional Neural Networks for Emotion and
-            Gender Classification](https://arxiv.org/abs/1710.07557)
+        Dictionary with inferred boxes2D, poses6D and image.
     """
-    def __init__(self, offsets=[0, 0], colors=EMOTION_COLORS):
-        super(DetectMiniXceptionFER, self).__init__()
-        self.offsets = offsets
-        self.colors = colors
-
-        # detection
-        self.detect = HaarCascadeFrontalFace()
-        self.square = SequentialProcessor()
-        self.square.add(pr.SquareBoxes2D())
-        self.square.add(pr.OffsetBoxes2D(offsets))
-        self.clip = pr.ClipBoxes2D()
-        self.crop = pr.CropBoxes2D()
-
-        # classification
-        self.classify = MiniXceptionFER()
-
-        # drawing and wrapping
-        self.class_names = self.classify.class_names
-        self.draw = pr.DrawBoxes2D(self.class_names, self.colors, True)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D'])
-
-    def call(self, image):
-        boxes2D = self.detect(image.copy())['boxes2D']
-        boxes2D = self.square(boxes2D)
-        boxes2D = self.clip(image, boxes2D)
-        cropped_images = self.crop(image, boxes2D)
-        for cropped_image, box2D in zip(cropped_images, boxes2D):
-            predictions = self.classify(cropped_image)
-            box2D.class_name = predictions['class_name']
-            box2D.score = np.amax(predictions['scores'])
-        image = self.draw(image, boxes2D)
-        return self.wrap(image, boxes2D)
-
-
-class DetectKeypoints2D(Processor):
-    def __init__(self, detect, estimate_keypoints, offsets=[0, 0], radius=3):
-        """General detection and keypoint estimator pipeline.
-
-        # Arguments
-            detect: Function for detecting objects. The output should be a
-                dictionary with key ``Boxes2D`` containing a list
-                of ``Boxes2D`` messages.
-            estimate_keypoints: Function for estimating keypoints. The output
-                should be a dictionary with key ``keypoints`` containing
-                a numpy array of keypoints.
-            offsets: List of two elements. Each element must be between [0, 1].
-            radius: Int indicating the radius of the keypoints to be drawn.
-        """
-        super(DetectKeypoints2D, self).__init__()
+    def __init__(self, detect, name_to_model, name_to_size, camera, offsets,
+                 epsilon=0.15, resize=False, draw=True):
+        super(MultiInstanceMultiClassPIX2POSE6D, self).__init__()
+        if set(name_to_model.keys()) != set(name_to_size.keys()):
+            raise ValueError('models and sizes must have same class names')
         self.detect = detect
-        self.estimate_keypoints = estimate_keypoints
-        self.num_keypoints = estimate_keypoints.num_keypoints
-        self.square = SequentialProcessor()
-        self.square.add(pr.SquareBoxes2D())
-        self.square.add(pr.OffsetBoxes2D(offsets))
+        self.name_to_pix2points = self._build_pix2points(
+            name_to_model, name_to_size, epsilon, resize)
+        valid_names = list(self.name_to_model.keys())
+        self.postprocess_boxes = PostprocessBoxes2D(offsets, valid_names)
+        self.draw_boxes2D = pr.DrawBoxes2D(valid_names)
+        self.draw_RGBmask = self._build_draw_RGBmask(name_to_size)
+        self.draw_pose6D = self._build_draw_pose6D(name_to_size, camera)
+        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'points3D', 'poses6D'])
+        self.solvePnP = pr.SolveChangingObjectPnPRANSAC(camera.intrinsics)
         self.clip = pr.ClipBoxes2D()
         self.crop = pr.CropBoxes2D()
-        self.change_coordinates = pr.ChangeKeypointsCoordinateSystem()
-        self.draw = pr.DrawKeypoints2D(self.num_keypoints, radius, False)
-        self.draw_boxes = pr.DrawBoxes2D(detect.class_names, detect.colors)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'keypoints'])
+        self.draw = draw
+
+    def _build_pix2points(self, name_to_model, name_to_size, epsilon, resize):
+        name_to_pix2points = {}
+        print(name_to_model)
+        for name, model in name_to_model.items():
+            pix2points = Pix2Points(model, name_to_size[name], epsilon, resize)
+            name_to_pix2points[name] = pix2points
+        return name_to_pix2points
+
+    def _build_draw_pose6D(self, name_to_size, camera):
+        name_to_draw = {}
+        for name, object_sizes in name_to_size.items():
+            draw = pr.DrawPose6D(object_sizes, camera.intrinsics)
+            name_to_draw[name] = draw
+        return name_to_draw
+
+    def _build_draw_RGBmask(self, name_to_size):
+        name_to_draw = {}
+        for name, object_sizes in name_to_size.items():
+            draw = pr.DrawRGBMask(object_sizes)
+            name_to_draw[name] = draw
+        return name_to_draw
+
+    def estimate_pose(self, image, box2D):
+        inferences = self.name_to_pix2points[box2D.class_name](image)
+        points2D = inferences['points2D']
+        points3D = inferences['points3D']
+        points2D = denormalize_keypoints2D(points2D, *image.shape[:2])
+        points2D = translate_points2D_origin(points2D, box2D.coordinates)
+        pose6D = None
+        if len(points3D) > self.solvePnP.MIN_REQUIRED_POINTS:
+            success, R, T = self.solvePnP(points3D, points2D)
+            if success:
+                pose6D = Pose6D.from_rotation_vector(R, T, box2D.class_name)
+        return points2D, points3D, pose6D
 
     def call(self, image):
         boxes2D = self.detect(image)['boxes2D']
-        boxes2D = self.square(boxes2D)
+        boxes2D = self.postprocess_boxes(boxes2D)
         boxes2D = self.clip(image, boxes2D)
         cropped_images = self.crop(image, boxes2D)
-        keypoints2D = []
-        for cropped_image, box2D in zip(cropped_images, boxes2D):
-            keypoints = self.estimate_keypoints(cropped_image)['keypoints']
-            keypoints = self.change_coordinates(keypoints, box2D)
-            keypoints2D.append(keypoints)
-            image = self.draw(image, keypoints)
-        image = self.draw_boxes(image, boxes2D)
-        return self.wrap(image, boxes2D, keypoints2D)
-
-
-class DetectFaceKeypointNet2D32(DetectKeypoints2D):
-    """Frontal face detection pipeline with facial keypoint estimation.
-
-    # Arguments
-        offsets: List of two elements. Each element must be between [0, 1].
-        radius: Int indicating the radius of the keypoints to be drawn.
+        points2D, points3D, poses6D = [], [], []
+        for crop, box2D in zip(cropped_images, boxes2D):
+            inferences = self.estimate_pose(crop, box2D)
+            append_lists(inferences, [points2D, points3D, poses6D])
+        if self.draw:
+            image = self.draw_boxes2D(image, boxes2D)
+            for box2D, pose6D in zip(boxes2D, poses6D):
+                name = box2D.class_name
+                image = self.draw_pose6D[name](image, pose6D)
+            for box2D, p2D, p3D in zip(boxes2D, points2D, points3D):
+                image = self.draw_RGBmask[name](image, p2D, p3D)
+        return self.wrap(image, boxes2D, points3D, poses6D)
+
+
+class PIX2YCBTools6D(MultiInstanceMultiClassPIX2POSE6D):
+    """Predicts poses6D of multiple instances of the YCB tools:
+        '035_power_drill', '051_large_clamp', '037_scissors'
+
+    # Arguments
+        camera: PAZ Camera with intrinsic matrix.
+        score_thresh: Float between [0, 1] for filtering Boxes2D.
+        nsm_thresh: Float between [0, 1] non-maximum-supression filtering.
+        offsets: List of length two containing floats e.g. (x_scale, y_scale)
+        epsilon: Float. Values below this value would be replaced by 0.
+        resize: Boolean. If True RGB mask is resized before computing PnP.
+        draw: Boolean. If True drawing functions are applied to output image.
 
-    # Example
-        ``` python
-        from paz.pipelines import DetectFaceKeypointNet2D32
-
-        detect = DetectFaceKeypointNet2D32()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
+        Dictionary with inferred boxes2D, poses6D and image.
     """
-    def __init__(self, offsets=[0, 0], radius=3):
-        detect = HaarCascadeFrontalFace(draw=False)
-        estimate_keypoints = FaceKeypointNet2D32(draw=False)
-        super(DetectFaceKeypointNet2D32, self).__init__(
-            detect, estimate_keypoints, offsets, radius)
-
-
-class SSD512HandDetection(DetectSingleShot):
-    """Minimal hand detection with SSD512Custom trained on OPenImageV6.
+    def __init__(self, camera, score_thresh=0.45, nms_thresh=0.15,
+                 offsets=[0.25, 0.25], epsilon=0.15, resize=False, draw=True):
 
-    # Arguments
-        score_thresh: Float between [0, 1]
-        nms_thresh: Float between [0, 1].
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
-
-    # Example
-        ``` python
-        from paz.pipelines import SSD512HandDetection
-
-        detect = SSD512HandDetection()
-
-        # apply directly to an image (numpy-array)
-        inferences = detect(image)
-        ```
-     # Returns
-        A function that takes an RGB image and outputs the predictions
-        as a dictionary with ``keys``: ``image`` and ``boxes2D``.
-        The corresponding values of these keys contain the image with the drawn
-        inferences and a list of ``paz.abstract.messages.Boxes2D``.
-
-    # Reference
-        - [SSD: Single Shot MultiBox
-            Detector](https://arxiv.org/abs/1512.02325)
-    """
-    def __init__(self, score_thresh=0.40, nms_thresh=0.45, draw=True):
-        class_names = ['background', 'hand']
-        num_classes = len(class_names)
-        model = SSD512(num_classes, base_weights='OIV6Hand',
-                       head_weights='OIV6Hand')
-        super(SSD512HandDetection, self).__init__(
-            model, class_names, score_thresh, nms_thresh, draw=draw)
+        self.detect = SSD300FAT(score_thresh, nms_thresh, draw=False)
+        self.name_to_sizes = self._build_name_to_sizes()
+        self.name_to_model = self._build_name_to_model()
+        super(PIX2YCBTools6D, self).__init__(
+            self.detect, self.name_to_model, self.name_to_sizes, camera,
+            offsets, epsilon, resize, draw)
+
+    def _build_name_to_model(self):
+        URL = ('https://github.com/oarriaga/altamira-data/'
+               'releases/download/v0.13/')
+
+        UNET_power_drill = UNET_VGG16(3, (128, 128, 3))
+        name = 'UNET-VGG16_POWERDRILL_weights.hdf5'
+        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
+        UNET_power_drill.load_weights(weights_path)
+
+        UNET_large_clamp = UNET_VGG16(3, (128, 128, 3))
+        name = 'UNET-VGG16_LARGE-CLAMP_weights.hdf5'
+        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
+        UNET_large_clamp.load_weights(weights_path)
+
+        UNET_scissors = UNET_VGG16(3, (128, 128, 3))
+        name = 'UNET-VGG16_SCISSORS_weights.hdf5'
+        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
+        UNET_scissors.load_weights(weights_path)
+
+        name_to_model = {'035_power_drill': UNET_power_drill,
+                         '051_large_clamp': UNET_large_clamp,
+                         '037_scissors': UNET_scissors
+                         }
+        return name_to_model
+
+    def _build_name_to_sizes(self):
+        name_to_sizes = {
+            '035_power_drill': np.array([1840, 1874, 572]) / 10000,
+            '051_large_clamp': np.array([2022, 1652, 362]) / 10000,
+            '037_scissors': np.array([960, 2014, 156]) / 10000
+        }
+        return name_to_sizes
```

### Comparing `pypaz-0.1.9/paz/pipelines/heatmaps.py` & `pypaz-0.2.4/paz/pipelines/heatmaps.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/pipelines/image.py` & `pypaz-0.2.4/paz/pipelines/image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/pipelines/keypoints.py` & `pypaz-0.2.4/paz/pipelines/keypoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import numpy as np
+
 from tensorflow.keras.utils import get_file
 
 from .renderer import RenderTwoViews
 from .image import PreprocessImageHigherHRNet
 from .heatmaps import GetHeatmapsAndTags
 
 from .. import processors as pr
 from ..abstract import SequentialProcessor, Processor
-from ..models import KeypointNet2D, HigherHRNet, DetNet
+from ..models import KeypointNet2D, HigherHRNet, DetNet, SimpleBaseline
 from .angles import IKNetHandJointAngles
 
-
-from ..backend.image import get_affine_transform, flip_left_right, lincolor
+from ..backend.image import get_affine_transform, lincolor
 from ..backend.keypoints import flip_keypoints_left_right, uv_to_vu
 from ..datasets import JOINT_CONFIG, FLIP_CONFIG
 
+from ..datasets.human36m import data_mean2D, data_stdev2D, args_to_mean
+from ..datasets.human36m import data_mean3D, data_stdev3D, dim_to_use3D
+from ..datasets.human36m import h36m_to_coco_joints2D
+
 
 class KeypointNetSharedAugmentation(SequentialProcessor):
     """Wraps ``RenderTwoViews`` as a sequential processor for using it directly
         with a ``paz.GeneratingSequence``.
 
     # Arguments
         renderer: ``RenderTwoViews`` processor.
@@ -272,32 +277,34 @@
         keypoints2D: Array [num_joints, 2]. 2D location of keypoints.
         keypoints3D: Array [num_joints, 3]. 3D location of keypoints.
     """
     def __init__(self, shape=(128, 128), draw=True, right_hand=False):
         super(DetNetHandKeypoints).__init__()
         self.draw = draw
         self.right_hand = right_hand
-        self.preprocess = pr.SequentialProcessor(
-            [pr.ResizeImage(shape), pr.ExpandDims(axis=0)])
-        self.hand_estimator = DetNet()
+        self.preprocess = pr.SequentialProcessor()
+        self.preprocess.add(pr.ResizeImage(shape))
+        self.preprocess.add(pr.ExpandDims(axis=0))
+        if self.right_hand:
+            self.preprocess.add(pr.FlipLeftRightImage())
+        self.predict = pr.Predict(model=DetNet(), preprocess=self.preprocess)
         self.scale_keypoints = pr.ScaleKeypoints(scale=4, shape=shape)
         self.draw_skeleton = pr.DrawHandSkeleton()
         self.wrap = pr.WrapOutput(['image', 'keypoints3D', 'keypoints2D'])
 
-    def call(self, input_image):
-        image = self.preprocess(input_image)
-        if self.right_hand:
-            image = flip_left_right(image)
-        keypoints3D, keypoints2D = self.hand_estimator.predict(image)
+    def call(self, image):
+        keypoints3D, keypoints2D = self.predict(image)
+        keypoints3D = keypoints3D.numpy()
+        keypoints2D = keypoints2D.numpy()
         if self.right_hand:
             keypoints2D = flip_keypoints_left_right(keypoints2D)
         keypoints2D = uv_to_vu(keypoints2D)
-        keypoints2D = self.scale_keypoints(keypoints2D, input_image)
+        keypoints2D = self.scale_keypoints(keypoints2D, image)
         if self.draw:
-            image = self.draw_skeleton(input_image, keypoints2D)
+            image = self.draw_skeleton(image, keypoints2D)
         return self.wrap(image, keypoints3D, keypoints2D)
 
 
 class MinimalHandPoseEstimation(pr.Processor):
     """Estimate 2D and 3D keypoints from minimal hand and draw a skeleton.
        Estimate absolute and relative joint angle for the minimal hand joints
        using the 3D keypoint locations.
@@ -378,7 +385,65 @@
                 inference['relative_angles'])
             box2D.class_name = hand_closure_status
             keypoints2D.append(keypoints)
             keypoints3D.append(inference['keypoints3D'])
             image = self.draw(image, keypoints)
         image = self.draw_boxes(image, boxes2D)
         return self.wrap(image, boxes2D, keypoints2D, keypoints3D)
+
+
+class EstimateHumanPose3D(Processor):
+    """ Estimate human pose 3D from 2D human pose.
+
+    # Arguments
+    input_shape: tuple
+    num_keypoints: Int. Number of keypoints.
+
+    # Return
+        keypoints3D: human pose 3D
+    """
+    def __init__(self, input_shape=(32,), num_keypoints=16):
+        super(EstimateHumanPose3D, self).__init__()
+        self.model = SimpleBaseline(input_shape, num_keypoints)
+        self.preprocessing = SequentialProcessor(
+            [pr.MergeKeypoints2D(args_to_mean),
+             pr.FilterKeypoints2D(args_to_mean, h36m_to_coco_joints2D),
+             pr.StandardizeKeypoints2D(data_mean2D, data_stdev2D)])
+        self.postprocess = pr.DestandardizeKeypoints2D(
+            data_mean3D, data_stdev3D, dim_to_use3D)
+        self.predict = pr.Predict(self.model, self.preprocessing,
+                                  self.postprocess)
+
+    def call(self, keypoints2D):
+        keypoints3D = self.predict(keypoints2D)
+        return keypoints3D
+
+
+class EstimateHumanPose(pr.Processor):
+    """ Estimates 2D and 3D keypoints of human from an image
+
+    # Arguments
+        estimate_keypoints_3D: 3D simple baseline model
+        args_to_mean: keypoints indices
+        h36m_to_coco_joints2D: h36m joints indices
+
+    # Returns
+        keypoints2D, keypoints3D
+    """
+    def __init__(self, filter=True):
+        super(EstimateHumanPose, self).__init__()
+        self.filter = filter
+        self.estimate_keypoints_2D = HigherHRNetHumanPose2D()
+        self.filter_keypoints2D = SequentialProcessor(
+            [pr.MergeKeypoints2D(args_to_mean),
+             pr.FilterKeypoints2D(args_to_mean, h36m_to_coco_joints2D)])
+        self.estimate_keypoints_3D = EstimateHumanPose3D()
+        self.wrap = pr.WrapOutput(['keypoints2D', 'keypoints3D'])
+
+    def call(self, image):
+        inferences2D = self.estimate_keypoints_2D(image)
+        keypoints2D = np.array(inferences2D['keypoints'])
+        if self.filter:
+            filter_keypoints2D = self.filter_keypoints2D(keypoints2D)
+        keypoints3D = self.estimate_keypoints_3D(keypoints2D)
+        keypoints3D = np.reshape(keypoints3D, (-1, 32, 3))
+        return self.wrap(filter_keypoints2D, keypoints3D)
```

### Comparing `pypaz-0.1.9/paz/pipelines/masks.py` & `pypaz-0.2.4/paz/pipelines/masks.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/pipelines/pose.py` & `pypaz-0.2.4/paz/processors/geometric.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,470 +1,554 @@
 import numpy as np
-from tensorflow.keras.utils import get_file
 
-from .. import processors as pr
-from ..abstract import Processor, SequentialProcessor, Pose6D
-from ..models import UNET_VGG16
-from ..backend.image.draw import draw_points2D, points3D_to_RGB
-from ..backend.standard import append_lists
-from ..backend.keypoints import (
-    translate_points2D_origin, denormalize_keypoints2D)
-
-from .masks import Pix2Points
-from .detection import HaarCascadeFrontalFace
-from .keypoints import FaceKeypointNet2D32
-from .detection import SSD300FAT, PostprocessBoxes2D
-
-
-class EstimatePoseKeypoints(Processor):
-    def __init__(self, detect, estimate_keypoints, camera, offsets,
-                 model_points, class_to_dimensions, radius=3, thickness=1):
-        """Pose estimation pipeline using keypoints.
-
-        # Arguments
-            detect: Function that outputs a dictionary with a key
-                ``boxes2D`` having a list of ``Box2D`` messages.
-            estimate_keypoints: Function that outputs a dictionary
-                with a key ``keypoints`` with numpy array as value
-            camera: Instance of ``paz.backend.camera.Camera`` with
-                camera intrinsics.
-            offsets: List of floats indicating the scaled offset to
-                be added to the ``Box2D`` coordinates.
-            model_points: Numpy array of shape ``(num_keypoints, 3)``
-                indicating the 3D coordinates of the predicted keypoints
-                from the ``esimate_keypoints`` function.
-            class_to_dimensions: Dictionary with keys being the class labels
-                of the predicted ``Box2D`` messages and the values a list of
-                three integers indicating the width, height and depth of the
-                object e.g. {'PowerDrill': [30, 20, 10]}.
-            radius: Int. radius of keypoint to be drawn.
-            thickness: Int. thickness of 3D box.
-
-        # Returns
-            A function that takes an RGB image and outputs the following
-            inferences as keys of a dictionary:
-                ``image``, ``boxes2D``, ``keypoints`` and ``poses6D``.
-
-        """
-        super(EstimatePoseKeypoints, self).__init__()
-        self.num_keypoints = estimate_keypoints.num_keypoints
-        self.detect = detect
-        self.estimate_keypoints = estimate_keypoints
-        self.square = SequentialProcessor()
-        self.square.add(pr.SquareBoxes2D())
-        self.square.add(pr.OffsetBoxes2D(offsets))
-        self.clip = pr.ClipBoxes2D()
-        self.crop = pr.CropBoxes2D()
-        self.change_coordinates = pr.ChangeKeypointsCoordinateSystem()
-        self.solve_PNP = pr.SolvePNP(model_points, camera)
-        self.draw_keypoints = pr.DrawKeypoints2D(self.num_keypoints, radius)
-        self.draw_box = pr.DrawBoxes3D(camera, class_to_dimensions,
-                                       thickness=thickness)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'keypoints', 'poses6D'])
+from ..abstract import Processor
+
+from ..backend.boxes import flip_left_right
+from ..backend.boxes import to_image_coordinates
+from ..backend.boxes import to_normalized_coordinates
+from ..backend.boxes import compute_iou
+from ..backend.image import warp_affine
+from ..backend.image import translate_image
+from ..backend.image import sample_scaled_translation
+from ..backend.image import get_rotation_matrix
+from ..backend.image import calculate_image_center
+from ..backend.keypoints import translate_keypoints
+from ..backend.keypoints import rotate_point2D
+from ..backend.standard import resize_with_same_aspect_ratio
+from ..backend.standard import get_transformation_scale
+
+
+class RandomFlipBoxesLeftRight(Processor):
+    """Flips image and implemented labels horizontally.
+    """
+    def __init__(self):
+        super(RandomFlipBoxesLeftRight, self).__init__()
+
+    def call(self, image, boxes):
+        if np.random.randint(0, 2):
+            boxes = flip_left_right(boxes, image.shape[1])
+            image = image[:, ::-1]
+        return image, boxes
+
+
+class ToImageBoxCoordinates(Processor):
+    """Convert normalized box coordinates to image-size box coordinates.
+    """
+    def __init__(self):
+        super(ToImageBoxCoordinates, self).__init__()
+
+    def call(self, image, boxes):
+        boxes = to_image_coordinates(boxes, image)
+        return image, boxes
+
+
+class ToNormalizedBoxCoordinates(Processor):
+    """Convert image-size box coordinates to normalized box coordinates.
+    """
+    def __init__(self):
+        super(ToNormalizedBoxCoordinates, self).__init__()
+
+    def call(self, image, boxes):
+        boxes = to_normalized_coordinates(boxes, image)
+        return image, boxes
+
+
+class RandomSampleCrop(Processor):
+    """Crops image while adjusting the normalized corner form
+    bounding boxes.
+
+    # Arguments
+        probability: Float between ''[0, 1]''.
+    """
+    def __init__(self, probability=0.50, max_trials=50):
+        self.probability = probability
+        self.max_trials = max_trials
+        self.jaccard_min_max = (
+            None,
+            (0.1, np.inf),
+            (0.3, np.inf),
+            (0.7, np.inf),
+            (0.9, np.inf),
+            (-np.inf, np.inf))
+
+    def call(self, image, boxes):
+
+        if self.probability < np.random.rand():
+            return image, boxes
+
+        labels = boxes[:, -1:]
+        boxes = boxes[:, :4]
+        H_original, W_original = image.shape[:2]
+
+        mode = np.random.randint(0, len(self.jaccard_min_max), 1)[0]
+        if self.jaccard_min_max[mode] is not None:
+            min_iou, max_iou = self.jaccard_min_max[mode]
+            for trial_arg in range(self.max_trials):
+                W = np.random.uniform(0.3 * W_original, W_original)
+                H = np.random.uniform(0.3 * H_original, H_original)
+                aspect_ratio = H / W
+                if (aspect_ratio < 0.5) or (aspect_ratio > 2):
+                    continue
+                x_min = np.random.uniform(W_original - W)
+                y_min = np.random.uniform(H_original - H)
+                x_max = int(x_min + W)
+                y_max = int(y_min + H)
+                x_min = int(x_min)
+                y_min = int(y_min)
+
+                image_crop_box = np.array([x_min, y_min, x_max, y_max])
+                overlap = compute_iou(image_crop_box, boxes)
+                if ((overlap.max() < min_iou) or (overlap.min() > max_iou)):
+                    continue
+
+                centers = (boxes[:, :2] + boxes[:, 2:]) / 2.0
+                centers_above_x_min = x_min < centers[:, 0]
+                centers_above_y_min = y_min < centers[:, 1]
+                centers_below_x_max = x_max > centers[:, 0]
+                centers_below_y_max = y_max > centers[:, 1]
+                mask = (centers_above_x_min * centers_above_y_min *
+                        centers_below_x_max * centers_below_y_max)
+                if not mask.any():
+                    continue
+
+                cropped_image = image[y_min:y_max, x_min:x_max, :].copy()
+                masked_boxes = boxes[mask, :].copy()
+                masked_labels = labels[mask].copy()
+                # should we use the box left and top corner or the crop's
+                masked_boxes[:, :2] = np.maximum(masked_boxes[:, :2],
+                                                 image_crop_box[:2])
+                # adjust to crop (by substracting crop's left,top)
+                masked_boxes[:, :2] -= image_crop_box[:2]
+                masked_boxes[:, 2:] = np.minimum(masked_boxes[:, 2:],
+                                                 image_crop_box[2:])
+                # adjust to crop (by substracting crop's left,top)
+                masked_boxes[:, 2:] -= image_crop_box[:2]
+                return cropped_image, np.hstack([masked_boxes, masked_labels])
+
+        boxes = np.hstack([boxes, labels])
+        return image, boxes
+
+
+class Expand(Processor):
+    """Expand image size up to 2x, 3x, 4x and fill values with mean color.
+    This transformation is applied with a probability of 50%.
+
+    # Arguments
+        max_ratio: Float.
+        mean: None/List: If `None` expanded image is filled with
+            the image mean.
+        probability: Float between ''[0, 1]''.
+    """
+    def __init__(self, max_ratio=2, mean=None, probability=0.5):
+        super(Expand, self).__init__()
+        self.max_ratio = max_ratio
+        self.mean = mean
+        self.probability = probability
+
+    def call(self, image, boxes):
+        if self.probability < np.random.rand():
+            return image, boxes
+        height, width, num_channels = image.shape
+        ratio = np.random.uniform(1, self.max_ratio)
+        left = np.random.uniform(0, width * ratio - width)
+        top = np.random.uniform(0, height * ratio - height)
+        expanded_image = np.zeros((int(height * ratio),
+                                   int(width * ratio), num_channels),
+                                  dtype=image.dtype)
+
+        if self.mean is None:
+            expanded_image[:, :, :] = np.mean(image, axis=(0, 1))
+        else:
+            expanded_image[:, :, :] = self.mean
+
+        expanded_image[int(top):int(top + height),
+                       int(left):int(left + width)] = image
+        expanded_boxes = boxes.copy()
+        expanded_boxes[:, 0:2] = boxes[:, 0:2] + (int(left), int(top))
+        expanded_boxes[:, 2:4] = boxes[:, 2:4] + (int(left), int(top))
+        return expanded_image, expanded_boxes
+
+
+class ApplyTranslation(Processor):
+    """Applies a translation of image and labels.
+
+    # Arguments
+        translation: A list of length two indicating the x,y translation values
+        fill_color: List of three integers indicating the
+            color values e.g. ''[0, 0, 0]''
+    """
+    def __init__(self, translation, fill_color=None):
+        super(ApplyTranslation, self).__init__()
+        self._matrix = np.zeros((2, 3), dtype=np.float32)
+        self._matrix[0, 0], self._matrix[1, 1] = 1.0, 1.0
+        self.fill_color = fill_color
+        self.translation = translation
+
+    @property
+    def translation(self):
+        return self._translation
+
+    @translation.setter
+    def translation(self, translation):
+        if translation is None:
+            self._translation = None
+        elif len(translation) == 2:
+            self._translation = translation
+            self._matrix[0, 2], self._matrix[1, 2] = translation
+        else:
+            raise ValueError('Translation should be `None` or have length two')
+
+    def call(self, image, keypoints=None):
+        height, width = image.shape[:2]
+        if self.fill_color is None:
+            fill_color = np.mean(image, axis=(0, 1))
+        image = warp_affine(image, self._matrix, fill_color)
+        if keypoints is not None:
+            keypoints[:, 0] = keypoints[:, 0] + self.translation[0]
+            keypoints[:, 1] = keypoints[:, 1] + self.translation[1]
+            return image, keypoints
+        return image
+
+
+class RandomTranslation(Processor):
+    """Applies a random translation to image and labels
+
+    # Arguments
+        delta_scale: List with two elements having the normalized deltas.
+            e.g. ''[.25, .25]''.
+
+        fill_color: List of three integers indicating the
+            color values e.g. ''[0, 0, 0]''.
+    """
+    def __init__(
+            self, delta_scale=[0.25, 0.25], fill_color=None):
+        super(RandomTranslation, self).__init__()
+        self.delta_scale = delta_scale
+        self.apply_translation = ApplyTranslation(None, fill_color)
+
+    @property
+    def delta_scale(self):
+        return self._delta_scale
+
+    @delta_scale.setter
+    def delta_scale(self, delta_scale):
+        x_delta_scale, y_delta_scale = delta_scale
+        if (x_delta_scale < 0) or (y_delta_scale < 0):
+            raise ValueError('Delta scale values should be a positive scalar')
+        self._delta_scale = delta_scale
 
     def call(self, image):
-        boxes2D = self.detect(image)['boxes2D']
-        boxes2D = self.square(boxes2D)
-        boxes2D = self.clip(image, boxes2D)
-        cropped_images = self.crop(image, boxes2D)
-        poses6D, keypoints2D = [], []
-        for cropped_image, box2D in zip(cropped_images, boxes2D):
-            keypoints = self.estimate_keypoints(cropped_image)['keypoints']
-            keypoints = self.change_coordinates(keypoints, box2D)
-            pose6D = self.solve_PNP(keypoints)
-            image = self.draw_keypoints(image, keypoints)
-            image = self.draw_box(image, pose6D)
-            keypoints2D.append(keypoints)
-            poses6D.append(pose6D)
-        return self.wrap(image, boxes2D, keypoints2D, poses6D)
-
-
-class HeadPoseKeypointNet2D32(EstimatePoseKeypoints):
-    """Head pose estimation pipeline using a ``HaarCascade`` face detector
-        and a pre-trained ``KeypointNet2D`` estimation model.
-
-        # Arguments
-            camera: Instance of ``paz.backend.camera.Camera`` with
-                camera intrinsics.
-            offsets: List of floats indicating the scaled offset to
-                be added to the ``Box2D`` coordinates.
-            radius: Int. radius of keypoint to be drawn.
-
-        # Example
-            ``` python
-            from paz.pipelines import HeadPoseKeypointNet2D32
-
-            estimate_pose = HeadPoseKeypointNet2D32()
-
-            # apply directly to an image (numpy-array)
-            inferences = estimate_pose(image)
-            ```
-
-        # Returns
-            A function that takes an RGB image and outputs the following
-            inferences as keys of a dictionary:
-                ``image``, ``boxes2D``, ``keypoints`` and ``poses6D``.
-        """
-    def __init__(self, camera, offsets=[0, 0], radius=5, thickness=2):
-        detect = HaarCascadeFrontalFace(draw=False)
-        estimate_keypoints = FaceKeypointNet2D32(draw=False)
-        """
-                               4--------1
-                              /|       /|
-                             / |      / |
-                            3--------2  |
-                            |  8_____|__5
-                            | /      | /
-                            |/       |/
-                            7--------6
-
-                   Z (depth)
-                  /
-                 /_____X (width)
-                 |
-                 |
-                 Y (height)
-        """
-        KEYPOINTS3D = np.array([
-            [-220, 1138, 678],  # left--center-eye
-            [+220, 1138, 678],  # right-center-eye
-            [-131, 1107, 676],  # left--eye close to nose
-            [-294, 1123, 610],  # left--eye close to ear
-            [+131, 1107, 676],  # right-eye close to nose
-            [+294, 1123, 610],  # right-eye close to ear
-            [-106, 1224, 758],  # left--eyebrow close to nose
-            [-375, 1208, 585],  # left--eyebrow close to ear
-            [+106, 1224, 758],  # right-eyebrow close to nose
-            [+375, 1208, 585],  # right-eyebrow close to ear
-            [0.0, 919, 909],  # nose
-            [-183, 683, 691],  # lefty-lip
-            [+183, 683, 691],  # right-lip
-            [0.0, 754, 826],  # up---lip
-            [0.0, 645, 815],  # down-lip
-        ])
-        KEYPOINTS3D = KEYPOINTS3D - np.mean(KEYPOINTS3D, axis=0)
-        super(HeadPoseKeypointNet2D32, self).__init__(
-            detect, estimate_keypoints, camera, offsets,
-            KEYPOINTS3D, {None: [900, 1200, 800]}, radius, thickness)
-
-
-class SingleInstancePIX2POSE6D(Processor):
-    """Predicts a single pose6D from an image. Optionally if a box2D message is
-        given it translates the predicted points2D to new origin located at
-        box2D top-left corner.
-
-    # Arguments
-        model: Keras segmentation model.
-        object_sizes: Array (3) determining the (width, height, depth)
-        camera: PAZ Camera with intrinsic matrix.
-        epsilon: Float. Values below this value would be replaced by 0.
-        resize: Boolean. If True RGB mask is resized before computing PnP.
-        class_name: Str indicating object name.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred points2D, points3D, pose6D and image.
-    """
-    def __init__(self, model, object_sizes, camera,
-                 epsilon=0.15, resize=False, class_name=None, draw=True):
-        super(SingleInstancePIX2POSE6D, self).__init__()
-        self.camera = camera
-        self.pix2points = Pix2Points(model, object_sizes, epsilon, resize)
-        self.solvePnP = pr.SolveChangingObjectPnPRANSAC(self.camera.intrinsics)
-        self.draw_pose6D = pr.DrawPose6D(object_sizes, self.camera.intrinsics)
-        self.wrap = pr.WrapOutput(['image', 'points2D', 'points3D', 'pose6D'])
-        self.class_name = str(class_name)
-        self.object_sizes = object_sizes
-        self.draw = draw
-
-    def call(self, image, box2D=None):
-        inferences = self.pix2points(image)
-        points2D = inferences['points2D']
-        points3D = inferences['points3D']
-        points2D = denormalize_keypoints2D(points2D, *image.shape[:2])
-        if box2D is not None:
-            points2D = translate_points2D_origin(points2D, box2D.coordinates)
-            self.class_name = box2D.class_name
-        pose6D = None
-        if len(points3D) > self.solvePnP.MIN_REQUIRED_POINTS:
-            success, R, T = self.solvePnP(points3D, points2D)
-            if success:
-                pose6D = Pose6D.from_rotation_vector(R, T, self.class_name)
-        if (self.draw and (box2D is None) and (pose6D is not None)):
-            colors = points3D_to_RGB(points3D, self.object_sizes)
-            image = draw_points2D(image, points2D, colors)
-            image = self.draw_pose6D(image, pose6D)
-        inferences = self.wrap(image, points2D, points3D, pose6D)
-        return inferences
-
-
-class MultiInstancePIX2POSE6D(Processor):
-    """Predicts poses6D of multiple instances the same object from a single image.
-
-    # Arguments
-        estimate_pose: Function that takes as input an image and outputs a
-            dictionary with points2D, points3D and pose6D messages e.g
-            SingleInstancePIX2POSE6D
-        offsets: List of length two containing floats e.g. (x_scale, y_scale)
-        camera: PAZ Camera with intrinsic matrix.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred boxes2D, poses6D and image.
-    """
-    def __init__(self, estimate_pose, offsets, camera=None, draw=True):
-        super(MultiInstancePIX2POSE6D, self).__init__()
-        self.draw = draw
-        self.estimate_pose = estimate_pose
-        self.object_sizes = self.estimate_pose.object_sizes
-        self.camera = self.estimate_pose.camera if camera is None else camera
-        valid_names = [self.estimate_pose.class_name]
-        self.postprocess_boxes = PostprocessBoxes2D(offsets, valid_names)
-
-        self.append_values = pr.AppendValues(
-            ['pose6D', 'points2D', 'points3D'])
-        self.clip = pr.ClipBoxes2D()
-        self.crop = pr.CropBoxes2D()
-        self.draw_RGBmask = pr.DrawRGBMasks(self.object_sizes)
-        self.draw_boxes2D = pr.DrawBoxes2D(valid_names, colors=[[0, 255, 0]])
-        self.draw_poses6D = pr.DrawPoses6D(
-            self.object_sizes, camera.intrinsics)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'poses6D'])
-
-    def call(self, image, boxes2D):
-        boxes2D = self.postprocess_boxes(boxes2D)
-        boxes2D = self.clip(image, boxes2D)
-        cropped_images = self.crop(image, boxes2D)
-        poses6D, points2D, points3D = [], [], []
-        for crop, box2D in zip(cropped_images, boxes2D):
-            inferences = self.estimate_pose(crop, box2D)
-            self.append_values(inferences, [poses6D, points2D, points3D])
-        if self.draw:
-            image = self.draw_boxes2D(image, boxes2D)
-            image = self.draw_RGBmask(image, points2D, points3D)
-            image = self.draw_poses6D(image, poses6D)
-        return self.wrap(image, boxes2D, poses6D)
-
-
-class SinglePowerDrillPIX2POSE6D(SingleInstancePIX2POSE6D):
-    """Predicts the pose6D of the YCB 035_power_drill object from an image.
-        Optionally if a box2D message is given it translates the predicted
-        points2D to new origin located at box2D top-left corner.
-
-    # Arguments
-        camera: PAZ Camera with intrinsic matrix.
-        epsilon: Float. Values below this value would be replaced by 0.
-        resize: Boolean. If True RGB mask is resized before computing PnP.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred points2D, points3D, pose6D and image.
-    """
-    def __init__(self, camera, epsilon=0.15, resize=False, draw=True):
-        model = UNET_VGG16(3, (128, 128, 3))
-        URL = ('https://github.com/oarriaga/altamira-data/'
-               'releases/download/v0.13/')
-        name = 'UNET-VGG16_POWERDRILL_weights.hdf5'
-        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
-        print('Loading %s model weights' % weights_path)
-        model.load_weights(weights_path)
-        object_sizes = np.array([1840, 1870, 520]) / 10000
-        class_name = '035_power_drill'
-        super(SinglePowerDrillPIX2POSE6D, self).__init__(
-            model, object_sizes, camera, epsilon, resize, class_name, draw)
-
-
-class MultiPowerDrillPIX2POSE6D(MultiInstancePIX2POSE6D):
-    """Predicts poses6D of multiple instances the YCB 035_power_drill object
-        from an image.
-
-    # Arguments
-        camera: PAZ Camera with intrinsic matrix.
-        offsets: List of length two containing floats e.g. (x_scale, y_scale)
-        epsilon: Float. Values below this value would be replaced by 0.
-        resize: Boolean. If True RGB mask is resized before computing PnP.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred boxes2D, poses6D and image.
-    """
-    def __init__(self, camera, offsets, epsilon=0.15, resize=False, draw=True):
-        estimate_pose = SinglePowerDrillPIX2POSE6D(
-            camera, epsilon, resize, draw=False)
-        super(MultiPowerDrillPIX2POSE6D, self).__init__(
-            estimate_pose, offsets, camera, draw)
-
-
-class PIX2POSEPowerDrill(Processor):
-    """PIX2POSE inference pipeline with SSD300 trained on FAT and UNET-VGG16
-        trained with domain randomization for the YCB object 035_power_drill.
-
-    # Arguments
-        score_thresh: Float between [0, 1] for object detector.
-        nms_thresh: Float between [0, 1] indicating the non-maximum supression.
-        offsets: List of length two containing floats e.g. (x_scale, y_scale)
-        epsilon: Float. Values below this value would be replaced by 0.
-        draw: Boolean. If ``True`` prediction are drawn in the returned image.
-
-    # Returns
-        Dictionary with inferred boxes2D, poses6D and image.
-    """
-    def __init__(self, camera, score_thresh=0.50, nms_thresh=0.45,
-                 offsets=[0.5, 0.5], epsilon=0.15, resize=False, draw=True):
-        self.detect = SSD300FAT(score_thresh, nms_thresh, draw=False)
-        self.estimate_pose = MultiPowerDrillPIX2POSE6D(
-            camera, offsets, epsilon, resize, draw)
+        height, width = image.shape[:2]
+        x_delta_scale, y_delta_scale = self.delta_scale
+        x = image.shape[1] * np.random.uniform(-x_delta_scale, x_delta_scale)
+        y = image.shape[0] * np.random.uniform(-y_delta_scale, y_delta_scale)
+        self.apply_translation.translation = [x, y]
+        return self.apply_translation(image)
+
+
+class RandomKeypointTranslation(Processor):
+    """Applies a random translation to image and keypoints.
+
+    # Arguments
+        delta_scale: List with two elements having the normalized deltas.
+            e.g. ''[.25, .25]''.
+        fill_color: ''None'' or List of three integers indicating the
+            color values e.g. ''[0, 0, 0]''. If ''None'' mean channel values of
+            the image will be calculated as fill values.
+        probability: Float between ''[0, 1]''.
+    """
+    def __init__(self, delta_scale=[.2, .2], fill_color=None, probability=0.5):
+        super(RandomKeypointTranslation, self).__init__()
+        self.delta_scale = delta_scale
+        self.fill_color = fill_color
+        self.probability = probability
+
+    @property
+    def probability(self):
+        return self._probability
+
+    @probability.setter
+    def probability(self, value):
+        if not (0.0 < value <= 1.0):
+            raise ValueError('Probability should be between "[0, 1]".')
+        self._probability = value
+
+    @property
+    def delta_scale(self):
+        return self._delta_scale
+
+    @delta_scale.setter
+    def delta_scale(self, delta_scale):
+        x_delta_scale, y_delta_scale = delta_scale
+        if (x_delta_scale < 0) or (y_delta_scale < 0):
+            raise ValueError('Delta scale values should be positive')
+        if (x_delta_scale > 1) or (y_delta_scale > 1):
+            raise ValueError('Delta scale values should be less than one')
+        self._delta_scale = delta_scale
+
+    def _sample_random_translation(self, delta_scale, image_shape):
+        x_delta_scale, y_delta_scale = delta_scale
+        x = image_shape[1] * np.random.uniform(-x_delta_scale, x_delta_scale)
+        y = image_shape[0] * np.random.uniform(-y_delta_scale, y_delta_scale)
+        return [x, y]
+
+    def call(self, image, keypoints):
+        if self.probability >= np.random.rand():
+            shape = image.shape[:2]
+            translation = sample_scaled_translation(self.delta_scale, shape)
+            if self.fill_color is None:
+                fill_color = np.mean(image, axis=(0, 1))
+            image = translate_image(image, translation, fill_color)
+            keypoints = translate_keypoints(keypoints, translation)
+        return image, keypoints
+
+
+class RandomKeypointRotation(Processor):
+    """Randomly rotate an images with its corresponding keypoints.
+
+    # Arguments
+        rotation_range: Int. indicating the max and min values in degrees
+            of the uniform distribution ''[-range, range]'' from which the
+            angles are sampled.
+        fill_color: ''None'' or List of three integers indicating the
+            color values e.g. ''[0, 0, 0]''. If ''None'' mean channel values of
+            the image will be calculated as fill values.
+    """
+    def __init__(self, rotation_range=30, fill_color=None, probability=0.5):
+        super(RandomKeypointRotation, self).__init__()
+        self.rotation_range = rotation_range
+        self.fill_color = fill_color
+        self.probability = probability
+
+    @property
+    def probability(self):
+        return self._probability
+
+    @probability.setter
+    def probability(self, value):
+        if not (0.0 < value <= 1.0):
+            raise ValueError('Probability should be between "[0, 1]".')
+        self._probability = value
+
+    def _calculate_image_center(self, image):
+        return (int(image.shape[0] / 2), int(image.shape[1] / 2))
+
+    def _rotate_image(self, image, degrees):
+        center = self._calculate_image_center(image)
+        matrix = get_rotation_matrix(center, degrees)
+        if self.fill_color is None:
+            fill_color = np.mean(image, axis=(0, 1))
+        return warp_affine(image, matrix, fill_color)
+
+    def _degrees_to_radians(self, degrees):
+        # negative sign changes rotation direction to follow openCV convention.
+        return - (3.14159 / 180) * degrees
+
+    def _build_rotation_matrix(self, radians):
+        return np.array([[np.cos(radians), - np.sin(radians)],
+                         [np.sin(radians), + np.cos(radians)]])
+
+    def _rotate_keypoints(self, keypoints, radians, image_center):
+        keypoints = keypoints - image_center
+        matrix = self._build_rotation_matrix(radians)
+        keypoints = np.matmul(matrix, keypoints.T).T
+        keypoints = keypoints + image_center
+        return keypoints
+
+    def _sample_rotation(self, rotation_range):
+        return np.random.uniform(-rotation_range, rotation_range)
+
+    def call(self, image, keypoints):
+        if self.probability >= np.random.rand():
+            degrees = self._sample_rotation(self.rotation_range)
+            image = self._rotate_image(image, degrees)
+            center = self._calculate_image_center(image)
+            radians = self._degrees_to_radians(degrees)
+            keypoints = self._rotate_keypoints(keypoints, radians, center)
+        return image, keypoints
+
+
+class RandomRotation(Processor):
+    """Randomly rotate an images
+
+    # Arguments
+        rotation_range: Int. indicating the max and min values in degrees
+            of the uniform distribution ``[-range, range]`` from which the
+            angles are sampled.
+        fill_color: ''None'' or List of three integers indicating the
+            color values e.g. ``[0, 0, 0]``. If ``None`` mean channel values of
+            the image will be calculated as fill values.
+        probability: Float between 0 and 1.
+    """
+    def __init__(self, rotation_range=30, fill_color=None, probability=0.5):
+        super(RandomRotation, self).__init__()
+        self.rotation_range = rotation_range
+        self.fill_color = fill_color
+        self.probability = probability
+
+    @property
+    def probability(self):
+        return self._probability
+
+    @probability.setter
+    def probability(self, value):
+        if not (0.0 < value <= 1.0):
+            raise ValueError('Probability should be between "[0, 1]".')
+        self._probability = value
+
+    def _calculate_image_center(self, image):
+        return (int(image.shape[0] / 2), int(image.shape[1] / 2))
+
+    def _rotate_image(self, image, degrees):
+        center = self._calculate_image_center(image)
+        matrix = get_rotation_matrix(center, degrees)
+        if self.fill_color is None:
+            fill_color = np.mean(image, axis=(0, 1))
+        return warp_affine(image, matrix, fill_color)
+
+    def _sample_rotation(self, rotation_range):
+        return np.random.uniform(-rotation_range, rotation_range)
 
     def call(self, image):
-        return self.estimate_pose(image, self.detect(image)['boxes2D'])
+        if self.probability >= np.random.rand():
+            degrees = self._sample_rotation(self.rotation_range)
+            image = self._rotate_image(image, degrees)
+        return image
+
+
+class TranslateImage(Processor):
+    """Applies a translation of image.
+    The translation is a list of length two indicating the x, y values.
 
+    # Arguments
+        fill_color: List of three integers indicating the
+            color values e.g. ``[0, 0, 0]``
+    """
+    def __init__(self, fill_color=None):
+        super(TranslateImage, self).__init__()
+        self.fill_color = fill_color
+
+    def call(self, image, translation):
+        return translate_image(image, translation, self.fill_color)
 
-class MultiInstanceMultiClassPIX2POSE6D(Processor):
-    """Predicts poses6D of multiple instances of multiple objects from an image
+
+class GetTransformationSize(Processor):
+    """Calculate the transformation size for the imgae.
+    The size is tuple of length two indicating the x, y values.
 
     # Arguments
-        detect: Function that takes as input an image and outputs a dictionary
-            containing Boxes2D messages.
-        name_to_model: Dictionary with class name as key and as value a
-            Keras segmentation model.
-        name_to_size: Dictionary with class name as key and as value the
-            object sizes.
-        camera: PAZ Camera with intrinsic matrix.
-        offsets: List of length two containing floats e.g. (x_scale, y_scale)
-        epsilon: Float. Values below this value would be replaced by 0.
-        resize: Boolean. If True RGB mask is resized before computing PnP.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred boxes2D, poses6D and image.
-    """
-    def __init__(self, detect, name_to_model, name_to_size, camera, offsets,
-                 epsilon=0.15, resize=False, draw=True):
-        super(MultiInstanceMultiClassPIX2POSE6D, self).__init__()
-        if set(name_to_model.keys()) != set(name_to_size.keys()):
-            raise ValueError('models and sizes must have same class names')
-        self.detect = detect
-        self.name_to_pix2points = self._build_pix2points(
-            name_to_model, name_to_size, epsilon, resize)
-        valid_names = list(self.name_to_model.keys())
-        self.postprocess_boxes = PostprocessBoxes2D(offsets, valid_names)
-        self.draw_boxes2D = pr.DrawBoxes2D(valid_names)
-        self.draw_RGBmask = self._build_draw_RGBmask(name_to_size)
-        self.draw_pose6D = self._build_draw_pose6D(name_to_size, camera)
-        self.wrap = pr.WrapOutput(['image', 'boxes2D', 'points3D', 'poses6D'])
-        self.solvePnP = pr.SolveChangingObjectPnPRANSAC(camera.intrinsics)
-        self.clip = pr.ClipBoxes2D()
-        self.crop = pr.CropBoxes2D()
-        self.draw = draw
-
-    def _build_pix2points(self, name_to_model, name_to_size, epsilon, resize):
-        name_to_pix2points = {}
-        print(name_to_model)
-        for name, model in name_to_model.items():
-            pix2points = Pix2Points(model, name_to_size[name], epsilon, resize)
-            name_to_pix2points[name] = pix2points
-        return name_to_pix2points
-
-    def _build_draw_pose6D(self, name_to_size, camera):
-        name_to_draw = {}
-        for name, object_sizes in name_to_size.items():
-            draw = pr.DrawPose6D(object_sizes, camera.intrinsics)
-            name_to_draw[name] = draw
-        return name_to_draw
-
-    def _build_draw_RGBmask(self, name_to_size):
-        name_to_draw = {}
-        for name, object_sizes in name_to_size.items():
-            draw = pr.DrawRGBMask(object_sizes)
-            name_to_draw[name] = draw
-        return name_to_draw
-
-    def estimate_pose(self, image, box2D):
-        inferences = self.name_to_pix2points[box2D.class_name](image)
-        points2D = inferences['points2D']
-        points3D = inferences['points3D']
-        points2D = denormalize_keypoints2D(points2D, *image.shape[:2])
-        points2D = translate_points2D_origin(points2D, box2D.coordinates)
-        pose6D = None
-        if len(points3D) > self.solvePnP.MIN_REQUIRED_POINTS:
-            success, R, T = self.solvePnP(points3D, points2D)
-            if success:
-                pose6D = Pose6D.from_rotation_vector(R, T, box2D.class_name)
-        return points2D, points3D, pose6D
+        image: Numpy array
+    """
+    def __init__(self, input_size, multiple):
+        super(GetTransformationSize, self).__init__()
+        self.input_size = input_size
+        self.multiple = multiple
 
     def call(self, image):
-        boxes2D = self.detect(image)['boxes2D']
-        boxes2D = self.postprocess_boxes(boxes2D)
-        boxes2D = self.clip(image, boxes2D)
-        cropped_images = self.crop(image, boxes2D)
-        points2D, points3D, poses6D = [], [], []
-        for crop, box2D in zip(cropped_images, boxes2D):
-            inferences = self.estimate_pose(crop, box2D)
-            append_lists(inferences, [points2D, points3D, poses6D])
-        if self.draw:
-            image = self.draw_boxes2D(image, boxes2D)
-            for box2D, pose6D in zip(boxes2D, poses6D):
-                name = box2D.class_name
-                image = self.draw_pose6D[name](image, pose6D)
-            for box2D, p2D, p3D in zip(boxes2D, points2D, points3D):
-                image = self.draw_RGBmask[name](image, p2D, p3D)
-        return self.wrap(image, boxes2D, points3D, poses6D)
-
-
-class PIX2YCBTools6D(MultiInstanceMultiClassPIX2POSE6D):
-    """Predicts poses6D of multiple instances of the YCB tools:
-        '035_power_drill', '051_large_clamp', '037_scissors'
-
-    # Arguments
-        camera: PAZ Camera with intrinsic matrix.
-        score_thresh: Float between [0, 1] for filtering Boxes2D.
-        nsm_thresh: Float between [0, 1] non-maximum-supression filtering.
-        offsets: List of length two containing floats e.g. (x_scale, y_scale)
-        epsilon: Float. Values below this value would be replaced by 0.
-        resize: Boolean. If True RGB mask is resized before computing PnP.
-        draw: Boolean. If True drawing functions are applied to output image.
-
-    # Returns
-        Dictionary with inferred boxes2D, poses6D and image.
-    """
-    def __init__(self, camera, score_thresh=0.45, nms_thresh=0.15,
-                 offsets=[0.25, 0.25], epsilon=0.15, resize=False, draw=True):
-
-        self.detect = SSD300FAT(score_thresh, nms_thresh, draw=False)
-        self.name_to_sizes = self._build_name_to_sizes()
-        self.name_to_model = self._build_name_to_model()
-        super(PIX2YCBTools6D, self).__init__(
-            self.detect, self.name_to_model, self.name_to_sizes, camera,
-            offsets, epsilon, resize, draw)
-
-    def _build_name_to_model(self):
-        URL = ('https://github.com/oarriaga/altamira-data/'
-               'releases/download/v0.13/')
-
-        UNET_power_drill = UNET_VGG16(3, (128, 128, 3))
-        name = 'UNET-VGG16_POWERDRILL_weights.hdf5'
-        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
-        UNET_power_drill.load_weights(weights_path)
-
-        UNET_large_clamp = UNET_VGG16(3, (128, 128, 3))
-        name = 'UNET-VGG16_LARGE-CLAMP_weights.hdf5'
-        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
-        UNET_large_clamp.load_weights(weights_path)
-
-        UNET_scissors = UNET_VGG16(3, (128, 128, 3))
-        name = 'UNET-VGG16_SCISSORS_weights.hdf5'
-        weights_path = get_file(name, URL + name, cache_subdir='paz/models')
-        UNET_scissors.load_weights(weights_path)
-
-        name_to_model = {'035_power_drill': UNET_power_drill,
-                         '051_large_clamp': UNET_large_clamp,
-                         '037_scissors': UNET_scissors
-                         }
-        return name_to_model
-
-    def _build_name_to_sizes(self):
-        name_to_sizes = {
-            '035_power_drill': np.array([1840, 1874, 572]) / 10000,
-            '051_large_clamp': np.array([2022, 1652, 362]) / 10000,
-            '037_scissors': np.array([960, 2014, 156]) / 10000
-        }
-        return name_to_sizes
+        size = resize_with_same_aspect_ratio(image, self.input_size,
+                                             self.multiple)
+        H, W = image.shape[:2]
+        if W < H:
+            size[0], size[1] = size[1], size[0]
+        return size
+
+
+class GetTransformationScale(Processor):
+    """Calculate the transformation scale for the imgae.
+    The scale is a numpy array of size two indicating the
+    width and height scale.
+
+    # Arguments
+        image: Numpy array
+        size: Numpy array of length 2
+    """
+    def __init__(self, scaling_factor):
+        super(GetTransformationScale, self).__init__()
+        self.scaling_factor = scaling_factor
+
+    def call(self, image, size):
+        scale = get_transformation_scale(image, size, self.scaling_factor)
+        H, W = image.shape[:2]
+        if W < H:
+            scale[0], scale[1] = scale[1], scale[0]
+        return scale
+
+
+class GetSourceDestinationPoints(Processor):
+    """Returns the source and destination points for affine transformation.
+
+    # Arguments
+        center: Numpy array of shape (2,). Center coordinates of image
+        scale: Numpy array of shape (2,). Scale of width and height of image
+        size: List of length 2. Size of image
+    """
+    def __init__(self, scaling_factor):
+        super(GetSourceDestinationPoints, self).__init__()
+        self.scaling_factor = scaling_factor
+
+    def _calculate_third_point(self, point2D_a, point2D_b):
+        difference = point2D_a - point2D_b
+        return point2D_a + np.array([-difference[1],
+                                     difference[0]], dtype=np.float32)
+
+    def _get_transformation_source_point(self, scale, center):
+        scale = scale * self.scaling_factor
+        center_W = scale[0] / 2
+        direction_vector = rotate_point2D([0, -center_W], 0)
+        points = np.zeros((3, 2), dtype=np.float32)
+        points[0, :] = center
+        points[1, :] = center + direction_vector
+        points[2:, :] = self._calculate_third_point(points[0, :], points[1, :])
+        return points
+
+    def _get_transformation_destination_point(self, output_size):
+        center_W, center_H = np.array(output_size[:2]) / 2
+        direction_vector = np.array([0, -center_W], np.float32)
+        points = np.zeros((3, 2), dtype=np.float32)
+        points[0, :] = [center_W, center_H]
+        points[1, :] = np.array([center_W, center_H]) + direction_vector
+        points[2:, :] = self._calculate_third_point(points[0, :], points[1, :])
+        return points
+
+    def call(self, center, scale, size):
+        if not isinstance(scale, np.ndarray) and not isinstance(scale, list):
+            scale = np.array([scale, scale])
+        source_point = self._get_transformation_source_point(scale, center)
+        destination_point = self._get_transformation_destination_point(size)
+        return source_point, destination_point
+
+
+class GetImageCenter(Processor):
+    """Calculate the center of the image and add an offset to the center.
+
+    # Arguments
+        image: Numpy array
+        offset: Float
+    """
+    def __init__(self, offset=0.5):
+        super(GetImageCenter, self).__init__()
+        self.offset = offset
+
+    def _add_offset(self, x, offset):
+        return (x + offset)
+
+    def call(self, image):
+        center_W, center_H = calculate_image_center(image)
+        center_W = int(self._add_offset(center_W, self.offset))
+        center_H = int(self._add_offset(center_H, self.offset))
+        return np.array([center_W, center_H])
+
+
+class WarpAffine(Processor):
+    """Applies an affine transformation to an image
+
+    # Arguments
+        image: Numpy array
+        transform: Numpy array. Transformation matrix
+        size: Numpy array. Transformation size
+    """
+    def __init__(self):
+        super(WarpAffine, self).__init__()
+
+    def call(self, image, transform, size):
+        image = warp_affine(image, transform, size=size)
+        return image
```

### Comparing `pypaz-0.1.9/paz/pipelines/renderer.py` & `pypaz-0.2.4/paz/pipelines/renderer.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/processors/__init__.py` & `pypaz-0.2.4/paz/processors/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 from .detection import MatchBoxes
 from .detection import EncodeBoxes
 from .detection import DecodeBoxes
 from .detection import NonMaximumSuppressionPerClass
 from .detection import FilterBoxes
 from .detection import OffsetBoxes2D
 from .detection import CropImage
+from .detection import RemoveClass
+from .detection import ScaleBox
+from .detection import BoxesToBoxes2D
+from .detection import BoxesWithOneHotVectorsToBoxes2D
+from .detection import BoxesWithClassArgToBoxes2D
+from .detection import RoundBoxes
+from .detection import MergeNMSBoxWithClass
 
 from .draw import DrawBoxes2D
 from .draw import DrawKeypoints2D
 from .draw import DrawBoxes3D
 from .draw import DrawRandomPolygon
 from .draw import DrawPose6D
 from .draw import DrawPoses6D
@@ -53,19 +60,23 @@
 from .image import BlendRandomCroppedBackground
 from .image import AddOcclusion
 from .image import ImageToNormalizedDeviceCoordinates
 from .image import NormalizedDeviceCoordinatesToImage
 from .image import ReplaceLowerThanThreshold
 from .image import GetNonZeroArguments
 from .image import GetNonZeroValues
+from .image import FlipLeftRightImage
 from .image import ImagenetPreprocessInput
+from .image import DivideStandardDeviationImage
+from .image import ScaledResize
 
 
 from .image import BGR_IMAGENET_MEAN
 from .image import RGB_IMAGENET_MEAN
+from .image import RGB_IMAGENET_STDEV
 
 from .renderer import Render
 
 from .geometric import RandomFlipBoxesLeftRight
 from .geometric import ToImageBoxCoordinates
 from .geometric import ToNormalizedBoxCoordinates
 from .geometric import RandomSampleCrop
@@ -91,14 +102,20 @@
 from .keypoints import RemoveKeypointsDepth
 from .keypoints import TranslateKeypoints
 from .keypoints import DenormalizeKeypoints2D
 from .keypoints import NormalizeKeypoints2D
 from .keypoints import ArgumentsToImageKeypoints2D
 from .keypoints import ScaleKeypoints
 from .keypoints import ComputeOrientationVector
+from .keypoints import MergeKeypoints2D
+from .keypoints import FilterKeypoints2D
+from .keypoints import StandardizeKeypoints2D
+from .keypoints import DestandardizeKeypoints2D
+from .keypoints import OptimizeHumanPose3D
+
 
 from .standard import ControlMap
 from .standard import ExpandDomain
 from .standard import CopyDomain
 from .standard import ExtendInputs
 from .standard import SequenceWrapper
 from .standard import Predict
@@ -114,17 +131,19 @@
 from .standard import SelectElement
 from .standard import StochasticProcessor
 from .standard import Stochastic
 from .standard import UnwrapDictionary
 from .standard import Scale
 from .standard import AppendValues
 from .standard import BooleanToTextMessage
+from .standard import PrintTopics
 
 from .pose import SolvePNP
 from .pose import SolveChangingObjectPnPRANSAC
+from .pose import Translation3DFromBoxWidth
 
 from .groups import ToAffineMatrix
 from .groups import RotationVectorToQuaternion
 from .groups import RotationVectorToRotationMatrix
 
 from ..backend.image.opencv_image import RGB2BGR
 from ..backend.image.opencv_image import BGR2RGB
```

### Comparing `pypaz-0.1.9/paz/processors/angles.py` & `pypaz-0.2.4/paz/processors/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/processors/detection.py` & `pypaz-0.2.4/paz/processors/detection.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from ..abstract import Processor, Box2D
 from ..backend.boxes import match
 from ..backend.boxes import encode
 from ..backend.boxes import decode
 from ..backend.boxes import offset
 from ..backend.boxes import clip
 from ..backend.boxes import nms_per_class
+from ..backend.boxes import merge_nms_box_with_class
 from ..backend.boxes import denormalize_box
 from ..backend.boxes import make_box_square
+from ..backend.boxes import filter_boxes
+from ..backend.boxes import scale_box
 
 
 class SquareBoxes2D(Processor):
     """Transforms bounding rectangular boxes into square bounding boxes.
     """
     def __init__(self):
         super(SquareBoxes2D, self).__init__()
@@ -22,15 +25,16 @@
     def call(self, boxes2D):
         for box2D in boxes2D:
             box2D.coordinates = make_box_square(box2D.coordinates)
         return boxes2D
 
 
 class DenormalizeBoxes2D(Processor):
-    """Denormalizes boxes shapes to be in accordance to the original image size.
+    """Denormalizes boxes shapes to be in accordance to the original
+    image size.
 
     # Arguments:
         image_size: List containing height and width of an image.
     """
     def __init__(self):
         super(DenormalizeBoxes2D, self).__init__()
 
@@ -116,33 +120,142 @@
         return boxes2D
 
 
 class ToBoxes2D(Processor):
     """Transforms boxes from dataset into `Boxes2D` messages.
 
     # Arguments
-        class_names: List of class names ordered with respect to the class
-            indices from the dataset ``boxes``.
-    """
-    def __init__(self, class_names=None, one_hot_encoded=False):
+        class_names: List of class names ordered with respect to the
+            class indices from the dataset ``boxes``.
+        one_hot_encoded: Bool, indicating if scores are one hot vectors.
+        default_score: Float, score to set.
+        default_class: Str, class to set.
+        box_method: Int, method to convert boxes to ``Boxes2D``.
+
+    # Properties
+        one_hot_encoded: Bool.
+        box_processor: Callable.
+
+    # Methods
+        call()
+    """
+    def __init__(
+            self, class_names=None, one_hot_encoded=False,
+            default_score=1.0, default_class=None, box_method=0):
         if class_names is not None:
-            self.arg_to_class = dict(zip(range(len(class_names)), class_names))
+            arg_to_class = dict(zip(range(len(class_names)), class_names))
         self.one_hot_encoded = one_hot_encoded
+        method_to_processor = {
+            0: BoxesWithOneHotVectorsToBoxes2D(arg_to_class),
+            1: BoxesToBoxes2D(default_score, default_class),
+            2: BoxesWithClassArgToBoxes2D(arg_to_class, default_score)}
+        self.box_processor = method_to_processor[box_method]
         super(ToBoxes2D, self).__init__()
 
-    def call(self, boxes):
-        numpy_boxes2D, boxes2D = boxes, []
-        for numpy_box2D in numpy_boxes2D:
-            if self.one_hot_encoded:
-                class_name = self.arg_to_class[np.argmax(numpy_box2D[4:])]
-            elif numpy_box2D.shape[-1] == 5:
-                class_name = self.arg_to_class[numpy_box2D[-1]]
-            elif numpy_box2D.shape[-1] == 4:
-                class_name = None
-            boxes2D.append(Box2D(numpy_box2D[:4], 1.0, class_name))
+    def call(self, box_data):
+        return self.box_processor(box_data)
+
+
+class BoxesToBoxes2D(Processor):
+    """Transforms boxes from dataset into `Boxes2D` messages given no
+    class names and score.
+
+    # Arguments
+        default_score: Float, score to set.
+        default_class: Str, class to set.
+
+    # Properties
+        default_score: Float.
+        default_class: Str.
+
+    # Methods
+        call()
+    """
+    def __init__(self, default_score=1.0, default_class=None):
+        self.default_score = default_score
+        self.default_class = default_class
+        super(BoxesToBoxes2D, self).__init__()
+
+    def call(self, box_data):
+        boxes2D = []
+        for box in box_data:
+            boxes2D.append(
+                Box2D(box[:4], self.default_score, self.default_class))
+        return boxes2D
+
+
+class BoxesWithOneHotVectorsToBoxes2D(Processor):
+    """Transforms boxes from dataset into `Boxes2D` messages given boxes
+    with scores as one hot vectors.
+
+    # Arguments
+        arg_to_class: List, of classes.
+
+    # Properties
+        arg_to_class: List.
+
+    # Methods
+        call()
+    """
+    def __init__(self, arg_to_class):
+        self.arg_to_class = arg_to_class
+        super(BoxesWithOneHotVectorsToBoxes2D, self).__init__()
+
+    def call(self, box_data):
+        boxes2D = []
+        for box in box_data:
+            class_scores = box[4:]
+            class_arg = np.argmax(class_scores)
+            score = class_scores[class_arg]
+            class_name = self.arg_to_class[class_arg]
+            boxes2D.append(Box2D(box[:4], score, class_name))
+        return boxes2D
+
+
+class BoxesWithClassArgToBoxes2D(Processor):
+    """Transforms boxes from dataset into `Boxes2D` messages given boxes
+    with class argument.
+
+    # Arguments
+        default_score: Float, score to set.
+        arg_to_class: List, of classes.
+
+    # Properties
+        default_score: Float.
+        arg_to_class: List.
+
+    # Methods
+        call()
+    """
+    def __init__(self, arg_to_class, default_score=1.0):
+        self.default_score = default_score
+        self.arg_to_class = arg_to_class
+        super(BoxesWithClassArgToBoxes2D, self).__init__()
+
+    def call(self, box_data):
+        boxes2D = []
+        for box in box_data:
+            class_name = self.arg_to_class[box[-1]]
+            boxes2D.append(Box2D(box[:4], self.default_score, class_name))
+        return boxes2D
+
+
+class RoundBoxes(Processor):
+    """Rounds the floating value coordinates of the box coordinates
+    into integer type.
+
+    # Methods
+        call()
+    """
+    def __init__(self):
+        super(RoundBoxes, self).__init__()
+
+    def call(self, boxes2D):
+        for box2D in boxes2D:
+            box2D.coordinates = box2D.coordinates.astype(int)
         return boxes2D
 
 
 class MatchBoxes(Processor):
     """Match prior boxes with ground truth boxes.
 
     # Arguments
@@ -197,60 +310,113 @@
 
 
 class NonMaximumSuppressionPerClass(Processor):
     """Applies non maximum suppression per class.
 
     # Arguments
         nms_thresh: Float between [0, 1].
-        conf_thresh: Float between [0, 1].
+        epsilon: Float between [0, 1].
     """
-    def __init__(self, nms_thresh=.45, conf_thresh=0.01):
+    def __init__(self, nms_thresh=.45, epsilon=0.01):
         self.nms_thresh = nms_thresh
-        self.conf_thresh = conf_thresh
+        self.epsilon = epsilon
         super(NonMaximumSuppressionPerClass, self).__init__()
 
-    def call(self, boxes):
-        boxes = nms_per_class(boxes, self.nms_thresh, self.conf_thresh)
-        return boxes
+    def call(self, box_data):
+        box_data, class_labels = nms_per_class(
+            box_data, self.nms_thresh, self.epsilon)
+        return box_data, class_labels
+
+
+class MergeNMSBoxWithClass(Processor):
+    """Merges box coordinates with their corresponding class
+    defined by `class_labels` which is decided by best box geometry
+    by non maximum suppression (and not by the best scoring class)
+    into a single output.
+    """
+    def __init__(self):
+        super(MergeNMSBoxWithClass, self).__init__()
+
+    def call(self, box_data, class_labels):
+        box_data = merge_nms_box_with_class(box_data, class_labels)
+        return box_data
 
 
 class FilterBoxes(Processor):
-    """Filters boxes outputted from function ``detect`` as ``Box2D`` messages.
+    """Filters boxes outputted from function ``detect`` as
+    ``Box2D`` messages.
 
     # Arguments
         class_names: List of class names.
         conf_thresh: Float between [0, 1].
     """
     def __init__(self, class_names, conf_thresh=0.5):
         self.class_names = class_names
         self.conf_thresh = conf_thresh
         self.arg_to_class = dict(zip(
             list(range(len(self.class_names))), self.class_names))
         super(FilterBoxes, self).__init__()
 
-    def call(self, boxes):
-        num_classes = boxes.shape[0]
-        boxes2D = []
-        for class_arg in range(1, num_classes):
-            class_detections = boxes[class_arg, :]
-            confidence_mask = np.squeeze(
-                class_detections[:, -1] >= self.conf_thresh)
-            confident_class_detections = class_detections[confidence_mask]
-            if len(confident_class_detections) == 0:
-                continue
-            class_name = self.arg_to_class[class_arg]
-            for confident_class_detection in confident_class_detections:
-                coordinates = confident_class_detection[:4]
-                score = confident_class_detection[4]
-                boxes2D.append(Box2D(coordinates, score, class_name))
-        return boxes2D
+    def call(self, box_data):
+        box_data = filter_boxes(box_data, self.conf_thresh)
+        return box_data
 
 
 class CropImage(Processor):
     """Crop images using a list of ``box2D``.
     """
     def __init__(self):
         super(CropImage, self).__init__()
 
     def call(self, image, box2D):
         x_min, y_min, x_max, y_max = box2D.coordinates
         return image[y_min:y_max, x_min:x_max]
+
+
+class RemoveClass(Processor):
+    """Remove a particular class from the pipeline.
+
+    # Arguments
+        class_names: List, indicating given class names.
+        class_arg: Int, index of the class to be removed.
+        renormalize: Bool, if true scores are renormalized.
+
+    # Properties
+        class_arg: Int.
+        renormalize: Bool
+
+    # Methods
+        call()
+    """
+    def __init__(self, class_names, class_arg=None, renormalize=False):
+        self.class_arg = class_arg
+        self.renormalize = renormalize
+        if class_arg is not None:
+            del class_names[class_arg]
+        super(RemoveClass, self).__init__()
+
+    def call(self, box_data):
+        if not self.renormalize and self.class_arg is not None:
+            box_data = np.delete(box_data, 4 + self.class_arg, axis=1)
+        elif self.renormalize:
+            raise NotImplementedError
+        return box_data
+
+
+class ScaleBox(Processor):
+    """Scale box coordinates of the prediction.
+
+    # Arguments
+        scales: Array of shape `()`, value to scale boxes.
+
+    # Properties
+        scales: Int.
+
+    # Methods
+        call()
+    """
+    def __init__(self):
+        super(ScaleBox, self).__init__()
+
+    def call(self, boxes, scales):
+        boxes = scale_box(boxes, scales)
+        return boxes
```

### Comparing `pypaz-0.1.9/paz/processors/draw.py` & `pypaz-0.2.4/paz/processors/draw.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/processors/groups.py` & `pypaz-0.2.4/paz/processors/groups.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.1.9/paz/processors/heatmaps.py` & `pypaz-0.2.4/paz/processors/heatmaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         resized_output.append(resized_heatmaps)
         resized_output = np.stack(resized_output, axis=0)
         return resized_output
 
     def call(self, outputs):
         for arg in range(len(outputs)):
             H, W = outputs[arg].shape[-2:]
-            H, W = self.scale_factor*H, self.scale_factor*W
+            H, W = self.scale_factor * H, self.scale_factor * W
             if self.full_scaling:
                 outputs[arg] = self._resize_output(outputs[arg], (W, H))
             else:
                 if len(outputs) > 1 and arg != len(outputs) - 1:
                     outputs[arg] = self._resize_output(outputs[arg], (W, H))
         return outputs
 
@@ -169,15 +169,15 @@
         updated_tags = []
         for tag in tags:
             updated_tags.append(np.expand_dims(tag, -1))
         return updated_tags
 
     def _calculate_heatmaps_average(self, heatmaps):
         if self.with_flip:
-            heatmaps_average = (heatmaps[0] + heatmaps[1])/2.0
+            heatmaps_average = (heatmaps[0] + heatmaps[1]) / 2.0
         else:
             heatmaps_average = heatmaps[0]
         return heatmaps_average
 
     def call(self, heatmaps, tags):
         heatmaps_average = self._calculate_heatmaps_average(heatmaps)
         heatmaps = heatmaps_average + heatmaps_average
@@ -245,15 +245,15 @@
         return np.squeeze(gathered)
 
     def call(self, heatmaps, tags):
         tags = tags.astype(np.int64)
         heatmaps = self._filter_heatmaps(heatmaps)
         num_images, keypoints_count, H, W = heatmaps.shape[:4]
         heatmaps = np.reshape(heatmaps, [num_images, keypoints_count, -1])
-        tags = np.reshape(tags, [num_images, keypoints_count, W*H, -1])
+        tags = np.reshape(tags, [num_images, keypoints_count, W * H, -1])
 
         top_k_keypoints, indices = self._get_top_k_keypoints(
             heatmaps, self.k, self.use_numpy)
         top_k_tags = self._get_top_k_tags(tags, indices)
         top_k_locations = get_keypoints_locations(indices, W)
 
         top_k_keypoints = np.expand_dims(top_k_keypoints, axis=-1)
@@ -345,15 +345,15 @@
                     heatmap = heatmaps[batch_id][keypoint_id]
                     if keypoint[2] > 0:
                         y, x = keypoint[0:2]
                         y = compare_vertical_neighbours(x, y, heatmap)
                         x = compare_horizontal_neighbours(x, y, heatmap)
                         grouped_keypoints[batch_id][
                             object_id, keypoint_id, 0:2] = add_offset_to_point(
-                                                            (y, x), offset=0.5)
+                                (y, x), offset=0.5)
         return grouped_keypoints
 
 
 class GetScores(Processor):
     """Calculate the score of the detection results.
     # Arguments
         grouped_keypoints: numpy array. keypoints grouped by tag
```

### Comparing `pypaz-0.1.9/paz/processors/image.py` & `pypaz-0.2.4/paz/processors/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 from ..backend.image import cast_image
 from ..backend.image import load_image
 from ..backend.image import random_saturation
 from ..backend.image import random_brightness
 from ..backend.image import random_contrast
 from ..backend.image import random_hue
 from ..backend.image import resize_image
+from ..backend.image import scale_resize
 from ..backend.image import random_image_blur
 from ..backend.image import random_flip_left_right
 from ..backend.image import convert_color_space
 from ..backend.image import show_image
 from ..backend.image import blend_alpha_channel
 from ..backend.image import random_shape_crop
 from ..backend.image import make_random_plain_image
 from ..backend.image import concatenate_alpha_mask
 from ..backend.image import draw_filled_polygon
 from ..backend.image import gaussian_image_blur
 from ..backend.image import normalized_device_coordinates_to_image
 from ..backend.image import image_to_normalized_device_coordinates
 from ..backend.image import replace_lower_than_threshold
-from ..backend.image import BILINEAR, CUBIC
+from ..backend.image import flip_left_right
+from ..backend.image import BILINEAR
 from ..backend.image.tensorflow_image import imagenet_preprocess_input
 
 
 B_IMAGENET_MEAN, G_IMAGENET_MEAN, R_IMAGENET_MEAN = 104, 117, 123
 BGR_IMAGENET_MEAN = (B_IMAGENET_MEAN, G_IMAGENET_MEAN, R_IMAGENET_MEAN)
 RGB_IMAGENET_MEAN = (R_IMAGENET_MEAN, G_IMAGENET_MEAN, B_IMAGENET_MEAN)
+B_IMAGENET_STDEV, G_IMAGENET_STDEV, R_IMAGENET_STDEV = 57.3, 57.1, 58.4
+RGB_IMAGENET_STDEV = (R_IMAGENET_STDEV, G_IMAGENET_STDEV, B_IMAGENET_STDEV)
 
 
 class CastImage(Processor):
     """Cast image to given dtype.
 
     # Arguments
         dtype: Str or np.dtype
@@ -493,7 +497,66 @@
 
 class ImagenetPreprocessInput(Processor):
     def __init__(self):
         super(ImagenetPreprocessInput, self).__init__()
 
     def call(self, image):
         return imagenet_preprocess_input(image)
+
+
+class FlipLeftRightImage(Processor):
+    """Flips an image left and right.
+
+    # Arguments
+        image: Numpy array.
+    """
+    def __init__(self):
+        super(FlipLeftRightImage, self).__init__()
+
+    def call(self, image):
+        return flip_left_right(image)
+
+
+class DivideStandardDeviationImage(Processor):
+    """Divide channel-wise standard deviation to image.
+
+    # Arguments
+        standard_deviation: List of length 3, containing the
+            channel-wise standard deviation.
+
+    # Properties
+        standard_deviation: List.
+
+    # Methods
+        call()
+    """
+    def __init__(self, standard_deviation):
+        self.standard_deviation = standard_deviation
+        super(DivideStandardDeviationImage, self).__init__()
+
+    def call(self, image):
+        return image / self.standard_deviation
+
+
+class ScaledResize(Processor):
+    """Resizes image by returning the scales to original image.
+
+    # Arguments
+        image_size: Int, desired size of the model input.
+
+    # Properties
+        image_size: Int.
+
+    # Methods
+        call()
+    """
+    def __init__(self, image_size):
+        self.image_size = image_size
+        super(ScaledResize, self).__init__()
+
+    def call(self, image):
+        """
+        # Arguments
+            image: Array, raw input image.
+        """
+        output_image, image_scale = scale_resize(image, self.image_size)
+        return output_image, image_scale
```

### Comparing `pypaz-0.1.9/paz/processors/munkres.py` & `pypaz-0.2.4/paz/processors/munkres.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
                       5: self._step5,
                       6: self._step6}
 
     def compute(self, cost_matrix):
         self.H, self.W = np.array(cost_matrix).shape[:2]
         self.cost_matrix = pad_matrix(cost_matrix, padding='square')
         self.n = len(self.cost_matrix)
-        self.marked = np.zeros((self.n, self.n), dtype=np.int)
-        self.path = np.zeros((self.n * 2, self.n * 2), dtype=np.int)
-        self.row_covered = np.zeros((self.n, 1), dtype=bool)
-        self.col_covered = np.zeros((self.n, 1), dtype=bool)
+        self.marked = np.zeros((self.n, self.n), dtype='int')
+        self.path = np.zeros((self.n * 2, self.n * 2), dtype='int')
+        self.row_covered = np.zeros((self.n, 1), 'bool')
+        self.col_covered = np.zeros((self.n, 1), 'bool')
 
         step = 1
         while not self.done:
             step_func = self.steps[step]
             step = step_func()
             if step == 7:
                 break
```

### Comparing `pypaz-0.1.9/paz/processors/pose.py` & `pypaz-0.2.4/paz/processors/pose.py`

 * *Files 19% similar despite different names*

```diff
@@ -87,7 +87,43 @@
 
     def call(self, object_points3D, image_points2D):
         success, rotation_vector, translation = solve_PnP_RANSAC(
             object_points3D, image_points2D, self.camera_intrinsics,
             self.inlier_thresh, self.num_iterations)
         rotation_vector = np.squeeze(rotation_vector)
         return success, rotation_vector, translation
+
+
+class Translation3DFromBoxWidth(Processor):
+    """Computes 3D translation from box width and real width ratio.
+
+    # Arguments
+        camera: Instance of ''paz.backend.Camera'' containing as properties
+            the ``camera_intrinsics`` a Numpy array of shape ``[3, 3]``
+            usually calculated from the openCV ``calibrateCamera`` function,
+            and the ``distortion`` a Numpy array of shape ``[5]`` in which the
+            elements are usually obtained from the openCV
+            ``calibrateCamera`` function.
+        real_width: Real width of the predicted box2D.
+
+    # Returns
+        Array (num_boxes, 3) containing all 3D translations.
+    """
+    def __init__(self, camera, real_width=0.3):
+        super(Translation3DFromBoxWidth, self).__init__()
+        self.camera = camera
+        self.real_width = real_width
+        self.focal_length = self.camera.intrinsics[0, 0]
+        self.u_camera_center = self.camera.intrinsics[0, 2]
+        self.v_camera_center = self.camera.intrinsics[1, 2]
+
+    def call(self, boxes2D):
+        hands_center = []
+        for box in boxes2D:
+            u_box_center, v_box_center = box.center
+            z_center = (self.real_width * self.focal_length) / box.width
+            u = u_box_center - self.u_camera_center
+            v = v_box_center - self.v_camera_center
+            x_center = (z_center * u) / self.focal_length
+            y_center = (z_center * v) / self.focal_length
+            hands_center.append([x_center, y_center, z_center])
+        return np.array(hands_center)
```

### Comparing `pypaz-0.1.9/paz/processors/standard.py` & `pypaz-0.2.4/paz/processors/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from ..abstract import Processor
 from ..backend.boxes import to_one_hot
-from ..backend.standard import append_values
+from ..backend.standard import append_values, predict
 
 
 class ControlMap(Processor):
     """Controls which inputs are passed ''processor'' and the order of its
         outputs.
 
     # Arguments
@@ -240,20 +240,15 @@
     def __init__(self, model, preprocess=None, postprocess=None):
         super(Predict, self).__init__()
         self.model = model
         self.preprocess = preprocess
         self.postprocess = postprocess
 
     def call(self, x):
-        if self.preprocess is not None:
-            x = self.preprocess(x)
-        y = self.model.predict(x)
-        if self.postprocess is not None:
-            y = self.postprocess(y)
-        return y
+        return predict(x, self.model, self.preprocess, self.postprocess)
 
 
 class ToClassName(Processor):
     def __init__(self, labels):
         super(ToClassName, self).__init__()
         self.labels = labels
 
@@ -466,7 +461,24 @@
 
     def call(self, flag):
         if flag:
             message = self.true_message
         else:
             message = self.false_message
         return message
+
+
+class PrintTopics(Processor):
+    """Prints topics
+    # Arguments
+        topics: List of keys to the inputted dictionary
+
+    # Returns
+        Returns same dictionary but outputs to terminal topic values.
+    """
+    def __init__(self, topics):
+        super(PrintTopics, self).__init__()
+        self.topics = topics
+
+    def call(self, dictionary):
+        [print(dictionary[topic]) for topic in self.topics]
+        return dictionary
```

### Comparing `pypaz-0.1.9/pypaz.egg-info/SOURCES.txt` & `pypaz-0.2.4/pypaz.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 paz/applications.py
 paz/abstract/__init__.py
 paz/abstract/loader.py
 paz/abstract/messages.py
 paz/abstract/processor.py
 paz/abstract/sequence.py
 paz/backend/__init__.py
+paz/backend/anchors.py
 paz/backend/angles.py
 paz/backend/boxes.py
 paz/backend/camera.py
 paz/backend/heatmaps.py
 paz/backend/keypoints.py
 paz/backend/munkres.py
 paz/backend/render.py
@@ -29,35 +30,44 @@
 paz/datasets/CMU_poanoptic.py
 paz/datasets/__init__.py
 paz/datasets/cityscapes.py
 paz/datasets/coco.py
 paz/datasets/fat.py
 paz/datasets/fer.py
 paz/datasets/ferplus.py
+paz/datasets/human36m.py
+paz/datasets/omniglot.py
 paz/datasets/open_images.py
 paz/datasets/shapes.py
 paz/datasets/utils.py
 paz/datasets/voc.py
 paz/evaluation/__init__.py
 paz/evaluation/detection.py
 paz/models/__init__.py
 paz/models/layers.py
 paz/models/classification/__init__.py
+paz/models/classification/protonet.py
 paz/models/classification/xception.py
 paz/models/detection/__init__.py
 paz/models/detection/haar_cascade.py
 paz/models/detection/ssd300.py
 paz/models/detection/ssd512.py
 paz/models/detection/utils.py
+paz/models/detection/efficientdet/__init__.py
+paz/models/detection/efficientdet/efficientdet.py
+paz/models/detection/efficientdet/efficientdet_blocks.py
+paz/models/detection/efficientdet/efficientnet.py
+paz/models/detection/efficientdet/layers.py
 paz/models/keypoint/__init__.py
 paz/models/keypoint/detnet.py
 paz/models/keypoint/hrnet.py
 paz/models/keypoint/iknet.py
 paz/models/keypoint/keypointnet.py
 paz/models/keypoint/projector.py
+paz/models/keypoint/simplebaselines.py
 paz/models/pose_estimation/__init__.py
 paz/models/pose_estimation/higher_hrnet.py
 paz/models/segmentation/__init__.py
 paz/models/segmentation/unet.py
 paz/optimization/__init__.py
 paz/optimization/callbacks.py
 paz/optimization/losses/__init__.py
@@ -87,12 +97,15 @@
 paz/processors/heatmaps.py
 paz/processors/image.py
 paz/processors/keypoints.py
 paz/processors/munkres.py
 paz/processors/pose.py
 paz/processors/renderer.py
 paz/processors/standard.py
+paz/utils/__init__.py
+paz/utils/documentation.py
+paz/utils/logger.py
 pypaz.egg-info/PKG-INFO
 pypaz.egg-info/SOURCES.txt
 pypaz.egg-info/dependency_links.txt
 pypaz.egg-info/requires.txt
 pypaz.egg-info/top_level.txt
```

