# Comparing `tmp/jittor-1.3.7.9.tar.gz` & `tmp/jittor-1.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jittor-1.3.7.9.tar", last modified: Tue Apr  4 15:15:59 2023, max compression
+gzip compressed data, was "jittor-1.3.8.1.tar", last modified: Fri Jun  9 17:02:51 2023, max compression
```

## Comparing `jittor-1.3.7.9.tar` & `jittor-1.3.8.1.tar`

### file list

```diff
@@ -1,780 +1,788 @@
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.473381 jittor-1.3.7.9/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11613 2022-04-22 13:00:57.000000 jittor-1.3.7.9/LICENSE.txt
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       88 2021-07-31 06:19:50.000000 jittor-1.3.7.9/MANIFEST.in
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-04-04 15:15:59.473381 jittor-1.3.7.9/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11809 2023-03-31 13:28:11.000000 jittor-1.3.7.9/README.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.202548 jittor-1.3.7.9/python/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.213381 jittor-1.3.7.9/python/jittor/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    66631 2023-04-04 14:16:52.000000 jittor-1.3.7.9/python/jittor/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   244353 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/__init__.pyi
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6545 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/attention.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.213381 jittor-1.3.7.9/python/jittor/ccl/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       86 2022-12-02 14:36:01.000000 jittor-1.3.7.9/python/jittor/ccl/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8866 2022-12-02 14:36:01.000000 jittor-1.3.7.9/python/jittor/ccl/ccl_2d.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10077 2022-12-02 14:36:01.000000 jittor-1.3.7.9/python/jittor/ccl/ccl_3d.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11051 2022-12-02 14:36:01.000000 jittor-1.3.7.9/python/jittor/ccl/ccl_link.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    24870 2023-04-02 23:46:15.000000 jittor-1.3.7.9/python/jittor/compile_extern.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    53975 2023-04-04 10:43:23.000000 jittor-1.3.7.9/python/jittor/compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9039 2023-03-20 07:53:05.000000 jittor-1.3.7.9/python/jittor/contrib.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/dataset/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      201 2023-01-07 09:03:52.000000 jittor-1.3.7.9/python/jittor/dataset/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6439 2021-06-16 12:20:56.000000 jittor-1.3.7.9/python/jittor/dataset/cifar.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    26798 2023-01-07 09:00:29.000000 jittor-1.3.7.9/python/jittor/dataset/dataset.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8320 2021-09-04 06:27:26.000000 jittor-1.3.7.9/python/jittor/dataset/mnist.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3323 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/dataset/sampler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2326 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/dataset/utils.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2410 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/dataset/voc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/demo/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3591 2022-04-04 06:54:03.000000 jittor-1.3.7.9/python/jittor/demo/simple_cgan.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15663 2023-01-06 08:38:43.000000 jittor-1.3.7.9/python/jittor/depthwise_conv.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5492 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/distributions.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/einops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      262 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8494 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/_backends.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    33864 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/einops.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/einops/experimental/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)        0 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/experimental/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15167 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/experimental/indexing.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/einops/layers/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2933 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/layers/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8720 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/layers/_einmix.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2057 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/layers/jittor.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6848 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/einops/parsing.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/acl/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2379 2022-10-26 06:26:41.000000 jittor-1.3.7.9/python/jittor/extern/acl/acl_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    14964 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/acl/acl_error_code.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11204 2022-10-26 06:29:43.000000 jittor-1.3.7.9/python/jittor/extern/acl/acl_jittor.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      644 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/acl/acl_jittor.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/corex/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3816 2023-01-06 08:38:43.000000 jittor-1.3.7.9/python/jittor/extern/corex/corex_compiler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/cub/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/cuda/cub/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9072 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/inc/cub_test.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3913 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      911 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3424 2023-04-01 10:13:42.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      931 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4891 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      809 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1144 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      624 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_test_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3679 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_where_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1146 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_where_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      973 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.224214 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4418 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      905 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5393 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      953 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3998 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      771 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      879 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      639 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12200 2021-07-26 07:27:48.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      990 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1606 2020-12-03 05:10:19.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/helper_cublas.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4906 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      842 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11561 2023-04-01 22:35:11.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1143 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11327 2023-04-01 22:35:17.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1151 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11535 2023-04-01 22:35:22.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1029 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12570 2023-04-01 22:34:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1116 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12027 2023-04-01 22:35:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1121 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12423 2023-04-01 22:37:36.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1061 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8286 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1470 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9384 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1375 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1093 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      628 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    39400 2021-12-30 07:13:56.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2914 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1070 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      161 2021-07-26 07:24:52.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/helper_cudnn.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6280 2022-03-30 06:36:09.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/inc/cufft_utils.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      717 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3201 2022-07-31 12:01:49.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      821 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1002 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/curand/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.235048 jittor-1.3.7.9/python/jittor/extern/cuda/curand/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      632 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/curand/inc/curand_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/curand/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1632 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/curand/ops/curand_random_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      759 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/curand/ops/curand_random_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/curand/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1078 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/curand/src/curand_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1933 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/curand/src/helper_curand.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1052 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      629 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3823 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      775 2021-04-15 10:38:17.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      888 2021-11-01 03:42:19.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      559 2021-07-26 07:18:24.000000 jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      588 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/fp16_dev.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5639 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/fp16_emu.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12641 2022-10-25 03:25:21.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_cuda.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1173 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_functions.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    27554 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_image.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    33798 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_string.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    14855 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_timer.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      656 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1771 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      782 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1838 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      808 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1877 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      799 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3785 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      644 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1923 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/cuda/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1323 2021-07-26 07:15:57.000000 jittor-1.3.7.9/python/jittor/extern/cuda/src/fp16_dev.cu
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5303 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/extern/cuda/src/fp16_emu.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11787 2021-07-26 07:13:54.000000 jittor-1.3.7.9/python/jittor/extern/cuda/src/helper_cuda.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.245881 jittor-1.3.7.9/python/jittor/extern/llvm/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15734 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/mkl/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/extern/mkl/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    36034 2022-03-22 14:48:20.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8788 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1043 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8850 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1048 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7552 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1035 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2210 2022-06-04 15:11:34.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_matmul_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      762 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_matmul_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      810 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      595 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.191714 jittor-1.3.7.9/python/jittor/extern/mpi/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/extern/mpi/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2014 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/inc/mpi_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/extern/mpi/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2899 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1110 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2222 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1028 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_broadcast_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2989 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1171 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1102 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      641 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/extern/mpi/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3452 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/extern/mpi/src/mpi_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/extern/rocm/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   115033 2022-08-09 11:21:18.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_cache.tar.gz
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6235 2022-10-26 06:26:28.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1712 2022-08-09 11:21:18.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_config.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      497 2022-08-09 11:21:18.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_config.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      538 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_jittor.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6598 2022-08-09 11:21:18.000000 jittor-1.3.7.9/python/jittor/extern/rocm/rocm_wrapper.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    23687 2023-03-20 07:29:07.000000 jittor-1.3.7.9/python/jittor/init.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1715 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/init_cupy.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    16949 2023-03-20 10:37:35.000000 jittor-1.3.7.9/python/jittor/linalg.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/loss3d/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      105 2021-06-30 08:15:49.000000 jittor-1.3.7.9/python/jittor/loss3d/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5553 2021-06-30 08:15:49.000000 jittor-1.3.7.9/python/jittor/loss3d/chamfer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    16008 2021-06-30 08:15:49.000000 jittor-1.3.7.9/python/jittor/loss3d/emd.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7936 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/lr_scheduler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/math_util/
--rw-r--r--   0 cjld      (1000) cjld      (1000)       26 2023-03-31 05:12:08.000000 jittor-1.3.7.9/python/jittor/math_util/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12763 2023-03-31 05:12:08.000000 jittor-1.3.7.9/python/jittor/math_util/gamma.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    74939 2023-04-01 10:13:35.000000 jittor-1.3.7.9/python/jittor/misc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.256714 jittor-1.3.7.9/python/jittor/models/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      513 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/models/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2246 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/alexnet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6745 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/densenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6328 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/googlenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11821 2022-04-04 06:54:03.000000 jittor-1.3.7.9/python/jittor/models/inception.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4821 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/mnasnet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4602 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/mobilenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8032 2021-10-19 11:51:01.000000 jittor-1.3.7.9/python/jittor/models/res2net.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9657 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/resnet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5575 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/shufflenetv2.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4028 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/squeezenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3711 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/models/vgg.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)   115470 2023-04-03 04:35:24.000000 jittor-1.3.7.9/python/jittor/nn.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.267548 jittor-1.3.7.9/python/jittor/notebook/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.267548 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      297 2021-07-14 13:51:52.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/README.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   243006 2021-07-14 13:51:52.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/mnist.png
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5047 2021-07-14 13:51:52.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    29117 2021-07-14 13:51:52.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    62291 2022-03-15 13:17:00.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   136962 2022-03-15 13:17:00.000000 jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6314 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3487 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6752 2022-04-04 06:54:03.000000 jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/LSGAN.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7897 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/LSGAN.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/LSGAN.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      238 2022-03-15 13:17:00.000000 jittor-1.3.7.9/python/jittor/notebook/__main__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1243 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/basics.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1250 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/basics.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2111 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/basics.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2232 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/custom_op.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2249 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/custom_op.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2760 2021-07-16 06:09:15.000000 jittor-1.3.7.9/python/jittor/notebook/custom_op.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1996 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/example.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2152 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/example.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3099 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/example.src.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.267548 jittor-1.3.7.9/python/jittor/notebook/figs/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    41082 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/figs/mop.svg
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2203 2022-03-22 14:48:20.000000 jittor-1.3.7.9/python/jittor/notebook/md_to_ipynb.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7817 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/meta_op.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8068 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/meta_op.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10843 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/meta_op.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      235 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/profiler.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      264 2021-10-11 05:54:17.000000 jittor-1.3.7.9/python/jittor/notebook/profiler.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      459 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/notebook/profiler.src.md
--rw-r--r--   0 cjld      (1000) cjld      (1000)    18593 2023-03-22 11:47:26.000000 jittor-1.3.7.9/python/jittor/optim.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.267548 jittor-1.3.7.9/python/jittor/other/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4389 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/other/code_softmax.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    29598 2022-10-19 09:11:59.000000 jittor-1.3.7.9/python/jittor/pool.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    34612 2023-03-23 17:47:01.000000 jittor-1.3.7.9/python/jittor/pyjt_compiler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.278381 jittor-1.3.7.9/python/jittor/script/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1464 2021-05-12 08:13:24.000000 jittor-1.3.7.9/python/jittor/script/Dockerfile_cuda11
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      890 2021-06-19 09:21:11.000000 jittor-1.3.7.9/python/jittor/script/build_aarch64_mkl.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      893 2021-05-04 00:57:17.000000 jittor-1.3.7.9/python/jittor/script/converter_server.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4134 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/script/inference_perf.py
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     2265 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/script/install.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2543 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/script/install_llvm.sh
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)      632 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/script/install_mkl.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1569 2022-03-15 13:17:00.000000 jittor-1.3.7.9/python/jittor/script/make_doc.py
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     4359 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/script/tmpi
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)      144 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/script/update.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1759 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/sparse.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.289214 jittor-1.3.7.9/python/jittor/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1326 2023-04-01 05:52:20.000000 jittor-1.3.7.9/python/jittor/src/common.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1056 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/core.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1573 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/event_queue.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2392 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/event_queue.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    26798 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/executor.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1043 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/executor.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8249 2022-11-16 06:44:35.000000 jittor-1.3.7.9/python/jittor/src/fused_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1936 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/fused_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      643 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/fuser.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9857 2023-04-03 03:54:46.000000 jittor-1.3.7.9/python/jittor/src/grad.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      712 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/grad.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5820 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/graph.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4668 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/graph.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2730 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/init.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1091 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/init.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9383 2022-10-25 06:56:02.000000 jittor-1.3.7.9/python/jittor/src/jit_compiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      652 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/jit_compiler.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3262 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/jit_key.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7600 2022-10-05 08:12:58.000000 jittor-1.3.7.9/python/jittor/src/jit_key.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2031 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/lock.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      864 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/lock.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.289214 jittor-1.3.7.9/python/jittor/src/mem/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.300048 jittor-1.3.7.9/python/jittor/src/mem/allocator/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1188 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/aligned_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      779 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/aligned_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1461 2023-04-01 01:00:45.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_device_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      805 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_device_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1107 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_dual_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4172 2022-10-25 03:39:22.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_dual_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1087 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_host_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      802 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_host_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1190 2022-06-04 15:02:56.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_managed_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      856 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_managed_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1501 2022-08-13 11:48:55.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/foreign_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      948 2022-08-13 11:14:01.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/foreign_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1127 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/nfef_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1000 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/nfef_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9101 2023-04-03 03:42:16.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/sfrl_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3937 2023-03-31 22:56:13.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/sfrl_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1781 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/stat_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1071 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/stat_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3765 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/temp_allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2234 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator/temp_allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5001 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2237 2023-04-01 00:56:39.000000 jittor-1.3.7.9/python/jittor/src/mem/allocator.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11462 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/mem/mem_info.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1019 2023-04-01 09:49:49.000000 jittor-1.3.7.9/python/jittor/src/mem/mem_info.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8532 2023-04-04 14:34:50.000000 jittor-1.3.7.9/python/jittor/src/mem/swap.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2327 2023-04-01 10:59:22.000000 jittor-1.3.7.9/python/jittor/src/mem/swap.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6090 2023-04-03 01:34:16.000000 jittor-1.3.7.9/python/jittor/src/memory_profiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1417 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/memory_profiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.300048 jittor-1.3.7.9/python/jittor/src/misc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      485 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cpu_atomic.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1820 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cpu_atomic.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2362 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cpu_math.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      490 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cpu_math.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cstr.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5980 2023-03-31 10:39:36.000000 jittor-1.3.7.9/python/jittor/src/misc/cuda_atomic.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2794 2022-10-27 05:36:22.000000 jittor-1.3.7.9/python/jittor/src/misc/cuda_flags.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1142 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/cuda_flags.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2191 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/src/misc/cuda_limits.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/deleter.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2538 2022-05-28 06:19:44.000000 jittor-1.3.7.9/python/jittor/src/misc/fast_shared_ptr.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1000 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/hash.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      864 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/intrin.h
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)   326707 2023-03-30 05:25:05.000000 jittor-1.3.7.9/python/jittor/src/misc/miniz.cc
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)    69968 2023-04-01 02:27:50.000000 jittor-1.3.7.9/python/jittor/src/misc/miniz.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2519 2023-03-22 11:47:26.000000 jittor-1.3.7.9/python/jittor/src/misc/nan_checker.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2224 2023-03-30 09:57:02.000000 jittor-1.3.7.9/python/jittor/src/misc/nan_checker.cu
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      403 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/nan_checker.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5898 2022-10-05 08:50:12.000000 jittor-1.3.7.9/python/jittor/src/misc/nano_string.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7615 2023-03-30 13:33:51.000000 jittor-1.3.7.9/python/jittor/src/misc/nano_string.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9048 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/misc/nano_vector.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3368 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/ring_buffer.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6868 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/ring_buffer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1801 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/stack_vector.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1503 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/misc/string_view_map.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7512 2023-04-03 01:34:41.000000 jittor-1.3.7.9/python/jittor/src/node.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1902 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/numpy_func.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9371 2023-04-03 04:42:28.000000 jittor-1.3.7.9/python/jittor/src/op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2828 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    43093 2022-10-05 08:33:49.000000 jittor-1.3.7.9/python/jittor/src/op_compiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1766 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/op_compiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.321714 jittor-1.3.7.9/python/jittor/src/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7467 2022-09-01 14:50:47.000000 jittor-1.3.7.9/python/jittor/src/ops/arg_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1761 2022-08-13 06:08:14.000000 jittor-1.3.7.9/python/jittor/src/ops/arg_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6273 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/argsort_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2167 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/argsort_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4035 2023-04-01 10:14:29.000000 jittor-1.3.7.9/python/jittor/src/ops/array_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1098 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/array_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    14979 2023-03-30 12:29:34.000000 jittor-1.3.7.9/python/jittor/src/ops/binary_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      727 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/binary_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6900 2023-03-30 12:22:23.000000 jittor-1.3.7.9/python/jittor/src/ops/broadcast_to_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2794 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/broadcast_to_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3650 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/candidate_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1945 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/candidate_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1211 2022-05-11 09:29:38.000000 jittor-1.3.7.9/python/jittor/src/ops/clone_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      715 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/clone_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8685 2022-11-29 05:26:09.000000 jittor-1.3.7.9/python/jittor/src/ops/code_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10232 2022-11-29 05:32:10.000000 jittor-1.3.7.9/python/jittor/src/ops/code_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1425 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/copy_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      694 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/copy_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      685 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/empty_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      607 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/empty_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5104 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/fetch_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1771 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/fetch_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3766 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/fuse_transpose_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      774 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/fuse_transpose_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    19861 2022-12-05 04:48:44.000000 jittor-1.3.7.9/python/jittor/src/ops/getitem_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1555 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/getitem_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2724 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/index_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1986 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/src/ops/index_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5542 2022-04-23 08:12:13.000000 jittor-1.3.7.9/python/jittor/src/ops/numpy_code_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3394 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/numpy_code_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1508 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/op_register.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1544 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/op_register.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1577 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/op_utils.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2072 2023-03-30 12:21:00.000000 jittor-1.3.7.9/python/jittor/src/ops/random_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      686 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/random_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11807 2023-03-30 12:30:04.000000 jittor-1.3.7.9/python/jittor/src/ops/reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1019 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5836 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/reindex_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4093 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/reindex_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5603 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/reindex_reduce_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3610 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/reindex_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2069 2022-10-04 08:05:24.000000 jittor-1.3.7.9/python/jittor/src/ops/reshape_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1536 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/reshape_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1615 2023-03-31 12:13:44.000000 jittor-1.3.7.9/python/jittor/src/ops/safe_clip_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1008 2023-01-06 11:20:14.000000 jittor-1.3.7.9/python/jittor/src/ops/safe_clip_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12583 2022-12-04 13:13:35.000000 jittor-1.3.7.9/python/jittor/src/ops/setitem_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1130 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/setitem_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2984 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/tape_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1897 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/tape_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3745 2023-03-30 12:45:31.000000 jittor-1.3.7.9/python/jittor/src/ops/ternary_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      735 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/ternary_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3808 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/ops/transpose_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      761 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/transpose_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    26784 2023-03-30 12:45:19.000000 jittor-1.3.7.9/python/jittor/src/ops/unary_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      742 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/unary_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8196 2022-11-04 15:00:07.000000 jittor-1.3.7.9/python/jittor/src/ops/where_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1232 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/ops/where_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.332548 jittor-1.3.7.9/python/jittor/src/opt/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    38841 2022-06-23 13:14:46.000000 jittor-1.3.7.9/python/jittor/src/opt/expr.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5751 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/expr.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.332548 jittor-1.3.7.9/python/jittor/src/opt/gopt/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5511 2022-12-05 04:53:06.000000 jittor-1.3.7.9/python/jittor/src/opt/gopt/setitem_gopt.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3084 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/jit_searcher.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      748 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/jit_searcher.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    35269 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/kernel_ir.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8192 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/kernel_ir.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.354214 jittor-1.3.7.9/python/jittor/src/opt/pass/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2071 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/assume_aligned_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      572 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/assume_aligned_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      613 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/atomic_tuner_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6886 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/check_cache_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      613 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/check_cache_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1494 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/compile_shapes_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      572 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/compile_shapes_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1644 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/const_var_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      562 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/const_var_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1391 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/expand_empty_block_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      582 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/expand_empty_block_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6960 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/fake_main_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      557 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/fake_main_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3415 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/float_atomic_fix_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      590 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/float_atomic_fix_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1480 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/insert_profile_loop_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      585 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/insert_profile_loop_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4427 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/loop_to_func_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      564 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/loop_to_func_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12889 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/loop_var_analyze_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/loop_var_analyze_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1246 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/mark_raw_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      554 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/mark_raw_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2283 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      560 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6195 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_var_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      570 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_var_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      556 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/parallel_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      680 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      732 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1490 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/remove_intermediate_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      587 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/remove_intermediate_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      897 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/remove_loop_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      620 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/remove_loop_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      633 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/rename_loop_index_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      579 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/rename_loop_index_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2306 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/reorder_loop_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      610 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/reorder_loop_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3452 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/replace_for_num_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      868 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/replace_for_num_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5910 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/restride_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      556 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/restride_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      574 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/shared_reduce_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      604 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/solve_conflict_define_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      591 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/solve_conflict_define_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1362 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/split_loop_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      634 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/split_loop_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3719 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/unroll_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      562 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/unroll_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      944 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/use_movnt_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      610 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/use_movnt_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3411 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/vectorize_pass.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      559 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass/vectorize_pass.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4356 2022-09-15 15:23:50.000000 jittor-1.3.7.9/python/jittor/src/opt/pass_manager.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1954 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/pass_manager.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.354214 jittor-1.3.7.9/python/jittor/src/opt/tuner/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2242 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/broadcast_tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      670 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/broadcast_tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    16851 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/conv_tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      692 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/conv_tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4058 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/matmul_tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      622 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/matmul_tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2601 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/reduce_tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      689 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/reduce_tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1139 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/reorder_tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      593 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/reorder_tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      655 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/tuner.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      709 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner/tuner.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2310 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner_manager.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      797 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/tuner_manager.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7246 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/var_relay.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1733 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/opt/var_relay.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12839 2023-04-01 00:57:28.000000 jittor-1.3.7.9/python/jittor/src/parallel_compiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      589 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/parallel_compiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.365048 jittor-1.3.7.9/python/jittor/src/profiler/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      913 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/cache_info.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      717 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/cache_info.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1882 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/memory_checker.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1080 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/memory_checker.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    21971 2022-11-20 17:04:16.000000 jittor-1.3.7.9/python/jittor/src/profiler/profiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2317 2022-11-16 04:09:45.000000 jittor-1.3.7.9/python/jittor/src/profiler/profiler.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1914 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/profiler_guard.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2224 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/replacement.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1311 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/replacement.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3201 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/simple_profiler.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2609 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/profiler/vtop.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.365048 jittor-1.3.7.9/python/jittor/src/pybind/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1313 2022-05-10 07:52:19.000000 jittor-1.3.7.9/python/jittor/src/pybind/core.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15946 2023-04-04 08:01:54.000000 jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1950 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      558 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer_interface.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.365048 jittor-1.3.7.9/python/jittor/src/pyjt/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2688 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/numpy.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4020 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/numpy.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2093 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_arg_printer.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1044 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_arg_printer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6571 2023-04-01 08:41:31.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_array_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1116 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_caller.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      551 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_caller.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    26972 2023-04-04 09:37:07.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_converter.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2248 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_obj_holder.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8751 2022-05-08 11:48:51.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_ring_buffer.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1709 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/py_ring_buffer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15153 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/pyjt/pyjt_console.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.375881 jittor-1.3.7.9/python/jittor/src/test/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8024 2022-06-23 13:14:46.000000 jittor-1.3.7.9/python/jittor/src/test/test_expr.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      832 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_fast_shared_ptr.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2266 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/test/test_jit_key.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11949 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_kernel_ir.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2208 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_nano_vector.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      820 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_op_compiler.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3937 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/src/test/test_op_relay.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2040 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_setitem_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4738 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/test/test_sfrl_allocator.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.375881 jittor-1.3.7.9/python/jittor/src/type/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6593 2022-05-06 04:57:57.000000 jittor-1.3.7.9/python/jittor/src/type/common_op_type.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6265 2023-03-31 12:14:00.000000 jittor-1.3.7.9/python/jittor/src/type/fp16_compute.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7484 2022-11-04 15:41:27.000000 jittor-1.3.7.9/python/jittor/src/type/fp16_op_type.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6873 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/types.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.375881 jittor-1.3.7.9/python/jittor/src/utils/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15053 2023-04-01 08:29:26.000000 jittor-1.3.7.9/python/jittor/src/utils/cache_compile.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      746 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/cache_compile.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1706 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/cross_platform.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1286 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/flags.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      408 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/flags.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    20979 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/jit_utils.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    21467 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/log.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9277 2022-10-07 05:56:30.000000 jittor-1.3.7.9/python/jittor/src/utils/log.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1490 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/mwsr_list.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4766 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/mwsr_list.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6721 2021-10-01 11:48:38.000000 jittor-1.3.7.9/python/jittor/src/utils/seh.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7262 2022-10-12 17:02:09.000000 jittor-1.3.7.9/python/jittor/src/utils/str_utils.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1522 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/src/utils/str_utils.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7975 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/tracer.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      485 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/utils/tracer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       15 2021-10-01 11:48:38.000000 jittor-1.3.7.9/python/jittor/src/utils/vdp
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5522 2023-04-01 08:20:11.000000 jittor-1.3.7.9/python/jittor/src/var.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3286 2022-12-05 03:32:49.000000 jittor-1.3.7.9/python/jittor/src/var.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10034 2023-04-01 08:21:36.000000 jittor-1.3.7.9/python/jittor/src/var_holder.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10297 2023-04-01 00:10:16.000000 jittor-1.3.7.9/python/jittor/src/var_holder.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1202 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/var_slices.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2993 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/src/var_slices.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.440881 jittor-1.3.7.9/python/jittor/test/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2927 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/__main__.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.440881 jittor-1.3.7.9/python/jittor/test/misc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15224 2022-03-14 07:47:44.000000 jittor-1.3.7.9/python/jittor/test/misc/superglue.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.440881 jittor-1.3.7.9/python/jittor/test/perf/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8216 2022-03-22 14:48:20.000000 jittor-1.3.7.9/python/jittor/test/perf/perf.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.440881 jittor-1.3.7.9/python/jittor/test/system/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      358 2020-12-07 05:07:32.000000 jittor-1.3.7.9/python/jittor/test/system/test_all.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:52.000000 jittor-1.3.7.9/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:48.000000 jittor-1.3.7.9/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:44.000000 jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:39.000000 jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1844 2020-12-09 09:06:33.000000 jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1535 2020-12-09 09:06:26.000000 jittor-1.3.7.9/python/jittor/test/system/test_nocuda_ubuntu18.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      661 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5310 2022-10-26 12:24:38.000000 jittor-1.3.7.9/python/jittor/test/test_acl.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3269 2022-09-01 03:11:16.000000 jittor-1.3.7.9/python/jittor/test/test_adamw.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3007 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_affine_grid.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1453 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_allocator.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1573 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_allocator2.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12385 2021-08-04 11:28:54.000000 jittor-1.3.7.9/python/jittor/test/test_arg_pool_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5539 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_arg_reduce_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4327 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_argsort_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6742 2022-05-06 06:23:52.000000 jittor-1.3.7.9/python/jittor/test/test_array.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4192 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_asm_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2882 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_atomic_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2258 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_attention.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2134 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_auto_diff.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5576 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_batchnorm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12199 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_benchmark.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2177 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_bicubic.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7256 2022-10-25 09:28:10.000000 jittor-1.3.7.9/python/jittor/test/test_binary_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1591 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_bmm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4661 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_broadcast_to_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1819 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_broadcast_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4566 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_cache.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2662 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_candidate.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1143 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_clone.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    14087 2022-11-29 05:32:13.000000 jittor-1.3.7.9/python/jittor/test/test_code_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1137 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_compile_options.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6570 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_concat_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      963 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_console.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2464 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_contrib.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4874 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_conv_transpose.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6831 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_conv_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11127 2023-04-01 22:29:38.000000 jittor-1.3.7.9/python/jittor/test/test_core.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3460 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/test/test_cub_cumsum.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1538 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_cublas_test_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3801 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_cuda.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9134 2022-11-30 03:02:44.000000 jittor-1.3.7.9/python/jittor/test/test_cudnn_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-23 08:12:38.000000 jittor-1.3.7.9/python/jittor/test/test_cumprod_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2986 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_custom_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      869 2020-09-16 07:12:03.000000 jittor-1.3.7.9/python/jittor/test/test_cutt.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4068 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/test/test_cutt_transpose_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10487 2022-04-23 09:29:00.000000 jittor-1.3.7.9/python/jittor/test/test_dataset.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1455 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_default_var.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4289 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_densenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3130 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_depthwise_conv.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1587 2023-03-31 05:12:08.000000 jittor-1.3.7.9/python/jittor/test/test_digamma.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7920 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_distributions.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    28179 2022-11-07 04:02:17.000000 jittor-1.3.7.9/python/jittor/test/test_einops.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4462 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_einsum.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1138 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_emnist.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2195 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_error_msg.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2732 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_example.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3130 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_example_accumulate_grad.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1156 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_fetcher.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9165 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_fft_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1006 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_flags.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1958 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_fold.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12961 2023-03-31 12:17:11.000000 jittor-1.3.7.9/python/jittor/test/test_fp16.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9481 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_function.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    13063 2022-05-05 14:42:44.000000 jittor-1.3.7.9/python/jittor/test/test_fused_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1447 2022-04-23 10:07:08.000000 jittor-1.3.7.9/python/jittor/test/test_fuser.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6053 2022-05-05 14:39:19.000000 jittor-1.3.7.9/python/jittor/test/test_grad.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5585 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_group_conv_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2239 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_hook.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2686 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_image_folder.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5361 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_inception.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2312 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_index_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3247 2021-10-22 06:53:31.000000 jittor-1.3.7.9/python/jittor/test/test_init.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1216 2022-10-04 08:05:24.000000 jittor-1.3.7.9/python/jittor/test/test_interpolation.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1002 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_jit_tests.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1867 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_jtune.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1889 2022-05-06 04:57:57.000000 jittor-1.3.7.9/python/jittor/test/test_knn.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1364 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_lazy_execution.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11030 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_linalg.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2211 2022-07-04 16:11:21.000000 jittor-1.3.7.9/python/jittor/test/test_load_pth.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1089 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_lock.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1813 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_log.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2073 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_longest_dis_fuse.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9002 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/test/test_loss.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3392 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_loss3d.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1702 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_lr_scheduler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3814 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_lstm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    13954 2022-09-21 05:20:45.000000 jittor-1.3.7.9/python/jittor/test/test_matmul.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1648 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_matmul_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1263 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mem.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3818 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_memory_profiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2302 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_merge_loop_var_pass.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4523 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/test/test_merge_single_array_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6544 2022-09-01 15:17:10.000000 jittor-1.3.7.9/python/jittor/test/test_misc_issue.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    16899 2023-01-06 11:38:27.000000 jittor-1.3.7.9/python/jittor/test/test_misc_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8278 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mkl_conv_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      648 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mkl_test_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4056 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_models.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3220 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mpi.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4369 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mpi_batchnorm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1879 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_mpi_in_py.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2374 2022-06-02 05:33:14.000000 jittor-1.3.7.9/python/jittor/test/test_mpi_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2615 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_nano_string.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1581 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_nano_vector.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      703 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_nccl.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5181 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_nccl_ops.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1495 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_new_fused_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5550 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_node.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1630 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_notebooks.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6193 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_numpy_code_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6353 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_op_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1520 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_opt_state_dict.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_optimizer.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1883 2023-03-22 11:47:26.000000 jittor-1.3.7.9/python/jittor/test/test_optimizer_save_load.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3904 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_pad.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7853 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_parallel_pass.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1196 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_param_list.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1462 2022-11-16 08:04:41.000000 jittor-1.3.7.9/python/jittor/test/test_profiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8588 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_pytorch_converter.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3728 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_random_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4642 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_reduce_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1760 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_reduce_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11179 2022-04-24 05:57:04.000000 jittor-1.3.7.9/python/jittor/test/test_reindex_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3620 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_reindex_reduce_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3801 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_relu.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3383 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_reorder_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1670 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_repeat.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3237 2022-10-04 08:05:24.000000 jittor-1.3.7.9/python/jittor/test/test_reshape.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5310 2022-05-26 06:57:29.000000 jittor-1.3.7.9/python/jittor/test/test_resize_and_crop.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6181 2022-10-26 08:23:04.000000 jittor-1.3.7.9/python/jittor/test/test_resnet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2217 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_ring_buffer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3721 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_ring_buffer2.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    26660 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_rnn.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15920 2022-08-09 11:21:18.000000 jittor-1.3.7.9/python/jittor/test/test_rocm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1721 2021-03-23 11:08:33.000000 jittor-1.3.7.9/python/jittor/test/test_sampler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2368 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_search_sorted.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1549 2021-06-22 07:08:32.000000 jittor-1.3.7.9/python/jittor/test/test_searchsorted_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15402 2022-12-08 07:52:56.000000 jittor-1.3.7.9/python/jittor/test/test_setitem.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1481 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_single_process_scope.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6304 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_slice.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1371 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_sparse.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1732 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_stop_fuse.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3872 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_superglue.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2088 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_ternary_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6552 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_trace_var.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1439 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_tracer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    40470 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_transform.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5469 2022-04-24 07:29:02.000000 jittor-1.3.7.9/python/jittor/test/test_transpose_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4342 2022-11-04 15:12:11.000000 jittor-1.3.7.9/python/jittor/test/test_unary_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1869 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/test/test_unique.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2230 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_utils.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2074 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_var.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3731 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/test/test_vgg.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2790 2022-11-04 15:03:32.000000 jittor-1.3.7.9/python/jittor/test/test_where_op.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.440881 jittor-1.3.7.9/python/jittor/transform/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    54004 2023-03-19 10:34:00.000000 jittor-1.3.7.9/python/jittor/transform/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    23971 2022-07-31 12:18:09.000000 jittor-1.3.7.9/python/jittor/transform/function_pil.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.451714 jittor-1.3.7.9/python/jittor/utils/
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     5419 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/asm_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      352 2022-12-01 04:53:11.000000 jittor-1.3.7.9/python/jittor/utils/bench_klo.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      685 2020-12-13 14:03:17.000000 jittor-1.3.7.9/python/jittor/utils/converter_server.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   437003 2023-04-03 01:38:42.000000 jittor-1.3.7.9/python/jittor/utils/data.gz
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-06-23 13:14:46.000000 jittor-1.3.7.9/python/jittor/utils/dlink_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1276 2022-03-15 13:17:00.000000 jittor-1.3.7.9/python/jittor/utils/dumpdef.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9761 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor/utils/gen_pyi.py
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     1926 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/jtune.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2190 2021-10-01 11:48:38.000000 jittor-1.3.7.9/python/jittor/utils/local_doc_builder.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1214 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/nvtx.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4895 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/polish.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2484 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/polish_centos.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1834 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/publish.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    28291 2022-11-16 03:31:13.000000 jittor-1.3.7.9/python/jittor/utils/pytorch_converter.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      837 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor/utils/tracer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       41 2021-06-18 14:24:21.000000 jittor-1.3.7.9/python/jittor/version
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.213381 jittor-1.3.7.9/python/jittor.egg-info/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-04-04 15:15:59.000000 jittor-1.3.7.9/python/jittor.egg-info/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)    27920 2023-04-04 15:15:59.000000 jittor-1.3.7.9/python/jittor.egg-info/SOURCES.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-04-04 15:15:59.000000 jittor-1.3.7.9/python/jittor.egg-info/dependency_links.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       75 2023-04-04 15:15:59.000000 jittor-1.3.7.9/python/jittor.egg-info/requires.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       20 2023-04-04 15:15:59.000000 jittor-1.3.7.9/python/jittor.egg-info/top_level.txt
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.462548 jittor-1.3.7.9/python/jittor_utils/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    24778 2023-04-04 11:29:23.000000 jittor-1.3.7.9/python/jittor_utils/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15503 2022-03-22 14:48:20.000000 jittor-1.3.7.9/python/jittor_utils/auto_diff.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1290 2022-05-08 11:48:51.000000 jittor-1.3.7.9/python/jittor_utils/auto_git_tag.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-04-04 15:15:59.462548 jittor-1.3.7.9/python/jittor_utils/class/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      993 2021-10-12 06:29:13.000000 jittor-1.3.7.9/python/jittor_utils/class/motd
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      472 2021-10-12 06:29:13.000000 jittor-1.3.7.9/python/jittor_utils/class/setup.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5595 2022-05-09 07:41:55.000000 jittor-1.3.7.9/python/jittor_utils/class/setup_env.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1634 2023-04-04 08:01:14.000000 jittor-1.3.7.9/python/jittor_utils/clean_cache.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3812 2021-10-01 11:48:38.000000 jittor-1.3.7.9/python/jittor_utils/config.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      710 2022-05-08 11:48:51.000000 jittor-1.3.7.9/python/jittor_utils/github_release.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6081 2022-11-30 03:03:51.000000 jittor-1.3.7.9/python/jittor_utils/install_cuda.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      504 2021-10-01 11:48:38.000000 jittor-1.3.7.9/python/jittor_utils/install_msvc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11112 2023-04-04 05:10:47.000000 jittor-1.3.7.9/python/jittor_utils/load_pytorch.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10438 2023-03-30 09:43:29.000000 jittor-1.3.7.9/python/jittor_utils/load_pytorch_old.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2608 2022-04-22 13:37:44.000000 jittor-1.3.7.9/python/jittor_utils/lock.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5441 2023-01-06 08:38:43.000000 jittor-1.3.7.9/python/jittor_utils/misc.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3093 2022-07-06 05:24:42.000000 jittor-1.3.7.9/python/jittor_utils/pack_offline.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      799 2021-10-12 06:29:13.000000 jittor-1.3.7.9/python/jittor_utils/pip_publish.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      852 2021-10-13 11:17:19.000000 jittor-1.3.7.9/python/jittor_utils/query_cuda_cc.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8822 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor_utils/ring_buffer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2168 2022-04-22 13:00:57.000000 jittor-1.3.7.9/python/jittor_utils/student_queue.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2844 2022-09-15 16:59:59.000000 jittor-1.3.7.9/python/jittor_utils/translator.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-04-04 15:15:59.473381 jittor-1.3.7.9/setup.cfg
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2464 2021-10-12 06:29:13.000000 jittor-1.3.7.9/setup.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.349713 jittor-1.3.8.1/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11613 2023-05-01 08:04:48.000000 jittor-1.3.8.1/LICENSE.txt
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       88 2021-07-31 06:19:50.000000 jittor-1.3.8.1/MANIFEST.in
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-09 17:02:51.349713 jittor-1.3.8.1/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11809 2023-03-31 13:28:11.000000 jittor-1.3.8.1/README.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.840547 jittor-1.3.8.1/python/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.862214 jittor-1.3.8.1/python/jittor/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    66981 2023-06-09 16:58:10.000000 jittor-1.3.8.1/python/jittor/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   244353 2022-09-15 16:59:59.000000 jittor-1.3.8.1/python/jittor/__init__.pyi
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6545 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/attention.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.862214 jittor-1.3.8.1/python/jittor/ccl/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       86 2022-12-02 14:36:01.000000 jittor-1.3.8.1/python/jittor/ccl/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8866 2022-12-02 14:36:01.000000 jittor-1.3.8.1/python/jittor/ccl/ccl_2d.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10077 2022-12-02 14:36:01.000000 jittor-1.3.8.1/python/jittor/ccl/ccl_3d.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11051 2022-12-02 14:36:01.000000 jittor-1.3.8.1/python/jittor/ccl/ccl_link.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    24872 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/compile_extern.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    54031 2023-05-13 22:54:20.000000 jittor-1.3.8.1/python/jittor/compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9039 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/contrib.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.873047 jittor-1.3.8.1/python/jittor/dataset/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      201 2023-01-07 09:03:52.000000 jittor-1.3.8.1/python/jittor/dataset/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6439 2021-06-16 12:20:56.000000 jittor-1.3.8.1/python/jittor/dataset/cifar.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26798 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/dataset/dataset.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8320 2021-09-04 06:27:26.000000 jittor-1.3.8.1/python/jittor/dataset/mnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3323 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/dataset/sampler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2326 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/dataset/utils.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2410 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/dataset/voc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.873047 jittor-1.3.8.1/python/jittor/demo/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3591 2022-04-04 06:54:03.000000 jittor-1.3.8.1/python/jittor/demo/simple_cgan.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15663 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/depthwise_conv.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6546 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/distributions.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.873047 jittor-1.3.8.1/python/jittor/einops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      262 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8494 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/_backends.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    33864 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/einops.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.873047 jittor-1.3.8.1/python/jittor/einops/experimental/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)        0 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/experimental/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15167 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/experimental/indexing.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/einops/layers/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2933 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/layers/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8720 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/layers/_einmix.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2057 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/layers/jittor.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6848 2022-11-07 04:02:17.000000 jittor-1.3.8.1/python/jittor/einops/parsing.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/extern/acl/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2379 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/acl/acl_compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    14964 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/acl/acl_error_code.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11204 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/acl/acl_jittor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/acl/acl_jittor.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/extern/corex/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3816 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/corex/corex_compiler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/cuda/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.818880 jittor-1.3.8.1/python/jittor/extern/cuda/cub/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/extern/cuda/cub/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     9072 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/inc/cub_test.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3918 2023-06-06 14:46:30.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      911 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3424 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      931 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4891 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      809 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1144 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      624 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_test_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3679 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_where_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1146 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_where_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.818880 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.883880 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      973 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.894713 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4418 2023-05-16 15:04:55.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      905 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5778 2023-05-13 23:06:10.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      953 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4387 2023-06-09 16:51:49.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      771 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      879 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      639 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.894713 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12200 2021-07-26 07:27:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      990 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1606 2020-12-03 05:10:19.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/helper_cublas.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.818880 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.894713 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4906 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      842 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11561 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11327 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1151 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11535 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1029 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12570 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12027 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1121 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12423 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1061 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8286 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1470 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9384 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1375 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1093 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      628 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    39400 2021-12-30 07:13:56.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2914 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1070 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      161 2021-07-26 07:24:52.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/helper_cudnn.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.818880 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6280 2022-03-30 06:36:09.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/inc/cufft_utils.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3201 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      821 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/cuda/curand/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.905547 jittor-1.3.8.1/python/jittor/extern/cuda/curand/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      632 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/curand/inc/curand_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/curand/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1632 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/curand/ops/curand_random_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      759 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/curand/ops/curand_random_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/curand/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1078 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/curand/src/curand_wrapper.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1933 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/curand/src/helper_curand.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1052 2022-05-26 06:57:29.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      629 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3868 2023-05-16 06:12:13.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      775 2021-04-15 10:38:17.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      888 2021-11-01 03:42:19.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      559 2021-07-26 07:18:24.000000 jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      588 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/fp16_dev.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5639 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/fp16_emu.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12641 2022-10-25 03:25:21.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_cuda.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1173 2023-04-08 05:52:12.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_functions.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    27554 2023-04-08 05:52:07.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_image.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    33798 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_string.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    14855 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_timer.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      656 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.916380 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1771 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      782 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1838 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      808 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1877 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      799 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3785 2022-05-26 06:57:29.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.927214 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1923 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.927214 jittor-1.3.8.1/python/jittor/extern/cuda/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1323 2021-07-26 07:15:57.000000 jittor-1.3.8.1/python/jittor/extern/cuda/src/fp16_dev.cu
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5303 2022-07-04 16:11:21.000000 jittor-1.3.8.1/python/jittor/extern/cuda/src/fp16_emu.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11787 2021-07-26 07:13:54.000000 jittor-1.3.8.1/python/jittor/extern/cuda/src/helper_cuda.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.927214 jittor-1.3.8.1/python/jittor/extern/llvm/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15734 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/mkl/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/extern/mkl/ops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    36034 2022-03-22 14:48:20.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8788 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8850 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1048 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7552 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1035 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2210 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      762 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      810 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      595 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.829714 jittor-1.3.8.1/python/jittor/extern/mpi/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/extern/mpi/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2014 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/inc/mpi_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/extern/mpi/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2899 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1110 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2222 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1028 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_broadcast_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2989 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1171 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_reduce_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1102 2022-05-26 06:57:29.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      641 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/extern/mpi/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/extern/mpi/src/mpi_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/extern/rocm/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   115033 2022-08-09 11:21:18.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_cache.tar.gz
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6235 2022-10-26 06:26:28.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_compiler.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1712 2022-08-09 11:21:18.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_config.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      497 2022-08-09 11:21:18.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_config.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      538 2022-07-04 16:11:21.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_jittor.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6598 2022-08-09 11:21:18.000000 jittor-1.3.8.1/python/jittor/extern/rocm/rocm_wrapper.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23687 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/init.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1715 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/init_cupy.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16949 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/linalg.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.938047 jittor-1.3.8.1/python/jittor/loss3d/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      105 2021-06-30 08:15:49.000000 jittor-1.3.8.1/python/jittor/loss3d/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5553 2021-06-30 08:15:49.000000 jittor-1.3.8.1/python/jittor/loss3d/chamfer.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    16008 2021-06-30 08:15:49.000000 jittor-1.3.8.1/python/jittor/loss3d/emd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7936 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/lr_scheduler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.948880 jittor-1.3.8.1/python/jittor/math_util/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       64 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/math_util/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15722 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/math_util/gamma.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      671 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/math_util/igamma.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.948880 jittor-1.3.8.1/python/jittor/math_util/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5520 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/math_util/src/gamma_grad.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    29181 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/math_util/src/igamma.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    76767 2023-06-06 14:33:24.000000 jittor-1.3.8.1/python/jittor/misc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.948880 jittor-1.3.8.1/python/jittor/models/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      513 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/models/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2246 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/alexnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6745 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/densenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6328 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/googlenet.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11821 2022-04-04 06:54:03.000000 jittor-1.3.8.1/python/jittor/models/inception.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4821 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/mnasnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4602 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/mobilenet.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8032 2021-10-19 11:51:01.000000 jittor-1.3.8.1/python/jittor/models/res2net.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9657 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/resnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5575 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/shufflenetv2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4028 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/squeezenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3711 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/models/vgg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)   122453 2023-06-09 17:01:30.000000 jittor-1.3.8.1/python/jittor/nn.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.959714 jittor-1.3.8.1/python/jittor/notebook/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.970547 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      297 2021-07-14 13:51:52.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/README.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   243006 2021-07-14 13:51:52.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/mnist.png
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5047 2021-07-14 13:51:52.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    29117 2021-07-14 13:51:52.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    62291 2022-03-15 13:17:00.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   136962 2022-03-15 13:17:00.000000 jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6314 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3487 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6752 2022-04-04 06:54:03.000000 jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/LSGAN.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     7897 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/LSGAN.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/LSGAN.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      238 2022-03-15 13:17:00.000000 jittor-1.3.8.1/python/jittor/notebook/__main__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1243 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/basics.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1250 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/basics.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2111 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/basics.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2232 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/custom_op.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2249 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/custom_op.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2760 2021-07-16 06:09:15.000000 jittor-1.3.8.1/python/jittor/notebook/custom_op.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1996 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/example.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2152 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/example.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3099 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/example.src.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.981380 jittor-1.3.8.1/python/jittor/notebook/figs/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    41082 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/figs/mop.svg
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2203 2022-03-22 14:48:20.000000 jittor-1.3.8.1/python/jittor/notebook/md_to_ipynb.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     7817 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/meta_op.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8068 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/meta_op.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10843 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/meta_op.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      235 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/profiler.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      264 2021-10-11 05:54:17.000000 jittor-1.3.8.1/python/jittor/notebook/profiler.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      459 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/notebook/profiler.src.md
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23255 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/optim.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.981380 jittor-1.3.8.1/python/jittor/other/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     4777 2023-05-14 05:03:20.000000 jittor-1.3.8.1/python/jittor/other/code_softmax.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    29598 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/pool.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    35074 2023-05-13 04:29:28.000000 jittor-1.3.8.1/python/jittor/pyjt_compiler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.981380 jittor-1.3.8.1/python/jittor/script/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1464 2021-05-12 08:13:24.000000 jittor-1.3.8.1/python/jittor/script/Dockerfile_cuda11
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      890 2021-06-19 09:21:11.000000 jittor-1.3.8.1/python/jittor/script/build_aarch64_mkl.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      893 2021-05-04 00:57:17.000000 jittor-1.3.8.1/python/jittor/script/converter_server.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/script/inference_perf.py
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)     2265 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/script/install.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2543 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/script/install_llvm.sh
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)      632 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/script/install_mkl.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1569 2022-03-15 13:17:00.000000 jittor-1.3.8.1/python/jittor/script/make_doc.py
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)     4359 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/script/tmpi
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)      144 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/script/update.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1759 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/sparse.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.992214 jittor-1.3.8.1/python/jittor/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1326 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/common.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1056 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/core.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/event_queue.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2392 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/event_queue.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26839 2023-06-04 15:48:06.000000 jittor-1.3.8.1/python/jittor/src/executor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/executor.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8249 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/fused_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1936 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/fused_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      643 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/fuser.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10134 2023-05-22 01:02:36.000000 jittor-1.3.8.1/python/jittor/src/grad.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      712 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/grad.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5885 2023-05-16 07:23:39.000000 jittor-1.3.8.1/python/jittor/src/graph.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4724 2023-05-16 07:23:32.000000 jittor-1.3.8.1/python/jittor/src/graph.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2730 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/init.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1091 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/init.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9383 2023-06-04 21:24:53.000000 jittor-1.3.8.1/python/jittor/src/jit_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      652 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/jit_compiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3262 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/jit_key.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7600 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/jit_key.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2031 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/lock.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/lock.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.003047 jittor-1.3.8.1/python/jittor/src/mem/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.013880 jittor-1.3.8.1/python/jittor/src/mem/allocator/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1188 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/aligned_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      779 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/aligned_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1407 2023-05-22 03:02:50.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_device_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      805 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_device_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1107 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_dual_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4172 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_dual_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1087 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_host_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      802 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_host_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1190 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_managed_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      856 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_managed_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1501 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/foreign_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      948 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/foreign_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1127 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/nfef_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/nfef_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9259 2023-06-04 17:35:51.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/sfrl_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3883 2023-06-04 16:31:06.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/sfrl_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1781 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/stat_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1071 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/stat_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3765 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/temp_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2234 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator/temp_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5170 2023-06-04 16:35:41.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2237 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11462 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/mem_info.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/mem_info.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8807 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/swap.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2427 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/mem/swap.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6373 2023-05-22 03:19:52.000000 jittor-1.3.8.1/python/jittor/src/memory_profiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1429 2023-05-22 03:29:05.000000 jittor-1.3.8.1/python/jittor/src/memory_profiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.035547 jittor-1.3.8.1/python/jittor/src/misc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cpu_atomic.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1820 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cpu_atomic.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2362 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cpu_math.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      490 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cpu_math.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cstr.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7264 2023-05-13 08:27:34.000000 jittor-1.3.8.1/python/jittor/src/misc/cuda_atomic.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2794 2023-06-02 03:30:13.000000 jittor-1.3.8.1/python/jittor/src/misc/cuda_flags.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1142 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cuda_flags.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2191 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/cuda_limits.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/deleter.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2538 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/fast_shared_ptr.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/hash.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/intrin.h
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)   326707 2023-03-30 05:25:05.000000 jittor-1.3.8.1/python/jittor/src/misc/miniz.cc
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)    69968 2023-04-01 02:27:50.000000 jittor-1.3.8.1/python/jittor/src/misc/miniz.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2519 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/nan_checker.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3046 2023-05-13 12:40:54.000000 jittor-1.3.8.1/python/jittor/src/misc/nan_checker.cu
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      403 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/nan_checker.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5953 2023-05-16 04:56:35.000000 jittor-1.3.8.1/python/jittor/src/misc/nano_string.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7634 2023-05-13 20:28:36.000000 jittor-1.3.8.1/python/jittor/src/misc/nano_string.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9048 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/nano_vector.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3368 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/ring_buffer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6868 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/ring_buffer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1801 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/stack_vector.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1503 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/misc/string_view_map.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7512 2023-05-16 14:49:25.000000 jittor-1.3.8.1/python/jittor/src/node.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1902 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/numpy_func.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9475 2023-05-19 23:16:17.000000 jittor-1.3.8.1/python/jittor/src/op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2828 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    43093 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/op_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1766 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/op_compiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.089713 jittor-1.3.8.1/python/jittor/src/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7467 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/arg_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1761 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/arg_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6273 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/argsort_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2167 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/argsort_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4035 2023-06-04 21:24:23.000000 jittor-1.3.8.1/python/jittor/src/ops/array_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1098 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/array_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15124 2023-05-16 05:07:55.000000 jittor-1.3.8.1/python/jittor/src/ops/binary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      727 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/binary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6900 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/broadcast_to_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2794 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/broadcast_to_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3650 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/candidate_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1945 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/candidate_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1211 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/clone_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      715 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/clone_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8685 2023-05-13 17:11:35.000000 jittor-1.3.8.1/python/jittor/src/ops/code_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10232 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/code_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1425 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/copy_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      694 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/copy_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      685 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/empty_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      607 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/empty_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5104 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/fetch_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2540 2023-06-04 20:08:00.000000 jittor-1.3.8.1/python/jittor/src/ops/fetch_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3766 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/fuse_transpose_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      774 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/fuse_transpose_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    19861 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/getitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1555 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/getitem_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2724 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/index_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1986 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/index_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5542 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/numpy_code_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3394 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/numpy_code_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1508 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/op_register.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1544 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/op_register.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1577 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/op_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2072 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/random_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      686 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/random_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12858 2023-05-16 14:58:04.000000 jittor-1.3.8.1/python/jittor/src/ops/reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5836 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reindex_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4093 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reindex_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5603 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reindex_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3610 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reindex_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2069 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reshape_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1536 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/reshape_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1615 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/safe_clip_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1008 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/safe_clip_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12583 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/setitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1130 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/setitem_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3004 2023-05-13 19:25:10.000000 jittor-1.3.8.1/python/jittor/src/ops/tape_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1897 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/tape_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3745 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/ternary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      735 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/ternary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3808 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/transpose_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      761 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/transpose_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26784 2023-05-13 12:41:11.000000 jittor-1.3.8.1/python/jittor/src/ops/unary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      742 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/unary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8196 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/where_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1232 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/ops/where_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.089713 jittor-1.3.8.1/python/jittor/src/opt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    38841 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/expr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5751 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/expr.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.089713 jittor-1.3.8.1/python/jittor/src/opt/gopt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5511 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/gopt/setitem_gopt.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3084 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/jit_searcher.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      748 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/jit_searcher.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    35269 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/kernel_ir.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8192 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/kernel_ir.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.165547 jittor-1.3.8.1/python/jittor/src/opt/pass/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2071 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/assume_aligned_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/assume_aligned_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/atomic_tuner_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6886 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/check_cache_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/check_cache_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1494 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/compile_shapes_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/compile_shapes_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1644 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/const_var_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/const_var_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1391 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/expand_empty_block_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      582 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/expand_empty_block_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6960 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/fake_main_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      557 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/fake_main_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3545 2023-05-11 12:13:21.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/float_atomic_fix_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      590 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/float_atomic_fix_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1480 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/insert_profile_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      585 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/insert_profile_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4427 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/loop_to_func_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      564 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/loop_to_func_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12889 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/loop_var_analyze_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/loop_var_analyze_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1246 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/mark_raw_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      554 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/mark_raw_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2283 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      560 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6195 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_var_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      570 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_var_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/parallel_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      680 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      732 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/remove_intermediate_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      587 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/remove_intermediate_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      897 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/remove_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      620 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/remove_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      633 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/rename_loop_index_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      579 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/rename_loop_index_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2306 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/reorder_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/reorder_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/replace_for_num_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      868 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/replace_for_num_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5910 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/restride_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/restride_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      574 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/shared_reduce_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      604 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/solve_conflict_define_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      591 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/solve_conflict_define_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1362 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/split_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      634 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/split_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3719 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/unroll_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/unroll_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      944 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/use_movnt_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/use_movnt_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3411 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/vectorize_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      559 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass/vectorize_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4356 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass_manager.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1954 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/pass_manager.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.176380 jittor-1.3.8.1/python/jittor/src/opt/tuner/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2242 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/broadcast_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      670 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/broadcast_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16851 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/conv_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      692 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/conv_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4058 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/matmul_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      622 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/matmul_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2601 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/reduce_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      689 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/reduce_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1139 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/reorder_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      593 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/reorder_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      655 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      709 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner/tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2310 2023-06-04 21:11:55.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner_manager.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      797 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/tuner_manager.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7246 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/var_relay.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1733 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/opt/var_relay.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12839 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/parallel_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      589 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/parallel_compiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.187214 jittor-1.3.8.1/python/jittor/src/profiler/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      913 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/cache_info.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/cache_info.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1882 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/memory_checker.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1080 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/memory_checker.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21999 2023-05-16 04:35:30.000000 jittor-1.3.8.1/python/jittor/src/profiler/profiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2317 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/profiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1914 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/profiler_guard.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2224 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/replacement.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1311 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/replacement.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3201 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/simple_profiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2609 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/profiler/vtop.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.208880 jittor-1.3.8.1/python/jittor/src/pybind/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1313 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pybind/core.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16013 2023-05-16 04:35:32.000000 jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1950 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      558 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer_interface.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.208880 jittor-1.3.8.1/python/jittor/src/pyjt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2688 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/numpy.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4020 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/numpy.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2093 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_arg_printer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_arg_printer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6571 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_array_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_caller.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      551 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_caller.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    27513 2023-06-04 20:44:12.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_converter.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2248 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_obj_holder.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8751 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_ring_buffer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1709 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/py_ring_buffer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15153 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/pyjt/pyjt_console.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.230547 jittor-1.3.8.1/python/jittor/src/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8024 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_expr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      832 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_fast_shared_ptr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2266 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_jit_key.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11949 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_kernel_ir.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2208 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_nano_vector.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      820 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_op_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3937 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_op_relay.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2040 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_setitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4738 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/test/test_sfrl_allocator.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.230547 jittor-1.3.8.1/python/jittor/src/type/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6593 2023-05-13 22:53:57.000000 jittor-1.3.8.1/python/jittor/src/type/common_op_type.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6265 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/type/fp16_compute.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7484 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/type/fp16_op_type.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6873 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/types.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.241380 jittor-1.3.8.1/python/jittor/src/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15087 2023-05-13 08:17:57.000000 jittor-1.3.8.1/python/jittor/src/utils/cache_compile.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      746 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/cache_compile.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1706 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/cross_platform.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1286 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/flags.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      408 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/flags.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    20979 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/jit_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21467 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/log.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9277 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/log.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/mwsr_list.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4766 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/mwsr_list.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6721 2021-10-01 11:48:38.000000 jittor-1.3.8.1/python/jittor/src/utils/seh.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7262 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/str_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/str_utils.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7975 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/tracer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/utils/tracer.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       15 2021-10-01 11:48:38.000000 jittor-1.3.8.1/python/jittor/src/utils/vdp
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5563 2023-06-04 18:38:09.000000 jittor-1.3.8.1/python/jittor/src/var.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3286 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/var.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10034 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/var_holder.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10636 2023-06-04 20:52:46.000000 jittor-1.3.8.1/python/jittor/src/var_holder.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1202 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/var_slices.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2993 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/src/var_slices.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.328047 jittor-1.3.8.1/python/jittor/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2927 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/__main__.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.328047 jittor-1.3.8.1/python/jittor/test/misc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15224 2022-03-14 07:47:44.000000 jittor-1.3.8.1/python/jittor/test/misc/superglue.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.328047 jittor-1.3.8.1/python/jittor/test/perf/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8216 2022-03-22 14:48:20.000000 jittor-1.3.8.1/python/jittor/test/perf/perf.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.328047 jittor-1.3.8.1/python/jittor/test/system/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      358 2020-12-07 05:07:32.000000 jittor-1.3.8.1/python/jittor/test/system/test_all.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:52.000000 jittor-1.3.8.1/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:48.000000 jittor-1.3.8.1/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:44.000000 jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:39.000000 jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1844 2020-12-09 09:06:33.000000 jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1535 2020-12-09 09:06:26.000000 jittor-1.3.8.1/python/jittor/test/system/test_nocuda_ubuntu18.04.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      661 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_acl.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3269 2022-09-01 03:11:16.000000 jittor-1.3.8.1/python/jittor/test/test_adamw.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3007 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_affine_grid.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1453 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_allocator.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_allocator2.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12385 2021-08-04 11:28:54.000000 jittor-1.3.8.1/python/jittor/test/test_arg_pool_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5539 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_arg_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4327 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_argsort_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6742 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_array.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4192 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_asm_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2882 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_atomic_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2258 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_attention.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2134 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_auto_diff.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5576 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_batchnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12199 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_benchmark.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2177 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_bicubic.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7256 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_binary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1591 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_bmm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4661 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_broadcast_to_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1819 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_broadcast_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4566 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_cache.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_candidate.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_clone.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    14087 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_code_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1137 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_compile_options.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6570 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_concat_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      963 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_console.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2464 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_contrib.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4874 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_conv_transpose.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6831 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_conv_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11127 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_core.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3460 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_cub_cumsum.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1538 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_cublas_test_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_cuda.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9134 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_cudnn_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-23 08:12:38.000000 jittor-1.3.8.1/python/jittor/test/test_cumprod_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2986 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_custom_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      869 2020-09-16 07:12:03.000000 jittor-1.3.8.1/python/jittor/test/test_cutt.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     4068 2022-09-15 16:59:59.000000 jittor-1.3.8.1/python/jittor/test/test_cutt_transpose_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10487 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_dataset.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1455 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_default_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4289 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_densenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_depthwise_conv.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1571 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_digamma.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7920 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_distributions.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28179 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_einops.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4462 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_einsum.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1138 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_emnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2195 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_error_msg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2732 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_example.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_example_accumulate_grad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1156 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fetcher.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9165 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fft_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1006 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_flags.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1958 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fold.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12961 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fp16.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9481 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_function.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    13063 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fused_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1447 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_fuser.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1730 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_gamma_distribution.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6053 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_grad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5585 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_group_conv_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1556 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_histc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2239 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_hook.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2686 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_image_folder.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5361 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_inception.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2312 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_index_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3247 2021-10-22 06:53:31.000000 jittor-1.3.8.1/python/jittor/test/test_init.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1216 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_interpolation.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_jit_tests.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1867 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_jtune.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1889 2022-05-06 04:57:57.000000 jittor-1.3.8.1/python/jittor/test/test_knn.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1364 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_lazy_execution.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11030 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_linalg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2211 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_load_pth.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1089 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_lock.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1813 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_log.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2073 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_longest_dis_fuse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9002 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_loss.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3392 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_loss3d.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1702 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_lr_scheduler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3814 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_lstm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    13954 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_matmul.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1648 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_matmul_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1263 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mem.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3818 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_memory_profiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2302 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_merge_loop_var_pass.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4523 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_merge_single_array_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6544 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_misc_issue.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16899 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_misc_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8278 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mkl_conv_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      648 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mkl_test_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4056 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_models.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3220 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mpi.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4369 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mpi_batchnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1879 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mpi_in_py.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2374 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_mpi_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2615 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_nano_string.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1581 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_nano_vector.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      703 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_nccl.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5181 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_nccl_ops.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1495 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_new_fused_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5550 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_node.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1630 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_notebooks.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6193 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_numpy_code_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6353 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_op_compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1520 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_opt_state_dict.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_optimizer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1883 2023-03-22 11:47:26.000000 jittor-1.3.8.1/python/jittor/test/test_optimizer_save_load.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3904 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_pad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7853 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_parallel_pass.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1196 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_param_list.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1462 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_profiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8588 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_pytorch_converter.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3728 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_random_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4642 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1760 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reduce_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11179 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reindex_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3620 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reindex_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_relu.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3383 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reorder_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1670 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_repeat.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3237 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_reshape.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_resize_and_crop.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6181 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_resnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2217 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_ring_buffer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3721 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_ring_buffer2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26660 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_rnn.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15920 2022-08-09 11:21:18.000000 jittor-1.3.8.1/python/jittor/test/test_rocm.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1721 2021-03-23 11:08:33.000000 jittor-1.3.8.1/python/jittor/test/test_sampler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2368 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_search_sorted.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1549 2021-06-22 07:08:32.000000 jittor-1.3.8.1/python/jittor/test/test_searchsorted_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15402 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_setitem.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1481 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_single_process_scope.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6304 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_slice.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1371 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_sparse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1732 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_stop_fuse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3872 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_superglue.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2088 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_ternary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6552 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_trace_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1439 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_tracer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    40470 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_transform.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5469 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_transpose_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4342 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_unary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1869 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_unique.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2230 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_utils.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2074 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3731 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_vgg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2202 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_weightnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2790 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/test/test_where_op.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.328047 jittor-1.3.8.1/python/jittor/transform/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    54004 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/transform/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23971 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/transform/function_pil.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.349713 jittor-1.3.8.1/python/jittor/utils/
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)     5419 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/asm_tuner.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      352 2022-12-01 04:53:11.000000 jittor-1.3.8.1/python/jittor/utils/bench_klo.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      685 2020-12-13 14:03:17.000000 jittor-1.3.8.1/python/jittor/utils/converter_server.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   437003 2023-04-03 01:38:42.000000 jittor-1.3.8.1/python/jittor/utils/data.gz
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-06-23 13:14:46.000000 jittor-1.3.8.1/python/jittor/utils/dlink_compiler.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1276 2022-03-15 13:17:00.000000 jittor-1.3.8.1/python/jittor/utils/dumpdef.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9761 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/gen_pyi.py
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)     1926 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/jtune.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2190 2021-10-01 11:48:38.000000 jittor-1.3.8.1/python/jittor/utils/local_doc_builder.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1214 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/nvtx.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4895 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/polish.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2484 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/polish_centos.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1834 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/publish.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28291 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/pytorch_converter.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      837 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor/utils/tracer.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       41 2021-06-18 14:24:21.000000 jittor-1.3.8.1/python/jittor/version
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2878 2023-04-04 18:16:13.000000 jittor-1.3.8.1/python/jittor/weightnorm.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:50.862214 jittor-1.3.8.1/python/jittor.egg-info/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-09 17:02:50.000000 jittor-1.3.8.1/python/jittor.egg-info/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28177 2023-06-09 17:02:50.000000 jittor-1.3.8.1/python/jittor.egg-info/SOURCES.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-09 17:02:50.000000 jittor-1.3.8.1/python/jittor.egg-info/dependency_links.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       75 2023-06-09 17:02:50.000000 jittor-1.3.8.1/python/jittor.egg-info/requires.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       20 2023-06-09 17:02:50.000000 jittor-1.3.8.1/python/jittor.egg-info/top_level.txt
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.349713 jittor-1.3.8.1/python/jittor_utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    24838 2023-05-22 03:28:13.000000 jittor-1.3.8.1/python/jittor_utils/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15503 2022-03-22 14:48:20.000000 jittor-1.3.8.1/python/jittor_utils/auto_diff.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1290 2022-05-08 11:48:51.000000 jittor-1.3.8.1/python/jittor_utils/auto_git_tag.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-09 17:02:51.349713 jittor-1.3.8.1/python/jittor_utils/class/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      993 2021-10-12 06:29:13.000000 jittor-1.3.8.1/python/jittor_utils/class/motd
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      472 2021-10-12 06:29:13.000000 jittor-1.3.8.1/python/jittor_utils/class/setup.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5595 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/class/setup_env.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1634 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/clean_cache.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3812 2021-10-01 11:48:38.000000 jittor-1.3.8.1/python/jittor_utils/config.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      710 2022-05-08 11:48:51.000000 jittor-1.3.8.1/python/jittor_utils/github_release.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6105 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/install_cuda.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      504 2021-10-01 11:48:38.000000 jittor-1.3.8.1/python/jittor_utils/install_msvc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11596 2023-05-16 08:35:45.000000 jittor-1.3.8.1/python/jittor_utils/load_pytorch.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10438 2023-03-30 09:43:29.000000 jittor-1.3.8.1/python/jittor_utils/load_pytorch_old.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2608 2022-04-22 13:37:44.000000 jittor-1.3.8.1/python/jittor_utils/lock.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5441 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/misc.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3093 2022-07-06 05:24:42.000000 jittor-1.3.8.1/python/jittor_utils/pack_offline.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      799 2021-10-12 06:29:13.000000 jittor-1.3.8.1/python/jittor_utils/pip_publish.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      852 2021-10-13 11:17:19.000000 jittor-1.3.8.1/python/jittor_utils/query_cuda_cc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8822 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/ring_buffer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2168 2023-05-01 08:04:48.000000 jittor-1.3.8.1/python/jittor_utils/student_queue.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2844 2022-09-15 16:59:59.000000 jittor-1.3.8.1/python/jittor_utils/translator.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-09 17:02:51.349713 jittor-1.3.8.1/setup.cfg
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2464 2021-10-12 06:29:13.000000 jittor-1.3.8.1/setup.py
```

### Comparing `jittor-1.3.7.9/LICENSE.txt` & `jittor-1.3.8.1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Jittor. All Rights Reserved
+Copyright (c) 2023 Jittor. All Rights Reserved
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -184,15 +184,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022 Jittor. All Rights Reserved.
+   Copyright (c) 2023 Jittor. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `jittor-1.3.7.9/PKG-INFO` & `jittor-1.3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittor
-Version: 1.3.7.9
+Version: 1.3.8.1
 Summary: a Just-in-time(JIT) deep learning framework
 Home-page: http://jittor.org
 Author: Jittor Group
 Author-email: ran.donglang@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `jittor-1.3.7.9/README.md` & `jittor-1.3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/__init__.py` & `jittor-1.3.8.1/python/jittor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Dun Liang <randonlang@gmail.com>.
 #   Meng-Hao Guo <guomenghao1997@gmail.com>
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 
-__version__ = '1.3.7.9'
+__version__ = '1.3.8.1'
 from jittor_utils import lock
 with lock.lock_scope():
     ori_int = int
     ori_float = float
     ori_bool = bool
     from . import compiler
     from .compiler import LOG, has_cuda
@@ -340,14 +340,15 @@
         return inner
     return outer
 
 def clean():
     import gc
     # make sure python do a full collection
     gc.collect()
+    core.gc()
 
 cast = unary
 Var.cast = Var.cast
 
 def array(data, dtype=None):
     ''' Constructs a jittor Var from a number, List, numpy array or another jittor Var.
 
@@ -839,14 +840,17 @@
         jt.Var([[-0.33272865 -0.4951588   1.4128606   0.13734372]
                 [-1.633469    0.19593953 -0.7803732  -0.5260756 ]], dtype=float32)
         >>> a.argmax(dim=0)
         (jt.Var([0 1 0 0], dtype=int32), jt.Var([-0.33272865  0.19593953  1.4128606   0.13734372], dtype=float32))
         >>> a.argmax(dim=1)
         (jt.Var([2 1], dtype=int32), jt.Var([1.4128606  0.19593953], dtype=float32))
     '''
+    if dim is None:
+        dim = 0
+        x = x.flatten()
     return jt.arg_reduce(x, "max", dim, keepdims)
 Var.argmax = argmax
 
 def argmin(x, dim: int, keepdims:bool=False):
     ''' Returns the indices and values of the minimum elements along the specified dimension.
 
     :param x: the input Var.
@@ -1283,14 +1287,16 @@
             dc = v.__dict__
             if isinstance(v, nn.ParameterList):
                 dc = v.params
             for k2, p in dc.items():
                 if isinstance(k2, str) and k2.startswith("_"): continue
                 if isinstance(p, Var):
                     if id(p) in uniq_set: continue
+                    if not getattr(p, "persistent", True):
+                        continue
                     uniq_set.add(id(p))
                     pname = ".".join(stack[1:]+[str(k2)])
                     ps[pname] = p
                     if len(pname) > len(p.name()):
                         p.name(pname)
         def callback_leave(parents, k, v, n):
             stack.pop()
@@ -1706,15 +1712,16 @@
 
     def __setattr__(self, key, value):
         object.__setattr__(self, key, value)
 
     def __getattr__(self, key):
         return object.__getattribute__(self, key)
 
-    def register_buffer(self, key, value):
+    def register_buffer(self, key, value, persistent=True):
+        value.persistent = persistent
         object.__setattr__(self, key, value)
         return value
 
     def float64(self):
         '''convert all parameters to float16'''
         self._amp_level = 0
         for p in self.parameters():
@@ -1813,14 +1820,16 @@
     d.stop_grad()
     da, db = jt.grad(c+d*3, [a, b])
     assert da.data == 4
     assert db.data == 0
 
     '''
     def __call__(self, *args):
+        if flags.no_grad:
+            return self.execute(*args)
         backup = args
         args = list(args)
         taped_inputs = []
         taped_outputs = []
         input_mask = [-1] * len(args)
         for i,v in enumerate(args):
             if isinstance(v, Var):
@@ -2087,7 +2096,9 @@
     new_k = k+"_"
     if hasattr(Var, new_k): continue
     def inplace_wrapper(new_k, prev_func):
         setattr(Var, new_k, lambda x, *args, **kw: x.assign(prev_func(x, *args, **kw)))
     inplace_wrapper(new_k, v)
 
 from . import math_util
+from .math_util import *
+from . import distributions
```

### Comparing `jittor-1.3.7.9/python/jittor/__init__.pyi` & `jittor-1.3.8.1/python/jittor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/attention.py` & `jittor-1.3.8.1/python/jittor/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/ccl/ccl_2d.py` & `jittor-1.3.8.1/python/jittor/ccl/ccl_2d.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/ccl/ccl_3d.py` & `jittor-1.3.8.1/python/jittor/ccl/ccl_3d.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/ccl/ccl_link.py` & `jittor-1.3.8.1/python/jittor/ccl/ccl_link.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/compile_extern.py` & `jittor-1.3.8.1/python/jittor/compile_extern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os, sys, shutil
 import platform
 from .compiler import *
@@ -515,15 +515,15 @@
     global mpicc_path, has_mpi
     use_mpi = os.environ.get("use_mpi", "1")=="1"
     mpi_ops = None
     mpi = None
     has_mpi = False
     mpicc_path = env_or_try_find('mpicc_path', 'mpicc')
     if mpicc_path == "":
-        LOG.i("mpicc not found, distribution disabled.")
+        # LOG.i("mpicc not found, distribution disabled.")
         use_mpi = False
     else:
         use_mpi = True
         has_mpi = True
     if not use_mpi:
         return
```

### Comparing `jittor-1.3.7.9/python/jittor/compiler.py` & `jittor-1.3.8.1/python/jittor/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import subprocess as sp
 import os
 import re
@@ -1361,19 +1361,21 @@
 
 flags = core.Flags()
 
 if has_cuda and is_cuda:
     nvcc_flags = " " + os.environ.get("nvcc_flags", "") + " "
     nvcc_flags += convert_nvcc_flags(cc_flags)
     nvcc_version = list(jit_utils.get_int_version(nvcc_path))
-    max_arch = 86
+    max_arch = 89
     if nvcc_version < [11,]:
         max_arch = 75
     elif nvcc_version < [11,1]:
         max_arch = 80
+    elif nvcc_version < [11,8]:
+        max_arch = 86
     if len(flags.cuda_archs):
         min_arch = 30
         archs = []
         for arch in flags.cuda_archs:
             if arch<min_arch:
                 LOG.w(f"CUDA arch({arch})<{min_arch} is not supported")
                 continue
```

### Comparing `jittor-1.3.7.9/python/jittor/contrib.py` & `jittor-1.3.8.1/python/jittor/contrib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/dataset/cifar.py` & `jittor-1.3.8.1/python/jittor/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/dataset/dataset.py` & `jittor-1.3.8.1/python/jittor/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/dataset/mnist.py` & `jittor-1.3.8.1/python/jittor/dataset/mnist.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/dataset/sampler.py` & `jittor-1.3.8.1/python/jittor/dataset/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Hao-Yang Peng
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/dataset/utils.py` & `jittor-1.3.8.1/python/jittor/dataset/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>.
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/dataset/voc.py` & `jittor-1.3.8.1/python/jittor/dataset/voc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/demo/simple_cgan.py` & `jittor-1.3.8.1/python/jittor/demo/simple_cgan.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/depthwise_conv.py` & `jittor-1.3.8.1/python/jittor/depthwise_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/distributions.py` & `jittor-1.3.8.1/python/jittor/distributions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import math
+import os
 import numpy as np
 import jittor as jt
+from jittor import nn
 from jittor.nn import binary_cross_entropy_with_logits
+from jittor import lgamma, igamma
+from jittor.math_util.gamma import gamma_grad, sample_gamma
 
 def simple_presum(x):
     src = '''
 __inline_static__
 @python.jittor.auto_parallel(1)
 void kernel(int n0, int i0, in0_type* x, in0_type* out, int nl) {
     out[i0*(nl+1)] = 0;
@@ -134,14 +138,44 @@
     def log_prob(self, x):
         return x*jt.safe_log(-self.prob+1)+jt.safe_log(self.prob)
     
     def entropy(self):
         return binary_cross_entropy_with_logits(jt.array(self.logits),jt.array(self.prob)) / self.prob
 
 
+class GammaDistribution:
+    '''
+    For now only support gamma distribution.
+    '''
+    def __init__(self, concentration, rate):
+        self.concentration = concentration
+        self.rate = rate
+        self.lgamma_alpha = lgamma.apply(jt.array([concentration,]))
+
+    def sample(self, shape):
+        return sample_gamma(self.concentration, shape)
+    
+    def cdf(self, value):
+        return igamma(self.concentration, value)
+    
+    def log_prob(self, value):
+        return (self.concentration * jt.log(self.rate) +
+                (self.concentration - 1) * jt.log(value) -
+                self.rate * value - self.lgamma_alpha)
+    
+    def mean(self):
+        return self.concentration / self.rate
+    
+    def mode(self):
+        return np.minimum((self.concentration - 1) / self.rate, 1)
+    
+    def variance(self):
+        return self.concentration / (self.rate * self.rate)
+
+
 def kl_divergence(cur_dist, old_dist):
     assert isinstance(cur_dist, type(old_dist))
     if isinstance(cur_dist, Normal):
         vr = (cur_dist.sigma / old_dist.sigma)**2
         t1 = ((cur_dist.mu - old_dist.mu) / old_dist.sigma)**2
         return 0.5*(vr+t1-1-jt.safe_log(vr))
     if isinstance(cur_dist, Categorical) or isinstance(cur_dist,OneHotCategorical):
```

### Comparing `jittor-1.3.7.9/python/jittor/einops/_backends.py` & `jittor-1.3.8.1/python/jittor/einops/_backends.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/einops.py` & `jittor-1.3.8.1/python/jittor/einops/einops.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/experimental/indexing.py` & `jittor-1.3.8.1/python/jittor/einops/experimental/indexing.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/layers/__init__.py` & `jittor-1.3.8.1/python/jittor/einops/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/layers/_einmix.py` & `jittor-1.3.8.1/python/jittor/einops/layers/_einmix.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/layers/jittor.py` & `jittor-1.3.8.1/python/jittor/einops/layers/jittor.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/einops/parsing.py` & `jittor-1.3.8.1/python/jittor/einops/parsing.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/acl/acl_compiler.py` & `jittor-1.3.8.1/python/jittor/extern/acl/acl_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os
 from jittor_utils import env_or_try_find
 import jittor_utils
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/acl/acl_error_code.cc` & `jittor-1.3.8.1/python/jittor/extern/acl/acl_error_code.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 #include "common.h"
 using std::string;
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/acl/acl_jittor.cc` & `jittor-1.3.8.1/python/jittor/extern/acl/acl_jittor.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "acl_jittor.h"
 #include "utils/str_utils.h"
 #include <chrono>
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/acl/acl_jittor.h` & `jittor-1.3.8.1/python/jittor/extern/acl/acl_jittor.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include <acl/acl.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/corex/corex_compiler.py` & `jittor-1.3.8.1/python/jittor/extern/corex/corex_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os
 from jittor_utils import env_or_try_find
 import jittor_utils
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/inc/cub_test.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/inc/cub_test.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -101,15 +101,15 @@
     d_temp_storage = exe.temp_allocator->alloc(temp_storage_bytes, allocation);
     // Run sorting operation
     cub::DeviceSegmentedReduce::@FUNC@@(d_temp_storage, temp_storage_bytes,
         xp, d_out, num_segments, offsetsp, offsetsp + 1);
 
     auto* __restrict__ yp = y->ptr<int>();
     auto* __restrict__ y_keyp = y_key->ptr<Tx>();
-    split<<<max(1,num_segments/1024),1024>>>(d_out, y_keyp, yp, num_segments);
+    split<<<std::max(1,num_segments/1024),1024>>>(d_out, y_keyp, yp, num_segments);
 
     exe.temp_allocator->free(d_temp_storage, temp_storage_bytes, allocation);
     exe.temp_allocator->free(d_out, sizeof(cub::KeyValuePair<int, Tx>) * num_segments, allocation_dout);
 }
 #endif // JIT_cuda
 #endif // JIT
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_test_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_test_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_where_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_where_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Xiangli Li <1905692338@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cub/ops/cub_where_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cub/ops/cub_where_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Xiangli Li <1905692338@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Meng-Hao Guo <guomenghao1997@gmail.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -98,14 +98,18 @@
 #else // JIT
 #ifdef JIT_cuda
 #pragma clang diagnostic ignored "-Wtautological-compare"
 void CublasBatchedMatmulOp::jit_run() {
     cublasHandle_t& handle_ = cublas_handle;
     const T alpha = 1.0f;
     const T beta  = 0.0f;
+    const float alpha_f = 1.0f;
+    const float beta_f  = 0.0f;
+    void* alpha_p = (void*)&alpha;
+    void* beta_p = (void*)&beta;
 
     const auto& as = a->shape;
     const auto& bs = b->shape;
     auto adim = as.size();
     auto batch_size = as[0];
     for (int i=1; i<adim-2; i++)
         batch_size *= as[i];
@@ -128,15 +132,20 @@
     } else if (use_tensorcore==2) {
         computeType = CUBLAS_COMPUTE_32F_FAST_16BF;
     } else if (use_tensorcore==1) {
         computeType = CUBLAS_COMPUTE_32F_FAST_TF32;
     }
     if (a->dtype() == ns_float16
         || b->dtype() == ns_float16 || c->dtype() == ns_float16) {
-        computeType = CUBLAS_COMPUTE_16F;
+        computeType = use_tensorcore ? CUBLAS_COMPUTE_16F : CUBLAS_COMPUTE_32F;
+        algo = use_tensorcore ? CUBLAS_GEMM_DEFAULT : CUBLAS_GEMM_DEFAULT_TENSOR_OP;
+    }
+    if (computeType == CUBLAS_COMPUTE_32F) {
+        alpha_p = (void*)&alpha_f;
+        beta_p = (void*)&beta_f;
     }
     #else 
     cublasGemmAlgo_t algo = CUBLAS_GEMM_DEFAULT;
     cudaDataType_t computeType = CUDA_R_32F;
     if (use_tensorcore) {
         algo = CUBLAS_GEMM_DEFAULT_TENSOR_OP;
     }
@@ -144,17 +153,17 @@
         || b->dtype() == ns_float16 || c->dtype() == ns_float16) {
         computeType = CUDA_R_16F;
         algo = CUBLAS_GEMM_DEFAULT_TENSOR_OP;
     }
     #endif
     checkCudaErrors(cublasGemmStridedBatchedEx(handle_,
     CUBLAS_OP_@Trans_b, CUBLAS_OP_@Trans_a,
-    k, n, m, &alpha,
+    k, n, m, alpha_p,
     b->ptr<T>(),get_dtype(b->dtype()), '@Trans_b' == 'N' ? k : m, k * m, 
-    a->ptr<T>(),get_dtype(a->dtype()), '@Trans_a' == 'N' ? m : n, n * m, &beta,
+    a->ptr<T>(),get_dtype(a->dtype()), '@Trans_a' == 'N' ? m : n, n * m, beta_p,
     c->ptr<T>(),get_dtype(c->dtype()), k, k * n,
     batch_size,computeType,algo));
     // checkCudaErrors(cublas@op@@gemmStridedBatched(handle_,
     // CUBLAS_OP_@Trans_b, CUBLAS_OP_@Trans_a,
     // k, n, m, &alpha,
     // b->ptr<T>(), '@Trans_b' == 'N' ? k : m, k * m, 
     // a->ptr<T>(), '@Trans_a' == 'N' ? m : n, n * m, &beta,
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Meng-Hao Guo <guomenghao1997@gmail.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -59,14 +59,18 @@
 #else // JIT
 #pragma clang diagnostic ignored "-Wtautological-compare"
 
 void CublasMatmulOp::jit_run() {
     cublasHandle_t& handle_ = cublas_handle;
     const T alpha = 1.0f;
     const T beta  = 0.0f;
+    const float alpha_f = 1.0f;
+    const float beta_f  = 0.0f;
+    void* alpha_p = (void*)&alpha_f;
+    void* beta_p = (void*)&beta_f;
 
     const auto& as = a->shape;
     const auto& bs = b->shape;
     auto n = as[0];
     auto m = as[1];
     auto k = bs[1];
     if ('@Trans_a'=='T') {
@@ -85,15 +89,20 @@
     } else if (use_tensorcore==2) {
         computeType = CUBLAS_COMPUTE_32F_FAST_16BF;
     } else if (use_tensorcore==1) {
         computeType = CUBLAS_COMPUTE_32F_FAST_TF32;
     }
     if (a->dtype() == ns_float16
         || b->dtype() == ns_float16 || c->dtype() == ns_float16) {
-        computeType = CUBLAS_COMPUTE_16F;
+        computeType = use_tensorcore ? CUBLAS_COMPUTE_16F : CUBLAS_COMPUTE_32F;
+        algo = use_tensorcore ? CUBLAS_GEMM_DEFAULT : CUBLAS_GEMM_DEFAULT_TENSOR_OP;
+    }
+    if (computeType == CUBLAS_COMPUTE_32F) {
+        alpha_p = (void*)&alpha_f;
+        beta_p = (void*)&beta_f;
     }
     #else
     cublasGemmAlgo_t algo = CUBLAS_GEMM_DEFAULT;
     cudaDataType_t computeType = get_dtype(c->dtype());
     if (use_tensorcore) {
         algo = CUBLAS_GEMM_DEFAULT_TENSOR_OP;
     }
@@ -101,17 +110,17 @@
         || b->dtype() == ns_float16 || c->dtype() == ns_float16) {
         computeType = CUDA_R_16F;
         algo = CUBLAS_GEMM_DEFAULT_TENSOR_OP;
     }
     #endif
     checkCudaErrors(cublasGemmEx(handle_, 
     CUBLAS_OP_@Trans_b, CUBLAS_OP_@Trans_a, 
-    k, n, m, &alpha, 
+    k, n, m, alpha_p, 
     b->ptr<T>(),get_dtype(b->dtype()), '@Trans_b' == 'N' ? k : m, 
-    a->ptr<T>(),get_dtype(a->dtype()), '@Trans_a' == 'N' ? m : n, &beta, 
+    a->ptr<T>(),get_dtype(a->dtype()), '@Trans_a' == 'N' ? m : n, beta_p, 
     c->ptr<T>(),get_dtype(c->dtype()), k,
     computeType, algo));
     // checkCudaErrors(cublas@op@@gemm(handle_, 
     // CUBLAS_OP_@Trans_b, CUBLAS_OP_@Trans_a, 
     // k, n, m, &alpha, 
     // b->ptr<T>(), '@Trans_b' == 'N' ? k : m, 
     // a->ptr<T>(), '@Trans_a' == 'N' ? m : n, &beta,
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cublas/src/helper_cublas.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cublas/src/helper_cublas.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <cuda_runtime.h>
 #include <cudnn.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "cudnn_conv3d_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "cudnn_conv_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "cudnn_rnn_descriptor.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "cudnn_rnn_descriptor.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //      Zheng-Ning Liu <lzhengning@gmail.com>
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "cudnn_rnn_descriptor.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "cudnn_wrapper.h"
 #include "misc/cuda_flags.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cufft/inc/cufft_utils.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cufft/inc/cufft_utils.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/curand/inc/curand_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/curand/inc/curand_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/curand/ops/curand_random_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/curand/ops/curand_random_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/curand/ops/curand_random_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/curand/ops/curand_random_op.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/curand/src/curand_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/curand/src/curand_wrapper.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/curand/src/helper_curand.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/curand/src/helper_curand.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     for (; i<axes.size(); i++)
         if (i!=axes[i]) break;
     if (i==axes.size() && axes.size()) {
         forward(x);
         return;
     }
     y = create_output(nullptr, x->dtype());
+    flags.set(NodeFlags::_manual_set_vnbb);
 }
 
 void CuttTransposeOp::infer_shape() {
     auto xdim = x->shape.size();
     CHECK(xdim);
     if (!axes.size()) {
         for (int i=0; i<(int)xdim; i++)
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/fp16_dev.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/fp16_dev.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/fp16_emu.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/fp16_emu.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_cuda.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_cuda.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_functions.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_functions.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_image.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_image.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_string.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_string.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/inc/helper_timer.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/inc/helper_timer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.
+// Copyright (c) 2023 Jittor.
 // All Rights Reserved. 
 // Maintainers:
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 
 namespace jittor {
 
-struct NcclBroadcastOp : Op {
+struct NcclReduceOp : Op {
     Var* x, * y;
     int root;
 
-    NcclBroadcastOp(Var* x, int root=0);
+    NcclReduceOp(Var* x, int root=0);
     void infer_shape() override;
     
-    const char* name() const override { return "nccl_broadcast"; }
+    const char* name() const override { return "nccl_reduce"; }
     VarPtr grad(Var* out, Var* dout, Var* v, int v_index) override;
     DECLARE_jit_run;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guoye Yang <498731903@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 
 namespace jittor {
 
-struct NcclReduceOp : Op {
+struct NcclBroadcastOp : Op {
     Var* x, * y;
     int root;
 
-    NcclReduceOp(Var* x, int root=0);
+    NcclBroadcastOp(Var* x, int root=0);
     void infer_shape() override;
     
-    const char* name() const override { return "nccl_reduce"; }
+    const char* name() const override { return "nccl_broadcast"; }
     VarPtr grad(Var* out, Var* dout, Var* v, int v_index) override;
     DECLARE_jit_run;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.
+// Copyright (c) 2023 Jittor.
 // All Rights Reserved. 
 // Maintainers:
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.
+// Copyright (c) 2023 Jittor.
 // All Rights Reserved. 
 // Maintainers:
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/src/fp16_dev.cu` & `jittor-1.3.8.1/python/jittor/extern/cuda/src/fp16_dev.cu`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/src/fp16_emu.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/src/fp16_emu.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/cuda/src/helper_cuda.cc` & `jittor-1.3.8.1/python/jittor/extern/cuda/src/helper_cuda.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc` & `jittor-1.3.8.1/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_op.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 
 namespace jittor {
 
-struct MklConvBackwardXOp : Op {
-    Var* w, * dy, * dx;
-    int xh, xw, strideh, stridew, paddingh, paddingw, dilationh, dilationw, groups;
+struct MklConvOp : Op {
+    Var* x, * w, * y;
+    int strideh, stridew, paddingh, paddingw, dilationh, dilationw, groups;
     string xformat, wformat, yformat;
-
-    MklConvBackwardXOp(Var* w, Var* y, int height, int width, int strideh, int stridew, int paddingh, int paddingw, int dilationh, int dilationw, int groups=1, string xformat="abcd", string wformat="oihw", string yformat="abcd");
+    /* MklConvOp: xformat abcd represents nchw */
+    MklConvOp(Var* x, Var* w, int strideh, int stridew, int paddingh, int paddingw, int dilationh=1, int dilationw=1, int groups=1, string xformat="abcd", string wformat="oihw", string yformat="");
     
-    const char* name() const override { return "mkl_conv_backward_x"; }
+    const char* name() const override { return "mkl_conv"; }
     void infer_shape() override;
     DECLARE_jit_run;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_conv_op.h` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 
 namespace jittor {
 
-struct MklConvOp : Op {
-    Var* x, * w, * y;
-    int strideh, stridew, paddingh, paddingw, dilationh, dilationw, groups;
+struct MklConvBackwardXOp : Op {
+    Var* w, * dy, * dx;
+    int xh, xw, strideh, stridew, paddingh, paddingw, dilationh, dilationw, groups;
     string xformat, wformat, yformat;
-    /* MklConvOp: xformat abcd represents nchw */
-    MklConvOp(Var* x, Var* w, int strideh, int stridew, int paddingh, int paddingw, int dilationh=1, int dilationw=1, int groups=1, string xformat="abcd", string wformat="oihw", string yformat="");
+
+    MklConvBackwardXOp(Var* w, Var* y, int height, int width, int strideh, int stridew, int paddingh, int paddingw, int dilationh, int dilationw, int groups=1, string xformat="abcd", string wformat="oihw", string yformat="abcd");
     
-    const char* name() const override { return "mkl_conv"; }
+    const char* name() const override { return "mkl_conv_backward_x"; }
     void infer_shape() override;
     DECLARE_jit_run;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_matmul_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_matmul_op.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_matmul_op.h` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_matmul_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_test_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mkl/ops/mkl_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/mkl/ops/mkl_test_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/inc/mpi_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/mpi/inc/mpi_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.
+// Copyright (c) 2023 Jittor.
 // All Rights Reserved. 
 // Maintainers:
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mpi_wrapper.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mpi_wrapper.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_broadcast_op.h` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_broadcast_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_reduce_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mpi_wrapper.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_reduce_op.h` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_reduce_op.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Guowei Yang <471184555@qq.com>. 
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_test_op.cc` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/ops/mpi_test_op.h` & `jittor-1.3.8.1/python/jittor/extern/mpi/ops/mpi_test_op.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.  
+// Copyright (c) 2023 Jittor. All Rights Reserved.  
 //     Dun Liang <randonlang@gmail.com>. 
 // All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/mpi/src/mpi_wrapper.cc` & `jittor-1.3.8.1/python/jittor/extern/mpi/src/mpi_wrapper.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.
+// Copyright (c) 2023 Jittor.
 // All Rights Reserved. 
 // Maintainers:
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/extern/rocm/rocm_cache.tar.gz` & `jittor-1.3.8.1/python/jittor/extern/rocm/rocm_cache.tar.gz`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/rocm/rocm_compiler.py` & `jittor-1.3.8.1/python/jittor/extern/rocm/rocm_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/rocm/rocm_config.cc` & `jittor-1.3.8.1/python/jittor/extern/rocm/rocm_config.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/rocm/rocm_jittor.h` & `jittor-1.3.8.1/python/jittor/extern/rocm/rocm_jittor.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/extern/rocm/rocm_wrapper.h` & `jittor-1.3.8.1/python/jittor/extern/rocm/rocm_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/init.py` & `jittor-1.3.8.1/python/jittor/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/init_cupy.py` & `jittor-1.3.8.1/python/jittor/init_cupy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/linalg.py` & `jittor-1.3.8.1/python/jittor/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/loss3d/chamfer.py` & `jittor-1.3.8.1/python/jittor/loss3d/chamfer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/loss3d/emd.py` & `jittor-1.3.8.1/python/jittor/loss3d/emd.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/lr_scheduler.py` & `jittor-1.3.8.1/python/jittor/lr_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/math_util/gamma.py` & `jittor-1.3.8.1/python/jittor/math_util/gamma.py`

 * *Files 21% similar despite different names*

```diff
@@ -337,8 +337,80 @@
             return dx
         else:
             return jt.code(x.shape, x.dtype, [x], cpu_header=self.cpu_header, cpu_src=self.cpu_src)
     
     def grad(self, grad_d):
         return grad_d * polygamma.apply(self.input, 1)
 
+def gamma_grad(x, alpha):
+    cuda_header = open(os.path.join(os.path.realpath(os.path.dirname(__file__)), "src", "gamma_grad.h"), "r").read()
+    cuda_src = '''
+    @alias(x, in0)
+    @alias(di_x, out0)
+    int block_num = x_stride0 == 1 ? 1 : x_shape0;
+    int batch_shape = x_stride0 == 1 ? x_shape0: x_stride0;
+    float alpha = data["alpha"];
+    gamma_grad_kenrel<<<block_num, 16>>>(x_p, di_x_p, alpha, batch_shape);
+    '''
+    grad = jt.code(x.shape, x.dtype, [x], cuda_header=cuda_header, cuda_src=cuda_src, data={"alpha":alpha})
+    return grad
 
+def sample_gamma(alpha, shape):
+    cuda_header = '''
+    #include <curand_kernel.h>
+
+    template<typename scalar_t, typename accscalar_t>
+    __device__ float sample_gamma(float alpha, curandState& state) {
+        accscalar_t scale = 1.0f;
+
+        // Boost alpha for higher acceptance probability.
+        if (alpha < 1.0f) {
+            if (alpha == 0.f) return 0.f;
+            scale *= pow(1 - curand_uniform(&state), 1.0f / alpha);
+            alpha += 1.0f;
+        }
+
+        // This implements the acceptance-rejection method of Marsaglia and Tsang (2000)
+        // doi:10.1145/358407.358414
+        const accscalar_t d = alpha - 1.0f / 3.0f;
+        const accscalar_t c = 1.0f / sqrt(9.0f * d + 1e-8);
+        for (;;) {
+            accscalar_t x, y;
+            do {
+            x = curand_normal(&state);
+            y = 1.0f + c * x;
+            } while (y <= 0);
+            const accscalar_t v = y * y * y;
+            const accscalar_t u = 1 - curand_uniform(&state);
+            const accscalar_t xx = x * x;
+            if (u < 1.0f - 0.0331f * xx * xx)
+                return static_cast<scalar_t>(scale * d * v);
+            if (log(u) < 0.5f * xx + d * (1.0f - v + log(v)))
+                return static_cast<scalar_t>(scale * d * v);
+        }
+    }
+
+    __global__ void sample_gamma_kernel(float* out,
+                            float alpha,
+                            int seed,
+                            int batch_shape) 
+    {
+        int tidx = threadIdx.x;
+        int start = batch_shape / blockDim.x * tidx;
+        int end = threadIdx.x == blockDim.x - 1 ? batch_shape : start + batch_shape / blockDim.x;
+        if(start > end) 
+            return;
+        float* bout = out + batch_shape * blockIdx.x;
+        curandState state;
+        curand_init(clock64(), threadIdx.x, 0, &state);
+        for(int i=start;i<end;i++) bout[i] = sample_gamma<float, float>(alpha, state);
+    }
+    '''
+    cuda_src = '''
+    @alias(lx ,out0)
+    int batch_size = lx_stride0 == 1 ? 1 : lx_shape0;
+    int batch_shape = lx_shape0 * lx_stride0 / batch_size;
+    float alpha = data["alpha"];
+    sample_gamma_kernel<<<batch_size, 16>>>(lx_p, alpha, time(NULL), batch_shape);
+    '''
+    samples = jt.code(shape, jt.float32, [], cuda_header=cuda_header, cuda_src=cuda_src, data={"alpha":alpha})
+    return samples
```

### Comparing `jittor-1.3.7.9/python/jittor/misc.py` & `jittor-1.3.8.1/python/jittor/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Dun Liang <randonlang@gmail.com>.
 #   Wenyang Zhou <576825820@qq.com>
 #   Guoye Yang <498731903@qq.com>
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
@@ -2001,17 +2001,31 @@
 jt.Var.isposinf = isposinf
 
 # fake torch interface
 def contiguous(x): return x.clone()
 jt.Var.contiguous = contiguous
 def cpu(x): return x.clone()
 jt.Var.cpu = cpu
-def to(x, *args, **kargs): return x.clone()
+def to(x, *args, **kargs):
+    if len(args) >= 1:
+        s = args[0]
+        if isinstance(s, jt.NanoString) or callable(s):
+            return x.cast(s)
+        s = str(s)
+        if "cuda" in s:
+            jt.flags.use_cuda = 1
+        elif "cpu" in s:
+            jt.flags.use_cuda = 0
+    return x.clone()
 jt.Var.to = to
 
+def rsqrt(x):
+    return 1/jt.sqrt(x)
+jt.Var.rsqrt = rsqrt
+
 def from_torch(x):
     '''
     Convert torch Tensor to Jittor Var
     '''
     return jt.Var(x.cpu().numpy())
 
 def triu(input: jt.Var, diagonal:int=0) -> jt.Var:
@@ -2132,8 +2146,62 @@
         assert num_samples <= weights.shape[-1], "num_samples larger than the input"
         # prevent rand generate 1, 1^inf = 1, with override other result
         a = jt.rand(weights.shape).minimum(0.999999)
         rand = a ** (1/weights)
         _, indices = jt.topk(rand, num_samples)
         return indices
 
+def histc(input, bins, min=0., max=0.):
+    ''' Return the histogram of the input N-d array.
+
+    :param input: the input array.
+    :param bins: number of bins.
+    :param min: min of the range.
+    :param max: max of the range.
+
+    Example::
+
+        inputs = jt.randn((40,40))
+        joup = jt.histc(x, bins=10)
+        
+    '''
+    if min == 0 and max == 0:
+        min, max = input.min(), input.max()
+    assert min < max
+    bin_length = (max - min) / bins
+    histc = jt.floor((input[jt.logical_and(input >= min, input <= max)] - min) / bin_length).int().reshape(-1)
+    hist = jt.ones_like(histc).float().reindex_reduce("add", [bins,], ["@e0(i0)"], extras=[histc])
+    if hist.sum() != histc.shape[0]:
+        hist[-1] += 1
+    return hist
+
+def peek_s(x):
+    if isinstance(x, jt.Var):
+        return x.peek()
+    if isinstance(x, (list, tuple)):
+        res = "["
+        for a in x:
+            res += peek_s(a)
+            res += ", "
+        res += "]"
+        return res
+    if isinstance(x, dict):
+        res = "{"
+        for a in x:
+            res += a
+            res += ":"
+            res += peek_s(x[a])
+            res += ", "
+        res += "}"
+        return res
+    if isinstance(x, str):
+        return x
+    return x.__class__.__name__
+
+def peek(x):
+    print(peek_s(x))
+
+def finfo(dtype):
+    return np.finfo(str(dtype).split('.')[-1])
 
+def iinfo(dtype):
+    return np.iinfo(str(dtype).split('.')[-1])
```

### Comparing `jittor-1.3.7.9/python/jittor/models/__init__.py` & `jittor-1.3.8.1/python/jittor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/models/alexnet.py` & `jittor-1.3.8.1/python/jittor/models/alexnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/densenet.py` & `jittor-1.3.8.1/python/jittor/models/densenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/googlenet.py` & `jittor-1.3.8.1/python/jittor/models/googlenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/inception.py` & `jittor-1.3.8.1/python/jittor/models/inception.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/models/mnasnet.py` & `jittor-1.3.8.1/python/jittor/models/mnasnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/mobilenet.py` & `jittor-1.3.8.1/python/jittor/models/mobilenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/res2net.py` & `jittor-1.3.8.1/python/jittor/models/res2net.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/models/resnet.py` & `jittor-1.3.8.1/python/jittor/models/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/models/shufflenetv2.py` & `jittor-1.3.8.1/python/jittor/models/shufflenetv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/squeezenet.py` & `jittor-1.3.8.1/python/jittor/models/squeezenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/models/vgg.py` & `jittor-1.3.8.1/python/jittor/models/vgg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/nn.py` & `jittor-1.3.8.1/python/jittor/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guowei Yang <471184555@qq.com>
 #     Guoye Yang <498731903@qq.com>
 #     Wenyang Zhou <576825820@qq.com>
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>.
 #     Zheng-Ning Liu <lzhengning@gmail.com>
@@ -32,15 +32,15 @@
     if len(a.shape) != 2:
         aa = a.reshape((-1, a.shape[-1]))
         cc = matmul_transpose(aa, b)
         return cc.reshape(a.shape[:-1]+(-1,))
     assert len(a.shape) == 2 and len(b.shape) == 2
 
     shape = list(a.shape)[:-1] + list(b.shape)
-    with jt.flag_scope(amp_reg = jt.flags.amp_reg | 4):
+    with jt.flag_scope(amp_reg = jt.flags.amp_reg | 36):
         a = a.broadcast(shape, [len(shape)-2])
         b = b.broadcast(shape)
         return (a*b).sum(len(shape)-1)
 
 
 def bmm_transpose(a, b):
     '''
@@ -110,15 +110,15 @@
     assert c.shape == [10, 3, 5]
 
     a = jt.random([8, 1, 3, 4])
     b = jt.random([10, 4, 5])
     c = jt.matmul(a, b)
     assert c.shape == [8, 10, 3, 5]
     '''
-    with jt.flag_scope(amp_reg = jt.flags.amp_reg | 4):
+    with jt.flag_scope(amp_reg = jt.flags.amp_reg | 36):
         len_a = len(a.shape)
         len_b = len(b.shape)
         if len_b == 1:
             # a: [n, m], b:[m], c:[n]
             return (a*b).sum(-1)
         if len_a == 1:
             # a: [n], b:[n,k], c:[k]
@@ -375,15 +375,15 @@
     target_shape = target.shape
     if len(output.shape) == 4:
         c_dim = output.shape[1]
         output = output.transpose((0, 2, 3, 1))
         output = output.reshape((-1, c_dim))
 
     target = target.reshape((-1, ))
-    target_weight = jt.ones(target.shape[0], dtype='float32')
+    target_weight = ((target >= 0) & (target < output.shape[1])).float32() 
     if weight is not None:
         target_weight = weight[target]
     if ignore_index is not None:
         target_weight = jt.ternary(
             target==ignore_index,
             jt.array(0).broadcast(target_weight),
             target_weight
@@ -956,15 +956,15 @@
         elif self.groups == 1:
             N,C,H,W = x.shape
             Kh, Kw = self.kernel_size
             assert C==self.in_channels
             oh = (H+self.padding[0]*2-Kh*self.dilation[0]+self.dilation[0]-1)//self.stride[0]+1
             ow = (W+self.padding[1]*2-Kw*self.dilation[1]+self.dilation[1]-1)//self.stride[1]+1
             assert oh>0 and ow>0
-            with jt.flag_scope(amp_reg = jt.flags.amp_reg | 4):
+            with jt.flag_scope(amp_reg = jt.flags.amp_reg | 36):
                 xx = x.reindex([N,self.out_channels,C,oh,ow,Kh,Kw], [
                     'i0', # Nid
                     'i2', # Cid
                     f'i3*{self.stride[0]}-{self.padding[0]}+i5*{self.dilation[0]}', # Hid+Khid
                     f'i4*{self.stride[1]}-{self.padding[1]}+i6*{self.dilation[1]}', # Wid+KWid
                 ])
                 ww = self.weight.broadcast(xx.shape, [0,3,4])
@@ -1185,15 +1185,15 @@
     out_channels = weight.shape[0]
 
     if groups == 1:
         N,C,H,W = x.shape
         Kh, Kw = weight.shape[-2:]
         oh = (H+padding[0]*2-Kh*dilation[0]+dilation[0]-1)//stride[0]+1
         ow = (W+padding[1]*2-Kw*dilation[1]+dilation[1]-1)//stride[1]+1
-        with jt.flag_scope(amp_reg = jt.flags.amp_reg | 4):
+        with jt.flag_scope(amp_reg = jt.flags.amp_reg | 36):
             xx = x.reindex([N,out_channels,C,oh,ow,Kh,Kw], [
                     'i0', # Nid
                     'i2', # Cid
                     f'i3*{stride[0]}-{padding[0]}+i5*{dilation[0]}', # Hid+Khid
                     f'i4*{stride[1]}-{padding[1]}+i6*{dilation[1]}', # Wid+KWid
                 ])
             ww = weight.broadcast(xx.shape, [0,3,4])
@@ -1735,18 +1735,21 @@
             >>> x = jt.int32([1, 2, 3, 3])
             >>> embedding(x)
             jt.Var([[ 1.1128596   0.19169547  0.706642]
              [ 1.2047412   1.9668795   0.9932192]
              [ 0.14941819  0.57047683 -1.3217674]
              [ 0.14941819  0.57047683 -1.3217674]], dtype=float32)
     '''
-    def __init__(self, num_embeddings, embedding_dim, dtype="float32"):
-        self.num = num_embeddings
-        self.dim = embedding_dim
-        self.weight = jt.init.gauss([self.num, self.dim], dtype).stop_grad()
+    def __init__(self, num_embeddings, embedding_dim, padding_idx=None, dtype="float32"):
+        self.num_embeddings = num_embeddings
+        self.embedding_dim = embedding_dim
+        self.padding_idx = padding_idx
+        self.weight = jt.init.gauss([self.num_embeddings, self.embedding_dim], dtype).stop_grad()
+        if padding_idx is not None:
+            self.weight[padding_idx] = 0
 
     def execute(self, x):
         res = self.weight[x]
         return res
 
 def embedding(input, weight):
     return weight[input]
@@ -2943,14 +2946,179 @@
     assert(len(x.shape) == 4)
     assert(x.shape[3] == 2)
     y = jt.compile_extern.cufft_ops.cufft_fft(x, inverse)
     if inverse:
         y /= x.shape[1] * x.shape[2]
     return y
 
+class ComplexNumber:
+    ''' Applys Complex number class.
+
+        It's saved as jt.stack(real, imag, dim=-1)
+
+        You can construct ComplexNumber with real part and imaginary part like ComplexNumber(real, imag)
+        or real part only with ComplexNumber(real)
+        or value after jt.stack with ComplexNumber(value, is_concat_value=True)
+
+        add, sub, mul and truediv between ComplexNumber and ComplexNumber, jt.Var, int, float are implemented
+
+        You can use 'shape', 'reshape' etc. as jt.Var
+
+    Example:
+        >>> real = jt.array([[[1., -2., 3.]]])
+        >>> imag = jt.array([[[0., 1., 6.]]])
+        >>> a = ComplexNumber(real, imag)
+        >>> a + a
+        >>> a / a
+        >>> a.norm()                # sqrt(real^2+imag^2)
+        >>> a.exp()                 # e^real(cos(imag)+isin(imag))
+        >>> a.conj()                # ComplexNumber(real, -imag)
+        >>> a.fft2()                # cuda only now. len(real.shape) equals 3
+        >>> a.ifft2()               # cuda only now. len(real.shape) equals 3
+    '''
+    def __init__(self, real: jt.Var, imag: jt.Var=None, is_concat_value=False):
+        if is_concat_value:
+            assert real.shape[-1] == 2
+            assert imag is None
+            self.value = real
+        elif imag is None:
+            self.value = jt.stack([real, jt.zeros_like(real)], dim=-1)
+        else:
+            assert real.shape == imag.shape
+            assert real.dtype == imag.dtype
+            self.value = jt.stack([real, imag], dim=-1)
+
+    @property
+    def real(self):
+        return self.value[..., 0]
+
+    @property
+    def imag(self):
+        return self.value[..., 1]
+
+    @property
+    def shape(self):
+        return self.value.shape[:-1]
+
+    def norm(self):
+        return jt.sqrt(jt.sqr(self.real) + jt.sqr(self.imag))
+
+    def stop_grad(self):
+        return ComplexNumber(self.value.stop_grad(), is_concat_value=True)
+
+    def start_grad(self):
+        return ComplexNumber(self.value.start_grad(), is_concat_value=True)
+    
+    def detach(self):
+        return ComplexNumber(self.value.detach(), is_concat_value=True)
+
+    def unsqueeze(self, dim=0):
+        return ComplexNumber(jt.unsqueeze(self.real, dim=dim), jt.unsqueeze(self.imag, dim=dim))
+
+    def squeeze(self, dim=0):
+        return ComplexNumber(jt.squeeze(self.real, dim=dim), jt.squeeze(self.imag, dim=dim))
+
+    def reshape(self, shape):
+        return ComplexNumber(jt.reshape(self.real, shape), jt.reshape(self.imag, shape))
+    
+    def permute(self, axes):
+        return ComplexNumber(jt.permute(self.real, axes), jt.permute(self.imag, axes))
+
+    def exp(self):
+        er = jt.exp(self.real)
+        return ComplexNumber(er * jt.cos(self.imag), er * jt.sin(self.imag))
+
+    def conj(self):
+        return ComplexNumber(self.real, -self.imag)
+
+    def __add__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(self.real + other.real, self.imag + other.imag)
+        elif isinstance(other, (jt.Var, int, float)):
+            return ComplexNumber(self.real + other, self.imag)
+        else:
+            raise NotImplementedError
+
+    def __radd__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(other.real + self.real, other.imag + self.imag)
+        elif isinstance(other, (jt.Var, int, float)):
+            return ComplexNumber(other + self.real, self.imag)
+        else:
+            raise NotImplementedError
+
+    def __sub__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(self.real - other.real, self.imag - other.imag)
+        elif isinstance(other, (jt.Var, int, float)):
+            return ComplexNumber(self.real - other, self.imag)
+        else:
+            raise NotImplementedError
+
+    def __rsub__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(other.real - self.real, other.imag - self.imag)
+        elif isinstance(other, (jt.Var, int, float)):
+            return ComplexNumber(other - self.real, self.imag)
+        else:
+            raise NotImplementedError
+
+    def __mul__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(self.real * other.real - self.imag * other.imag,
+                                 self.real * other.imag + self.imag * other.real)
+        elif isinstance(other, (int, float)):
+            return ComplexNumber(self.value * other, is_concat_value=True)
+        elif isinstance(other, jt.Var):
+            return ComplexNumber(self.real * other, self.imag * other)
+        else:
+            raise NotImplementedError
+
+    def __rmul__(self, other):
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber(other.real * self.real - other.imag * self.imag,
+                                 other.imag * self.real + other.real * self.imag)
+        elif isinstance(other, (int, float)):
+            return ComplexNumber(other * self.value, is_concat_value=True)
+        elif isinstance(other, jt.Var):
+            return ComplexNumber(other * self.real, other * self.imag)
+        else:
+            raise NotImplementedError
+
+    def __truediv__(self, other):
+        if isinstance(other, ComplexNumber):
+            norm = jt.sqr(other.real) + jt.sqr(other.imag)
+            return ComplexNumber((self.real * other.real + self.imag * other.imag) / norm,
+                                 (self.imag * other.real - self.real * other.imag) / norm)
+        elif isinstance(other, (int, float)):
+            return ComplexNumber(self.value / other, is_concat_value=True)
+        elif isinstance(other, jt.Var):
+            return ComplexNumber(self.real / other, self.imag / other)
+        else:
+            raise NotImplementedError
+
+    def __rtruediv__(self, other):
+        norm = jt.sqr(self.real) + jt.sqr(self.imag)
+        if isinstance(other, ComplexNumber):
+            return ComplexNumber((other.real * self.real + other.imag * self.imag) / norm,
+                                 (other.imag * self.real - other.real * self.imag) / norm)
+        elif isinstance(other, (int, float, jt.Var)):
+            return ComplexNumber(other * self.real / norm, - other * self.imag / norm)
+        else:
+            raise NotImplementedError
+
+    def __repr__(self) -> str:
+        return f'ComplexNumber(real={self.real.__repr__()}, imag={self.imag.__repr__()})'
+    
+    def fft2(self):
+        return ComplexNumber(_fft2(self.value, inverse=False), is_concat_value=True)
+
+    def ifft2(self):
+        return ComplexNumber(_fft2(self.value, inverse=True), is_concat_value=True)
+
 
 def one_hot(x: jt.Var, num_classes: int=-1) -> jt.Var:
     ''' Returns the one_hot encoding of inputs.
 
     :param x: class values of any shape
     :type x: jt.Var with bool or integer dtype
 
@@ -3041,11 +3209,11 @@
 reference: Mish - A Self Regularized Non-Monotonic Neural Activation Function.
         '''
         pass
     def execute(self, x):
         return x * jt.tanh(jt.softplus(x))
 
 def mish(x, inplace=False):
-    return x * jt.tanh(jt.softplus(x))
+    return x * jt.tanh(jt.nn.softplus(x))
 
 def skip_init(module_cls, *args, **kw):
     return module_cls(*args, **kw)
```

### Comparing `jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/mnist.png` & `jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/mnist.png`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb` & `jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb` & `jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb` & `jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb` & `jittor-1.3.8.1/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.md` & `jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/ConditionGAN.src.md` & `jittor-1.3.8.1/python/jittor/notebook/ConditionGAN.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/LSGAN.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/LSGAN.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/LSGAN.md` & `jittor-1.3.8.1/python/jittor/notebook/LSGAN.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/LSGAN.src.md` & `jittor-1.3.8.1/python/jittor/notebook/LSGAN.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/basics.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/basics.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/basics.md` & `jittor-1.3.8.1/python/jittor/notebook/basics.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/basics.src.md` & `jittor-1.3.8.1/python/jittor/notebook/basics.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/custom_op.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/custom_op.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/custom_op.md` & `jittor-1.3.8.1/python/jittor/notebook/custom_op.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/custom_op.src.md` & `jittor-1.3.8.1/python/jittor/notebook/custom_op.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/example.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/example.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/example.md` & `jittor-1.3.8.1/python/jittor/notebook/example.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/example.src.md` & `jittor-1.3.8.1/python/jittor/notebook/example.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/figs/mop.svg` & `jittor-1.3.8.1/python/jittor/notebook/figs/mop.svg`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/md_to_ipynb.py` & `jittor-1.3.8.1/python/jittor/notebook/md_to_ipynb.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/meta_op.cn.md` & `jittor-1.3.8.1/python/jittor/notebook/meta_op.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/meta_op.md` & `jittor-1.3.8.1/python/jittor/notebook/meta_op.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/notebook/meta_op.src.md` & `jittor-1.3.8.1/python/jittor/notebook/meta_op.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/optim.py` & `jittor-1.3.8.1/python/jittor/optim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guowei Yang <471184555@qq.com>
 #     Guoye Yang <498731903@qq.com>
 #     Wenyang Zhou <576825820@qq.com>
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
@@ -463,15 +463,118 @@
                 bias_correction2 = 1 - b1 ** n
                 m.update(b0 * m + (1-b0) * g) #exp_avg
                 v.update(b1 * v + (1-b1) * g * g) #exp_avg_sq
                 denom = jt.sqrt(v) / jt.sqrt(bias_correction2) + eps
                 step_size = lr / bias_correction1
                 p.update(p - step_size * m / denom)
         self.post_step()
+          
 
+class Adan(Optimizer):
+    """ Adan Optimizer.
+    Adan was proposed in
+    Adan: Adaptive Nesterov Momentum Algorithm for
+        Faster Optimizing Deep Models[J].arXiv preprint arXiv:2208.06677, 2022.
+    https://arxiv.org/abs/2208.06677
+    Adan is an efficient optimizer for most DNN frameworks:
+    - About 2x fewer computational load than SOTAs
+    - Robust to training setting and batch size
+    - Easy to Plug-and-play
+
+    Arguments:
+        params (iterable): iterable of parameters to optimize or
+            dicts defining parameter groups.
+        lr (float, optional): learning rate. (default: 1e-3)
+        betas (Tuple[float, float, flot], optional): coefficients used for
+            first- and second-order moments. (default: (0.98, 0.92, 0.99))
+        eps (float, optional): term added to the denominator to improve
+            numerical stability. (default: 1e-8)
+        weight_decay (float, optional): decoupled weight decay
+            (L2 penalty) (default: 0)
+        max_grad_norm (float, optional): value used to clip
+            global grad norm (default: 0.0 no clip)
+    """
+    def __init__(self, params, lr=1e-3, betas=(0.98, 0.92, 0.99),
+                eps=1e-8, weight_decay=0.0, max_grad_norm=0.0):
+        super().__init__(params, lr)
+        self.betas = betas
+        self.eps = eps
+        self.weight_decay = weight_decay
+        self.max_grad_norm = max_grad_norm
+        
+        for pg in self.param_groups:
+            pg["m"] = []
+            pg["v"] = []
+            pg["d"] = []
+            pg["pre_grad"] = []
+            for p in pg["params"]:
+                pg["m"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+                pg["v"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+                pg["d"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+                pg["pre_grad"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+                
+                
+    def add_param_group(self, group):
+        group["m"] = []
+        group["v"] = []
+        group["d"] = []
+        group["pre_grad"] = []
+        for p in group["params"]:
+            group["m"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+            group["v"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+            group["d"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+            group["pre_grad"].append(jt.zeros(p.shape, p.dtype).stop_grad())
+        self.param_groups.append(group)
+
+    def step(self, loss=None, retain_graph=False):
+        self.pre_step(loss, retain_graph)
+        n = float(self.n_step)
+        for pg in self.param_groups:
+            lr = pg.get("lr", self.lr)
+            betas = pg.get("betas", self.betas)
+            eps = pg.get("eps", self.eps)
+            weight_decay = pg.get("weight_decay", self.weight_decay)
+            max_grad_norm = pg.get("max_grad_norm", self.max_grad_norm)
+            if max_grad_norm>0: self.clip_grad_norm(max_grad_norm)
+            beta1, beta2, beta3 = betas
+            
+            bias_correction1 = 1 - beta1 ** n
+            bias_correction2 = 1 - beta2 ** n
+            bias_correction3_sqrt = jt.sqrt(1 - beta3 ** n)
+            
+            
+            step_size_diff = lr * beta2 * bias_correction3_sqrt / bias_correction2
+            step_size = lr * bias_correction3_sqrt / bias_correction1
+            eps_bias_sqrt = eps * bias_correction3_sqrt
+            
+            for p, g, m, v, d, pre_g in zip(pg["params"], 
+                                            pg["grads"], 
+                                            pg["m"], 
+                                            pg["v"], 
+                                            pg["d"], 
+                                            pg["pre_grad"]):
+                if p.is_stop_grad(): continue
+
+                if self.n_step>0:
+                    pre_g.update(g - pre_g)  # Update pre_g as grad_diff
+
+                
+                m.update(beta1 * m + (1 - beta1) * g)
+                d.update(beta2 * d + (1 - beta2) * pre_g)  # Use pre_g as grad_diff
+                
+                pre_g.update(jt.multiply(pre_g, beta2) + g)  # Update pre_g as update (g + beta2 * grad_diff)
+                
+                v.update(beta3 * v + (1 - beta3) * pre_g * pre_g)  # Use pre_g as update
+                
+                p.update(p - (step_size * m + step_size_diff * d) / (jt.sqrt(v) + eps_bias_sqrt))
+                p.update(p / (1 + lr * weight_decay))
+                
+                pre_g.update(g)  # Update pre_g for the next iteration
+        self.post_step()
+        
 
 class LRScheduler:
     def __init__(self,optimizer, last_epoch=-1):
         assert isinstance(optimizer,Optimizer)
         self.optimizer = optimizer
         
         if last_epoch==-1:
```

### Comparing `jittor-1.3.7.9/python/jittor/other/code_softmax.py` & `jittor-1.3.8.1/python/jittor/other/code_softmax.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     for_loop = f"""
     #pragma unroll
     for (int i=0; i<{per_thread}; i++)
     """
     if length % tnum != 0:
         for_loop += f"if ((i*{tnum}+threadIdx.x)*{ILP} < len)\n"
 
-    return jt.code(a.shape, a.dtype, [a], cuda_header=f'''
+    class CodeSoftmax(jt.Function):
+        def execute(self, x):
+            self.save_vars = jt.code(x.shape, x.dtype, [x], cuda_header=f'''
 #include <{jt.compile_extern.cub_home}cub/cub.cuh>
 #include <type/fp16_compute.h>
 ''', cuda_src=f'''
 __global__ void kernel(in0_type* x, out0_type* y, int len) {{
     typedef cub::BlockReduce<float, {tnum}> BlockReduce;
     constexpr int need_log = {int(log)};
     __shared__ typename BlockReduce::TempStorage temp_storage;
@@ -90,16 +92,25 @@
         vload<sizeof(in0_type)*{ILP}>(&y[id+(i*{tnum}+threadIdx.x)*{ILP}], v[i]);
 }}
 int len = in0->shape[in0->shape.size()-1];
 int bnum = in0->numel() / len;
 cudaGetLastError();
 kernel<<<bnum, {tnum}>>>(in0_p, out0_p, len);
 CHECK(0 == cudaGetLastError());
-''', cuda_grad_src=[f"""
-__global__ void kernel(pout0_type* x, dout_type* y, out0_type* z, int len) {{
+''')
+            return self.save_vars
+
+        def grad(self, grad_x):
+            x = self.save_vars
+            return jt.code(x.shape, x.dtype, [x, grad_x], cuda_header=f'''
+#include <{jt.compile_extern.cub_home}cub/cub.cuh>
+#include <type/fp16_compute.h>
+''', 
+                cuda_src=f"""
+__global__ void kernel(in0_type* x, in1_type* y, out0_type* z, int len) {{
     int id = blockIdx.x * len;
     in0_type vx[{per_thread}][{ILP}];
     in0_type vy[{per_thread}][{ILP}];
     {for_loop} {{
         vload<sizeof(in0_type)*{ILP}>(vx[i], &x[id+(i*{tnum}+threadIdx.x)*{ILP}]);
         vload<sizeof(in0_type)*{ILP}>(vy[i], &y[id+(i*{tnum}+threadIdx.x)*{ILP}]);
     }}
@@ -128,10 +139,11 @@
     {for_loop}
         vload<sizeof(in0_type)*{ILP}>(&z[id+(i*{tnum}+threadIdx.x)*{ILP}],
             vx[i]);
 }}
 int len = in0->shape[in0->shape.size()-1];
 int bnum = in0->numel() / len;
 cudaGetLastError();
-kernel<<<bnum, {tnum}>>>(pout0_p, dout_p, out0_p, len);
+kernel<<<bnum, {tnum}>>>(in0_p, in1_p, out0_p, len);
 CHECK(0 == cudaGetLastError());
-"""])
+""")
+    return CodeSoftmax()(a)
```

### Comparing `jittor-1.3.7.9/python/jittor/pool.py` & `jittor-1.3.8.1/python/jittor/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guowei Yang <471184555@qq.com>
 #     Wenyang Zhou <576825820@qq.com>
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 #
```

### Comparing `jittor-1.3.7.9/python/jittor/pyjt_compiler.py` & `jittor-1.3.8.1/python/jittor/pyjt_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import re
 import os
 from jittor_utils import LOG, run_cmd, simple_timer
@@ -171,15 +171,15 @@
                             for (int i=0; i<kw_n; i++) {{
                                 auto ko = PyTuple_GET_ITEM(kw, i);
                                 auto vo = args[i+n];
                                 auto ks = PyUnicode_AsUTF8(ko);
                                 uint khash = hash(ks);
                                 {"".join([
                                 f'''
-                                if (khash == {get_hash(args[aid][1])}u) {{
+                                if ({get_hash_condition(args[aid][1])}) {{
                                     // hash match {args[aid][1]}
                                     CHECK(({get_pytype_map(args[aid][0],2)}(vo)));
                                     arg{aid} = {pytypes[aid]}(vo{holder_set_array[aid]});
                                     arg_filled |= 1ull << {aid};
                                     continue;
                                 }}
                                 '''
@@ -237,14 +237,18 @@
         mul &= mask
     if v in hash_to_key_map:
         assert hash_to_key_map[v] == s, \
             f"hash conflict {hash_to_key_map[v]} {s} {hash_to_key_map}"
     hash_to_key_map[v] = s
     return v
 
+def get_hash_condition(s):
+    if s == "keepdims":
+        return f"khash == {get_hash(s)}u || khash == {get_hash('keepdim')}u"
+    return f"khash == {get_hash(s)}u"
 
 reg = re.compile(
     '(/\\*(.*?)\\*/\\s*)?(//\\s*@pyjt\\(([^\\n]*)\\)\\s*)'
     # ^^^^^^^^^^^^^^^^^          ^^^^    ^^^^
     # doc string $1              pyjt    args $3
     +
     '(//\\s*@attrs\\(([^\\n]*)\\)\\s*)?'
@@ -584,14 +588,23 @@
             func_head = "(PyObject* self) -> PyObject*"
             func_fill = """
                 int64 n = 1;
                 PyObject* args[] = {self};
                 (void)n, (void)args;
             """
         
+        elif name == "__str__":
+            slot_name = "tp_str"
+            func_head = "(PyObject* self) -> PyObject*"
+            func_fill = """
+                int64 n = 0;
+                PyObject* args[] = {self};
+                (void)n, (void)args;
+            """
+        
         elif name == "__richcmp__":
             slot_name = "tp_richcompare"
             func_head = "(PyObject* self, PyObject* b, int op) -> PyObject*"
             func_fill = """
                 int64 n = 2;
                 PyObject* args[] = {self, b};
                 (void)n, (void)args;
```

### Comparing `jittor-1.3.7.9/python/jittor/script/Dockerfile_cuda11` & `jittor-1.3.8.1/python/jittor/script/Dockerfile_cuda11`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/build_aarch64_mkl.sh` & `jittor-1.3.8.1/python/jittor/script/build_aarch64_mkl.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/converter_server.sh` & `jittor-1.3.8.1/python/jittor/script/converter_server.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/inference_perf.py` & `jittor-1.3.8.1/python/jittor/script/inference_perf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/script/install.sh` & `jittor-1.3.8.1/python/jittor/script/install.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/install_llvm.sh` & `jittor-1.3.8.1/python/jittor/script/install_llvm.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/install_mkl.sh` & `jittor-1.3.8.1/python/jittor/script/install_mkl.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/make_doc.py` & `jittor-1.3.8.1/python/jittor/script/make_doc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/script/tmpi` & `jittor-1.3.8.1/python/jittor/script/tmpi`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/sparse.py` & `jittor-1.3.8.1/python/jittor/sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Dun Liang <randonlang@gmail.com>.
 #   Xiangli Li <190569238@qq.com>
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/src/common.h` & `jittor-1.3.8.1/python/jittor/src/common.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <memory>
 #include <functional>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/core.h` & `jittor-1.3.8.1/python/jittor/src/core.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/event_queue.cc` & `jittor-1.3.8.1/python/jittor/src/event_queue.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "event_queue.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/event_queue.h` & `jittor-1.3.8.1/python/jittor/src/event_queue.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <thread>
 #include <mutex>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/executor.cc` & `jittor-1.3.8.1/python/jittor/src/executor.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 //     Guoye Yang <498731903@qq.com>
 //
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -173,14 +173,15 @@
     jittor::LogFatalVoidify() && logf;
 }
 
 static void top_weak_sync(vector<Var*>& vars) {
     auto t = ++tflag_count;
     int64 max_id=0;
     for (auto v : vars) {
+        if (v->is_finished()) continue;
         max_id = std::max(v->id, max_id);
         v->tflag = t;
     }
     while (true) {
         if (sync_ptr == hold_vars.begin())
             break;
         auto next_ptr = std::prev(sync_ptr);
```

### Comparing `jittor-1.3.7.9/python/jittor/src/executor.h` & `jittor-1.3.8.1/python/jittor/src/executor.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 //     Guoye Yang <498731903@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/fused_op.cc` & `jittor-1.3.8.1/python/jittor/src/fused_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "fused_op.h"
 #include "var.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/fused_op.h` & `jittor-1.3.8.1/python/jittor/src/fused_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 #include "opt/var_relay.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/fuser.h` & `jittor-1.3.8.1/python/jittor/src/fuser.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/grad.cc` & `jittor-1.3.8.1/python/jittor/src/grad.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "pybind/py_var_tracer.h"
 #include "grad.h"
 #include "var.h"
@@ -12,16 +12,20 @@
 #include "ops/op_register.h"
 #include "var_holder.h"
 
 namespace jittor {
 
 #define PREVENT_LARGE_FUSED_OP 16
 
+DECLARE_FLAG(int, auto_mixed_precision_level);
+
 static auto make_binary = get_op_info("binary")
     .get_constructor<VarPtr, Var*, Var*, NanoString>();
+static auto make_unary = get_op_info("unary")
+    .get_constructor<VarPtr, Var*, NanoString>();
 static auto make_number = get_op_info("number")
     .get_constructor<VarPtr, float, Var*>();
 
 #ifdef _WIN32
 template<class T> struct StackIniter {
     T* a;
     int n;
@@ -240,14 +244,17 @@
                         }
                         #endif
                         assign_attrs(grad.ptr, var);
                     }
                 }
             }
         }
+        if (auto_mixed_precision_level == 3 && grad->ns != var->ns) {
+            grad = make_unary(grad, var->ns);
+        }
     }
     trace_grad_op = nullptr;
     // set zero grad
     for (size_t i=0; i<results.size(); i++) {
         Var* var = targets[i];
         VarPtr& grad = results[i];
         auto id = target_id[i];
```

### Comparing `jittor-1.3.7.9/python/jittor/src/grad.h` & `jittor-1.3.8.1/python/jittor/src/grad.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "ops/tape_op.h"
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/graph.cc` & `jittor-1.3.8.1/python/jittor/src/graph.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include <algorithm>
 #include "graph.h"
@@ -79,25 +79,26 @@
                 continue;
             LOGf << "ERROR dnode" << (void*)node << kv.second << node;
         }
     }
 }
 
 DumpGraphs dump_all_graphs() {
+    DumpGraphs graphs;
     vector<Node*> queue;
     auto t = ++tflag_count;
     for (auto& vh : hold_vars)
         if (vh->var->tflag != t) {
             vh->var->tflag = t;
             queue.push_back(vh->var);
+            graphs.hold_vars.emplace_back(ss_convert(vh->var));
         }
     bfs_both(queue, [](Node*){return true;});
     std::sort(queue.begin(), queue.end(),
         [](Node* a, Node* b) { return a->id < b->id;});
-    DumpGraphs graphs;
     for (uint i=0; i<queue.size(); i++)
         queue[i]->custom_data = i;
     for (Node* node : queue) {
         graphs.nodes_info.emplace_back(ss_convert(node));
         
         graphs.inputs.emplace_back();
         auto& inputs = graphs.inputs.back();
```

### Comparing `jittor-1.3.7.9/python/jittor/src/graph.h` & `jittor-1.3.8.1/python/jittor/src/graph.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "node.h"
 
 namespace jittor {
 
 DECLARE_FLAG(int, check_graph);
 
 // this struct is used for debug and visualization
 // @pyjt(DumpGraphs)
 struct DumpGraphs {
+    // @pyjt(hold_vars)
+    vector<string> hold_vars;
     // @pyjt(nodes_info)
     vector<string> nodes_info;
     // @pyjt(inputs)
     vector<vector<int>> inputs;
     // @pyjt(outputs)
     vector<vector<int>> outputs;
 };
```

### Comparing `jittor-1.3.7.9/python/jittor/src/init.cc` & `jittor-1.3.8.1/python/jittor/src/init.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "helper_cuda.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/init.h` & `jittor-1.3.8.1/python/jittor/src/init.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <random>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/jit_compiler.cc` & `jittor-1.3.8.1/python/jittor/src/jit_compiler.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <fstream>
 #include <streambuf>
 #include <stdlib.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/jit_compiler.h` & `jittor-1.3.8.1/python/jittor/src/jit_compiler.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/jit_key.cc` & `jittor-1.3.8.1/python/jittor/src/jit_key.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifndef _WIN32
 #include <sys/mman.h>
 #include <unistd.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/jit_key.h` & `jittor-1.3.8.1/python/jittor/src/jit_key.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <cstring>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/lock.cc` & `jittor-1.3.8.1/python/jittor/src/lock.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Wenyang Zhou <576825820@qq.com>
 //     Dun Liang <randonlang@gmail.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/lock.h` & `jittor-1.3.8.1/python/jittor/src/lock.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Wenyang Zhou <576825820@qq.com>
 //     Dun Liang <randonlang@gmail.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/aligned_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/aligned_allocator.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mem/allocator/aligned_allocator.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/aligned_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/aligned_allocator.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_device_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_device_allocator.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "mem/mem_info.h"
@@ -23,17 +23,16 @@
     try {
         checkCudaErrors(cudaMalloc(&ptr, size));
         return ptr;
     } catch (...) {
         // clean the last error
         cudaGetLastError();
     }
-    LOGw << "Unable to alloc cuda device memory, use unify memory instead. "
-        "This may cause low performance.";
     display_memory_info(__FILELINE__);
+    LOGf << "Unable to alloc cuda device memory for size" << size;
     checkCudaErrors(cudaMallocManaged(&ptr, size));
     return ptr;
 }
 
 void CudaDeviceAllocator::free(void* mem_ptr, size_t size, const size_t& allocation) {
     if (size==0) return;
     if (no_cuda_error_when_free) return;
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_device_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_device_allocator.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #ifdef HAS_CUDA
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_dual_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_dual_allocator.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include "misc/cuda_flags.h"
 #include "mem/allocator/cuda_dual_allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_dual_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_dual_allocator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #ifdef HAS_CUDA
 #include <list>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_host_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_host_allocator.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "helper_cuda.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_host_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/nfef_allocator.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
-#ifdef HAS_CUDA
+#include <unordered_map>
+#include <forward_list>
 #include "mem/allocator.h"
 
 namespace jittor {
 
-struct CudaHostAllocator : Allocator {
-    inline uint64 flags() const override { return 0; }
+// Never free exact fit allocator
+struct NFEFAllocator : Allocator {
+    Allocator* underlying;
+    std::unordered_map<size_t, std::forward_list<void*>> freed;
+
+    void setup(Allocator* underlying);
+    uint64 flags() const override { return underlying->flags(); }
     const char* name() const override;
     void* alloc(size_t size, size_t& allocation) override;
     void free(void* mem_ptr, size_t size, const size_t& allocation) override;
 };
 
-EXTERN_LIB CudaHostAllocator cuda_host_allocator;
-
-}
+DECLARE_FLAG(int, use_nfef_allocator);
 
-#endif
+} // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_managed_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_managed_allocator.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "helper_cuda.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/cuda_managed_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/cuda_managed_allocator.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #ifdef HAS_CUDA
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/foreign_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/foreign_allocator.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mem/allocator/foreign_allocator.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/foreign_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/foreign_allocator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/nfef_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/nfef_allocator.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mem/allocator/nfef_allocator.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/sfrl_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/sfrl_allocator.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 #include "mem/allocator/sfrl_allocator.h"
 
 namespace jittor {
 
 DEFINE_FLAG(int, use_sfrl_allocator, 1, "Enable sfrl allocator");
-
+DEFINE_FLAG(int64, sfrl_large_block_size, 20971520, "sfrl_large_block_size, larger will reduce memory shard");
+#define LARGE_BLOCK_SIZE sfrl_large_block_size
 
 std::vector<size_t> CachingBlockPool::block_ids;
     //start from 1
 size_t CachingBlockPool::tot_block_id = 0;
 std::unique_ptr<CachingBlock*[]> CachingBlockPool::occupied_id_mapper(
     new CachingBlock*[CachingBlockPool::ID_LIMIT]);
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/sfrl_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/sfrl_allocator.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -60,15 +60,14 @@
 struct SFRLAllocator : Allocator {
     CachingBlockPool small_blocks, large_blocks;
     std::map<void*, CachingBlock*> occupied_blocks;
     Allocator* underlying;
 
     static const size_t ALIGN_SIZE = 512;
     static const size_t SMALL_BLOCK_SIZE = 1048576;
-    static const size_t LARGE_BLOCK_SIZE = 20971520;
     static const size_t LARGE_ALIGN_SIZE = 2097152;
     float free_ratio, min_free_size;
     static list<SFRLAllocator*> sfrl_allocators;
     list<SFRLAllocator*>::iterator iter;
     CachingBlockPool* get_blocks(size_t size);
     size_t align_size(size_t size);
     size_t allocation_size(size_t size);
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/stat_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/stat_allocator.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "mem/allocator/stat_allocator.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/stat_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/stat_allocator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/temp_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/temp_allocator.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator/temp_allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator/temp_allocator.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator.cc` & `jittor-1.3.8.1/python/jittor/src/mem/allocator.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <typeinfo>
 #include "misc/cuda_flags.h"
 
 #include "mem/allocator/aligned_allocator.h"
 #ifdef HAS_CUDA
 #include "mem/allocator/cuda_managed_allocator.h"
 #include "mem/allocator/cuda_device_allocator.h"
+#include "mem/allocator/cuda_host_allocator.h"
 #include "mem/allocator/cuda_dual_allocator.h"
 #endif
 #include "mem/allocator/stat_allocator.h"
 #include "mem/allocator/sfrl_allocator.h"
 #include "mem/allocator/nfef_allocator.h"
 #include "mem/allocator/temp_allocator.h"
 #include "mem/swap.h"
 #include "var.h"
 
 namespace jittor {
 
+DEFINE_FLAG(int, use_cuda_host_allocator, 1, "use cuda host allocator for cpu memory globally");
 
 struct pair_hash {
 	template <class T1, class T2>
 	std::size_t operator() (const std::pair<T1, T2> &pair) const {
 		return std::hash<T1>()(pair.first) ^ std::hash<T2>()(pair.second);
 	}
 };
@@ -57,15 +59,17 @@
         if (use_cuda_managed_allocator) {
             LOGvv << "Using cuda_managed_allocator";
             allocator = &cuda_managed_allocator;
         } else {
             LOGvv << "Using cuda_device_allocator";
             allocator = &cuda_device_allocator;
         }
-    }
+    } else
+    if (use_cuda_host_allocator)
+        allocator = &cuda_host_allocator;
 #endif
     if (!allocator) {
         LOGvv << "Using aligned_allocator";
         allocator = &aligned_allocator;
     }
     if (use_stat_allocator==1) {
         LOGvv << "Using stat_allocator";
@@ -133,16 +137,14 @@
     #ifdef HAS_CUDA
     // only happend when not using use_cuda_managed_allocator
     if (save_mem) {
         if (swap_timestamp != var->tflag) {
             swap_timestamp = ++tflag_count;
             var->tflag = swap_timestamp;
         }
-        if (var->id == 336770)
-            LOGir << var;
         move_with_swap(var, allocator, true);
         return;
     }
     Allocation a(allocator, var->size);
     checkCudaErrors(cudaMemcpy(a.ptr, var->mem_ptr, var->size, cudaMemcpyHostToDevice));
     var->allocator->free(var->mem_ptr, var->size, var->allocation);
     var->mem_ptr = a.ptr;
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/allocator.h` & `jittor-1.3.8.1/python/jittor/src/mem/allocator.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/mem_info.cc` & `jittor-1.3.8.1/python/jittor/src/mem/mem_info.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <iomanip>
 #include <algorithm>
 #if defined(__linux__)
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/mem_info.h` & `jittor-1.3.8.1/python/jittor/src/mem/mem_info.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/swap.cc` & `jittor-1.3.8.1/python/jittor/src/mem/swap.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,230 +1,233 @@
-// ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: 
-//     Dun Liang <randonlang@gmail.com>
-//
-// This file is subject to the terms and conditions defined in
-// file 'LICENSE.txt', which is part of this source code package.
-// ***************************************************************
-#ifdef HAS_CUDA
-#include <cuda_runtime.h>
-#include <stdio.h>
-#include <unistd.h>
-#endif
-#include "var.h"
-#include "mem/swap.h"
-#include "mem/mem_info.h"
-
-namespace jittor {
-
-int64 swap_timestamp;
-int64 swap_total;
-constexpr int64 SWAP_BUF_SIZE = 1<<23; // 8M
-extern string cache_path;
-static int _pid = getpid();
-
-DEFINE_FLAG(int64, cpu_mem_limit, -1, "cpu_mem_limit");
-DEFINE_FLAG(int64, device_mem_limit, -1, "device_mem_limit");
-
-struct Swap {
-    map<pair<int64,int64>, Var*> lived;
-};
-
-unordered_map<Allocator*, Swap> swaps;
-
-void swap_to_disk(Var* x, Swap& swap) {
-    swap_total += x->size;
-    ASSERT(!x->flags.get(NodeFlags::_is_swapped));
-    string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
-    #ifdef HAS_CUDA
-    if (x->allocator->is_cuda()) {
-        static char* buffer = new char[SWAP_BUF_SIZE];
-        auto* memptr = (char*)x->mem_ptr;
-        auto* fd = fopen(path.c_str(), "wb");
-        CHECK(fd) << "swap file open failed:" << path << x;
-        for (int64 i=0; i<x->size; i+=SWAP_BUF_SIZE) {
-            int64 cp_size = std::min(x->size-i, SWAP_BUF_SIZE);
-            cudaMemcpy(buffer, memptr+i, cp_size, cudaMemcpyDeviceToHost);
-            auto res = fwrite(buffer, cp_size, 1, fd);
-            if (res==1) {
-                fclose(fd);
-                LOGf << "swap file write failed" << path << x;
-            }
-        }
-        fclose(fd); 
-    } else
-    #endif
-    {
-        auto* fd = fopen(path.c_str(), "wb");
-        auto res = fwrite(x->mem_ptr, x->size, 1, fd);
-        CHECK(res==1) << "failed to write swap file" << path << res << x->size << x;
-        fclose(fd); 
-    }
-    auto iter = swap.lived.find({x->size, x->id});
-    ASSERT(iter != swap.lived.end());
-    swap.lived.erase(iter);
-    x->allocator->free(x->mem_ptr, x->size, x->allocation);
-    x->mem_ptr = nullptr;
-    x->allocator = nullptr;
-    x->allocation = 0;
-    x->flags.set(NodeFlags::_is_swapped);
-}
-
-bool alloc_with_swap(Var* x, Allocator* allocator, bool force) {
-
-    auto& swap = swaps[allocator];
-    if (x->allocator) {
-        // shared memory, no need alloc
-        if (x->alloc(allocator)) {
-            swap.lived[{x->size, x->id}] = x;
-            return true;
-        }
-    }
-    bool is_cpu = !allocator->is_cuda();
-    int64 limit = is_cpu ? cpu_mem_limit : device_mem_limit;
-    if (limit < 0) limit = 1ll<<60;
-    if (allocator->used_memory + allocator->unused_memory + x->size > limit)
-        allocator->gc();
-    if (force && allocator->used_memory + allocator->unused_memory + x->size > limit) {
-        auto iter = swap.lived.upper_bound({x->size, -1});
-        auto unused_target = allocator->unused_memory + x->size;
-        while (iter != swap.lived.end()) {
-            auto* var = iter->second;
-            iter++;
-            if (var->tflag == swap_timestamp)
-                continue;
-            ASSERT(var->mem_ptr) << var->exist() << (void*)var << iter->first << (display_memory_info(), 1);
-            if (!is_cpu) {
-                // try move to cpu
-                if (!move_with_swap(var, cpu_allocator, false))
-                    swap_to_disk(var, swap);
-            } else
-                swap_to_disk(var, swap);
-            if (allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target) break;
-        }
-        // if still no space, swap other smaller var
-        if (!(allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target)) {
-            auto iter = swap.lived.end();
-            if (swap.lived.size()) iter = std::prev(iter);
-            while (iter != swap.lived.end()) {
-                auto var = iter->second;
-                iter = iter==swap.lived.begin() ? swap.lived.end() : std::prev(iter);
-                if (var->tflag == swap_timestamp)
-                    continue;
-                ASSERT(var->mem_ptr) << x << var;
-                if (!is_cpu) {
-                    // try move to cpu
-                    if (!move_with_swap(var, cpu_allocator, false))
-                        swap_to_disk(var, swap);
-                } else
-                    swap_to_disk(var, swap);
-                allocator->gc();
-                if (allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target) break;
-            }
-            if (!(allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target)) {
-                display_memory_info();
-                LOGw << "unable to alloc var" << x;
-            }
-        }
-    }
-    if (x->alloc(allocator)) {
-        swap.lived[{x->size, x->id}] = x;
-        return true;
-    }
-    return false;
-}
-
-void free_with_swap(Var* x) {
-    if (x->flags.get(NodeFlags::_is_swapped)) {
-        string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
-        if (remove(path.c_str()) != 0)
-            LOGe << "failed to remove swap file" << path << x->shape << x->dtype();
-    } else {
-        if (!x->mem_ptr) return;
-        auto& swap = swaps[x->allocator];
-        auto iter = swap.lived.find({x->size, x->id});
-        if (iter != swap.lived.end())
-            swap.lived.erase(iter);
-        x->allocator->free(x->mem_ptr, x->size, x->allocation);
-        x->mem_ptr = nullptr;
-        x->allocator = nullptr;
-        x->allocation = 0;
-    }
-}
-
-bool move_with_swap(Var* x, Allocator* allocator, bool force) {
-    if (allocator == x->allocator) return true;
-    swap_total += x->size;
-    Allocation allocation(x->mem_ptr, x->allocation, x->size, x->allocator);
-    x->mem_ptr = nullptr;
-    x->allocator = nullptr;
-    x->allocation = 0;
-    if (!alloc_with_swap(x, allocator, force)) {
-        x->mem_ptr = allocation.ptr;
-        x->allocator = allocation.allocator;
-        x->allocation = allocation.allocation;
-        allocation.ptr = nullptr;
-        allocation.allocation = 0;
-        return false;
-    }
-    if (x->flags.get(NodeFlags::_is_swapped)) {
-        string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
-        #ifdef HAS_CUDA
-        if (x->allocator->is_cuda()) {
-            static char* buffer = new char[SWAP_BUF_SIZE];
-            auto* memptr = (char*)x->mem_ptr;
-            auto* fd = fopen(path.c_str(), "rb");
-            CHECK(fd) << "swap file open failed:" << path << x;
-            for (int64 i=0; i<x->size; i+=SWAP_BUF_SIZE) {
-                int64 cp_size = std::min(x->size-i, SWAP_BUF_SIZE);
-                auto res = fread(buffer, cp_size, 1, fd);
-                cudaMemcpy(memptr+i, buffer, cp_size, cudaMemcpyHostToDevice);
-                if (res != 1) {
-                    fclose(fd);
-                    LOGf << "swap file read failed" << path << x;
-                }
-            }
-            fclose(fd); 
-        } else
-        #endif
-        {
-            auto* fd = fopen(path.c_str(), "rb");
-            auto res = fread(x->mem_ptr, x->size, 1, fd);
-            CHECK(res==1);
-            fclose(fd); 
-        }
-            
-        if (remove(path.c_str()) != 0)
-            LOGe << "failed to remove swap file" << path << x->shape << x->dtype();
-        x->flags.set(NodeFlags::_is_swapped, 0);
-    } else {
-        #ifdef HAS_CUDA
-        if (x->allocator->is_cuda()) {
-            if (allocation.allocator->is_cuda())
-                cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyDeviceToDevice);
-            else
-                cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyHostToDevice);
-        } else
-        if (allocation.allocator->is_cuda()) {
-            cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyDeviceToHost);
-        } else
-        #endif
-        {
-            std::memcpy(x->mem_ptr, allocation.ptr, x->size);
-        }
-    }
-    if (allocation.ptr) {
-        auto& swap = swaps[allocation.allocator];
-        auto iter = swap.lived.find({x->size, x->id});
-        if (iter != swap.lived.end())
-            swap.lived.erase(iter);
-    }
-    return true;
-}
-
-void registe_swap(Var* x) {
-    auto& swap = swaps[x->allocator];
-    swap.lived[{x->size, x->id}] = x;
-}
-
-}
+// ***************************************************************
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: 
+//     Dun Liang <randonlang@gmail.com>
+//
+// This file is subject to the terms and conditions defined in
+// file 'LICENSE.txt', which is part of this source code package.
+// ***************************************************************
+#ifdef HAS_CUDA
+#include <cuda_runtime.h>
+#endif
+#include <stdio.h>
+#include <thread>
+#ifndef _MSC_VER
+#include <unistd.h>
+#endif
+#include "var.h"
+#include "mem/swap.h"
+#include "mem/mem_info.h"
+
+namespace jittor {
+
+int64 swap_timestamp;
+int64 swap_total;
+constexpr int64 SWAP_BUF_SIZE = 1<<23; // 8M
+extern string cache_path;
+static int _pid = getpid();
+
+DEFINE_FLAG(int64, cpu_mem_limit, -1, "cpu_mem_limit");
+DEFINE_FLAG(int64, device_mem_limit, -1, "device_mem_limit");
+
+struct Swap {
+    map<pair<int64,int64>, Var*> lived;
+};
+
+unordered_map<Allocator*, Swap> swaps;
+
+void swap_to_disk(Var* x, Swap& swap) {
+    swap_total += x->size;
+    ASSERT(!x->flags.get(NodeFlags::_is_swapped));
+    string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
+    #ifdef HAS_CUDA
+    if (x->allocator->is_cuda()) {
+        static char* buffer = new char[SWAP_BUF_SIZE];
+        auto* memptr = (char*)x->mem_ptr;
+        auto* fd = fopen(path.c_str(), "wb");
+        CHECK(fd) << "swap file open failed:" << path << x;
+        for (int64 i=0; i<x->size; i+=SWAP_BUF_SIZE) {
+            int64 cp_size = std::min(x->size-i, SWAP_BUF_SIZE);
+            cudaMemcpy(buffer, memptr+i, cp_size, cudaMemcpyDeviceToHost);
+            auto res = fwrite(buffer, cp_size, 1, fd);
+            if (res==1) {
+                fclose(fd);
+                LOGf << "swap file write failed" << path << x;
+            }
+        }
+        fclose(fd); 
+    } else
+    #endif
+    {
+        auto* fd = fopen(path.c_str(), "wb");
+        auto res = fwrite(x->mem_ptr, x->size, 1, fd);
+        CHECK(res==1) << "failed to write swap file" << path << res << x->size << x;
+        fclose(fd); 
+    }
+    auto iter = swap.lived.find({x->size, x->id});
+    ASSERT(iter != swap.lived.end());
+    swap.lived.erase(iter);
+    x->allocator->free(x->mem_ptr, x->size, x->allocation);
+    x->mem_ptr = nullptr;
+    x->allocator = nullptr;
+    x->allocation = 0;
+    x->flags.set(NodeFlags::_is_swapped);
+}
+
+bool alloc_with_swap(Var* x, Allocator* allocator, bool force) {
+
+    auto& swap = swaps[allocator];
+    if (x->allocator) {
+        // shared memory, no need alloc
+        if (x->alloc(allocator)) {
+            swap.lived[{x->size, x->id}] = x;
+            return true;
+        }
+    }
+    bool is_cpu = !allocator->is_cuda();
+    int64 limit = is_cpu ? cpu_mem_limit : device_mem_limit;
+    if (limit < 0) limit = 1ll<<60;
+    if (allocator->used_memory + allocator->unused_memory + x->size > limit)
+        allocator->gc();
+    if (force && allocator->used_memory + allocator->unused_memory + x->size > limit) {
+        auto iter = swap.lived.upper_bound({x->size, -1});
+        auto unused_target = allocator->unused_memory + x->size;
+        while (iter != swap.lived.end()) {
+            auto* var = iter->second;
+            iter++;
+            if (var->tflag == swap_timestamp)
+                continue;
+            ASSERT(var->mem_ptr) << var->exist() << (void*)var << iter->first << (display_memory_info(), 1);
+            if (!is_cpu) {
+                // try move to cpu
+                if (!move_with_swap(var, cpu_allocator, false))
+                    swap_to_disk(var, swap);
+            } else
+                swap_to_disk(var, swap);
+            if (allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target) break;
+        }
+        // if still no space, swap other smaller var
+        if (!(allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target)) {
+            auto iter = swap.lived.end();
+            if (swap.lived.size()) iter = std::prev(iter);
+            while (iter != swap.lived.end()) {
+                auto var = iter->second;
+                iter = iter==swap.lived.begin() ? swap.lived.end() : std::prev(iter);
+                if (var->tflag == swap_timestamp)
+                    continue;
+                ASSERT(var->mem_ptr) << x << var;
+                if (!is_cpu) {
+                    // try move to cpu
+                    if (!move_with_swap(var, cpu_allocator, false))
+                        swap_to_disk(var, swap);
+                } else
+                    swap_to_disk(var, swap);
+                allocator->gc();
+                if (allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target) break;
+            }
+            if (!(allocator->used_memory + allocator->unused_memory + x->size <= limit || allocator->unused_memory >= unused_target)) {
+                display_memory_info();
+                LOGw << "unable to alloc var" << x;
+            }
+        }
+    }
+    if (x->alloc(allocator)) {
+        swap.lived[{x->size, x->id}] = x;
+        return true;
+    }
+    return false;
+}
+
+void free_with_swap(Var* x) {
+    if (x->flags.get(NodeFlags::_is_swapped)) {
+        string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
+        if (remove(path.c_str()) != 0)
+            LOGe << "failed to remove swap file" << path << x->shape << x->dtype();
+    } else {
+        if (!x->mem_ptr) return;
+        auto& swap = swaps[x->allocator];
+        auto iter = swap.lived.find({x->size, x->id});
+        if (iter != swap.lived.end())
+            swap.lived.erase(iter);
+        x->allocator->free(x->mem_ptr, x->size, x->allocation);
+        x->mem_ptr = nullptr;
+        x->allocator = nullptr;
+        x->allocation = 0;
+    }
+}
+
+bool move_with_swap(Var* x, Allocator* allocator, bool force) {
+    if (allocator == x->allocator) return true;
+    swap_total += x->size;
+    Allocation allocation(x->mem_ptr, x->allocation, x->size, x->allocator);
+    x->mem_ptr = nullptr;
+    x->allocator = nullptr;
+    x->allocation = 0;
+    if (!alloc_with_swap(x, allocator, force)) {
+        x->mem_ptr = allocation.ptr;
+        x->allocator = allocation.allocator;
+        x->allocation = allocation.allocation;
+        allocation.ptr = nullptr;
+        allocation.allocation = 0;
+        return false;
+    }
+    if (x->flags.get(NodeFlags::_is_swapped)) {
+        string path = cache_path + "/tmp/" + S(_pid) + "-" + S(x->id) + ".bin";
+        #ifdef HAS_CUDA
+        if (x->allocator->is_cuda()) {
+            static char* buffer = new char[SWAP_BUF_SIZE];
+            auto* memptr = (char*)x->mem_ptr;
+            auto* fd = fopen(path.c_str(), "rb");
+            CHECK(fd) << "swap file open failed:" << path << x;
+            for (int64 i=0; i<x->size; i+=SWAP_BUF_SIZE) {
+                int64 cp_size = std::min(x->size-i, SWAP_BUF_SIZE);
+                auto res = fread(buffer, cp_size, 1, fd);
+                cudaMemcpy(memptr+i, buffer, cp_size, cudaMemcpyHostToDevice);
+                if (res != 1) {
+                    fclose(fd);
+                    LOGf << "swap file read failed" << path << x;
+                }
+            }
+            fclose(fd); 
+        } else
+        #endif
+        {
+            auto* fd = fopen(path.c_str(), "rb");
+            auto res = fread(x->mem_ptr, x->size, 1, fd);
+            CHECK(res==1);
+            fclose(fd); 
+        }
+            
+        if (remove(path.c_str()) != 0)
+            LOGe << "failed to remove swap file" << path << x->shape << x->dtype();
+        x->flags.set(NodeFlags::_is_swapped, 0);
+    } else {
+        #ifdef HAS_CUDA
+        if (x->allocator->is_cuda()) {
+            if (allocation.allocator->is_cuda())
+                cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyDeviceToDevice);
+            else
+                cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyHostToDevice);
+        } else
+        if (allocation.allocator->is_cuda()) {
+            cudaMemcpy(x->mem_ptr, allocation.ptr, x->size, cudaMemcpyDeviceToHost);
+        } else
+        #endif
+        {
+            std::memcpy(x->mem_ptr, allocation.ptr, x->size);
+        }
+    }
+    if (allocation.ptr) {
+        auto& swap = swaps[allocation.allocator];
+        auto iter = swap.lived.find({x->size, x->id});
+        if (iter != swap.lived.end())
+            swap.lived.erase(iter);
+    }
+    return true;
+}
+
+void registe_swap(Var* x) {
+    auto& swap = swaps[x->allocator];
+    swap.lived[{x->size, x->id}] = x;
+}
+
+}
```

### Comparing `jittor-1.3.7.9/python/jittor/src/mem/swap.h` & `jittor-1.3.8.1/python/jittor/src/mem/swap.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-// ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: 
-//     Dun Liang <randonlang@gmail.com>
-//
-// This file is subject to the terms and conditions defined in
-// file 'LICENSE.txt', which is part of this source code package.
-// ***************************************************************
-
-/*
-var heap
-    map allocator
-        lived: map size, var
-        swaped: set var
-
-    if gpu is full,
-        if cpu is ok:
-            swap to cpu
-        else
-            swap to disk
-
-    operation
-        take over all alloc,
-        mark time stamp
-        get_allocation(allocator, var)
-
-        alloc(allocator, size) -> Allocation
-        add_ts, mark_ts
-        signin, signout
-        move_to(own alloc)
-
-global
-    mem_save_mode
-    cpu_mem_limit_n
-    device_mem_limit_n
-
-share_with handle:
-    free var, until allocator reduce size
-
-TODO:
-    change exe.allocator->alloc to exe.temp_allocator->alloc
-    handle cutt jt_alloc
-    handle cupy jittor_cuda_malloc
-    search share_with
-    search migrate
-    check Allocation move
-        migrate_to_cpu
-        migrate_to_gpu
-        array op
-        fetch op
-    !!disable dual allocator, reuse array
-    handle foreign allocator, only handle cpu allocator and gpu allocator
-
-code change:
-    free var
-    alloc var
-    executor mark timestamp
-    migrate_to_cpu
-    migrate_to_gpu
-    array op: finish imm
-    fetch op
-    if is cached, access?
-        item, data, numpy, all calling migrate_to_cpu, handle in migrate_to_cpu
-    JT_SAVE_MEM env, global env for
-
-*/
-#pragma once
-#include "common.h"
-#include "mem/allocator.h"
-#include "var.h"
-
-namespace jittor {
-
-#ifdef JT_SAVE_MEM
-#if JT_SAVE_MEM != 0
-constexpr int save_mem = 1;
-#else
-constexpr int save_mem = 0;
-#endif
-#else
-constexpr int save_mem = 0;
-#endif
-extern int64 swap_timestamp;
-extern int64 swap_total;
-
-DECLARE_FLAG(int64, cpu_mem_limit);
-DECLARE_FLAG(int64, device_mem_limit);
-
-bool alloc_with_swap(Var* x, Allocator* allocator, bool force);
-void free_with_swap(Var* x);
-bool move_with_swap(Var* x, Allocator* allocator, bool force);
-void registe_swap(Var* x);
-
-inline void check_and_swap_out(Var* x, Allocator* allocator) {
-    if (x->flags.get(NodeFlags::_is_swapped))
-        move_with_swap(x, allocator, true);
-}
-
-
-}
+// ***************************************************************
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: 
+//     Dun Liang <randonlang@gmail.com>
+//
+// This file is subject to the terms and conditions defined in
+// file 'LICENSE.txt', which is part of this source code package.
+// ***************************************************************
+
+/*
+var heap
+    map allocator
+        lived: map size, var
+        swaped: set var
+
+    if gpu is full,
+        if cpu is ok:
+            swap to cpu
+        else
+            swap to disk
+
+    operation
+        take over all alloc,
+        mark time stamp
+        get_allocation(allocator, var)
+
+        alloc(allocator, size) -> Allocation
+        add_ts, mark_ts
+        signin, signout
+        move_to(own alloc)
+
+global
+    mem_save_mode
+    cpu_mem_limit_n
+    device_mem_limit_n
+
+share_with handle:
+    free var, until allocator reduce size
+
+TODO:
+    change exe.allocator->alloc to exe.temp_allocator->alloc
+    handle cutt jt_alloc
+    handle cupy jittor_cuda_malloc
+    search share_with
+    search migrate
+    check Allocation move
+        migrate_to_cpu
+        migrate_to_gpu
+        array op
+        fetch op
+    !!disable dual allocator, reuse array
+    handle foreign allocator, only handle cpu allocator and gpu allocator
+
+code change:
+    free var
+    alloc var
+    executor mark timestamp
+    migrate_to_cpu
+    migrate_to_gpu
+    array op: finish imm
+    fetch op
+    if is cached, access?
+        item, data, numpy, all calling migrate_to_cpu, handle in migrate_to_cpu
+    JT_SAVE_MEM env, global env for
+
+*/
+#pragma once
+#include "common.h"
+#include "mem/allocator.h"
+#include "var.h"
+
+namespace jittor {
+
+#ifdef JT_SAVE_MEM
+#if JT_SAVE_MEM != 0
+constexpr int save_mem = 1;
+#else
+constexpr int save_mem = 0;
+#endif
+#else
+constexpr int save_mem = 0;
+#endif
+extern int64 swap_timestamp;
+extern int64 swap_total;
+
+DECLARE_FLAG(int64, cpu_mem_limit);
+DECLARE_FLAG(int64, device_mem_limit);
+
+bool alloc_with_swap(Var* x, Allocator* allocator, bool force);
+void free_with_swap(Var* x);
+bool move_with_swap(Var* x, Allocator* allocator, bool force);
+void registe_swap(Var* x);
+
+inline void check_and_swap_out(Var* x, Allocator* allocator) {
+    if (x->flags.get(NodeFlags::_is_swapped))
+        move_with_swap(x, allocator, true);
+}
+
+
+}
```

### Comparing `jittor-1.3.7.9/python/jittor/src/memory_profiler.cc` & `jittor-1.3.8.1/python/jittor/src/memory_profiler.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -52,27 +52,27 @@
 void MemoryProfiler::clear() {
     allocations.clear();
     max_memory_size = 0;
     max_used_memory_size = 0;
 }
 
 std::pair<size_t, size_t> MemoryProfiler::get_memory_info() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     size_t used = 0;
     size_t unused = 0;
     //TODO add mssfrl allocator
     for (auto& a : SFRLAllocator::sfrl_allocators) {
         used += a->used_memory;
         unused += a->unused_memory;
     }
     return std::make_pair(used, unused);
 }
 
 void MemoryProfiler::check() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     std::pair<size_t, size_t> mem_info = get_memory_info();
     if (mem_info.first > max_used_memory_size) {
         max_used_memory_size = mem_info.first;
 
         allocations.clear();
         size_t memory_size = 0;
         std::vector<std::pair<std::pair<string, vector<Stack>>, size_t>> live_vars;
@@ -89,27 +89,33 @@
         backup_custom_data.resize(queue.size());
         for (int i=0; i<queue.size(); i++)
             backup_custom_data[i] = queue[i]->custom_data;
         toplogical_sort_forward(queue, queue2, [](Node*){});
         for (int i=0; i<queue.size(); i++)
             queue[i]->custom_data = backup_custom_data[i];
         queue.swap(queue2);
+        int64 cpu_sum = 0;
         for (Node* node : queue) {
             if (node->is_var()) {
                 Var* var = (Var*)node;
                 if (var->mem_ptr != nullptr) {
+                    if (profile_memory_enable == 2 && !var->allocator->is_cuda()) {
+                        cpu_sum += var->size;
+                        continue;
+                    }
                     vector<Stack> stacks = get_node_trace(var);
                     if (stacks.size() == 0) {
                         stacks.push_back(Stack());
                     }
-                    std::stringstream stream;
-                    stream << var;
-                    live_vars.push_back(std::make_pair(std::make_pair(stream.str(), stacks), var->size));
-                    if (!allocations.count(var->mem_ptr)) {
-                        allocations[var->mem_ptr] = 1;
+                    auto alloc = std::make_pair((void*)var->allocator, (void*)var->allocation);
+                    if (!allocations.count(alloc)) {
+                        std::stringstream stream;
+                        stream << var;
+                        live_vars.push_back(std::make_pair(std::make_pair(stream.str(), stacks), var->size));
+                        allocations[alloc] = 1;
                         memory_size += var->size;
                     }
                 }
             }
         }
         max_live_vars = live_vars;
         max_memory_size = memory_size;
@@ -117,15 +123,15 @@
 }
 
 bool MemoryProfiler::cmp(const std::pair<std::pair<string, vector<Stack>>, size_t>& a, const std::pair<std::pair<string, vector<Stack>>, size_t>& b) {
     return a.second > b.second;
 }
 
 void MemoryProfiler::display_max_memory_info() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     Log log("", 'i', 0);
     std::sort(max_live_vars.begin(), max_live_vars.end(), cmp);
     log << "\n=====display_max_memory_info=====\n";
     log << "max used memory" << FloatOutput_{(double)max_used_memory_size, " KMG", 1024, "B"} << "\n";
     log << "max var memory" << FloatOutput_{(double)max_memory_size, " KMG", 1024, "B"} << "\n\n";
     log << "[Size]" << "[Percent]" << "[Var Info]" << "\n";
     for (int i = 0; i < max_live_vars.size(); ++i) {
@@ -136,20 +142,20 @@
         << "\n\n";
     }
     log << "=========================\n";
     log.end();
 }
 
 void display_max_memory_info() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     memory_profiler.display_max_memory_info();
 }
 
 string MemoryProfiler::get_max_memory_info() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     std::stringstream out;
     string div1 = "[!@#div1!@#]";
     string div2 = "[!@#div2!@#]";
     string div3 = "[!@#div3!@#]";
 
     std::sort(max_live_vars.begin(), max_live_vars.end(), cmp);
     out << max_memory_size;
@@ -163,12 +169,12 @@
                 << max_live_vars[i].first.second[j].module_type << div2;
         }
     }
     return out.str();
 }
 
 string get_max_memory_info() {
-    ASSERT(profile_memory_enable == 1);
+    ASSERT(profile_memory_enable);
     return memory_profiler.get_max_memory_info();
 }
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/memory_profiler.h` & `jittor-1.3.8.1/python/jittor/src/memory_profiler.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -19,15 +19,15 @@
 
 // @pyjt(display_max_memory_info)
 void display_max_memory_info();
 // @pyjt(get_max_memory_info)
 string get_max_memory_info();
 
 struct MemoryProfiler {
-    std::map<void*, size_t> allocations;
+    std::map<pair<void*,void*>, size_t> allocations;
     // Max Infos
     vector<std::pair<std::pair<string, vector<Stack>>, size_t>> max_live_vars;
     size_t max_used_memory_size;
     size_t max_memory_size;
 
 
     MemoryProfiler();
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cpu_atomic.h` & `jittor-1.3.8.1/python/jittor/src/misc/cpu_atomic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <atomic>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cpu_math.cc` & `jittor-1.3.8.1/python/jittor/src/misc/cpu_math.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #define _USE_MATH_DEFINES
 #include <cmath>
 #include <limits>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cstr.h` & `jittor-1.3.8.1/python/jittor/src/misc/cstr.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <cstring>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cuda_atomic.h` & `jittor-1.3.8.1/python/jittor/src/misc/cuda_atomic.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
+#include <cuda_fp16.h>
 #include "common.h"
 
 namespace jittor {
 
 __device__ inline static int floatToOrderedInt(float floatVal) {
     int intVal = __float_as_int( floatVal );
     return (intVal >= 0 ) ? intVal : intVal ^ 0x7FFFFFFF;
@@ -91,14 +92,22 @@
     typedef float src;
     typedef int target;
     inline static __device__ target to_int(src a) { return __float_as_int(a); }
     inline static __device__ target* to_intp(src* a) { return (target*)a; }
     inline static __device__ src from_int(target a) { return __int_as_float(a); }
 };
 
+template <> struct int_mapper<__half> { 
+    typedef __half src;
+    typedef unsigned short target;
+    inline static __device__ target to_int(src a) { return __half_as_ushort(a); }
+    inline static __device__ target* to_intp(src* a) { return (target*)a; }
+    inline static __device__ src from_int(target a) { return __ushort_as_half(a); }
+};
+
 template <> struct int_mapper<double> { 
     typedef double src;
     typedef long long target;
     inline static __device__ target to_int(src a) { return __double_as_longlong(a); }
     inline static __device__ target* to_intp(src* a) { return (target*)a; }
     inline static __device__ src from_int(target a) { return __longlong_as_double(a); }
 };
@@ -113,14 +122,45 @@
         old = atomicCAS(a_i, assume, int_mapper<T>::to_int(old_f*b));
         old_f = int_mapper<T>::from_int(old);
         if (assume==old) break;
     }
     return old_f;
 }
 
+
+template<> __device__
+__half cuda_atomic_max(__half* a, __half b) {
+    auto old_f = *a;
+    auto old = int_mapper<__half>::to_int(old_f);
+    auto a_i = int_mapper<__half>::to_intp(a);
+    while (1) {
+        auto assume = old;
+        if (old_f>=b) break;
+        old = atomicCAS(a_i, assume, int_mapper<__half>::to_int(b));
+        old_f = int_mapper<__half>::from_int(old);
+        if (assume==old) break;
+    }
+    return old_f;
+}
+
+template<> __device__
+__half cuda_atomic_min(__half* a, __half b) {
+    auto old_f = *a;
+    auto old = int_mapper<__half>::to_int(old_f);
+    auto a_i = int_mapper<__half>::to_intp(a);
+    while (1) {
+        auto assume = old;
+        if (old_f<=b) break;
+        old = atomicCAS(a_i, assume, int_mapper<__half>::to_int(b));
+        old_f = int_mapper<__half>::from_int(old);
+        if (assume==old) break;
+    }
+    return old_f;
+}
+
 template<typename T>
 __device__ inline T shared_reduce_add(T a, T b) {
     return a + b;
 }
 
 template<typename T>
 __device__ inline T shared_reduce_mul(T a, T b) {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cuda_flags.cc` & `jittor-1.3.8.1/python/jittor/src/misc/cuda_flags.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 #include "common.h"
 #ifdef HAS_CUDA
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cuda_flags.h` & `jittor-1.3.8.1/python/jittor/src/misc/cuda_flags.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/cuda_limits.h` & `jittor-1.3.8.1/python/jittor/src/misc/cuda_limits.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 
 #ifdef IS_CUDA
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/deleter.h` & `jittor-1.3.8.1/python/jittor/src/misc/deleter.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include <functional>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/fast_shared_ptr.h` & `jittor-1.3.8.1/python/jittor/src/misc/fast_shared_ptr.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/hash.h` & `jittor-1.3.8.1/python/jittor/src/misc/hash.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/intrin.h` & `jittor-1.3.8.1/python/jittor/src/misc/intrin.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/miniz.cc` & `jittor-1.3.8.1/python/jittor/src/misc/miniz.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/miniz.h` & `jittor-1.3.8.1/python/jittor/src/misc/miniz.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/nan_checker.cc` & `jittor-1.3.8.1/python/jittor/src/misc/nan_checker.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cfloat>
 #include <cmath>
 #include "misc/nan_checker.h"
 #ifdef HAS_CUDA
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/nan_checker.cu` & `jittor-1.3.8.1/python/jittor/src/misc/nan_checker.cu`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,100 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "misc/nan_checker.h"
 #include "misc/cuda_flags.h"
 #include <cuda_runtime.h>
 #include <cuda_fp16.h>
 #include "helper_cuda.h"
 #include <cassert>
 
 namespace jittor {
 
+inline __device__ void print_nan(float v, int64 i, int* cnt) {
+    auto x = atomicAdd(cnt, 1);
+    if (x<10)
+        printf("detect a[%lld] = %f\n", i, v);
+}
 
 #ifdef HAS_CUDA
-__global__ void _check_nan_float16(__half* __restrict__ ptr, int64 num) {
+__global__ void _check_nan_float16(__half* __restrict__ ptr, int64 num, int* cnt) {
     int64 i = threadIdx.x + blockIdx.x * (int64)blockDim.x;
     if (i<num) {
         #if JT_CHECK_NAN == 2
         if (isnan(__half2float(ptr[i])))
         #else
         if (isnan(__half2float(ptr[i])) || __hisinf(ptr[i]))
         #endif
-            __trap();
+            print_nan(float(ptr[i]), i, cnt);
     }
 }
 
-__global__ void _check_nan_float32(float32* __restrict__ ptr, int64 num) {
+__global__ void _check_nan_float32(float32* __restrict__ ptr, int64 num, int* cnt) {
     int64 i = threadIdx.x + blockIdx.x * (int64)blockDim.x;
     if (i<num) {
         #if JT_CHECK_NAN == 2
         if (::isnan(ptr[i]))
         #else
         if (::isnan(ptr[i]) || ::isinf(ptr[i]))
         #endif
-            __trap();
+            print_nan(float(ptr[i]), i, cnt);
     }
 }
 
 
-__global__ void _check_nan_float64(float64* __restrict__ ptr, int64 num) {
+__global__ void _check_nan_float64(float64* __restrict__ ptr, int64 num, int* cnt) {
     int64 i = threadIdx.x + blockIdx.x * (int64)blockDim.x;
     if (i<num) {
         #if JT_CHECK_NAN == 2
         if (::isnan(ptr[i]))
         #else
         if (::isnan(ptr[i]) || ::isinf(ptr[i]))
         #endif
-            __trap();
+            print_nan(float(ptr[i]), i, cnt);
+    }
+}
+
+int* check_nan_get_device_ptr() {
+    static int* ptr = nullptr;
+    if (ptr) return ptr;
+    cudaMalloc(&ptr, 4);
+    cudaMemset(ptr, 0, 4);
+    return ptr;
+}
+
+void report_nan() {
+    int cnt;
+    auto ptr = check_nan_get_device_ptr();
+    cudaMemcpy(&cnt, ptr, 4, cudaMemcpyDeviceToHost);
+    if (cnt) {
+        cudaMemset(ptr, 0, 4);
+        LOGf << "detect" << cnt << "invalid value";
     }
 }
 
 void check_nan_float64(float64* ptr, int64 num) {
     int block_num = std::max((int64)1, (num-1)/1024+1);
     int thread_num = std::min((int64)1024, num);
-    _check_nan_float64<<<block_num, thread_num>>>(ptr, num);
+    _check_nan_float64<<<block_num, thread_num>>>(ptr, num, check_nan_get_device_ptr());
+    report_nan();
 }
 
 void check_nan_float32(float32* ptr, int64 num) {
     int block_num = std::max((int64)1, (num-1)/1024+1);
     int thread_num = std::min((int64)1024, num);
-    _check_nan_float32<<<block_num, thread_num>>>(ptr, num);
+    _check_nan_float32<<<block_num, thread_num>>>(ptr, num, check_nan_get_device_ptr());
+    report_nan();
 }
 
 void check_nan_float16(__half* ptr, int64 num) {
     int block_num = std::max((int64)1, (num-1)/1024+1);
     int thread_num = std::min((int64)1024, num);
-    _check_nan_float16<<<block_num, thread_num>>>(ptr, num);
+    _check_nan_float16<<<block_num, thread_num>>>(ptr, num, check_nan_get_device_ptr());
+    report_nan();
 }
 
 #endif
 
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/nano_string.cc` & `jittor-1.3.8.1/python/jittor/src/misc/nano_string.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cstring>
 #include "misc/nano_string.h"
 
@@ -164,14 +164,15 @@
 static unordered_set<string> no_need_back_out = {
     "void",
     "cast",
     "negative",
     "add",
     "subtract",
     "multiply",
+    "divide",
 };
 
 #define DEFINE_NS(T) NanoString ns_##T;
 FOR_ALL_NS(DEFINE_NS);
 
 unordered_map<string, NanoString> __string_to_ns;
 char __ns_to_string[ns_max_size*ns_max_len];
@@ -223,14 +224,15 @@
     __string_to_ns["min"] = ns_minimum;
     __string_to_ns["max"] = ns_maximum;
     __string_to_ns["half"] = ns_float16;
     __string_to_ns["float"] = ns_float32;
     __string_to_ns["double"] = ns_float64;
     __string_to_ns["int"] = ns_int32;
     __string_to_ns["uint"] = ns_uint32;
+    __string_to_ns["bool_"] = ns_bool;
     LOGvv << "init __string_to_ns" << __string_to_ns;
     LOGvv << "init __ns_to_string" << __ns_to_string;
 }
 
 int __init_ns = (init_ns(), 0);
 
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/nano_string.h` & `jittor-1.3.8.1/python/jittor/src/misc/nano_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 
@@ -23,14 +23,15 @@
     m(uint8) \
     m(uint16) \
     m(uint32) \
     m(uint64) \
     m(float16) \
     m(float32) \
     m(float64) \
+    m(bfloat16) \
 \
     m(pow) \
     m(maximum) \
     m(minimum) \
     m(add) \
     m(subtract) \
     m(multiply) \
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/nano_vector.h` & `jittor-1.3.8.1/python/jittor/src/misc/nano_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "misc/intrin.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/ring_buffer.cc` & `jittor-1.3.8.1/python/jittor/src/misc/ring_buffer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <chrono>
 #include <thread>
 #ifndef _WIN32
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/ring_buffer.h` & `jittor-1.3.8.1/python/jittor/src/misc/ring_buffer.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #ifdef _MSC_VER
 #include <windows.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/stack_vector.h` & `jittor-1.3.8.1/python/jittor/src/misc/stack_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "misc/nano_vector.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/misc/string_view_map.h` & `jittor-1.3.8.1/python/jittor/src/misc/string_view_map.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 
 #if defined(__clang__)
```

### Comparing `jittor-1.3.7.9/python/jittor/src/node.h` & `jittor-1.3.8.1/python/jittor/src/node.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "misc/nano_string.h"
@@ -68,15 +68,15 @@
         _manual_set_vnbb = _n+9,
         // bit9: prefer 32 bit
         _prefer_32=_n+10,
         // force 16 bit
         _prefer_16=_prefer_32+1,
         // reduce keep type unchange
         _reduce_keep=_prefer_32+2,
-        _custom_flag = _reduce_keep,
+        _custom_flag = _prefer_32+6,
     };
 
     inline void set(Flags f, int a=1, int nbits=1) {
         nf_t mask = (((1u<<nbits)-1)<<f);
         flags = (flags & ~mask) | ((a<<f)&mask);
     }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/numpy_func.h` & `jittor-1.3.8.1/python/jittor/src/numpy_func.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/op.cc` & `jittor-1.3.8.1/python/jittor/src/op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <limits>
 
 #include "node.h"
@@ -12,14 +12,15 @@
 #include "op_compiler.h"
 #include "profiler/profiler.h"
 #include "mem/allocator.h"
 #include "misc/cuda_flags.h"
 #include "pybind/py_var_tracer.h"
 #include "executor.h"
 #include "var_holder.h"
+#include "fused_op.h"
 
 namespace jittor {
 
 DECLARE_FLAG(string, cache_path);
 // DECLARE_FLAG(uint8, th_mode);
 extern uint8 th_mode;
 
@@ -30,15 +31,15 @@
 string_view_map<string> jit_key_mapper;
 
 int64 Op::number_of_lived_ops = 0;
 
 Op::Op() {
     flags.set(NodeFlags::_var, 0);
     flags.set(NodeFlags::_cpu, 1);
-    flags.flags |= ((amp_reg & 7) << NodeFlags::_prefer_32);
+    flags.flags |= ((amp_reg & 63) << NodeFlags::_prefer_32);
     number_of_lived_ops++;
     if (PREDICT_BRANCH_NOT_TAKEN(trace_py_var)) trace_data.record_node(this);
 }
 
 Op::~Op() {
     number_of_lived_ops--;
 }
@@ -316,11 +317,14 @@
     }
     os << ')';
     if (trace_py_var) {
         os << '{';
         print_node_trace(op, os);
         os << '}';
     }
+    if (op->name_ex() == "fused") {
+        os << ((FusedOp*)op)->ops;
+    }
     return os;
 }
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/op.h` & `jittor-1.3.8.1/python/jittor/src/op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "node.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/op_compiler.cc` & `jittor-1.3.8.1/python/jittor/src/op_compiler.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <regex>
 #include <algorithm>
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/op_compiler.h` & `jittor-1.3.8.1/python/jittor/src/op_compiler.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/arg_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/arg_reduce_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/arg_reduce_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/arg_reduce_op.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/argsort_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/argsort_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/argsort_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/argsort_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/array_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/array_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "helper_cuda.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/array_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/array_op.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 #include "mem/allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/binary_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/binary_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/binary_op.h"
@@ -447,16 +447,18 @@
     ASSERT(ns.is_binary());
     z = create_output(x->shape, binary_dtype_infer(op, x->ns, y->ns, x->flags.get(NodeFlags::_is_scalar), y->flags.get(NodeFlags::_is_scalar)));
     bool bin = ns.get(NanoString::_no_need_back_in);
     bool bout = ns.get(NanoString::_no_need_back_out);
     if (bin || bout) {
         flags.set(NodeFlags::_manual_set_vnbb);
         if (!bin) {
-            x->flags.set(NodeFlags::_needed_by_backward);
-            y->flags.set(NodeFlags::_needed_by_backward);
+            if (!(y->is_stop_grad() && (op==ns_multiply || op==ns_divide)))
+                x->flags.set(NodeFlags::_needed_by_backward);
+            if (!(x->is_stop_grad() && (op==ns_multiply)))
+                y->flags.set(NodeFlags::_needed_by_backward);
         }
         if (!bout) {
             z->flags.set(NodeFlags::_needed_by_backward);
         }
     }
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/binary_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/binary_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/broadcast_to_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/broadcast_to_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include <algorithm>
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/broadcast_to_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/broadcast_to_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/candidate_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/candidate_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "ops/candidate_op.h"
 #ifdef JIT_cuda
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/candidate_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/candidate_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/clone_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/clone_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/clone_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/clone_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/code_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/code_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/code_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/code_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/code_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/copy_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/copy_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/copy_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/copy_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/empty_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/empty_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/empty_op.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/check_cache_pass.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
+//     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
-#include "op.h"
+#include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct EmptyOp : Op {
-    EmptyOp(NanoVector shape, NanoString dtype=ns_float32);
-    
-    const char* name() const override { return "empty"; }
+struct CheckCachePass : Pass {
+    CheckCachePass() : Pass("check_cache") {};
+    void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/fetch_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/fetch_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. 
+// Copyright (c) 2023 Jittor. 
 // All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/fetch_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/fetch_op.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <functional>
 #include "op.h"
@@ -32,14 +32,35 @@
         if (deleter) {
             deleter();
         }
     }
     void operator =(FetchFunc&& other) { this->~FetchFunc(); new (this) FetchFunc(move(other)); }
 };
 
+
+struct SimpleFunc {
+    std::function<void(int64)> callback;
+    std::function<void()> deleter;
+    SimpleFunc() = default;
+    SimpleFunc(SimpleFunc&& other) : callback(other.callback), deleter(other.deleter) {
+        other.callback = nullptr;
+        other.deleter = nullptr;
+    };
+    SimpleFunc(const SimpleFunc&) = delete;
+    SimpleFunc(std::function<void(int64)>&& callback) : callback(move(callback)) {}
+    SimpleFunc(std::function<void(int64)>&& callback, std::function<void()>&& deleter)
+    : callback(move(callback)), deleter(move(deleter)) {};
+    ~SimpleFunc() {
+        if (deleter) {
+            deleter();
+        }
+    }
+    void operator =(SimpleFunc&& other) { this->~SimpleFunc(); new (this) SimpleFunc(move(other)); }
+};
+
 struct FetchResult {
     FetchFunc func;
     vector<Allocation> allocations;
     vector<ArrayArgs> arrays;
 
     inline void call() { func.callback(this); }
 };
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/fuse_transpose_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/fuse_transpose_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "ops/fuse_transpose_op.h"
 #include "var.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/fuse_transpose_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/fuse_transpose_op.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/getitem_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/getitem_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "executor.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/getitem_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/getitem_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.  All Rights Reserved.
+// Copyright (c) 2023 Jittor.  All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 #include "var_slices.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/index_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/index_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "ops/index_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/index_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/index_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/numpy_code_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/numpy_code_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/numpy_code_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/numpy_code_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/op_register.cc` & `jittor-1.3.8.1/python/jittor/src/ops/op_register.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "op.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/op_register.h` & `jittor-1.3.8.1/python/jittor/src/ops/op_register.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <typeinfo>
 #include <typeindex>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/op_utils.cc` & `jittor-1.3.8.1/python/jittor/src/ops/op_utils.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "ops/op_register.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/random_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/random_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <random>
 
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/random_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/random_op.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reduce_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/reduce_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include <limits>
 #include "var.h"
@@ -14,14 +14,20 @@
 namespace jittor {
 
 #ifndef JIT
 static auto make_broadcast_to = get_op_info("broadcast_to")
     .get_constructor<VarPtr, Var*, Var*, uint, uint>();
 static auto make_binary = get_op_info("binary")
     .get_constructor<VarPtr, Var*, Var*, NanoString>();
+static auto make_unary = get_op_info("unary")
+    .get_constructor<VarPtr, Var*, NanoString>();
+static auto make_reduce = get_op_info("reduce")
+    .get_constructor<VarPtr, Var*, NanoString, NanoVector, bool>();
+static auto make_reduce2 = get_op_info("reduce")
+    .get_constructor<VarPtr, Var*, NanoString, uint, uint>();
 static auto make_ternary = get_op_info("ternary")
     .get_constructor<VarPtr, Var*, Var*, Var*>();
 static auto make_number = get_op_info("number")
     .get_constructor<VarPtr, float, Var*>();
 
 unordered_set<string> reduce_ops = {
     /**
@@ -242,16 +248,26 @@
         jt.Var([[5.666667 ]
          [5.3333335]], dtype=float32)
      */
     // @pybind(mean)
     "mean",
 };
 
+EXTERN_LIB int amp_reg;
+
 ReduceOp::ReduceOp(Var* x, NanoString op, NanoVector dims, bool keepdims)
     : x(x) {
+    // improve float16 mean precision
+    if (!(amp_reg & 32) && x->dtype() == ns_float16 && (op == ns_mean || op == ns_add)) {
+        auto x_float32 = make_unary(x, ns_float32);
+        auto mean = make_reduce(x_float32, op, dims, keepdims);
+        mean = make_unary(mean, ns_float16);
+        forward(mean);
+        return;
+    }
     flags.set(NodeFlags::_cpu);
     flags.set(NodeFlags::_cuda);
     set_type(OpType::reduce);
     if (op.get(NanoString::_no_need_back_in))
         flags.set(NodeFlags::_manual_set_vnbb);
     ns = op;
     ASSERT(ns.is_binary());
@@ -272,14 +288,22 @@
         y = create_output(nullptr, ns_int32);
     else
         y = create_output(nullptr, reduce_dtype_infer(ns, x->ns));
 }
 
 ReduceOp::ReduceOp(Var* x, NanoString op, uint dims_mask, uint keepdims_mask)
     : x(x) {
+    // improve float16 mean precision
+    if (!(amp_reg & 32) && x->dtype() == ns_float16 && (op == ns_mean || op == ns_add)) {
+        auto x_float32 = make_unary(x, ns_float32);
+        auto mean = make_reduce2(x_float32, op, dims_mask, keepdims_mask);
+        mean = make_unary(mean, ns_float16);
+        forward(mean);
+        return;
+    }
     flags.set(NodeFlags::_cpu);
     flags.set(NodeFlags::_cuda);
     set_type(OpType::reduce);
     if (op.get(NanoString::_no_need_back_in))
         flags.set(NodeFlags::_manual_set_vnbb);
     ns = op;
     ASSERT(ns.is_binary());
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reduce_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/reduce_op.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reindex_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/reindex_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/reindex_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reindex_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/reindex_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reindex_reduce_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/reindex_reduce_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include <limits>
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reindex_reduce_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/reindex_reduce_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reshape_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/reshape_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/reshape_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/reshape_op.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/safe_clip_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/safe_clip_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/safe_clip_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/safe_clip_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/safe_clip_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/setitem_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/setitem_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/setitem_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/setitem_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/setitem_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.  All Rights Reserved.
+// Copyright (c) 2023 Jittor.  All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
 #include "var_slices.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/tape_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/tape_op.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
@@ -62,15 +62,15 @@
                     stop grad        stop grad
         i --> tape --> t_i ---> .... ---> o --> tape --> t_o
         |                                         ^
         +---> tapes ------------------------------+
     */
     // set tape output
     for (int i=0; i<taped_outputs.size(); i++) {
-        VarPtr out(0, ns_float32);
+        VarPtr out(0, taped_outputs[i]->var->dtype());
         out->add_inputs({this});
         auto v = taped_outputs[i]->var;
         auto op = v->input();
         op->add_inputs(vector<Node*>{out.ptr});
     }
     // set tapes input 
     vector<Var*> tin(taped_inputs.size());
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/tape_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/tape_op.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/ternary_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/ternary_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "ops/ternary_op.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/ternary_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/ternary_op.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/transpose_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/transpose_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "ops/transpose_op.h"
 #include "var.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/transpose_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/transpose_op.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/unary_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/unary_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "misc/cpu_math.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/unary_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/unary_op.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/where_op.cc` & `jittor-1.3.8.1/python/jittor/src/ops/where_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "ops/where_op.h"
 #include "misc/cuda_flags.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/ops/where_op.h` & `jittor-1.3.8.1/python/jittor/src/ops/where_op.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/expr.cc` & `jittor-1.3.8.1/python/jittor/src/opt/expr.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "opt/expr.h"
 #include "utils/str_utils.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/expr.h` & `jittor-1.3.8.1/python/jittor/src/opt/expr.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/gopt/setitem_gopt.cc` & `jittor-1.3.8.1/python/jittor/src/opt/gopt/setitem_gopt.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cmath>
 #include "var.h"
 #include "ops/setitem_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/jit_searcher.cc` & `jittor-1.3.8.1/python/jittor/src/opt/jit_searcher.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <chrono>
 #include <algorithm>
 #include <functional>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/jit_searcher.h` & `jittor-1.3.8.1/python/jittor/src/opt/jit_searcher.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/kernel_ir.cc` & `jittor-1.3.8.1/python/jittor/src/opt/kernel_ir.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <algorithm>
 #include "opt/kernel_ir.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/kernel_ir.h` & `jittor-1.3.8.1/python/jittor/src/opt/kernel_ir.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "utils/str_utils.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/assume_aligned_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/assume_aligned_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/assume_aligned_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/insert_profile_loop_pass.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct AssumeAlignedPass : Pass {
-    AssumeAlignedPass() : Pass("assume_aligned") {};
+struct InsertProfileLoopPass : Pass {
+    InsertProfileLoopPass() : Pass("insert_profile_loop") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/atomic_tuner_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/vectorize_pass.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: 
-//     Guowei Yang <471184555@qq.com>
-//     Dun Liang <randonlang@gmail.com>. 
-// 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct AtomicTunerPass : Pass {
-    AtomicTunerPass() : Pass("atomic") {};
+struct VectorizePass : Pass {
+    VectorizePass() : Pass("vectorize") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/check_cache_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/check_cache_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/check_cache_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/remove_loop_pass.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: 
-//     Guoye Yang <498731903@qq.com>
-//     Dun Liang <randonlang@gmail.com>. 
-// 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct CheckCachePass : Pass {
-    CheckCachePass() : Pass("check_cache") {};
+// this is a debug pass, remove i-th loop, key: removei
+struct RemoveLoopPass : Pass {
+    RemoveLoopPass() : Pass("remove_loop") {};
     void run() override;
 };
 
-} // jittor
+} // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/compile_shapes_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/compile_shapes_pass.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/compile_shapes_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/compile_shapes_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/const_var_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/const_var_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "opt/expr.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/const_var_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/fake_main_pass.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct ConstVarPass : Pass {
-    ConstVarPass() : Pass("const_var_pass") {};
+struct FakeMainPass : Pass {
+    FakeMainPass() : Pass("fake_main") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/expand_empty_block_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/expand_empty_block_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/expand_empty_block_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/expand_empty_block_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/fake_main_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/fake_main_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/fake_main_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_pass.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct FakeMainPass : Pass {
-    FakeMainPass() : Pass("fake_main") {};
+struct MergeLoopPass : Pass {
+    MergeLoopPass() : Pass("merge_loop") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/float_atomic_fix_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/float_atomic_fix_pass.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
@@ -75,13 +75,16 @@
         s = s.substr(0, s.size()-1);
         try {
             pm->oc->get_op_var_by_name(s, op_id, opvar_id, op, var);
         } catch (...) {
             return;
         }
         if (!var->dtype().is_float()) return;
+        if (var->dtype() == ns_float16)
+            // float16 use atomicCAS, because no float16 atomicMax
+            return;
         LOGvvvv << "find var" << var << "op" << op;
         fix_float_atomic(s, var);
     });
 }
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/float_atomic_fix_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/float_atomic_fix_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/insert_profile_loop_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/insert_profile_loop_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/insert_profile_loop_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/use_movnt_pass.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: Dun Liang <randonlang@gmail.com>. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: 
+//     Guowei Yang <471184555@qq.com>
+//     Dun Liang <randonlang@gmail.com>. 
+// 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct InsertProfileLoopPass : Pass {
-    InsertProfileLoopPass() : Pass("insert_profile_loop") {};
+struct UseMovntPass : Pass {
+    UseMovntPass() : Pass("use_movnt") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/loop_to_func_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/loop_to_func_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/loop_to_func_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/loop_to_func_pass.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/loop_var_analyze_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/loop_var_analyze_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/loop_var_analyze_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/loop_var_analyze_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/mark_raw_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/mark_raw_pass.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/mark_raw_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/mark_raw_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_pass.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_var_pass.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct MergeLoopPass : Pass {
-    MergeLoopPass() : Pass("merge_loop") {};
+struct MergeLoopVarPass : Pass {
+    MergeLoopVarPass() : Pass("merge_loop_var") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_var_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/merge_loop_var_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "opt/expr.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/merge_loop_var_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/parallel_pass.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct MergeLoopVarPass : Pass {
-    MergeLoopVarPass() : Pass("merge_loop_var") {};
+struct ParallelPass : Pass {
+    ParallelPass() : Pass("parallel") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/parallel_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/restride_pass.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct ParallelPass : Pass {
-    ParallelPass() : Pass("parallel") {};
+struct RestridePass : Pass {
+    RestridePass() : Pass("restride") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/pass.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "opt/pass/pass.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/pass.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "fused_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/remove_intermediate_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/remove_intermediate_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/remove_intermediate_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/remove_intermediate_pass.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/remove_loop_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/remove_loop_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/remove_loop_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/reorder_loop_pass.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-// this is a debug pass, remove i-th loop, key: removei
-struct RemoveLoopPass : Pass {
-    RemoveLoopPass() : Pass("remove_loop") {};
+struct ReorderLoopPass : Pass {
+    ReorderLoopPass() : Pass("reorder_loop") {};
     void run() override;
+    vector<int> search_parse_loop_order();
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/rename_loop_index_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/rename_loop_index_pass.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/rename_loop_index_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/rename_loop_index_pass.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/reorder_loop_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/reorder_loop_pass.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/replace_for_num_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/replace_for_num_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/replace_for_num_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/replace_for_num_pass.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/restride_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/restride_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/restride_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner_manager.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
-#include "opt/pass/pass.h"
+#include "common.h"
+#include "opt/tuner/tuner.h"
+#include "opt/jit_searcher.h"
 
 namespace jittor {
 
-struct RestridePass : Pass {
-    RestridePass() : Pass("restride") {};
-    void run() override;
+struct TunerManager {
+    OpCompiler* oc;
+    Searcher searcher;
+    Tuner* best_tuner;
+
+    vector<unique_ptr<Tuner>> tuners;
+
+    TunerManager(OpCompiler* oc);
+    string tune();
+
+    // run and store a tuner, return confidence
+    template <class T> void run_tuner(PassManager* pm);
 };
 
-} // jittor
+}
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/shared_reduce_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/shared_reduce_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Zheng-Ning Liu <lzhengning@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/solve_conflict_define_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/solve_conflict_define_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/solve_conflict_define_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/solve_conflict_define_pass.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/split_loop_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/split_loop_pass.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/split_loop_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/split_loop_pass.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/unroll_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/unroll_pass.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/unroll_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/unroll_pass.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/use_movnt_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/use_movnt_pass.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/use_movnt_pass.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass/const_var_pass.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
-// Maintainers: 
-//     Guowei Yang <471184555@qq.com>
-//     Dun Liang <randonlang@gmail.com>. 
-// 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
+// Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "opt/pass/pass.h"
 
 namespace jittor {
 
-struct UseMovntPass : Pass {
-    UseMovntPass() : Pass("use_movnt") {};
+struct ConstVarPass : Pass {
+    ConstVarPass() : Pass("const_var_pass") {};
     void run() override;
 };
 
 } // jittor
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass/vectorize_pass.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass/vectorize_pass.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #include "var.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass_manager.cc` & `jittor-1.3.8.1/python/jittor/src/opt/pass_manager.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var.h"
 #include "opt/pass_manager.h"
 #include "opt/pass/replace_for_num_pass.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/pass_manager.h` & `jittor-1.3.8.1/python/jittor/src/opt/pass_manager.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "fused_op.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/broadcast_tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/broadcast_tuner.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/broadcast_tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/conv_tuner.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "var.h"
 #include "opt/tuner_manager.h"
 
 namespace jittor {
 
-struct BroadcastTuner : Tuner {
-    BroadcastTuner() : Tuner("broadcast") {}
+struct ConvTuner : Tuner {
+    ConvTuner() : Tuner("conv") {}
+    void forwardTune(FusedOp* fop);
     void run(PassManager* pm, TunerManager* tm);
 };
 
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/conv_tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/conv_tuner.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/conv_tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/reduce_tuner.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "var.h"
+#include "ops/reduce_op.h"
 #include "opt/tuner_manager.h"
 
 namespace jittor {
 
-struct ConvTuner : Tuner {
-    ConvTuner() : Tuner("conv") {}
-    void forwardTune(FusedOp* fop);
+struct ReduceTuner : Tuner {
+    ReduceTuner() : Tuner("reduce") {}
     void run(PassManager* pm, TunerManager* tm);
 };
 
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/matmul_tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/matmul_tuner.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 //     Guoye Yang <498731903@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/matmul_tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/matmul_tuner.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/reduce_tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/reduce_tuner.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/reduce_tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/broadcast_tuner.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guowei Yang <471184555@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "var.h"
-#include "ops/reduce_op.h"
 #include "opt/tuner_manager.h"
 
 namespace jittor {
 
-struct ReduceTuner : Tuner {
-    ReduceTuner() : Tuner("reduce") {}
+struct BroadcastTuner : Tuner {
+    BroadcastTuner() : Tuner("broadcast") {}
     void run(PassManager* pm, TunerManager* tm);
 };
 
 }
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/reorder_tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/reorder_tuner.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "opt/tuner/reorder_tuner.h"
 #include "opt/pass_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/reorder_tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/reorder_tuner.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "opt/tuner_manager.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/tuner.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/tuner.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "opt/tuner/tuner.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner/tuner.h` & `jittor-1.3.8.1/python/jittor/src/opt/tuner/tuner.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/tuner_manager.cc` & `jittor-1.3.8.1/python/jittor/src/opt/tuner_manager.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "opt/pass_manager.h"
 #include "opt/tuner_manager.h"
 #include "opt/tuner/reorder_tuner.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/var_relay.cc` & `jittor-1.3.8.1/python/jittor/src/opt/var_relay.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <unordered_set>
 #include <sstream>
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/opt/var_relay.h` & `jittor-1.3.8.1/python/jittor/src/opt/var_relay.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/parallel_compiler.cc` & `jittor-1.3.8.1/python/jittor/src/parallel_compiler.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <atomic>
 #include <chrono>
 #include <thread>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/parallel_compiler.h` & `jittor-1.3.8.1/python/jittor/src/parallel_compiler.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/cache_info.cc` & `jittor-1.3.8.1/python/jittor/src/profiler/cache_info.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/cache_info.h` & `jittor-1.3.8.1/python/jittor/src/profiler/cache_info.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/memory_checker.cc` & `jittor-1.3.8.1/python/jittor/src/profiler/memory_checker.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/memory_checker.h` & `jittor-1.3.8.1/python/jittor/src/profiler/memory_checker.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/profiler.cc` & `jittor-1.3.8.1/python/jittor/src/profiler/profiler.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <chrono>
 #include <algorithm>
 #include <sstream>
@@ -90,15 +90,15 @@
     msg = dlerror();
     #endif
     CHECK(!msg) << "Loading symbol memory_checker from" << name << "failed:" << msg;
     
     return mm;
 }
 
-EXTERN_LIB string _get_stack_info(Node* node);
+EXTERN_LIB string _get_stack_info(Node* node, const char* change_line="");
 
 static  string get_stack_info(Op* op) {
     string stack_info = "stack info:\n";
     if (string("fused") == op->name()) {
         auto fop = (FusedOp*)op;
         map<string, int> stacks;
         for (Op* op : fop->ops) {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/profiler.h` & `jittor-1.3.8.1/python/jittor/src/profiler/profiler.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "profiler/cache_info.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/profiler_guard.h` & `jittor-1.3.8.1/python/jittor/src/profiler/profiler_guard.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "profiler/cache_info.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/replacement.cc` & `jittor-1.3.8.1/python/jittor/src/profiler/replacement.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/replacement.h` & `jittor-1.3.8.1/python/jittor/src/profiler/replacement.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/simple_profiler.h` & `jittor-1.3.8.1/python/jittor/src/profiler/simple_profiler.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <chrono>
 #include <iomanip>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/profiler/vtop.cc` & `jittor-1.3.8.1/python/jittor/src/profiler/vtop.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Guoye Yang <498731903@qq.com>
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pybind/core.cc` & `jittor-1.3.8.1/python/jittor/src/pybind/core.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "core.h"
 #include "grad.h"
 #include "pyjt/py_obj_holder.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer.cc` & `jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 //     Guoye Yang <498731903@qq.com>
 //
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -402,35 +402,36 @@
 void clear_trace_data() {
     trace_data.execute_op_info.clear();
     trace_data.jit_key_map.clear();
     trace_data.id_map.clear();
     trace_data.node_data.clear();
 }
 
-string _get_stack_info(Node* node) {
+string _get_stack_info(Node* node, const char* change_line) {
     string stack_info = "";
     auto iter = trace_data.id_map.find(node);
     if (iter == trace_data.id_map.end())
         return stack_info;
     auto node_id = iter->second;
     auto iter2 = trace_data.node_data.find(node_id);
     if (iter2 == trace_data.node_data.end())
         return stack_info;
     for (auto& stack : iter2->second.stacks) {
         stack_info += stack.module_name;
         stack_info += '(';
         stack_info += stack.module_type;
         stack_info += ')';
         stack_info += " -> ";
+        stack_info += change_line;
     }
     return stack_info;
 }
 
 void print_node_trace(const Node* node, std::ostream& os) {
-    os << _get_stack_info((Node*)node);
+    os << _get_stack_info((Node*)node, "\n");
 }
 
 vector<Stack> get_node_trace(Node* node) {
     auto iter = trace_data.id_map.find(node);
     if (iter == trace_data.id_map.end())
         return vector<Stack>();
     auto node_id = iter->second;
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer.h` & `jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pybind/py_var_tracer_interface.h` & `jittor-1.3.8.1/python/jittor/src/pybind/py_var_tracer_interface.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <Python.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/numpy.cc` & `jittor-1.3.8.1/python/jittor/src/pyjt/numpy.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "pyjt/numpy.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/numpy.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/numpy.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "pyjt/py_obj_holder.h"
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_arg_printer.cc` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_arg_printer.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "pyjt/py_arg_printer.h"
 #include "pyjt/py_obj_holder.h"
 #include "pyjt/py_converter.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_arg_printer.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_arg_printer.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <Python.h>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_array_op.cc` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_array_op.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
 #include "helper_cuda.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_caller.cc` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_caller.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "pyjt/py_obj_holder.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_caller.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_caller.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_converter.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_converter.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: 
 //     Dun Liang <randonlang@gmail.com>. 
 //     Guowei Yang <471184555@qq.com>
 // 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
@@ -178,14 +178,15 @@
 }
 
 
 DEF_IS(DumpGraphs, PyObject*) to_py_object(T&& a) {
     PyObjHolder obj(_PyObject_New(&PyjtDumpGraphs));
     auto ptr = GET_RAW_PTR(T, obj.obj);
     new (ptr) T();
+    ptr->hold_vars = std::move(a.hold_vars);
     ptr->nodes_info = std::move(a.nodes_info);
     ptr->inputs = std::move(a.inputs);
     ptr->outputs = std::move(a.outputs);
     return obj.release();
 }
 
 DEF_IS(DumpGraphs, const T&) from_py_object(PyObject* obj) {
@@ -611,14 +612,35 @@
         },
         // deleter
         [obj]() { Py_DECREF(obj); }
     );
     return func;
 }
 
+struct SimpleFunc;
+
+DEF_IS(SimpleFunc, bool) is_type(PyObject* obj) {
+    return PyCallable_Check(obj);
+}
+
+DEF_IS(SimpleFunc, T) from_py_object(PyObject* obj) {
+    // PyObject_Call
+    Py_INCREF(obj);
+    T func(
+        // callback
+        [obj](int64 result) {
+            PyObjHolder args(to_py_object(result));
+            PyObjHolder ret(PyObject_CallOneArg(obj, args.obj));
+        },
+        // deleter
+        [obj]() { Py_DECREF(obj); }
+    );
+    return func;
+}
+
 CHECK_IS_2(unordered_map);
 
 DEF_IS_2(unordered_map, bool) is_type(PyObject* obj) {
     return PyDict_CheckExact(obj);
 }
 
 DEF_IS_2(unordered_map, PyObject*) to_py_object(const T& a) {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_obj_holder.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_obj_holder.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <Python.h>
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_ring_buffer.cc` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_ring_buffer.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "pyjt/py_ring_buffer.h"
 #include "pyjt/py_obj_holder.h"
 #include "pyjt/py_converter.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/py_ring_buffer.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/py_ring_buffer.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <Python.h>
 #include "misc/ring_buffer.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/pyjt/pyjt_console.h` & `jittor-1.3.8.1/python/jittor/src/pyjt/pyjt_console.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <Python.h>
 #ifdef _WIN32
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_expr.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_expr.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "opt/expr.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_fast_shared_ptr.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_fast_shared_ptr.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "misc/fast_shared_ptr.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_jit_key.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_jit_key.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "jit_key.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_kernel_ir.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_kernel_ir.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "opt/kernel_ir.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_nano_vector.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_nano_vector.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "misc/nano_vector.h"
 
 namespace jittor {
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_op_compiler.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_op_compiler.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <regex>
 #include "op_compiler.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_op_relay.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_op_relay.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "op.h"
 #include "var.h"
 #include "opt/var_relay.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_setitem_op.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_setitem_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved.
+// Copyright (c) 2023 Jittor. All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "misc/nano_vector.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/test/test_sfrl_allocator.cc` & `jittor-1.3.8.1/python/jittor/src/test/test_sfrl_allocator.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
     
 #include "opt/kernel_ir.h"
 #include "mem/allocator/sfrl_allocator.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/type/common_op_type.cc` & `jittor-1.3.8.1/python/jittor/src/type/common_op_type.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "utils/str_utils.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/type/fp16_compute.h` & `jittor-1.3.8.1/python/jittor/src/type/fp16_compute.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/type/fp16_op_type.cc` & `jittor-1.3.8.1/python/jittor/src/type/fp16_op_type.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "common.h"
 #include "utils/str_utils.h"
 #include "ops/op_register.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/types.h` & `jittor-1.3.8.1/python/jittor/src/types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <vector>
 #include <list>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/cache_compile.cc` & `jittor-1.3.8.1/python/jittor/src/utils/cache_compile.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <fstream>
 #include <streambuf>
 #ifdef _WIN32
@@ -163,28 +163,28 @@
         if (i>=src.size()) break;
         if (src[i] == '#') {
             // #include "a.h"
             // i       jk    l
             auto j=i+1;
             while (j<src.size() && (src[j] != ' ' && src[j] != '\"' && src[j] != '\n' && src[j] != '\r')) j++;
             if (j>=src.size()) return;
-            if (j-i != 8 && j-i != 6) continue;
+            if (j-i != 8 && j-i != 6 && j-i != 3) continue;
             auto k=src[j] == '\"' ? j : j+1;
             while (k<src.size() && src[k] == ' ') k++;
             if (k>=src.size()) return;
             auto l=k+1;
             while (l<src.size() && (src[l] != ' ' && src[l] != '\n' && src[l] != '\r')) l++;
             if (src[k] == '"' && src[l-1] == '"' && j-i==8 && src.substr(i,j-i) == "#include") {
                 auto inc = src.substr(k+1, l-k-2);
                 if (inc != "test.h" && inc != "helper_cuda.h") {
                     LOGvvvv << "Found include" << inc; 
                     input_names.push_back(inc);
                 }
             }
-            if (l-k>2 && src[k] == 'J' && src[k+1] == 'T' && j-i==6 && src.substr(i,j-i) == "#ifdef") {
+            if (l-k>2 && src[k] == 'J' && src[k+1] == 'T' && (src.substr(i,j-i) == "#ifdef" || src.substr(i,j-i) == "#if")) {
                 auto inc = strip(src.substr(k, l-k));
                 auto env = getenv(inc.c_str());
                 if (env && string(env)!="0") {
                     auto senv = string(env);
                     string dflag = " -D"+inc+"="+senv;
                     if (cmd.find(dflag) == string::npos) {
                         // -D flags should insert before -o flag
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/cache_compile.h` & `jittor-1.3.8.1/python/jittor/src/utils/cache_compile.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/cross_platform.h` & `jittor-1.3.8.1/python/jittor/src/utils/cross_platform.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 #ifndef _WIN32
 #include <sys/wait.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/flags.cc` & `jittor-1.3.8.1/python/jittor/src/utils/flags.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 /*
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/jit_utils.cc` & `jittor-1.3.8.1/python/jittor/src/utils/jit_utils.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "utils/cache_compile.h"
 #include "pyjt/py_converter.h"
 #include "pyjt/py_arg_printer.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/log.cc` & `jittor-1.3.8.1/python/jittor/src/utils/log.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <string.h>
 #include <signal.h>
 #include <iomanip>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/log.h` & `jittor-1.3.8.1/python/jittor/src/utils/log.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <string>
 #include <sstream>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/mwsr_list.cc` & `jittor-1.3.8.1/python/jittor/src/utils/mwsr_list.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 
 #include "utils/mwsr_list.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/mwsr_list.h` & `jittor-1.3.8.1/python/jittor/src/utils/mwsr_list.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <list>
 #include <vector>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/seh.h` & `jittor-1.3.8.1/python/jittor/src/utils/seh.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/str_utils.cc` & `jittor-1.3.8.1/python/jittor/src/utils/str_utils.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cctype>
 #include "utils/str_utils.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/str_utils.h` & `jittor-1.3.8.1/python/jittor/src/utils/str_utils.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/utils/tracer.cc` & `jittor-1.3.8.1/python/jittor/src/utils/tracer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <stdio.h>
 #include <stdlib.h>
 #include <iostream>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var.cc` & `jittor-1.3.8.1/python/jittor/src/var.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <type_traits>
 
 #include "var.h"
@@ -21,15 +21,15 @@
 DEFINE_FLAG(bool, no_grad, 0, 
     "No grad for all jittor Var creation");
 DEFINE_FLAG(bool, no_fuse, 0, 
     "No fusion optimization for all jittor Var creation");
 DEFINE_FLAG(uint8, node_order, 0, "id prior");
 DEFINE_FLAG(uint8, th_mode, 0, "th mode");
 // TODO: fuse multiple flags
-DEFINE_FLAG(int, amp_reg, 0, "Auto mixed-precision control registers, bit 0: prefer 32; bit 1: prefer 16; bit 2: keep reduce type; bit 3 keep white list type; bit 4: array like op prefer too");
+DEFINE_FLAG(int, amp_reg, 0, "Auto mixed-precision control registers, bit 0: prefer 32; bit 1: prefer 16; bit 2: keep reduce type; bit 3 keep white list type; bit 4: array like op prefer too; bit 5, reduce16 intermediate not use 32");
 
 DEFINE_FLAG_WITH_SETTER(int, auto_mixed_precision_level, 0, "Auto mixed-precision optimization level, 0: not use fp16, 1-3: preserve level, not use fp16 for now; 4: perfer fp16, but some ops use fp32 e.g. sum,exp; 5: simular with 4, and array op will automatically convert to fp16; 6: all ops prefer fp16");
 
 void (*_var_free_hook)(Var*);
 
 void free_var(Var* v) {
     if (PREDICT_BRANCH_NOT_TAKEN((bool)_var_free_hook)) _var_free_hook(v);
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var.h` & `jittor-1.3.8.1/python/jittor/src/var.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "node.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var_holder.cc` & `jittor-1.3.8.1/python/jittor/src/var_holder.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <sstream>
 #ifdef HAS_CUDA
 #include <cuda_runtime.h>
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var_holder.h` & `jittor-1.3.8.1/python/jittor/src/var_holder.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "var.h"
@@ -141,14 +141,32 @@
      */
     // @pyjt(__get__nbytes)
     inline int64 nbytes() {
         return var->num * var->dsize();
     }
 
     /** 
+     * return id of this Var.
+     */
+    // @pyjt(__get__id)
+    inline int64 id() {
+        return var->id;
+    }
+
+    // @pyjt(__get__var_ptr)
+    inline int64 var_ptr() {
+        return (int64)var;
+    }
+
+    // @pyjt(__get__flags)
+    inline int32 flags() {
+        return (int32)(var->flags.flags);
+    }
+
+    /** 
      * disable the gradient calculation for the Var.
      */
     // @pyjt(stop_grad)
     // @attrs(return_self)
     inline VarHolder* stop_grad() {
         var->set_stop_grad();
         return this;
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var_slices.cc` & `jittor-1.3.8.1/python/jittor/src/var_slices.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.  All Rights Reserved.
+// Copyright (c) 2023 Jittor.  All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include "var_slices.h"
 #include "var.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/src/var_slices.h` & `jittor-1.3.8.1/python/jittor/src/var_slices.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor.  All Rights Reserved.
+// Copyright (c) 2023 Jittor.  All Rights Reserved.
 // Maintainers: Dun Liang <randonlang@gmail.com>.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 #include "misc/nano_vector.h"
```

### Comparing `jittor-1.3.7.9/python/jittor/test/__main__.py` & `jittor-1.3.8.1/python/jittor/test/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 
 if __name__ == "__main__":
     import unittest, os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/misc/superglue.py` & `jittor-1.3.8.1/python/jittor/test/misc/superglue.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/perf/perf.py` & `jittor-1.3.8.1/python/jittor/test/perf/perf.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/system/test_nocuda_ubuntu18.04.sh` & `jittor-1.3.8.1/python/jittor/test/system/test_nocuda_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test.h` & `jittor-1.3.8.1/python/jittor/test/test.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ***************************************************************
-// Copyright (c) 2022 Jittor. All Rights Reserved. 
+// Copyright (c) 2023 Jittor. All Rights Reserved. 
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include <functional>
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_acl.py` & `jittor-1.3.8.1/python/jittor/test/test_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from .test_core import expect_error
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_adamw.py` & `jittor-1.3.8.1/python/jittor/test/test_adamw.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_affine_grid.py` & `jittor-1.3.8.1/python/jittor/test/test_affine_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_allocator.py` & `jittor-1.3.8.1/python/jittor/test/test_allocator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import gc
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_allocator2.py` & `jittor-1.3.8.1/python/jittor/test/test_allocator2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_arg_pool_op.py` & `jittor-1.3.8.1/python/jittor/test/test_arg_pool_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_arg_reduce_op.py` & `jittor-1.3.8.1/python/jittor/test/test_arg_reduce_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_argsort_op.py` & `jittor-1.3.8.1/python/jittor/test/test_argsort_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_array.py` & `jittor-1.3.8.1/python/jittor/test/test_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_asm_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_asm_tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_atomic_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_atomic_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_attention.py` & `jittor-1.3.8.1/python/jittor/test/test_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_auto_diff.py` & `jittor-1.3.8.1/python/jittor/test/test_auto_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import numpy as np
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_batchnorm.py` & `jittor-1.3.8.1/python/jittor/test/test_batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_benchmark.py` & `jittor-1.3.8.1/python/jittor/test/test_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_bicubic.py` & `jittor-1.3.8.1/python/jittor/test/test_bicubic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_binary_op.py` & `jittor-1.3.8.1/python/jittor/test/test_binary_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_bmm.py` & `jittor-1.3.8.1/python/jittor/test/test_bmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Meng-Hao Guo <guomenghao1997@gmail.com>
 #   Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_broadcast_to_op.py` & `jittor-1.3.8.1/python/jittor/test/test_broadcast_to_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_broadcast_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_broadcast_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cache.py` & `jittor-1.3.8.1/python/jittor/test/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_candidate.py` & `jittor-1.3.8.1/python/jittor/test/test_candidate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_clone.py` & `jittor-1.3.8.1/python/jittor/test/test_clone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_code_op.py` & `jittor-1.3.8.1/python/jittor/test/test_code_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_compile_options.py` & `jittor-1.3.8.1/python/jittor/test/test_compile_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_concat_op.py` & `jittor-1.3.8.1/python/jittor/test/test_concat_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_console.py` & `jittor-1.3.8.1/python/jittor/test/test_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_contrib.py` & `jittor-1.3.8.1/python/jittor/test/test_contrib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_conv_transpose.py` & `jittor-1.3.8.1/python/jittor/test/test_conv_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_conv_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_conv_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_core.py` & `jittor-1.3.8.1/python/jittor/test/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cub_cumsum.py` & `jittor-1.3.8.1/python/jittor/test/test_cub_cumsum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cublas_test_op.py` & `jittor-1.3.8.1/python/jittor/test/test_cublas_test_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cuda.py` & `jittor-1.3.8.1/python/jittor/test/test_cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from .test_core import expect_error
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cudnn_op.py` & `jittor-1.3.8.1/python/jittor/test/test_cudnn_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cumprod_op.py` & `jittor-1.3.8.1/python/jittor/test/test_cumprod_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_custom_op.py` & `jittor-1.3.8.1/python/jittor/test/test_custom_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import os
 import jittor as jt
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cutt.py` & `jittor-1.3.8.1/python/jittor/test/test_cutt.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_cutt_transpose_op.py` & `jittor-1.3.8.1/python/jittor/test/test_cutt_transpose_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_dataset.py` & `jittor-1.3.8.1/python/jittor/test/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_default_var.py` & `jittor-1.3.8.1/python/jittor/test/test_default_var.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_densenet.py` & `jittor-1.3.8.1/python/jittor/test/test_densenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_depthwise_conv.py` & `jittor-1.3.8.1/python/jittor/test/test_depthwise_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_digamma.py` & `jittor-1.3.8.1/python/jittor/test/test_digamma.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
@@ -21,15 +21,15 @@
 @unittest.skipIf(not has_autograd, "No autograd found.")
 class TestDigamma(unittest.TestCase):
     def test_digamma(self):
         for i in range(30):
             nx = np.random.uniform(0, 1, (32, 32))
             x = jt.array(nx)
             tx = torch.autograd.Variable(torch.tensor(nx, dtype=torch.float32), requires_grad=True)
-            dx = jt.math_util.gamma.digamma.apply(x)
+            dx = jt.digamma.apply(x)
             tdx = torch.digamma(tx)
             np.testing.assert_allclose(dx.data, tdx.detach().numpy(), rtol=1e-4, atol=1e-6)
             jgdx = jt.grad(dx, x)
             tgdx = torch.autograd.grad(tdx, tx, torch.ones_like(tx))[0]
             np.testing.assert_allclose(jgdx.data, tgdx.detach().numpy(), rtol=1e-4, atol=1e-6)
 
 @unittest.skipIf(not jt.compiler.has_cuda, "No CUDA found")
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_distributions.py` & `jittor-1.3.8.1/python/jittor/test/test_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_einops.py` & `jittor-1.3.8.1/python/jittor/test/test_einops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers: DongYang Li <lidongyang2001@gmail.com>.
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 from collections import namedtuple
 import tempfile
 import pickle
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_einsum.py` & `jittor-1.3.8.1/python/jittor/test/test_einsum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_emnist.py` & `jittor-1.3.8.1/python/jittor/test/test_emnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_error_msg.py` & `jittor-1.3.8.1/python/jittor/test/test_error_msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #    Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_example.py` & `jittor-1.3.8.1/python/jittor/test/test_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from jittor import init, Module
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_example_accumulate_grad.py` & `jittor-1.3.8.1/python/jittor/test/test_example_accumulate_grad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from jittor import init, Module
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fetcher.py` & `jittor-1.3.8.1/python/jittor/test/test_fetcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fft_op.py` & `jittor-1.3.8.1/python/jittor/test/test_fft_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_flags.py` & `jittor-1.3.8.1/python/jittor/test/test_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from .test_core import expect_error
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fold.py` & `jittor-1.3.8.1/python/jittor/test/test_fold.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fp16.py` & `jittor-1.3.8.1/python/jittor/test/test_fp16.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_function.py` & `jittor-1.3.8.1/python/jittor/test/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fused_op.py` & `jittor-1.3.8.1/python/jittor/test/test_fused_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os
 os.environ['OPENBLAS_NUM_THREADS'] = '1'
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_fuser.py` & `jittor-1.3.8.1/python/jittor/test/test_fuser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_grad.py` & `jittor-1.3.8.1/python/jittor/test/test_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_group_conv_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_group_conv_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_hook.py` & `jittor-1.3.8.1/python/jittor/test/test_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_image_folder.py` & `jittor-1.3.8.1/python/jittor/test/test_image_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 #     Dun Liang <randonlang@gmail.com>. 
 # All Rights Reserved.
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 
 import jittor as jt
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_inception.py` & `jittor-1.3.8.1/python/jittor/test/test_inception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_index_op.py` & `jittor-1.3.8.1/python/jittor/test/test_index_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_init.py` & `jittor-1.3.8.1/python/jittor/test/test_init.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_interpolation.py` & `jittor-1.3.8.1/python/jittor/test/test_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_jit_tests.py` & `jittor-1.3.8.1/python/jittor/test/test_jit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from jittor import LOG
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_jtune.py` & `jittor-1.3.8.1/python/jittor/test/test_jtune.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_knn.py` & `jittor-1.3.8.1/python/jittor/test/test_knn.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_lazy_execution.py` & `jittor-1.3.8.1/python/jittor/test/test_lazy_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Meng-Hao Guo <guomenghao1997@gmail.com>
 #   Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_linalg.py` & `jittor-1.3.8.1/python/jittor/test/test_linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Haoyang Peng <2247838039@qq.com>
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_load_pth.py` & `jittor-1.3.8.1/python/jittor/test/test_load_pth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_lock.py` & `jittor-1.3.8.1/python/jittor/test/test_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_log.py` & `jittor-1.3.8.1/python/jittor/test/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import os
 import re
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_longest_dis_fuse.py` & `jittor-1.3.8.1/python/jittor/test/test_longest_dis_fuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_loss.py` & `jittor-1.3.8.1/python/jittor/test/test_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_loss3d.py` & `jittor-1.3.8.1/python/jittor/test/test_loss3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Zheng-Ning Liu <lzhengning@gmail.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_lr_scheduler.py` & `jittor-1.3.8.1/python/jittor/test/test_lr_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_lstm.py` & `jittor-1.3.8.1/python/jittor/test/test_lstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Zheng-Ning Liu <lzhengning@gmail.com> 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_matmul.py` & `jittor-1.3.8.1/python/jittor/test/test_matmul.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_matmul_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_matmul_tuner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import sys
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mem.py` & `jittor-1.3.8.1/python/jittor/test/test_mem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #    Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_memory_profiler.py` & `jittor-1.3.8.1/python/jittor/test/test_memory_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_merge_loop_var_pass.py` & `jittor-1.3.8.1/python/jittor/test/test_merge_loop_var_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as numpy
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_merge_single_array_op.py` & `jittor-1.3.8.1/python/jittor/test/test_merge_single_array_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_misc_issue.py` & `jittor-1.3.8.1/python/jittor/test/test_misc_issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_misc_op.py` & `jittor-1.3.8.1/python/jittor/test/test_misc_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mkl_conv_op.py` & `jittor-1.3.8.1/python/jittor/test/test_mkl_conv_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mkl_test_op.py` & `jittor-1.3.8.1/python/jittor/test/test_mkl_test_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_models.py` & `jittor-1.3.8.1/python/jittor/test/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mpi.py` & `jittor-1.3.8.1/python/jittor/test/test_mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mpi_batchnorm.py` & `jittor-1.3.8.1/python/jittor/test/test_mpi_batchnorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mpi_in_py.py` & `jittor-1.3.8.1/python/jittor/test/test_mpi_in_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_mpi_op.py` & `jittor-1.3.8.1/python/jittor/test/test_mpi_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_nano_string.py` & `jittor-1.3.8.1/python/jittor/test/test_nano_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import time
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_nano_vector.py` & `jittor-1.3.8.1/python/jittor/test/test_nano_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import time
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_nccl.py` & `jittor-1.3.8.1/python/jittor/test/test_nccl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import jittor as jt
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_nccl_ops.py` & `jittor-1.3.8.1/python/jittor/test/test_nccl_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_new_fused_op.py` & `jittor-1.3.8.1/python/jittor/test/test_new_fused_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_node.py` & `jittor-1.3.8.1/python/jittor/test/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_notebooks.py` & `jittor-1.3.8.1/python/jittor/test/test_notebooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest, os
 import jittor as jt
 from jittor import LOG
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_numpy_code_op.py` & `jittor-1.3.8.1/python/jittor/test/test_numpy_code_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_op_compiler.py` & `jittor-1.3.8.1/python/jittor/test/test_op_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 from jittor import LOG
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_opt_state_dict.py` & `jittor-1.3.8.1/python/jittor/test/test_opt_state_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_optimizer.py` & `jittor-1.3.8.1/python/jittor/test/test_optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #    Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_optimizer_save_load.py` & `jittor-1.3.8.1/python/jittor/test/test_optimizer_save_load.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_pad.py` & `jittor-1.3.8.1/python/jittor/test/test_pad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_parallel_pass.py` & `jittor-1.3.8.1/python/jittor/test/test_parallel_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_param_list.py` & `jittor-1.3.8.1/python/jittor/test/test_param_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_profiler.py` & `jittor-1.3.8.1/python/jittor/test/test_profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_pytorch_converter.py` & `jittor-1.3.8.1/python/jittor/test/test_pytorch_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_random_op.py` & `jittor-1.3.8.1/python/jittor/test/test_random_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reduce_op.py` & `jittor-1.3.8.1/python/jittor/test/test_reduce_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reduce_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_reduce_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reindex_op.py` & `jittor-1.3.8.1/python/jittor/test/test_reindex_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reindex_reduce_op.py` & `jittor-1.3.8.1/python/jittor/test/test_reindex_reduce_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_relu.py` & `jittor-1.3.8.1/python/jittor/test/test_relu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reorder_tuner.py` & `jittor-1.3.8.1/python/jittor/test/test_reorder_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_repeat.py` & `jittor-1.3.8.1/python/jittor/test/test_repeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Zheng-Ning Liu <lzhengning@gmail.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_reshape.py` & `jittor-1.3.8.1/python/jittor/test/test_reshape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_resize_and_crop.py` & `jittor-1.3.8.1/python/jittor/test/test_resize_and_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_resnet.py` & `jittor-1.3.8.1/python/jittor/test/test_resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_ring_buffer.py` & `jittor-1.3.8.1/python/jittor/test/test_ring_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 from jittor_utils.ring_buffer import *
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_ring_buffer2.py` & `jittor-1.3.8.1/python/jittor/test/test_ring_buffer2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import jittor as jt
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_rnn.py` & `jittor-1.3.8.1/python/jittor/test/test_rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Zheng-Ning Liu <lzhengning@gmail.com>
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_rocm.py` & `jittor-1.3.8.1/python/jittor/test/test_rocm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_sampler.py` & `jittor-1.3.8.1/python/jittor/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_search_sorted.py` & `jittor-1.3.8.1/python/jittor/test/test_search_sorted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_searchsorted_op.py` & `jittor-1.3.8.1/python/jittor/test/test_searchsorted_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/test/test_setitem.py` & `jittor-1.3.8.1/python/jittor/test/test_setitem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_single_process_scope.py` & `jittor-1.3.8.1/python/jittor/test/test_single_process_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_slice.py` & `jittor-1.3.8.1/python/jittor/test/test_slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor.
+# Copyright (c) 2023 Jittor.
 # All Rights Reserved. 
 # Maintainers:
 #     Dun Liang <randonlang@gmail.com>.
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_sparse.py` & `jittor-1.3.8.1/python/jittor/test/test_sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Xiangli Li <1905692338@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_stop_fuse.py` & `jittor-1.3.8.1/python/jittor/test/test_stop_fuse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_superglue.py` & `jittor-1.3.8.1/python/jittor/test/test_superglue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_ternary_op.py` & `jittor-1.3.8.1/python/jittor/test/test_ternary_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_trace_var.py` & `jittor-1.3.8.1/python/jittor/test/test_trace_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_tracer.py` & `jittor-1.3.8.1/python/jittor/test/test_tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import os
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_transform.py` & `jittor-1.3.8.1/python/jittor/test/test_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor.
+# Copyright (c) 2023 Jittor.
 # All Rights Reserved. 
 # Maintainers:
 #     Dun Liang <randonlang@gmail.com>. 
 #
 # Contributors:
 #     Xin Yao <yaox12@outlook.com>
 #
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_transpose_op.py` & `jittor-1.3.8.1/python/jittor/test/test_transpose_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_unary_op.py` & `jittor-1.3.8.1/python/jittor/test/test_unary_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_unique.py` & `jittor-1.3.8.1/python/jittor/test/test_unique.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 #     Xiangli Li <1905692338@qq.com>
 #     Jiapeng Zhang <zhangjp20@mails.tsinghua.edu.cn>
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_utils.py` & `jittor-1.3.8.1/python/jittor/test/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import os
 from jittor import LOG
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_var.py` & `jittor-1.3.8.1/python/jittor/test/test_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 #     Zheng-Ning Liu <lzhengning@gmail.com>
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_vgg.py` & `jittor-1.3.8.1/python/jittor/test/test_vgg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/test/test_where_op.py` & `jittor-1.3.8.1/python/jittor/test/test_where_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import unittest
 import jittor as jt
 import numpy as np
```

### Comparing `jittor-1.3.7.9/python/jittor/transform/__init__.py` & `jittor-1.3.8.1/python/jittor/transform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor.
+# Copyright (c) 2023 Jittor.
 # All Rights Reserved. 
 # Maintainers:
 #     Dun Liang <randonlang@gmail.com>. 
 #
 # Contributors:
 #     Xin Yao <yaox12@outlook.com>
 #
```

### Comparing `jittor-1.3.7.9/python/jittor/transform/function_pil.py` & `jittor-1.3.8.1/python/jittor/transform/function_pil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor.
+# Copyright (c) 2023 Jittor.
 # All Rights Reserved. 
 # Maintainers:
 #     Dun Liang <randonlang@gmail.com>. 
 #
 # Contributors:
 #     Xin Yao <yaox12@outlook.com>
 #
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/asm_tuner.py` & `jittor-1.3.8.1/python/jittor/utils/asm_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Guowei Yang <471184555@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/converter_server.py` & `jittor-1.3.8.1/python/jittor/utils/converter_server.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/utils/data.gz` & `jittor-1.3.8.1/python/jittor/utils/data.gz`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/utils/dlink_compiler.py` & `jittor-1.3.8.1/python/jittor/utils/dlink_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/utils/dumpdef.py` & `jittor-1.3.8.1/python/jittor/utils/dumpdef.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/utils/gen_pyi.py` & `jittor-1.3.8.1/python/jittor/utils/gen_pyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved.
+# Copyright (c) 2023 Jittor. All Rights Reserved.
 # Maintainers:
 #     Zheng-Ning Liu <lzhengning@com>
 #
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/jtune.py` & `jittor-1.3.8.1/python/jittor/utils/jtune.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 from ctypes import cdll
 import sys
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/local_doc_builder.py` & `jittor-1.3.8.1/python/jittor/utils/local_doc_builder.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor/utils/nvtx.py` & `jittor-1.3.8.1/python/jittor/utils/nvtx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor.
+# Copyright (c) 2023 Jittor.
 # All Rights Reserved. 
 # Maintainers:
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/polish.py` & `jittor-1.3.8.1/python/jittor/utils/polish.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 
 # Polish steps:
 # 1. create jittor-polish repo
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/polish_centos.py` & `jittor-1.3.8.1/python/jittor/utils/polish_centos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import jittor as jt
 import os
 import jittor_utils as jit_utils
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/publish.py` & `jittor-1.3.8.1/python/jittor/utils/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/pytorch_converter.py` & `jittor-1.3.8.1/python/jittor/utils/pytorch_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Wenyang Zhou <576825820@qq.com>
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor/utils/tracer.py` & `jittor-1.3.8.1/python/jittor/utils/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor.egg-info/PKG-INFO` & `jittor-1.3.8.1/python/jittor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittor
-Version: 1.3.7.9
+Version: 1.3.8.1
 Summary: a Just-in-time(JIT) deep learning framework
 Home-page: http://jittor.org
 Author: Jittor Group
 Author-email: ran.donglang@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `jittor-1.3.7.9/python/jittor.egg-info/SOURCES.txt` & `jittor-1.3.8.1/python/jittor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 python/jittor/misc.py
 python/jittor/nn.py
 python/jittor/optim.py
 python/jittor/pool.py
 python/jittor/pyjt_compiler.py
 python/jittor/sparse.py
 python/jittor/version
+python/jittor/weightnorm.py
 python/jittor.egg-info/PKG-INFO
 python/jittor.egg-info/SOURCES.txt
 python/jittor.egg-info/dependency_links.txt
 python/jittor.egg-info/requires.txt
 python/jittor.egg-info/top_level.txt
 python/jittor/ccl/__init__.py
 python/jittor/ccl/ccl_2d.py
@@ -164,14 +165,17 @@
 python/jittor/extern/rocm/rocm_jittor.h
 python/jittor/extern/rocm/rocm_wrapper.h
 python/jittor/loss3d/__init__.py
 python/jittor/loss3d/chamfer.py
 python/jittor/loss3d/emd.py
 python/jittor/math_util/__init__.py
 python/jittor/math_util/gamma.py
+python/jittor/math_util/igamma.py
+python/jittor/math_util/src/gamma_grad.h
+python/jittor/math_util/src/igamma.h
 python/jittor/models/__init__.py
 python/jittor/models/alexnet.py
 python/jittor/models/densenet.py
 python/jittor/models/googlenet.py
 python/jittor/models/inception.py
 python/jittor/models/mnasnet.py
 python/jittor/models/mobilenet.py
@@ -557,16 +561,18 @@
 python/jittor/test/test_fft_op.py
 python/jittor/test/test_flags.py
 python/jittor/test/test_fold.py
 python/jittor/test/test_fp16.py
 python/jittor/test/test_function.py
 python/jittor/test/test_fused_op.py
 python/jittor/test/test_fuser.py
+python/jittor/test/test_gamma_distribution.py
 python/jittor/test/test_grad.py
 python/jittor/test/test_group_conv_tuner.py
+python/jittor/test/test_histc.py
 python/jittor/test/test_hook.py
 python/jittor/test/test_image_folder.py
 python/jittor/test/test_inception.py
 python/jittor/test/test_index_op.py
 python/jittor/test/test_init.py
 python/jittor/test/test_interpolation.py
 python/jittor/test/test_jit_tests.py
@@ -644,14 +650,15 @@
 python/jittor/test/test_transform.py
 python/jittor/test/test_transpose_op.py
 python/jittor/test/test_unary_op.py
 python/jittor/test/test_unique.py
 python/jittor/test/test_utils.py
 python/jittor/test/test_var.py
 python/jittor/test/test_vgg.py
+python/jittor/test/test_weightnorm.py
 python/jittor/test/test_where_op.py
 python/jittor/test/misc/superglue.py
 python/jittor/test/perf/perf.py
 python/jittor/test/system/test_all.sh
 python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh
 python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh
 python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/__init__.py` & `jittor-1.3.8.1/python/jittor_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 from multiprocessing import Pool
 import multiprocessing as mp
 import subprocess as sp
@@ -671,15 +671,16 @@
     '''
     with open(source_name, "r", encoding="utf8") as f:
         src = f.read()
     with open(source_name, "w", encoding="utf8") as f:
         f.write(src + entry_src)
     jittor_path = os.path.join(os.path.dirname(__file__), "..", "jittor")
     jittor_path = os.path.abspath(jittor_path)
-    do_compile([f"\"{cc_path}\" \"{source_name}\" \"{jittor_path}/src/pyjt/py_arg_printer.cc\" {flags} -o \"{cache_path+'/'+lib_name}\" ",
+    from jittor.compiler import fix_cl_flags
+    do_compile([fix_cl_flags(f"\"{cc_path}\" \"{source_name}\" \"{jittor_path}/src/pyjt/py_arg_printer.cc\" {flags} -o \"{cache_path+'/'+lib_name}\" "),
         cache_path, jittor_path])
     with import_scope(os.RTLD_GLOBAL | os.RTLD_NOW):
         exec(f"import {hash}")
     mod = locals()[hash]
     return mod
 
 def process_jittor_source(device_type, callback):
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/auto_diff.py` & `jittor-1.3.8.1/python/jittor_utils/auto_diff.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/auto_git_tag.py` & `jittor-1.3.8.1/python/jittor_utils/auto_git_tag.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/class/motd` & `jittor-1.3.8.1/python/jittor_utils/class/motd`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/class/setup_env.py` & `jittor-1.3.8.1/python/jittor_utils/class/setup_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Guoye Yang <498731903@qq.com>
 #     Dun Liang <randonlang@gmail.com>.
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/clean_cache.py` & `jittor-1.3.8.1/python/jittor_utils/clean_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os, sys, shutil
 import glob
 import jittor_utils as jit_utils
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/config.py` & `jittor-1.3.8.1/python/jittor_utils/config.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/github_release.sh` & `jittor-1.3.8.1/python/jittor_utils/github_release.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/install_cuda.py` & `jittor-1.3.8.1/python/jittor_utils/install_cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: Dun Liang <randonlang@gmail.com>. 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import os
 import sys
 import subprocess as sp
@@ -107,30 +107,32 @@
         elif cuda_driver_version >= [11,]:
             cuda_tgz = "cuda11.0_cudnn8_win.zip"
             md5 = "7a248df76ee5e79623236b0560f8d1fd"
         elif cuda_driver_version >= [10,]:
             cuda_tgz = "cuda10.2_cudnn7_win.zip"
             md5 = "7dd9963833a91371299a2ba58779dd71"
         else:
-            raise RuntimeError(f"Unsupport cuda driver version: {cuda_driver_version}, at least 10.2")
+            LOG.w(f"Unsupport cuda driver version: {cuda_driver_version}, at least 10.2")
+            return None
     else:
         if cuda_driver_version >= [11,2]:
             cuda_tgz = "cuda11.2_cudnn8_linux.tgz"
             md5 = "b93a1a5d19098e93450ee080509e9836"
         elif cuda_driver_version >= [11,]:
             cuda_tgz = "cuda11.0_cudnn8_linux.tgz"
             md5 = "5dbdb43e35b4db8249027997720bf1ca"
         elif cuda_driver_version >= [10,2]:
             cuda_tgz = "cuda10.2_cudnn7_linux.tgz"
             md5 = "40f0563e8eb176f53e55943f6d212ad7"
         elif cuda_driver_version >= [10,]:
             cuda_tgz = "cuda10.0_cudnn7_linux.tgz"
             md5 = "f16d3ff63f081031d21faec3ec8b7dac"
         else:
-            raise RuntimeError(f"Unsupport cuda driver version: {cuda_driver_version}, at least 10.0")
+            LOG.w(f"Unsupport cuda driver version: {cuda_driver_version}, at least 10.0")
+            return None
     jtcuda_path = os.path.join(jit_utils.home(), ".cache", "jittor", "jtcuda")
     nvcc_path = os.path.join(jtcuda_path, cuda_tgz[:-4], "bin", "nvcc")
     if os.name=='nt': nvcc_path += '.exe'
     nvcc_lib_path = os.path.join(jtcuda_path, cuda_tgz[:-4], "lib64")
     sys.path.append(nvcc_lib_path)
     new_ld_path = os.environ.get("LD_LIBRARY_PATH", "") + ":" + nvcc_lib_path
     os.environ["LD_LIBRARY_PATH"] = new_ld_path
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/load_pytorch.py` & `jittor-1.3.8.1/python/jittor_utils/load_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 def _dtype_to_storage_type_map():
     return {
         np.float16: 'HalfStorage',
         np.float32: 'FloatStorage',
         np.int64: 'LongStorage',
         np.int32: 'IntStorage',
         np.int16: 'ShortStorage',
-        np.int8: 'CharStorage'
+        np.int8: 'CharStorage',
+        np.bool_: 'BoolStorage'
     }
 
 def _storage_type_to_dtype_map():
     dtype_map = {
         val: key for key, val in _dtype_to_storage_type_map().items()}
     return dtype_map
 
@@ -82,14 +83,16 @@
 def jittor_rebuild_var(data, requires_grad, backward_hooks):
     v = jt.array(data)
     v.requires_grad = requires_grad
     return v
 
 class UnpicklerWrapper(pickle.Unpickler):  # type: ignore[name-defined]
     def find_class(self, mod_name, name):
+        if mod_name.startswith("transformers"):
+            return super().find_class("collections", "OrderedDict")
         if type(name) is str and 'Storage' in name:
             try:
                 return StorageType(name)
             except KeyError:
                 pass
         if type(name) is str and '_rebuild_tensor_v2' in name:
             return super().find_class("jittor_utils.load_pytorch", "jittor_rebuild")
@@ -116,14 +119,17 @@
 
 def jittor_rebuild_var_direct(data, requires_grad, backward_hooks):
     v = ArrayWrapper(storage, requires_grad=requires_grad)
     return v
 
 class DirectUnpicklerWrapper(pickle.Unpickler):  # type: ignore[name-defined]
     def find_class(self, mod_name, name):
+        if mod_name.startswith("transformers"):
+            return super().find_class("collections", "OrderedDict")
+
         if type(name) is str and 'Storage' in name:
             try:
                 return StorageType(name)
             except KeyError:
                 pass
         if type(name) is str and '_rebuild_tensor_v2' in name:
             return super().find_class("jittor_utils.load_pytorch", "jittor_rebuild_direct")
@@ -189,14 +195,21 @@
                 deserialized_objects[view_key] = storage[offset:offset + view_size]
             return deserialized_objects[view_key]
         else:
             return storage
     else:
         raise RuntimeError("Unknown saved id type: %s" % saved_id[0])
 
+def clean_globals():
+    global contents, deserialized_objects, loaded_storages, prefix
+    loaded_storages = {}
+    deserialized_objects = {}
+    contents = None
+    prefix = ""
+
 def load_pytorch(fn_name):
     import jittor as jt
     global contents, deserialized_objects, loaded_storages, prefix
     loaded_storages = {}
     deserialized_objects = {}
     if not (fn_name.endswith(".pth") or fn_name.endswith(".pt") or fn_name.endswith(".bin")):
         print("This function is designed to load pytorch pth format files.")
@@ -266,13 +279,14 @@
                                 result[key] = result[key].reindex(params.size, [evals], extras=[jt.array(params.stride)])
                             else:
                                 result[key] = result[key].reshape(shape)
                         if requires_grad is not None:
                             result[key].requires_grad = requires_grad
                 return result
             result = dfs_results(result)
+        clean_globals()
         return result
 
 if __name__ == "__main__":
     result = load_pytorch("van_base.pth")
     for key, val in result.items():
         print(key, val.shape)
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/load_pytorch_old.py` & `jittor-1.3.8.1/python/jittor_utils/load_pytorch_old.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/lock.py` & `jittor-1.3.8.1/python/jittor_utils/lock.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/misc.py` & `jittor-1.3.8.1/python/jittor_utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #     Meng-Hao Guo <guomenghao1997@gmail.com>
 #     Dun Liang <randonlang@gmail.com>.
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/pack_offline.py` & `jittor-1.3.8.1/python/jittor_utils/pack_offline.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/pip_publish.py` & `jittor-1.3.8.1/python/jittor_utils/pip_publish.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/query_cuda_cc.py` & `jittor-1.3.8.1/python/jittor_utils/query_cuda_cc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/python/jittor_utils/ring_buffer.py` & `jittor-1.3.8.1/python/jittor_utils/ring_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers: 
 #     Dun Liang <randonlang@gmail.com>. 
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 import multiprocessing as mp
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/student_queue.py` & `jittor-1.3.8.1/python/jittor_utils/student_queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ***************************************************************
-# Copyright (c) 2022 Jittor. All Rights Reserved. 
+# Copyright (c) 2023 Jittor. All Rights Reserved. 
 # Maintainers:
 #   Dun Liang <randonlang@gmail.com>.
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 from socketserver import ThreadingTCPServer
```

### Comparing `jittor-1.3.7.9/python/jittor_utils/translator.py` & `jittor-1.3.8.1/python/jittor_utils/translator.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.7.9/setup.py` & `jittor-1.3.8.1/setup.py`

 * *Files identical despite different names*

