# Comparing `tmp/federa-0.0.2.tar.gz` & `tmp/federa-0.0.3.tar.gz`

## Comparing `federa-0.0.2.tar` & `federa-0.0.3.tar`

### file list

```diff
@@ -1,1374 +1,42 @@
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_131.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_178.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_38.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_46.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_56.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_57.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Breast_1_58.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_0_10192.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_0_2599.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_0_27.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_10_2647.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_10_7361.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_11_6369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_12_3194.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_12_6281.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_1_1545.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_2_10770.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_2_1294.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_2_2942.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_4808.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_563.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_8533.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_9185.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_9271.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_3_9492.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_5_10699.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_5_3477.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_5_756.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_5_7941.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_5_8493.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_6_7326.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_7_10995.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_7_8642.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_7_9211.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_8_2448.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Chestxray_9_1970.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_10252.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_10370.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_1901.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_2534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_4375.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_521.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_5368.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_7082.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_72818.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_7570.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_0_9852.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_1_757.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_2_26531.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_2_3752.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_2_8134.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_2_8207.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_2_9648.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_1567.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_1669.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_2292.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_2794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_4851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_4912.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_5127.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_5626.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_5777.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_6087.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_6417.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Oct_3_9802.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_10673.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_12024.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_12038.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_14742.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_1487.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_17483.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_18694.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_20122.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_2373.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_3171.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_411.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_4904.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_6028.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_7434.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_8139.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_8962.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_9511.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_0_9949.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_3_8272.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_3_9593.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_4_10949.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_4_16558.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_4_17314.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_4_18139.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_4_2355.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_5_17494.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_5_22443.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_11839.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_12194.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_13317.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_14084.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_15019.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_15092.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_15204.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_17363.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_19355.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_19528.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_21927.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_6_37014.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_14747.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_14849.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_18085.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_18646.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_21396.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_21427.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_2508.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_2884.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_7116.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/test/Tissue_7_7248.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_0.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_11.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_115.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_14.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_20.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_24.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_28.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_3.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_30.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_33.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_45.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_47.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_64.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_66.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_71.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_73.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_74.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_0_85.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_1.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_10.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_12.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_13.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_15.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_16.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_17.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_2.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_21.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_22.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_227.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_23.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_249.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_25.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_27.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_29.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_32.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_34.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_35.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_37.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_40.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_408.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_41.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_42.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_43.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_433.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_48.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_5.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_50.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_51.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_52.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_53.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_54.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_55.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_6.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_60.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_61.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_62.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_64.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_65.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_68.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_69.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_7.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_70.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_72.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_75.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_76.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_77.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_8.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Breast_1_9.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_10696.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_10927.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_11206.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_2549.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_44.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_4584.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_474.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_4858.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_5282.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6167.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6235.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6401.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6403.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6438.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_6482.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_7202.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_752.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_7551.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_0_8453.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_10_4463.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_1275.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_2068.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_3915.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_4063.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_64880.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_7570.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_11_9678.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_10521.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_1472.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_151.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_194.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_3225.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_3458.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_4112.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_4694.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_5795.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_7320.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_12_9084.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_10242.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_4797.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_6404.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_7034.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_7388.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_8324.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_8326.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_1_8907.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10082.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10125.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10149.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10349.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10524.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10638.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_10750.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_11137.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_1160.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_1177.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_1408.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_1727.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_1832.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_2029.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_2134.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_2535.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_3045.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_3462.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_3820.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_4261.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_5098.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_5125.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_5669.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_5987.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_6509.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_6807.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7015.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7113.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7131.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7152.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7430.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7706.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_7865.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_8054.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_8099.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_8955.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_9745.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_9882.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_9918.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_2_9951.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_10171.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_10717.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_1072.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_10733.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_11004.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_11050.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_1627.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_1767.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_18163.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2116.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2130.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_220.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2320.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2340.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2410.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2639.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_2759.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3346.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3435.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3561.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3650.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3761.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3919.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_3952.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_421.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4216.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4402.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_443.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4675.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4703.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4836.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4895.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4919.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_4949.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_512.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_5301.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_5605.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_6751.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_7412.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_7657.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_7667.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_7801.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_8160.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_8298.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_8713.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_8954.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_9047.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_9081.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_9523.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_9811.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_3_982.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_1067.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_1162.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_1173.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_2288.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_3105.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_4324.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_6177.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_7510.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_7946.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_8534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_8754.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_9122.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_9534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_4_9580.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_10800.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_1091.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_1776.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_3935.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_4079.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_554.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_5938.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_6184.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_6391.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_9471.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_5_9729.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_1513.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_3188.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_5225.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_5805.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_7399.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_8382.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_8988.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_9056.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_6_9185.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_10100.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_10571.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_1145.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_1717.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_3195.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_5008.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_503.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_61644.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_69.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_7171.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_7260.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_7293.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_7542.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_7828.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_823.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_7_9268.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_17335.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_187.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_2918.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_3663.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_4409.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_6667.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_6771.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_8104.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_8_9794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_9_2208.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_9_236.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_9_2714.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_9_6875.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Chestxray_9_7803.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_10255.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1033.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_10376.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_10487.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1060.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1173.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1250.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1373.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1380.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1399.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1517.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1524.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1662.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1684.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1746.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_1924.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2014.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2158.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2279.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2548.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2596.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2722.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2935.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2954.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_2972.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3006.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3027.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3071.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3482.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3485.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3571.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3607.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3642.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3859.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_3988.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_4289.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_4290.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_4333.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_449.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_450.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_4634.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5293.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5502.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5688.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5722.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5798.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_5857.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_596.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_6403.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_6663.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_6760.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_6922.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7047.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7081.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7107.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7151.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7218.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7233.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7331.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7354.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7581.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7616.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_772.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7767.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7831.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7892.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7906.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_7992.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8074.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8106.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8302.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8346.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8348.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8489.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8843.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_8955.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9002.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9224.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9362.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9377.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9453.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9587.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_0_9755.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_1207.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_1753.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_1796.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_2078.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_2182.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_2987.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_3566.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_4093.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_4149.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_4366.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_4436.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_5388.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_54.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_5800.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_6105.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_6414.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_65387.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_7773.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_8424.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_8527.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_8876.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_8976.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_9014.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_902.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_9097.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_1_9702.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_10143.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_10483.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_1052.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_10661.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_2610.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_26446.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_27682.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_3036.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_3249.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_4057.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_4370.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_5788.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_5962.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_5985.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_6369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_7924.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_8401.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_9099.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_9163.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_9652.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_2_9760.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10010.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10059.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10063.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10164.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10261.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10341.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10348.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10360.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10441.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10444.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_10811.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1092.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1269.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1370.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1588.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1671.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1799.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1820.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_1869.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2031.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2211.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2217.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2259.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2277.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2300.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2320.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2345.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2388.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_25.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2500.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2530.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2624.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_271.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2777.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2915.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_2921.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3087.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_314.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3240.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3282.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3379.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3447.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3492.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_36.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3660.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3685.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3771.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3895.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_3983.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4006.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4101.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4393.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4416.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4499.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4657.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4711.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4786.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_480.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4887.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4993.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4996.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_4997.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5083.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5087.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5098.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5157.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5187.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5425.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5501.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5650.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5657.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5765.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5805.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5859.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5967.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_5992.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6058.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6112.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_619.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6209.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6240.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6277.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6411.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6561.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6614.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6674.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_6903.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_7007.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_7102.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_7352.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_7453.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_7833.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8099.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_823.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8352.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8399.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8446.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_852.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8542.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8627.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8752.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8781.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8817.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8890.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_8911.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9019.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9356.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9482.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9592.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9744.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9875.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Oct_3_9938.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10065.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10235.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10275.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10363.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10501.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10715.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10876.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_10970.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_1104.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11215.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11293.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11304.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11407.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11543.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11564.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11609.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_11911.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_12370.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_12488.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_12745.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_12909.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_13156.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_13261.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_13568.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_13699.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_13863.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14042.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14286.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14385.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14542.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14599.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14672.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14761.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_14805.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_1507.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15264.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_154.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15446.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15489.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15550.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15846.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15920.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_15943.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16003.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16179.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16471.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16578.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16604.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16671.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16729.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16738.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16811.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_16840.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17170.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17171.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17285.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17376.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17412.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17486.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17613.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_17929.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18094.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18387.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18481.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18485.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18497.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18545.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18552.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18581.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18612.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18634.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18715.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18737.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18825.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_18933.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19059.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19110.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19120.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19162.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19290.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19312.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19356.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19436.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19781.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19861.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_19937.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20028.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20365.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20416.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20423.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20465.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20502.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20740.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_20901.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2091.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21093.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21164.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21240.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21398.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21504.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21546.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_21663.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2183.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22081.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22085.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22135.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22355.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22468.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22513.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22550.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22615.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2285.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22873.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_22928.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23157.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23203.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23279.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23295.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23422.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_23562.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2737.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2896.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_2965.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3072.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3132.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3156.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3214.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3264.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3382.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3487.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3652.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3802.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3864.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_3966.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4209.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4414.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4466.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4795.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_488.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4947.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_4996.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5025.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5105.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5182.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5184.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5350.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5512.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5714.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5863.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5916.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_5970.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6260.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6261.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6278.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6368.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_65.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_653.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6793.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_6952.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7195.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7443.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7602.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7610.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7645.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_77.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_7807.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8051.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8072.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8147.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8340.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_836.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8607.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8697.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8699.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8796.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_8870.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_913.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_961.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_9629.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_9702.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_0_9822.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_1213.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_13054.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_13876.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_14595.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_14914.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_15318.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_15828.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_17215.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_17772.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_18026.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_19496.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_19798.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_1987.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_20308.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_20756.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_21050.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_2323.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_4574.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_483.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_6495.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_7192.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_7418.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_8376.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_8601.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_8790.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_1_9741.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_12291.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_12512.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_13211.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_14652.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_1538.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_15651.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_17690.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_20081.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_20348.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_20909.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_22554.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_32155.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_4327.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_5861.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_6910.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_9569.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_9599.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_2_9684.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_10163.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_11736.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_12666.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_12794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_13262.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_13850.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_1443.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_15028.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_15037.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_1526.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_15283.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_15641.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_1584.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_16139.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_16275.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_16431.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_1673.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_17222.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_17288.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_17682.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_17823.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_18447.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_18679.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_18706.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_1891.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_19517.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_19530.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_19595.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_19725.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_21530.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_21678.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_21791.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_22927.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_23085.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_23161.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_3332.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_42135.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_480.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_492.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_5199.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_5292.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_5334.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_5376.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_5378.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6005.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6065.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6238.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6310.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6344.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6730.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_6861.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_7346.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_7502.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_7831.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_8562.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_3_9809.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_10991.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_11167.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_11184.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_11425.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_11664.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_11790.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_1208.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_12407.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_13305.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_14365.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_14431.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_14691.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_1501.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15191.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15266.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15269.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15273.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15333.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_15662.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_1600.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_16887.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_17707.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_17947.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_18588.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_19067.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_19602.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_20012.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_21513.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_22008.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_22293.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_22427.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_3675.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_3731.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_4221.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_4419.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_44906.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_4744.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_6584.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_6589.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_6739.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_6827.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_6904.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_7830.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_7968.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_8010.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_4_8585.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_1049.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_10618.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_12264.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_12835.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_12894.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_14246.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_14371.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_14841.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_1639.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_17423.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_19155.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_19755.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_20836.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_21381.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_23079.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_23084.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_23166.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_4184.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_4787.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_5071.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_677.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_7029.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_7723.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_7938.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_8424.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_5_8628.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10222.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10237.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10372.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10478.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10497.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10944.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_10972.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1101.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_11356.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_11461.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_11686.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_11775.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_119.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_12285.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_12712.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_12874.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1291.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1295.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_13046.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_13250.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_13321.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1335.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_13369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_13715.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_14052.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_14469.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1468.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_15347.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_15468.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_15472.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_15603.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_15999.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_16265.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_16560.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_16636.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_16930.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_16985.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17098.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1725.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17308.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17357.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17462.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17968.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_17979.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_18189.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1838.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_18661.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_18676.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_18883.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_18893.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19159.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19308.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19401.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19430.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_1946.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19776.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19930.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_19935.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20138.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20273.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20359.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20857.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_20977.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21009.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21052.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21207.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21295.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21514.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21539.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21926.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_21973.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2203.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22133.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22138.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22348.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22357.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22475.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22642.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22907.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2296.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_22988.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_23056.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_23287.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_23485.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2518.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2800.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2841.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2933.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_2978.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_3307.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_3309.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_3506.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_3536.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4076.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4133.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4359.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4373.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4524.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4591.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4726.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4749.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4882.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_4905.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5016.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5115.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5250.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5648.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5723.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_5879.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6110.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6229.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6292.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6439.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6542.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6602.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6749.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_6841.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_7207.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_7236.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_7756.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8011.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8196.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8227.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8382.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8700.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8818.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_8988.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9130.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9150.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_922.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_945.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9465.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9501.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9528.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9640.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_6_9849.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_1044.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_10916.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_10989.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_111.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_11487.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_11578.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_11828.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_12436.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_12736.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_12790.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_12842.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_13524.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_13934.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_1432.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_14811.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_14913.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_14926.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_14952.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_15198.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_15521.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_15876.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_1603.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_16273.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_16532.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_16716.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_17507.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_17704.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_17779.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_17938.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_18050.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_18300.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_18464.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_1861.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_20002.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_20065.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_2033.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_20552.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_2076.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_20864.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_21117.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_21211.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_21259.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_21986.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_22009.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_22260.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_22369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_2242.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_2259.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_23231.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_23478.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_2718.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_3229.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_3920.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_4142.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_45543.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_4694.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_4763.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_4809.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_4851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_5052.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_5664.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_6052.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_6219.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_640.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_6526.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_6702.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7044.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7065.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7235.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7722.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7859.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7914.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_7993.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_8054.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_8107.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_8200.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_904.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_9210.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_9691.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/client_custom_dataset/CUSTOM/train/Tissue_7_9759.npy
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_algorithms.json
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_datasets.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_models.json
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_modules.json
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_results.json
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 federa-0.0.2/configs/test_scalability.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 federa-0.0.2/federa/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/start_client.py
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/ClientConnection_pb2.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/ClientConnection_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/__init__.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/client.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/client_lib.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/data_utils.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/distribution.py
--rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/get_data.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/net.py
--rw-r--r--   0        0        0    15264 2020-02-02 00:00:00.000000 federa-0.0.2/federa/client/src/net_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/start_server.py
--rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/ClientConnection_pb2.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/ClientConnection_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/__init__.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/client_connection_servicer.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/client_manager.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/client_wrapper.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server_lib.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/verification.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/fedadagrad.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/fedadam.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/fedavg.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/fedavgm.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/feddyn.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/fedyogi.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/mime.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/mimelite.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/algorithms/scaffold.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server_evaluate/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server_evaluate/eval_lib.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server_evaluate/net.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 federa-0.0.2/federa/server/src/server_evaluate/net_lib.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_131.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_178.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_38.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_46.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_56.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_57.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Breast_1_58.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_0_10192.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_0_2599.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_0_27.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_10_2647.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_10_7361.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_11_6369.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_12_3194.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_12_6281.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_1_1545.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_2_10770.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_2_1294.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_2_2942.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_4808.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_563.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_8533.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_9185.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_9271.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_3_9492.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_5_10699.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_5_3477.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_5_756.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_5_7941.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_5_8493.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_6_7326.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_7_10995.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_7_8642.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_7_9211.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_8_2448.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Chestxray_9_1970.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_10252.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_10370.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_1901.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_2534.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_4375.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_521.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_5368.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_7082.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_72818.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_7570.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_0_9852.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_1_757.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_2_26531.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_2_3752.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_2_8134.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_2_8207.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_2_9648.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_1567.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_1669.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_2292.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_2794.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_4851.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_4912.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_5127.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_5626.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_5777.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_6087.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_6417.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Oct_3_9802.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_10673.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_12024.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_12038.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_14742.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_1487.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_17483.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_18694.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_20122.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_2373.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_3171.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_411.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_4904.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_6028.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_7434.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_8139.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_8962.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_9511.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_0_9949.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_3_8272.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_3_9593.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_4_10949.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_4_16558.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_4_17314.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_4_18139.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_4_2355.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_5_17494.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_5_22443.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_11839.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_12194.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_13317.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_14084.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_15019.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_15092.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_15204.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_17363.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_19355.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_19528.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_21927.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_6_37014.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_14747.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_14849.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_18085.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_18646.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_21396.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_21427.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_2508.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_2884.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_7116.npy
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 federa-0.0.2/server_custom_dataset/CUSTOM/test/Tissue_7_7248.npy
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/test/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 federa-0.0.2/test/misc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/test/benchtest/__init__.py
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 federa-0.0.2/test/benchtest/test_results.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 federa-0.0.2/test/benchtest/test_scalability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/test/unittest/__init__.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 federa-0.0.2/test/unittest/test_algorithms.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 federa-0.0.2/test/unittest/test_datasets.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 federa-0.0.2/test/unittest/test_models.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 federa-0.0.2/test/unittest/test_modules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 federa-0.0.2/LICENSE
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 federa-0.0.2/README.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 federa-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 federa-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 federa-0.0.3/federa/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/start_client.py
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/ClientConnection_pb2.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/ClientConnection_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/__init__.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/client.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/client_lib.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/data_utils.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/distribution.py
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/get_data.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/net.py
+-rw-r--r--   0        0        0    15264 2020-02-02 00:00:00.000000 federa-0.0.3/federa/client/src/net_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/start_server.py
+-rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/ClientConnection_pb2.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/ClientConnection_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/__init__.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/client_connection_servicer.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/client_manager.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/client_wrapper.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server_lib.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/verification.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/fedadagrad.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/fedadam.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/fedavg.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/fedavgm.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/feddyn.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/fedyogi.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/mime.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/mimelite.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/algorithms/scaffold.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server_evaluate/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server_evaluate/eval_lib.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server_evaluate/net.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 federa-0.0.3/federa/server/src/server_evaluate/net_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 federa-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 federa-0.0.3/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 federa-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 federa-0.0.3/PKG-INFO
```

### Comparing `federa-0.0.2/federa/client/start_client.py` & `federa-0.0.3/federa/client/start_client.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/ClientConnection_pb2.py` & `federa-0.0.3/federa/client/src/ClientConnection_pb2.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/ClientConnection_pb2_grpc.py` & `federa-0.0.3/federa/client/src/ClientConnection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/client.py` & `federa-0.0.3/federa/client/src/client.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/client_lib.py` & `federa-0.0.3/federa/client/src/client_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/data_utils.py` & `federa-0.0.3/federa/client/src/data_utils.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/distribution.py` & `federa-0.0.3/federa/client/src/distribution.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/get_data.py` & `federa-0.0.3/federa/client/src/get_data.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/net.py` & `federa-0.0.3/federa/client/src/net.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/client/src/net_lib.py` & `federa-0.0.3/federa/client/src/net_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/start_server.py` & `federa-0.0.3/federa/server/start_server.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/ClientConnection_pb2.py` & `federa-0.0.3/federa/server/src/ClientConnection_pb2.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/ClientConnection_pb2_grpc.py` & `federa-0.0.3/federa/server/src/ClientConnection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/client_connection_servicer.py` & `federa-0.0.3/federa/server/src/client_connection_servicer.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/client_manager.py` & `federa-0.0.3/federa/server/src/client_manager.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/client_wrapper.py` & `federa-0.0.3/federa/server/src/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/server.py` & `federa-0.0.3/federa/server/src/server.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/server_lib.py` & `federa-0.0.3/federa/server/src/server_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/verification.py` & `federa-0.0.3/federa/server/src/verification.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/fedadagrad.py` & `federa-0.0.3/federa/server/src/algorithms/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/fedadam.py` & `federa-0.0.3/federa/server/src/algorithms/fedadam.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/fedavg.py` & `federa-0.0.3/federa/server/src/algorithms/fedavg.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/fedavgm.py` & `federa-0.0.3/federa/server/src/algorithms/fedavgm.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/feddyn.py` & `federa-0.0.3/federa/server/src/algorithms/feddyn.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/fedyogi.py` & `federa-0.0.3/federa/server/src/algorithms/fedyogi.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/mime.py` & `federa-0.0.3/federa/server/src/algorithms/mime.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/mimelite.py` & `federa-0.0.3/federa/server/src/algorithms/mimelite.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/algorithms/scaffold.py` & `federa-0.0.3/federa/server/src/algorithms/scaffold.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/server_evaluate/net.py` & `federa-0.0.3/federa/server/src/server_evaluate/net.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/federa/server/src/server_evaluate/net_lib.py` & `federa-0.0.3/federa/server/src/server_evaluate/net_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/LICENSE` & `federa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `federa-0.0.2/README.md` & `federa-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Federated Learning Framework
-
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://pypi.org/project/federa/)
 [![Documentation Status](https://readthedocs.org/projects/federa/badge/?version=latest)](https://federa.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Ubuntu CI status](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/ubuntu.yml)
 [![Windows CI status](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/windows.yml/badge.svg)](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/windows.yml)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7362/badge)](https://bestpractices.coreinfrastructure.org/projects/7362)
+[![Downloads](https://static.pepy.tech/badge/federa)](https://pepy.tech/project/federa)
 
 `FedERA` is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases.
 
 ## Supported Devices
 
 FedERA has been extensively tested on and works with the following devices:
```

### Comparing `federa-0.0.2/pyproject.toml` & `federa-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "federa"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Anupam Borthakur", email="anupamborthakur@kgpian.iitkgp.ac.in" },
 ]
 description = "FedERA is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,28 +16,24 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "codecarbon>=2.1.4",
   "grpcio>=1.53.0",
-  "numpy~=1.23.4",
+  "numpy>=1.23.4",
   "Pillow>=9.5.0",
   "protobuf>=3.20.2",
   "torch>=2.0.0",
   "torchvision>=0.15.1",
   "tqdm>=4.65.0",
   "bandit"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/anupamkliv/FedERA"
 "Bug Tracker" = "https://github.com/anupamkliv/FedERA/issues"
 
 [tool.hatch.build]
 include = [
-  "/federa",
-  "/test",
-  "/client_custom_dataset",
-  "/server_custom_dataset",
-  "/configs",
+  "/federa"
 ]
```

### Comparing `federa-0.0.2/PKG-INFO` & `federa-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: federa
-Version: 0.0.2
+Version: 0.0.3
 Summary: FedERA is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases.
 Project-URL: Homepage, https://github.com/anupamkliv/FedERA
 Project-URL: Bug Tracker, https://github.com/anupamkliv/FedERA/issues
 Author-email: Anupam Borthakur <anupamborthakur@kgpian.iitkgp.ac.in>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bandit
 Requires-Dist: codecarbon>=2.1.4
 Requires-Dist: grpcio>=1.53.0
-Requires-Dist: numpy~=1.23.4
+Requires-Dist: numpy>=1.23.4
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: protobuf>=3.20.2
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.15.1
 Requires-Dist: tqdm>=4.65.0
 Description-Content-Type: text/markdown
 
 # Federated Learning Framework
-
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://pypi.org/project/federa/)
 [![Documentation Status](https://readthedocs.org/projects/federa/badge/?version=latest)](https://federa.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Ubuntu CI status](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/ubuntu.yml)
 [![Windows CI status](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/windows.yml/badge.svg)](https://github.com/anupam-kliv/fl_framework_initial/actions/workflows/windows.yml)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7362/badge)](https://bestpractices.coreinfrastructure.org/projects/7362)
+[![Downloads](https://static.pepy.tech/badge/federa)](https://pepy.tech/project/federa)
 
 `FedERA` is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases.
 
 ## Supported Devices
 
 FedERA has been extensively tested on and works with the following devices:
```

