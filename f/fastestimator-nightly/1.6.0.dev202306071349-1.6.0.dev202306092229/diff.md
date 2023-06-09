# Comparing `tmp/fastestimator-nightly-1.6.0.dev202306071349.tar.gz` & `tmp/fastestimator-nightly-1.6.0.dev202306092229.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastestimator-nightly-1.6.0.dev202306071349.tar", last modified: Wed Jun  7 13:49:39 2023, max compression
+gzip compressed data, was "fastestimator-nightly-1.6.0.dev202306092229.tar", last modified: Fri Jun  9 22:29:58 2023, max compression
```

## Comparing `fastestimator-nightly-1.6.0.dev202306071349.tar` & `fastestimator-nightly-1.6.0.dev202306092229.tar`

### file list

```diff
@@ -1,779 +1,784 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.388904 fastestimator-nightly-1.6.0.dev202306071349/
--rw-r--r--   0 root         (0) root         (0)    11356 2023-06-07 13:41:03.000000 fastestimator-nightly-1.6.0.dev202306071349/LICENSE
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-07 13:49:39.384904 fastestimator-nightly-1.6.0.dev202306071349/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6271 2023-06-07 13:41:03.000000 fastestimator-nightly-1.6.0.dev202306071349/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.120914 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.124914 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.124914 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1609 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7452 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/lenet.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/unet.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.128914 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/lenet.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/unet.py
--rw-r--r--   0 root         (0) root         (0)     5580 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.152913 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/
--rw-r--r--   0 root         (0) root         (0)    10420 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_abs.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_argmax.py
--rw-r--r--   0 root         (0) root         (0)     4853 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_cast.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_concat.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_convert_tensor_precision.py
--rw-r--r--   0 root         (0) root         (0)     7866 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_exp.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_flip.py
--rw-r--r--   0 root         (0) root         (0)     6816 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_gather_from_batch.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_shape.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_huber.py
--rw-r--r--   0 root         (0) root         (0)     4476 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_iwd.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     4558 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_load_model.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_maximum.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_permute.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_pow.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_roll.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_save_model.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_sign.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_smooth_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     5742 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     4229 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5214 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_update_model.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_watch.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_where.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.152913 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/history.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/logs.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/plot.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.160913 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16450 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/combined_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/csv_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.172912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)     4020 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifair10.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifair100.py
--rw-r--r--   0 root         (0) root         (0)     3511 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifar10.py
--rw-r--r--   0 root         (0) root         (0)     3552 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifar100.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cub200.py
--rw-r--r--   0 root         (0) root         (0)     5955 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/em_3d.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/food101.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/horse2zebra.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/imdb_review.py
--rw-r--r--   0 root         (0) root         (0)     4544 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/medmnist.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mendeley.py
--rw-r--r--   0 root         (0) root         (0)     4039 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mitmovie_ner.py
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mnist.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/montgomery.py
--rw-r--r--   0 root         (0) root         (0)    12377 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mscoco.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/nih_chestxray.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/omniglot.py
--rw-r--r--   0 root         (0) root         (0)     9835 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/pascal_voc.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/penn_treebank.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/shakespeare.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/skl_digits.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/svhn.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/svhn_cropped.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/tednmt.py
--rw-r--r--   0 root         (0) root         (0)     4183 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/tiny_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     5450 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/usps.py
--rw-r--r--   0 root         (0) root         (0)    20523 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    26096 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9840 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/op_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9011 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/siamese_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    32377 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.172912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.172912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1200 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.172912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/reflection_padding_2d.py
--rw-r--r--   0 root         (0) root         (0)    51046 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.176912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.176912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.176912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     5873 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4997 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.192912 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)     5956 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/affine.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/center_crop.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/crop.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     4920 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     4302 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/flip.py
--rw-r--r--   0 root         (0) root         (0)     4555 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     4807 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/multivariate.py
--rw-r--r--   0 root         (0) root         (0)     4654 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     5222 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_crop.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_scale.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     5023 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/read_mat.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/resize.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/rotate.py
--rw-r--r--   0 root         (0) root         (0)     6186 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/transpose.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)    16330 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.212911 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)    10320 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/binarize.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/blur.py
--rw-r--r--   0 root         (0) root         (0)     3497 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/brightness.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/calibate.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/clahe.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/color.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/contrast.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/downscale.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/equalize.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/from_float.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/median_blur.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/minmax.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2978 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/normalize.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/onehot.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/posterize.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_rain.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_snow.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/read_image.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/rua.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/sharpness.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/shear_x.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/solarize.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_array.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_float.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_gray.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/translate_x.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/translate_y.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/univariate.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/word_to_id.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.216911 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)     2326 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/argmax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.216911 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7214 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/cutmix_batch.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/mixup_batch.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/average.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.220911 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/fgsm.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/gradient.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.220911 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5748 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/dice_loss.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/hinge.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     9186 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.224910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.224910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10587 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/model.py
--rw-r--r--   0 root         (0) root         (0)    12067 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/update.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/normalize.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/permute.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/resize3d.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/tensorop.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)    35579 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.228910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)    10488 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.228910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/golden_section.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/grid_search.py
--rw-r--r--   0 root         (0) root         (0)     9239 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.232910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/cartesian.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/heatmap.py
--rw-r--r--   0 root         (0) root         (0)     4789 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/parallel_coordinate_plot.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/vis_util.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.236910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41454 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.236910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/log_parse.py
--rw-r--r--   0 root         (0) root         (0)    33817 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/log_plot.py
--rw-r--r--   0 root         (0) root         (0)     9909 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/summary.py
--rw-r--r--   0 root         (0) root         (0)    18174 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.236910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/nightly_util.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.240910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.240910 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)     1678 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3867 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.252909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/
--rw-r--r--   0 root         (0) root         (0)     2539 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7889 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     9018 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/grid_display.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/image_saver.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)    23754 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    22579 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/test_report.py
--rw-r--r--   0 root         (0) root         (0)    41429 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.252909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/meta/
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/meta/_per_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.256909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/
--rw-r--r--   0 root         (0) root         (0)     2419 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/accuracy.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/auc.py
--rw-r--r--   0 root         (0) root         (0)    10591 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/bleu_score.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/dice.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/f1_score.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/mcc.py
--rw-r--r--   0 root         (0) root         (0)    18372 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/precision.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/recall.py
--rw-r--r--   0 root         (0) root         (0)    21156 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/trace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.260909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10667 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/eigen_cam.py
--rw-r--r--   0 root         (0) root         (0)     7808 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/grad_cam.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     6905 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/label_tracker.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.268909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/
--rw-r--r--   0 root         (0) root         (0)     4061 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25329 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/base_util.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/cli_util.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/data.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/google_download_util.py
--rw-r--r--   0 root         (0) root         (0)    31984 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/img_data.py
--rw-r--r--   0 root         (0) root         (0)     8260 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/latex_util.py
--rw-r--r--   0 root         (0) root         (0)    58364 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    17105 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/util.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.268909 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/xai/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12171 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.384904 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-07 13:49:38.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35102 2023-06-07 13:49:39.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:49:38.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-07 13:49:38.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      700 2023-06-07 13:49:38.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-07 13:49:38.000000 fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 13:49:39.388904 fastestimator-nightly-1.6.0.dev202306071349/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4671 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.272909 fastestimator-nightly-1.6.0.dev202306071349/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.272909 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.272909 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.276908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_save_model_load_model.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_update_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.276908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4980 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.276908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/dataset/test_batch_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.280908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.280908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.280908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.280908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.280908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.284908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.284908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.284908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.288908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)    10341 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     8292 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.288908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.292908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
--rw-r--r--   0 root         (0) root         (0)    22429 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_average.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.292908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_arc.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14280 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.292908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.296908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/visualize/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/visualize/test_visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.296908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11980 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/test_system.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_estimator.py
--rw-r--r--   0 root         (0) root         (0)    28311 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_network.py
--rw-r--r--   0 root         (0) root         (0)    98463 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.300908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.300908 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.304907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     7106 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_image_saver.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     8180 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_test_report.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.308907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_accuracy.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_dice.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_f1_score.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_mcc.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_precision.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_recall.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_eval_essential.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_test_essential.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_trace.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_train_essential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.312907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/
--rw-r--r--   0 root         (0) root         (0)      702 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/test_label_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.312907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_img_data.py
--rw-r--r--   0 root         (0) root         (0)    11100 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.312907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.312907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.316907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.316907 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.332906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_abs.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     6396 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_cast.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     8362 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_exp.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_gather.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_gather_from_batch.py
--rwxr-xr-x   0 root         (0) root         (0)     3742 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_iwd.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_maximum.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_permute.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_pow.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_roll.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_sign.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_watch.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_where.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.336906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/cli/test_cli_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_combine_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_csv_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_data.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13000 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.340906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/loss/test_focal_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.344906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.344906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.352906 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/test_numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.368905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.372905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.372905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.372905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     7142 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     3686 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_tensorop.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.376905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.376905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_golden_section_search.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_grid_search.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.376905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.380905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/logs/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/logs/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/test_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.380905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/test/test_unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.380905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.380905 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/test_auc_score.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/test_bleu_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.384904 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    18690 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:49:39.384904 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/xai/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/xai/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-06-07 13:41:04.000000 fastestimator-nightly-1.6.0.dev202306071349/test/run_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.568087 fastestimator-nightly-1.6.0.dev202306092229/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-06-09 22:21:27.000000 fastestimator-nightly-1.6.0.dev202306092229/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-09 22:29:58.568087 fastestimator-nightly-1.6.0.dev202306092229/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-06-09 22:21:27.000000 fastestimator-nightly-1.6.0.dev202306092229/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.300096 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.300096 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.304096 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7452 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/unet.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.304096 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/unet.py
+-rw-r--r--   0 root         (0) root         (0)     5580 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.328095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/
+-rw-r--r--   0 root         (0) root         (0)    10420 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_cast.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_concat.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_convert_tensor_precision.py
+-rw-r--r--   0 root         (0) root         (0)     7866 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_flip.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_gather_from_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_shape.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_huber.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_roll.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_save_model.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_smooth_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     5742 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_update_model.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_watch.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_where.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.332095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/history.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.340095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16450 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/combined_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/csv_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.348095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifair10.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifair100.py
+-rw-r--r--   0 root         (0) root         (0)     3511 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifar10.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifar100.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/em_3d.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/food101.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/horse2zebra.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/imdb_review.py
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/medmnist.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mendeley.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mitmovie_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/montgomery.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mscoco.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/nih_chestxray.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/omniglot.py
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/pascal_voc.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/penn_treebank.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/shakespeare.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/skl_digits.py
+-rw-r--r--   0 root         (0) root         (0)     6097 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/svhn.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/svhn_cropped.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/tednmt.py
+-rw-r--r--   0 root         (0) root         (0)     4183 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/tiny_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/usps.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    26711 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/op_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/siamese_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    32435 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.352095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.352095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.352095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/reflection_padding_2d.py
+-rw-r--r--   0 root         (0) root         (0)    51450 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.352095 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.356094 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.356094 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.368094 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/affine.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/crop.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/flip.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/multivariate.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/read_mat.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/resize.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     6186 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/transpose.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)    16330 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.392093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/binarize.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/blur.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/brightness.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/calibate.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/clahe.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/color.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/equalize.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/from_float.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/onehot.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/posterize.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/read_image.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/rua.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/solarize.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/univariate.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/word_to_id.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.396093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/argmax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.396093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/cutmix_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/mixup_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/average.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.400093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.404093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/dice_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/hinge.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     9186 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.404093 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.408092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    12067 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/update.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/permute.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)    36182 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.408092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10488 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.408092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/golden_section.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     9239 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.412092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/cartesian.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/parallel_coordinate_plot.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/vis_util.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.416092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41454 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.416092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/log_parse.py
+-rw-r--r--   0 root         (0) root         (0)    33817 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/log_plot.py
+-rw-r--r--   0 root         (0) root         (0)     9909 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/summary.py
+-rw-r--r--   0 root         (0) root         (0)    18174 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.420092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/nightly_util.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.420092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.424092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.428092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/grid_display.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)    23754 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    22579 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/test_report.py
+-rw-r--r--   0 root         (0) root         (0)    41429 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.432092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/meta/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/meta/_per_ds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.436092 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/auc.py
+-rw-r--r--   0 root         (0) root         (0)    10591 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/bleu_score.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/dice.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/mcc.py
+-rw-r--r--   0 root         (0) root         (0)    18372 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/precision.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/recall.py
+-rw-r--r--   0 root         (0) root         (0)    21156 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/trace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.440091 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10667 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/eigen_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7808 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/grad_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/label_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.440091 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/types/
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.448091 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/
+-rw-r--r--   0 root         (0) root         (0)     4176 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27641 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/base_util.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/cli_util.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/data.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/google_download_util.py
+-rw-r--r--   0 root         (0) root         (0)    31984 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/img_data.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/latex_util.py
+-rw-r--r--   0 root         (0) root         (0)    58364 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    17405 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/util.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.448091 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/xai/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.568087 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35224 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      700 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-09 22:29:58.000000 fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 22:29:58.568087 fastestimator-nightly-1.6.0.dev202306092229/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.452091 fastestimator-nightly-1.6.0.dev202306092229/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.452091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.452091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.456091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_save_model_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_update_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.456091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.460091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/dataset/test_batch_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.460091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.460091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.460091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.460091 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.464090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.464090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.464090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.464090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.468090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)    10341 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.468090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.472090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
+-rw-r--r--   0 root         (0) root         (0)    22429 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_average.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.476090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_arc.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    14280 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.476090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.476090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/visualize/test_visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.476090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)    17978 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/test_system.py
+-rw-r--r--   0 root         (0) root         (0)    23833 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    28311 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_network.py
+-rw-r--r--   0 root         (0) root         (0)    98463 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.480090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.480090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.488090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4498 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     8180 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_test_report.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.492090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_dice.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_mcc.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_recall.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_eval_essential.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_test_essential.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_train_essential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.492090 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/test_label_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.496089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_img_data.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.496089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.496089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.496089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.500089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.516089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_cast.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_concat.py
+-rw-r--r--   0 root         (0) root         (0)     8362 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_gather_from_batch.py
+-rwxr-xr-x   0 root         (0) root         (0)     3742 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_roll.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_watch.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_where.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.516089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/cli/test_cli_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.520089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_combine_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_csv_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.520089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.520089 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.524088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.524088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.524088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/loss/test_focal_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.524088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.524088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.536088 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/test_numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.552087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.552087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.552087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.556087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     7142 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.556087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.560087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_golden_section_search.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.560087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.560087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/logs/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/test_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.560087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/test/test_unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.560087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.564087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/test_auc_score.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/test_bleu_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.564087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/types/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/types/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.564087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    19505 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 22:29:58.568087 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/xai/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/xai/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-06-09 22:21:28.000000 fastestimator-nightly-1.6.0.dev202306092229/test/run_pr_test.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/LICENSE` & `fastestimator-nightly-1.6.0.dev202306092229/LICENSE`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202306092229/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202306071349
+Version: 1.6.0.dev202306092229
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/README.md` & `fastestimator-nightly-1.6.0.dev202306092229/README.md`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/lenet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/resnet9.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/pytorch/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/pytorch/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/lenet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/resnet9.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/architecture/tensorflow/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/architecture/tensorflow/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_abs.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_argmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_cast.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_check_nan.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_concat.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_convert_tensor_precision.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_convert_tensor_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_dice_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_exp.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_gather.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_lr.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_get_shape.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_get_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_hinge.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_huber.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_huber.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_iwd.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_lambertw.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_load_model.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_matmul.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_maximum.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_ones_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_percentile.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_permute.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_pow.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_resize3d.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_roll.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_save_model.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_save_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_set_lr.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_sign.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_smooth_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_squeeze.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_shape.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_to_type.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_update_model.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_watch.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_where.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/backend/_zscore.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/backend/_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/history.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/logs.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/logs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/main.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/plot.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/run.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/run.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/cli/train.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/combined_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/combined_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,41 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-
 from typing import List
 
 from torch.utils.data import ConcatDataset, Dataset
 
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class CombinedDataset(ConcatDataset):
     def __init__(self, datasets: List[Dataset]) -> None:
-        """
-        Combines a list of PyTorch Dataset
+        """Combines a list of PyTorch Datasets,
 
         Args:
-            datasets (List[Dataset]): List of PyTorch Dataset
+            datasets: Pytorch (or FE) Datasets to be combined.
 
         Raises:
             AssertionError: raise exception when the input list has less than 2 datasets.
             KeyError: raise exception when the datasets does not have same keys.
         """
         super().__init__(datasets)
         keys = None
 
         for ds in datasets:
             if isinstance(ds, Dataset) and isinstance(ds[0], dict):
                 if keys is None:
                     keys = ds[0].keys()
                 elif ds[0].keys() != keys:
-                    raise KeyError("All datasets should have same keys.")
+                    raise KeyError("All datasets should have the same keys.")
             else:
-                raise AssertionError(
-                    "Each dataset should be a type of PyTorch Dataset and should return a dictionary."
-                )
+                raise AssertionError("Each dataset should be a type of PyTorch Dataset and should return a dictionary.")
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/breast_cancer.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifair10.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifair10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifair100.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifair100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifar10.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifar10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cifar100.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cifar100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/cub200.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/cub200.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/em_3d.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/em_3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/food101.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/food101.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/horse2zebra.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/imdb_review.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/imdb_review.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/medmnist.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/medmnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mendeley.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mendeley.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mitmovie_ner.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mitmovie_ner.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mnist.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/montgomery.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/montgomery.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/mscoco.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/mscoco.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/nih_chestxray.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/nih_chestxray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/omniglot.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/omniglot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/pascal_voc.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/penn_treebank.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/penn_treebank.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/shakespeare.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/skl_digits.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/skl_digits.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/svhn.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/svhn.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/svhn_cropped.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/svhn_cropped.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/tednmt.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/tednmt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/tiny_imagenet.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/data/usps.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/data/usps.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dataloader.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dataloader.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Any, Dict, Hashable, Iterable, List, Optional, Sequence, Tuple, Union, cast, overload
 
 import jsonpickle
 import numpy as np
 from torch.utils.data import Dataset
 from typing_extensions import Self
 
+from fastestimator.types import DataSequence
 from fastestimator.util.base_util import FEID, get_shape, get_type
 from fastestimator.util.traceability_util import FeSplitSummary, traceable
 
 
 class KeySummary:
     """A summary of the dataset attributes corresponding to a particular key.
 
@@ -303,16 +304,18 @@
             sample = self[idx]
             key = sample[stratify]
             if hasattr(key, "tobytes"):
                 key = key.tobytes()  # Makes numpy arrays hashable
             distribution[key].append(idx)
 
         supply = {key: len(values) for key, values in distribution.items()}
-        split_requests = [{key: (n_split * n_tot) / original_size
-                           for key, n_tot in supply.items()} for n_split in split_counts]
+        split_requests = [{
+            key: (n_split * n_tot) / original_size
+            for key, n_tot in supply.items()
+        } for n_split in split_counts]
 
         def transfer(source: Dict[Any, int], sink: Dict[Any, int], key: Any, request: int) -> int:
             allowance = min(request, source[key])
             source[key] -= allowance
             sink[key] += allowance
             return allowance
 
@@ -435,14 +438,22 @@
     def __init__(self, data: Dict[int, Dict[str, Any]]) -> None:
         self.data = data
         self._summary = None
 
     def __len__(self) -> int:
         return len(self.data)
 
+    @overload
+    def __getitem__(self, index: int) -> Dict[str, Any]:
+        ...
+
+    @overload
+    def __getitem__(self, index: str) -> Union[np.ndarray, List[Any]]:
+        ...
+
     def __getitem__(self, index: Union[int, str]) -> Union[Dict[str, Any], np.ndarray, List[Any]]:
         """Look up data from the dataset.
 
         ```python
         data = fe.dataset.InMemoryDataset(...)  # {"x": <100>}, len(data) == 1000
         element = data[0]  # {"x": <100>}
         column = data["x"]  # <1000x100>
@@ -461,15 +472,23 @@
             return self.data[index]
         else:
             result = [elem[index] for elem in self.data.values()]
             if isinstance(result[0], np.ndarray):
                 return np.array(result)
             return result
 
-    def __setitem__(self, key: Union[int, str], value: Union[Dict[str, Any], Sequence[Any]]) -> None:
+    @overload
+    def __setitem__(self, key: int, value: Dict[str, Any]) -> None:
+        ...
+
+    @overload
+    def __setitem__(self, key: str, value: DataSequence) -> None:
+        ...
+
+    def __setitem__(self, key: Union[int, str], value: Union[Dict[str, Any], DataSequence]) -> None:
         """Modify data in the dataset.
 
         ```python
         data = fe.dataset.InMemoryDataset(...)  # {"x": <100>}, len(data) == 1000
         column = data["x"]  # <1000x100>
         column = column - np.mean(column)
         data["x"] = column
@@ -481,17 +500,20 @@
             value: The value to be inserted for the given `key`. Must be a dictionary if `key` is an integer. Otherwise
                 must be a sequence with the same length as the current length of the dataset.
 
         Raises:
             AssertionError: If the `value` is inappropriate given the type of the `key`.
         """
         if isinstance(key, int):
-            assert isinstance(value, Dict), "if setting a value using an integer index, must provide a dictionary"
+            assert isinstance(value, Dict), \
+                f"if setting a value using an integer index, must provide a dictionary (got {type(value)})"
             self.data[key] = value
         else:
+            assert isinstance(value, DataSequence), \
+                f"if setting a value using a key index, must provide a sequence (got {type(value)})"
             assert len(value) == len(self.data), \
                 "input value must be of length {}, but had length {}".format(len(self.data), len(value))
             for i in range(len(self.data)):
                 self.data[i][key] = value[i]
         self._summary = None
 
     def _skip_init(self, data: Dict[int, Dict[str, Any]], **kwargs) -> Self:
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/numpy_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,8 +39,8 @@
                 current_size = len(val)
             else:
                 raise ValueError("Please ensure you are passing numpy array or list in the data dictionary.")
             if size is not None:
                 assert size == current_size, "All data arrays must have the same number of elements"
             else:
                 size = current_size
-        super().__init__({i: {k: v[i] for k, v in data.items()} for i in range(size)})
+        super().__init__({i: {k: v[i] for k, v in data.items()} for i in range(size)} if size else {})
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/op_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/op_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/dataset/siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/dataset/siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/estimator.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from fastestimator.summary.system import Summary, System
 from fastestimator.trace.io.best_model_saver import BestModelSaver
 from fastestimator.trace.io.model_saver import ModelSaver
 from fastestimator.trace.io.restore_wizard import RestoreWizard
 from fastestimator.trace.io.traceability import Traceability
 from fastestimator.trace.trace import EvalEssential, Logger, PerDSTrace, TestEssential, Trace, TrainEssential, \
     sort_traces
-from fastestimator.util.base_util import NonContext, to_list, to_set, warn
+from fastestimator.util.base_util import NonContext, filter_nones, to_list, to_set, warn
 from fastestimator.util.data import Data, FilteredData
 from fastestimator.util.traceability_util import traceable
 from fastestimator.util.util import Suppressor, draw
 
 
 def _verify_dependency_versions() -> None:
     """Print warning messages if the user is using unexpected versions of TF or torch.
@@ -89,26 +89,26 @@
 
     def __init__(self,
                  pipeline: Pipeline,
                  network: BaseNetwork,
                  epochs: int,
                  train_steps_per_epoch: Optional[int] = None,
                  eval_steps_per_epoch: Optional[int] = None,
-                 traces: Union[None, Trace, Scheduler[Trace], Iterable[Union[Trace, Scheduler[Trace]]]] = None,
+                 traces: Union[None, Trace, Scheduler[Trace], Sequence[Union[None, Trace, Scheduler[Trace]]]] = None,
                  log_steps: Optional[int] = 100,
                  eval_log_steps: Sequence[int] = (),
-                 monitor_names: Union[None, str, Iterable[str]] = None):
+                 monitor_names: Union[None, str, Iterable[Optional[str]]] = None):
         self.traces_in_use = []
         self.filepath = os.path.realpath(inspect.stack()[2].filename)  # Record this for history tracking
         assert log_steps is None or log_steps >= 0, \
             "log_steps must be None or positive (or 0 to disable only train logging)"
-        self.monitor_names = to_set(monitor_names) | network.get_loss_keys()
+        self.monitor_names = filter_nones(to_set(monitor_names)) | network.get_loss_keys()
         self.system = System(network=network,
                              pipeline=pipeline,
-                             traces=to_list(traces),
+                             traces=filter_nones(to_list(traces)),
                              log_steps=log_steps,
                              total_epochs=epochs,
                              train_steps_per_epoch=train_steps_per_epoch,
                              eval_steps_per_epoch=eval_steps_per_epoch,
                              eval_log_steps=eval_log_steps,
                              system_config=self.fe_summary())
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/pytorch/hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/pytorch/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/instance_norm.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/layers/tensorflow/reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/layers/tensorflow/reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/network.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from fastestimator.backend._load_model import load_model
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.op.numpyop import Batch, NumpyOp, RemoveIf, forward_numpyop
 from fastestimator.op.op import get_inputs_by_op, write_outputs_by_op
 from fastestimator.op.tensorop.model.update import UpdateOp
 from fastestimator.op.tensorop.tensorop import TensorOp
 from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
-from fastestimator.util.base_util import NonContext, to_list, warn
+from fastestimator.util.base_util import NonContext, filter_nones, to_list, warn
 from fastestimator.util.traceability_util import trace_model, traceable
 from fastestimator.util.util import Suppressor, detach_tensors, get_batch_size, get_device, get_num_gpus, \
     move_tensors_to_device
 
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 T = TypeVar('T')
 
@@ -65,24 +65,25 @@
     Raises:
         ValueError: Mixed precision settings for all models are not the same.
     """
     def __init__(
         self,
         target_type: str,
         device: Optional[torch.device],
-        ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
+                                                                                Scheduler[NumpyOp]]]] = None
     ) -> None:
-        self.ops = to_list(ops)
+        self.ops = filter_nones(to_list(ops))
         self.target_type = target_type
         self.device = device
         for op in get_current_items(self.ops):
             op.build(framework=self.target_type, device=self.device)
-        self.models = to_list(_collect_models(ops))
-        self.postprocessing = to_list(postprocessing)
+        self.models = to_list(_collect_models(self.ops))
+        self.postprocessing = filter_nones(to_list(postprocessing))
         for pop in self.postprocessing:
             if isinstance(pop, RemoveIf):
                 raise ValueError("Filtering is currently not supported in network post-processing")
             if isinstance(pop, Batch):
                 raise ValueError("Post-processing data is already batched, so Batch Op is not supported here.")
         self._verify_inputs()
         self.effective_inputs = dict()
@@ -305,34 +306,37 @@
         self.load_epoch(mode, epoch, ds_id, warmup=False, eager=True)
         data = to_tensor(data, target_type=self.target_type)
         data, prediction = self.run_step(data)
         self.unload_epoch()
         return {**data, **prediction}
 
 
-def _collect_models(ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]]) -> Set[Model]:
+def _collect_models(
+    ops: Union[None, TensorOp, Scheduler[TensorOp], Iterable[Union[None, TensorOp,
+                                                                   Scheduler[TensorOp]]]]) -> Set[Model]:
     """Collect all model instances from amongst a list of ops.
 
     Args:
         ops: The ops to be searched through.
 
     Returns:
         All of the model instances contained within the `ops`.
     """
     models = set()
-    for op in get_current_items(ops):
+    ops_list = filter_nones(to_list(ops))
+    for op in get_current_items(ops_list):
         models |= op.get_fe_models()
     return models
 
 
 # noinspection PyPep8Naming
 def Network(
-        ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        pops: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp,
-                                                                      Scheduler[NumpyOp]]]] = None) -> BaseNetwork:
+    ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
+    pops: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp, Scheduler[NumpyOp]]]] = None
+) -> BaseNetwork:
     """A function to automatically instantiate the correct Network derived class based on the given `ops`.
 
     Args:
         ops: A collection of Ops defining the graph for this Network. It should contain at least one ModelOp, and all
             models should be either TensorFlow or Pytorch. We currently do not support mixing TensorFlow and Pytorch
             models within the same network.
         pops: Postprocessing Ops. A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been
@@ -342,15 +346,14 @@
     Returns:
         A network instance containing the given `ops`.
 
     Raises:
         AssertionError: If TensorFlow and PyTorch models are mixed, or if no models are provided.
         ValueError: If a model is provided whose type cannot be identified as either TensorFlow or PyTorch.
     """
-    ops = to_list(ops)
     models = _collect_models(ops)
     framework = set()
     model_names = set()
     for model in models:
         # 'Model' and 'model' should not be considered unique in case you are saving on a non-case-sensitive filesystem
         model_names.add(model.model_name.lower())
         if isinstance(model, tf.keras.Model):
@@ -384,16 +387,17 @@
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
 
     """
     device: torch.device
 
     def __init__(
         self,
-        ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
+                                                                                Scheduler[NumpyOp]]]] = None
     ) -> None:
         super().__init__(target_type='torch', device=get_device(), ops=ops, postprocessing=postprocessing)
 
     def load_epoch(self,
                    mode: str,
                    epoch: int,
                    ds_id: str,
@@ -526,16 +530,17 @@
     Args:
         ops: The ops defining the execution graph for this Network.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
     """
     def __init__(
         self,
-        ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
+                                                                                Scheduler[NumpyOp]]]] = None
     ) -> None:
         super().__init__(target_type='tf', device=None, ops=ops, postprocessing=postprocessing)
 
     def load_epoch(self,
                    mode: str,
                    epoch: int,
                    ds_id: str,
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/affine.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/center_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/multivariate.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/multivariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_scale.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/read_mat.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/resize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/rotate.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/multivariate/vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/multivariate/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/numpyop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/autocontrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/binarize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/brightness.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/calibate.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/calibate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/clahe.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/color.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/color_jitter.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/contrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/downscale.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/equalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/expand_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/from_float.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/from_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/image_compression.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/invert_img.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/iso_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/median_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/minmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/motion_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/onehot.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/posterize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_fog.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_gamma.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_rain.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_shadow.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_shapes.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_snow.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/read_image.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/rua.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/sharpness.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/shear_x.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/shear_y.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/solarize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_array.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_float.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_gray.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/to_sepia.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/tokenize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/translate_x.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/translate_y.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/univariate.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/univariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/numpyop/univariate/word_to_id.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/numpyop/univariate/word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/op.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/argmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/augmentation/mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/augmentation/mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/average.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gather.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/fgsm.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/gradient.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/gradient/watch.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/gradient/watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/dice_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/dice_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/focal_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/hinge.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/l1_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/loss/super_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/loss/super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/model.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/model/update.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/model/update.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/permute.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/resize3d.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/tensorop.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/op/tensorop/un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/op/tensorop/un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/pipeline.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 import gc
 import multiprocessing as mp
 import os
 import time
 from copy import deepcopy
 from operator import mul
 from threading import Lock
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union, cast
 
 import numpy as np
 import tensorflow as tf
 from torch.utils.data import DataLoader, Dataset
 
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.dataset.dataloader import FEDataLoader
 from fastestimator.dataset.op_dataset import OpDataset
 from fastestimator.op.numpyop.meta.fuse import Fuse
 from fastestimator.op.numpyop.meta.one_of import OneOf
 from fastestimator.op.numpyop.meta.repeat import Repeat
 from fastestimator.op.numpyop.meta.sometimes import Sometimes
 from fastestimator.op.numpyop.numpyop import Batch, NumpyOp, forward_numpyop
 from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
-from fastestimator.util.base_util import to_list, to_set, warn
+from fastestimator.util.base_util import filter_nones, to_list, to_set, warn
 from fastestimator.util.data import FilteredData
 from fastestimator.util.traceability_util import traceable
 from fastestimator.util.util import cpu_count, get_num_devices
 
 DataSource = TypeVar('DataSource', Dataset, DataLoader, tf.data.Dataset)
 
 
@@ -66,24 +66,30 @@
     ops: List[Union[NumpyOp, Scheduler[NumpyOp]]]
     data: Dict[str, Dict[str, Union[DataSource, Scheduler[DataSource]]]]  # {"mode": {"ds_id": ds}}
 
     def __init__(self,
                  train_data: Union[None,
                                    DataSource,
                                    Scheduler[DataSource],
-                                   Dict[str, Union[DataSource, Scheduler[DataSource]]]] = None,
-                 eval_data: Union[None, DataSource, Scheduler[DataSource], Dict[str, DataSource]] = None,
-                 test_data: Union[None, DataSource, Scheduler[DataSource], Dict[str, DataSource]] = None,
+                                   Dict[str, Union[None, DataSource, Scheduler[DataSource]]]] = None,
+                 eval_data: Union[None,
+                                  DataSource,
+                                  Scheduler[DataSource],
+                                  Dict[str, Union[None, DataSource, Scheduler[DataSource]]]] = None,
+                 test_data: Union[None,
+                                  DataSource,
+                                  Scheduler[DataSource],
+                                  Dict[str, Union[None, DataSource, Scheduler[DataSource]]]] = None,
                  batch_size: Union[None, int, Scheduler[int]] = None,
-                 ops: Union[None, NumpyOp, Scheduler[NumpyOp], List[Union[NumpyOp, Scheduler[NumpyOp]]]] = None,
+                 ops: Union[None, NumpyOp, Scheduler[NumpyOp], List[Union[None, NumpyOp, Scheduler[NumpyOp]]]] = None,
                  num_process: Optional[int] = None):
         data = {x: y for (x, y) in zip(["train", "eval", "test"], [train_data, eval_data, test_data]) if y}
         self.data = self._register_ds_ids(data)
         self.batch_size = batch_size
-        self.ops = to_list(ops)
+        self.ops = filter_nones(to_list(ops))
         if mp.get_start_method(allow_none=True) is None and os.name != 'nt':
             mp.set_start_method('fork')
         self.num_process = num_process if num_process is not None else min(cpu_count(), 32 * get_num_devices())
         if mp.get_start_method(allow_none=True) != 'fork' and self.num_process > 0 and not self.mp_warned:
             warn("Pipeline multiprocessing is disabled. OS must support the 'fork' start method.")
             self.num_process = 0
             self.mp_warned = True
@@ -100,15 +106,16 @@
         self.ctx_ops = []
         self.ctx_batch_info = Batch()
         self.ctx_batch_ops = []
         self.ctx_batch_input_keys = set()
 
     @staticmethod
     def _register_ds_ids(
-        data: Dict[str, Union[DataSource, Scheduler[DataSource], Dict[str, Union[DataSource, Scheduler[DataSource]]]]]
+        data: Dict[str,
+                   Union[DataSource, Scheduler[DataSource], Dict[str, Union[None, DataSource, Scheduler[DataSource]]]]]
     ) -> Dict[str, Dict[str, Union[DataSource, Scheduler[DataSource]]]]:
         """Associate dataset of each mode with a `ds_id`.
 
         Args:
             data: A dictionary with mode as key, dataset as value.
         """
         forbidden_ds_id_chars = {":", "!", ";", "|"}
@@ -116,33 +123,34 @@
             if isinstance(dataset, dict):
                 for ds_name in dataset:
                     assert isinstance(ds_name, str) and len(ds_name) > 0, \
                         "dataset id must be a string, found {}".format(ds_name)
                     assert not any(char in ds_name for char in forbidden_ds_id_chars), \
                         "dataset id should not contain forbidden characters like ':', ';', '!', '|', " + \
                         "found {} in pipeline".format(ds_name)
+                data[mode] = filter_nones(dataset)
             else:
                 # Empty string is special, matches against ops which require '!ds1' but not 'ds1'
                 data[mode] = {"": dataset}
-        return data
+        return cast(Dict[str, Dict[str, Union[DataSource, Scheduler[DataSource]]]], data)
 
     def _verify_inputs(self, **kwargs) -> None:
         """A helper method to ensure that the Pipeline inputs are valid.
 
         Args:
             **kwargs: A collection of variable / value pairs to validate.
 
         Raises:
             AssertionError: If `batch_size`, `ops`, or `num_process` were specified in the absence of a FastEstimator
                 Dataset.
         """
         fe_dataset = False
         for dataset in get_current_items(set(d for ds in self.data.values() for d in ds.values())):
             fe_dataset = self._verify_dataset(dataset, **kwargs) or fe_dataset
-        if not fe_dataset:
+        if self.data and not fe_dataset:  # If the user provided no datasets at all, still let them use ops for infer
             assert kwargs['batch_size'] is None, "Pipeline only supports batch_size with built-in (FE) datasets"
             assert kwargs['ops'] is None, "Pipeline only supports ops with built-in (FE) datasets"
             assert kwargs['num_process'] is None, "Pipeline only support num_process with built-in (FE) datasets"
         # Make sure that the user provides at most 1 Batch Op for a given epoch/mode/ds_id
         batch_ops = []
         schedule_epochs = {1}
         schedule_cycles = set()
@@ -164,17 +172,18 @@
                             schedule_epochs |= {*range(1, 100)}
                         break
         # After m*n steps all possible m and n combinations will be visited
         schedule_cycles = functools.reduce(mul, schedule_cycles, 1)
         # Consider x + m*n epochs for each epoch scheduler x value
         schedule_epochs = sorted({
             epoch
-            for base_epoch in schedule_epochs for epoch in list(range(base_epoch, base_epoch + schedule_cycles))
+            for base_epoch in schedule_epochs
+            for epoch in list(range(base_epoch, base_epoch + schedule_cycles))
         })
-        for mode, id_ds in self.data.items():
+        for mode, id_ds in list(self.data.items()) + [('infer', {'': None})]:
             for ds_id in id_ds.keys():
                 for epoch in schedule_epochs:
                     ops = get_current_items(batch_ops, run_modes=mode, epoch=epoch, ds_id=ds_id)
                     # We have to do an instance check again since the user could technically use a scheduler that has a
                     # Batch Op at one point, but some other Op (or None) at a different point
                     ops = [op for op in ops if isinstance(op, Batch)]
                     assert len(ops) < 2, "You may provide at most 1 batch op for a given epoch/mode/ds_id combination"
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/schedule/schedule.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/golden_section.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/golden_section.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/grid_search.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/search.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/cartesian.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/cartesian.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/heatmap.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/heatmap.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/parallel_coordinate_plot.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/parallel_coordinate_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/vis_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/vis_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/search/visualize/visualize.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/search/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/history.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/log_parse.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/log_parse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/logs/log_plot.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/logs/log_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/summary.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/summary/system.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/summary/system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/nightly_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/nightly_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/test/unittest_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/test/unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/early_stopping.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/adapt/terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/adapt/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/batch_display.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/csv_logger.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/grid_display.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/grid_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/image_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/image_viewer.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/model_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/tensorboard.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/test_report.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/io/traceability.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/io/traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/meta/_per_ds.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/meta/_per_ds.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/accuracy.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/auc.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/auc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/bleu_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/calibration_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/dice.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/f1_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/mcc.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/precision.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/metric/recall.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/metric/recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/trace.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/eigen_cam.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/grad_cam.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/grad_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/label_tracker.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/trace/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/trace/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,34 @@
                                             submod_attrs={'data': ['Data'],
                                                           'img_data': ['ImageDisplay', 'BatchDisplay', 'GridDisplay'],
                                                           'latex_util': ['AdjustBox', 'Center', 'ContainerList',
                                                                          'HrefFEID', 'PyContainer', 'Verbatim'],
                                                           'traceability_util': ['FeSplitSummary', 'trace_model',
                                                                                 'traceable'],
                                                           'base_util': ['to_set', 'to_list', 'param_to_range',
-                                                                        'NonContext', 'LogSplicer',
+                                                                        'NonContext', 'LogSplicer', 'IfElse',
                                                                         'prettify_metric_name', 'strip_suffix',
                                                                         'strip_prefix', 'get_type', 'check_io_names',
-                                                                        'parse_modes', 'check_ds_id', 'is_number',
-                                                                        'DefaultKeyDict', 'FEID', 'Flag', 'in_notebook',
-                                                                        'get_shape', 'get_colors', 'list_files',
-                                                                        'warn'],
-                                                          'util': ['Suppressor', 'Timer', 'cpu_count', 'draw', 'get_batch_size',
-                                                                   'get_device', 'get_num_devices', 'get_num_gpus',
-                                                                   'pad_batch', 'pad_data', 'to_number', 'move_tensors_to_device',
+                                                                        'filter_nones', 'parse_modes', 'check_ds_id',
+                                                                        'is_number', 'DefaultKeyDict', 'FEID', 'Flag',
+                                                                        'in_notebook', 'get_shape', 'get_colors',
+                                                                        'list_files', 'warn'],
+                                                          'util': ['Suppressor', 'Timer', 'cpu_count', 'draw',
+                                                                   'get_batch_size', 'get_device', 'get_num_devices',
+                                                                   'get_num_gpus', 'pad_batch', 'pad_data',
+                                                                   'to_number', 'move_tensors_to_device',
                                                                    'detach_tensors'],
                                                           'cli_util': ['parse_string_to_python'],
                                                           'wget_util': ['bar_custom', 'callback_progress']
                                                           })
 
 if TYPE_CHECKING:
-    from fastestimator.util.base_util import FEID, DefaultKeyDict, Flag, LogSplicer, NonContext, check_ds_id, \
-        check_io_names, get_colors, get_shape, get_type, in_notebook, is_number, list_files, param_to_range, \
-        parse_modes, prettify_metric_name, strip_prefix, strip_suffix, to_list, to_set, warn
+    from fastestimator.util.base_util import FEID, DefaultKeyDict, Flag, IfElse, LogSplicer, NonContext, check_ds_id, \
+        check_io_names, filter_nones, get_colors, get_shape, get_type, in_notebook, is_number, list_files, \
+        param_to_range, parse_modes, prettify_metric_name, strip_prefix, strip_suffix, to_list, to_set, warn
     from fastestimator.util.cli_util import parse_string_to_python
     from fastestimator.util.data import Data
     from fastestimator.util.img_data import BatchDisplay, GridDisplay, ImageDisplay
     from fastestimator.util.latex_util import AdjustBox, Center, ContainerList, HrefFEID, PyContainer, Verbatim
     from fastestimator.util.traceability_util import FeSplitSummary, trace_model, traceable
     from fastestimator.util.util import Suppressor, Timer, cpu_count, detach_tensors, draw, get_batch_size, \
         get_device, get_num_devices, get_num_gpus, move_tensors_to_device, pad_batch, pad_data, to_number
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/base_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/base_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 import colorsys
+import itertools
 import os
 import re
 import string
 import sys
-from typing import Any, Callable, Dict, Iterable, KeysView, List, Literal, Optional, Set, TextIO, Tuple, Type, \
-    TypeVar, Union, overload
+from typing import Any, Callable, Collection, Dict, Iterable, KeysView, List, Literal, Mapping, Optional, Set, TextIO, \
+    Tuple, Type, TypeVar, Union, overload
 
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 from plotly.graph_objs import Figure
 
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 
 KT = TypeVar('KT')  # Key type.
@@ -123,14 +124,108 @@
         if isinstance(data, (tuple, set)):
             data = list(data)
         else:
             data = [data]
     return data
 
 
+@overload
+def filter_nones(ins: Set[Union[VT, None]]) -> Set[VT]:
+    ...
+
+
+@overload
+def filter_nones(ins: Tuple[Union[VT, None], ...]) -> Tuple[VT]:
+    ...
+
+
+@overload
+def filter_nones(ins: List[Union[VT, None]]) -> List[VT]:
+    ...
+
+
+@overload
+def filter_nones(ins: Mapping[KT, Union[VT, None]]) -> Dict[KT, VT]:
+    ...
+
+
+def filter_nones(ins: Collection) -> Collection:
+    """Remove any None values from the input collection.
+
+    For dictionaries this removes keys whose values are None.
+
+    Args:
+        ins: The collection to be filtered.
+
+    Returns:
+        The filtered collection.
+    """
+    if isinstance(ins, dict):
+        filtered = {k: v for k, v in ins.items() if v is not None}
+        return filtered
+    filtered = itertools.filterfalse(lambda item: not item, ins)
+    if isinstance(ins, set):
+        return set(filtered)
+    if isinstance(ins, tuple):
+        return tuple(filtered)
+    else:
+        return list(filtered)
+
+
+@overload
+def IfElse(cond: Literal[True], y: KT, n: VT = None) -> KT:
+    ...
+
+
+@overload
+def IfElse(cond: Literal[False], y: KT, n: VT = None) -> VT:
+    ...
+
+
+def IfElse(cond: bool, y: KT, n: VT = None) -> Union[KT, VT]:
+    """This is a helper function to make code look cleaner while using config files.
+
+    One mock example where this might be useful:
+
+    ```python
+    from fastestimator.util import IfElse
+    extra_augs = True
+    ...
+
+    fe.Pipeline(...,
+                ops=[...,
+                     IfElse(extra_augs, RandomJitter(image_in="x", image_out="x"))
+                     ]
+                )
+    ```
+
+    If instantiating the objects in each branch is expensive, you may want to defer that until later by converting your
+    constructors to lambda functions and then invoking the functions after the return from the IfElse:
+
+    ```python
+    from fastestimator.util import IfElse
+    use_lots_of_data = True
+    ...
+
+    train_data = IfElse(use_lots_of_data, lambda: BigInMemoryDataset(), lambda: SmallInMemoryDataset())()
+    ```
+
+    Args:
+        cond: Which branch to return.
+        y: The return value when `cond` is True.
+        n: The return value when `cond` is False.
+
+    Returns:
+        The value according to the given cond.
+    """
+    if cond:
+        return y
+    return n
+
+
 def param_to_range(
         data: Union[int, float, Tuple[int, int], Tuple[float, float]]) -> Union[Tuple[int, int], Tuple[float, float]]:
     """Convert a single int or float value to a tuple signifying a range.
 
     ```python
     x = fe.util.param_to_tuple(7)  # (-7, 7)
     x = fe.util.param_to_tuple([7, 8])  # (7,8))
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/cli_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/data.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/google_download_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/google_download_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/img_data.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/latex_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/latex_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/traceability_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,28 +140,35 @@
         if self.show_if_exception:
             self.fake = os.open(self.stash_name, os.O_RDWR)
         else:
             self.fake = os.open(os.devnull, os.O_RDWR)
         self.reals = [os.dup(1), os.dup(2)]  # [stdout, stderr]
         os.dup2(self.fake, 1)
         os.dup2(self.fake, 2)
+        # This avoids "OSError: [WinError 6] The handle is invalid" while logging tensorflow information in windows
+        for handler in tf.get_logger().handlers:
+            handler.setStream(sys.stderr)
         if self.allow_pyprint:
             tf.print = _custom_tf_print
 
     def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
         # If there was an error, display any print messages
         if exc[0] is not None and self.show_if_exception and not isinstance(exc[1],
                                                                             (StopIteration, StopAsyncIteration)):
             for line in open(self.stash_name):
                 os.write(self.reals[0], line.encode('utf-8'))
         # Set the print pointers back
         os.dup2(self.reals[0], 1)
         os.dup2(self.reals[1], 2)
         # Set the python pointers back too
         sys.stdout, sys.stderr = self.py_reals[0], self.py_reals[1]
+
+        for handler in tf.get_logger().handlers:
+            handler.setStream(sys.stderr)
+
         # Clean up the descriptors
         for fd in self.reals:
             os.close(fd)
         os.close(self.fake)
         if self.show_if_exception:
             # Clear the file
             open(self.stash_name, 'w').close()
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/util/wget_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/util/wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202306071349
+Version: 1.6.0.dev202306092229
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/SOURCES.txt` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -332,14 +332,15 @@
 ./fastestimator/trace/metric/recall.py
 ./fastestimator/trace/xai/__init__.py
 ./fastestimator/trace/xai/eigen_cam.py
 ./fastestimator/trace/xai/grad_cam.py
 ./fastestimator/trace/xai/instance_tracker.py
 ./fastestimator/trace/xai/label_tracker.py
 ./fastestimator/trace/xai/saliency.py
+./fastestimator/types/__init__.py
 ./fastestimator/util/__init__.py
 ./fastestimator/util/base_util.py
 ./fastestimator/util/cli_util.py
 ./fastestimator/util/data.py
 ./fastestimator/util/google_download_util.py
 ./fastestimator/util/img_data.py
 ./fastestimator/util/latex_util.py
@@ -665,14 +666,16 @@
 ./test/PR_test/unit_test/summary/logs/test_metrics.py
 ./test/PR_test/unit_test/test/__init__.py
 ./test/PR_test/unit_test/test/test_unittest_util.py
 ./test/PR_test/unit_test/trace/__init__.py
 ./test/PR_test/unit_test/trace/metric/__init__.py
 ./test/PR_test/unit_test/trace/metric/test_auc_score.py
 ./test/PR_test/unit_test/trace/metric/test_bleu_score.py
+./test/PR_test/unit_test/types/__init__.py
+./test/PR_test/unit_test/types/test_types.py
 ./test/PR_test/unit_test/util/__init__.py
 ./test/PR_test/unit_test/util/test_data.py
 ./test/PR_test/unit_test/util/test_traceability_util.py
 ./test/PR_test/unit_test/util/test_util.py
 ./test/PR_test/unit_test/util/test_wget_util.py
 ./test/PR_test/unit_test/xai/__init__.py
 ./test/PR_test/unit_test/xai/test_saliency.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/fastestimator_nightly.egg-info/requires.txt` & `fastestimator-nightly-1.6.0.dev202306092229/fastestimator_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/setup.py` & `fastestimator-nightly-1.6.0.dev202306092229/setup.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_get_lr.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_save_model_load_model.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_save_model_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_set_lr.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/backend/test_update_model.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/backend/test_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/test_main.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/cli/test_train.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/cli/test_train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/test_modelop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/test_modelop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/model/test_updateop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/model/test_updateop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_average.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_arc.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_arc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/schedule/test_schedule.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/schedule/test_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/search/visualize/test_visualize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/search/visualize/test_visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/summary/test_system.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/summary/test_system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_estimator.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_network.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/test_pipeline.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_early_stopping.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_batch_display.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_csv_logger.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_image_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_image_viewer.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_model_saver.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_tensorboard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_test_report.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/io/test_traceability.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/io/test_traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_accuracy.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_calibration_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_dice.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_f1_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_mcc.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_precision.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/metric/test_recall.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/metric/test_recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_eval_essential.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_eval_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_logger.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_test_essential.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_test_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_trace.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/test_train_essential.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/test_train_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/test_instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/test_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/trace/xai/test_label_tracker.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/trace/xai/test_label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_img_data.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/integration_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/integration_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_unet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_abs.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_cast.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_check_nan.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_concat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_dice_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_exp.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_gather.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_iwd.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_lambertw.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_matmul.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_maximum.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_ones_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_percentile.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_permute.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_pow.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_roll.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_sign.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_squeeze.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_shape.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_to_type.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_watch.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_where.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/backend/test_zscore.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/backend/test_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/cli/test_cli_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_combine_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_combine_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         sample = combined_ds[12]
         self.assertEqual(type(sample), dict)
         self.assertEqual(list(sample.keys()), ["x", "y"])
 
     def test_error_dataset(self):
         with self.assertRaises(AssertionError) as err_msg:
             fe.dataset.CombinedDataset([])
-        self.assertEqual(
-            "datasets should not be an empty iterable", str(err_msg.exception)
-        )
+        self.assertEqual("datasets should not be an empty iterable", str(err_msg.exception))
 
     def test_invalid_index_dataset(self):
         ds1 = GeneratorDataset(generator=inputs(), samples_per_epoch=10)
         ds2 = GeneratorDataset(generator=inputs(), samples_per_epoch=10)
         combined_ds = fe.dataset.CombinedDataset(datasets=[ds1, ds2])
 
         with self.assertRaises(IndexError) as err_msg:
@@ -62,17 +60,15 @@
         )
 
     def test_invalid_keys(self):
         ds1 = GeneratorDataset(generator=inputs(), samples_per_epoch=10)
         ds2 = GeneratorDataset(generator=inputs2(), samples_per_epoch=5)
         with self.assertRaises(KeyError) as err_msg:
             combined_ds = fe.dataset.CombinedDataset(datasets=[ds1, ds2])
-        self.assertEqual(
-            "All datasets should have same keys.", err_msg.exception.args[0]
-        )
+        self.assertEqual("All datasets should have the same keys.", err_msg.exception.args[0])
 
     def test_invalid_return_type_dataset(self):
         ds1 = GeneratorDataset(generator=inputs(), samples_per_epoch=10)
         ds2 = GeneratorDataset(generator=inputs3(), samples_per_epoch=5)
         with self.assertRaises(AssertionError) as err_msg:
             combined_ds = fe.dataset.CombinedDataset(datasets=[ds1, ds2])
         self.assertEqual(
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_data.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/pytorch/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/pytorch/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/loss/test_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/loss/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/test_numpyop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/test_numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_color.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/tensorop/test_tensorop.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/tensorop/test_tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_golden_section_search.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_golden_section_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_grid_search.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/search/test_search.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/search/test_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/logs/test_metrics.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/summary/test_summary.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/summary/test_summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/test/test_unittest_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/test/test_unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/test_auc_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/test_auc_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/trace/metric/test_bleu_score.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/trace/metric/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_data.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,36 @@
         self.assertEqual(x, {None, "2", (3, 4)})
 
     def test_to_set_input_set(self):
         x = fe.util.to_set({3, 4})
         self.assertEqual(x, {3, 4})
 
 
+class TestFilterNones(unittest.TestCase):
+    def test_with_list(self):
+        x = fe.util.filter_nones([1, None, "A", None, 0.9])
+        self.assertTrue(isinstance(x, list))
+        self.assertListEqual(x, [1, "A", 0.9])
+
+    def test_with_tuple(self):
+        x = fe.util.filter_nones((1, None, "A", None, 0.9))
+        self.assertTrue(isinstance(x, tuple))
+        self.assertTupleEqual(x, (1, "A", 0.9))
+
+    def test_with_set(self):
+        x = fe.util.filter_nones({1, None, "A", None, 0.9})
+        self.assertTrue(isinstance(x, set))
+        self.assertSetEqual(x, {1, "A", 0.9})
+
+    def test_with_dict(self):
+        x = fe.util.filter_nones({'a': 1, 'b': None, 'c': "A", 'd': None, 'e': 0.9})
+        self.assertTrue(isinstance(x, dict))
+        self.assertDictEqual(x, {'a': 1, 'c': "A", 'e': 0.9})
+
+
 class TestParamToRange(unittest.TestCase):
     def test_param_to_range_int(self):
         x = fe.util.param_to_range(3)
         self.assertEqual(x, (-3, 3))
 
     def test_param_to_range_float(self):
         x = fe.util.param_to_range(2.3)
```

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/util/test_wget_util.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/util/test_wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/PR_test/unit_test/xai/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/PR_test/unit_test/xai/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306071349/test/run_pr_test.py` & `fastestimator-nightly-1.6.0.dev202306092229/test/run_pr_test.py`

 * *Files identical despite different names*

